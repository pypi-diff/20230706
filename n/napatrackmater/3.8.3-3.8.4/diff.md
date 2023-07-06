# Comparing `tmp/napatrackmater-3.8.3.tar.gz` & `tmp/napatrackmater-3.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.8.3.tar", last modified: Thu Jul  6 18:34:49 2023, max compression
+gzip compressed data, was "napatrackmater-3.8.4.tar", last modified: Thu Jul  6 19:25:52 2023, max compression
```

## Comparing `napatrackmater-3.8.3.tar` & `napatrackmater-3.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 18:34:49.872019 napatrackmater-3.8.3/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.3/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-06 18:34:49.866611 napatrackmater-3.8.3/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.3/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 18:34:49.618458 napatrackmater-3.8.3/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.3/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.3/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110476 2023-07-06 18:34:15.000000 napatrackmater-3.8.3/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.3/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.3/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14327 2023-07-03 20:00:06.000000 napatrackmater-3.8.3/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.3/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.3/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.3/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-06 18:34:23.000000 napatrackmater-3.8.3/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 18:34:49.827344 napatrackmater-3.8.3/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-06 18:34:48.000000 napatrackmater-3.8.3/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-06 18:34:49.000000 napatrackmater-3.8.3/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-06 18:34:48.000000 napatrackmater-3.8.3/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-06 18:34:48.000000 napatrackmater-3.8.3/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-06 18:34:48.000000 napatrackmater-3.8.3/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-06 18:34:48.000000 napatrackmater-3.8.3/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-06 18:34:49.874023 napatrackmater-3.8.3/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.3/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 19:25:52.769118 napatrackmater-3.8.4/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.4/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-06 19:25:52.764152 napatrackmater-3.8.4/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.4/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 19:25:52.549660 napatrackmater-3.8.4/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.4/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.4/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110955 2023-07-06 19:25:26.000000 napatrackmater-3.8.4/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.4/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.4/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    14327 2023-07-03 20:00:06.000000 napatrackmater-3.8.4/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.4/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.4/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.4/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-06 19:25:34.000000 napatrackmater-3.8.4/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 19:25:52.729333 napatrackmater-3.8.4/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-06 19:25:51.000000 napatrackmater-3.8.4/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-06 19:25:52.000000 napatrackmater-3.8.4/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-06 19:25:51.000000 napatrackmater-3.8.4/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-06 19:25:51.000000 napatrackmater-3.8.4/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-06 19:25:51.000000 napatrackmater-3.8.4/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-06 19:25:51.000000 napatrackmater-3.8.4/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-06 19:25:52.771636 napatrackmater-3.8.4/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.4/setup.py
```

### Comparing `napatrackmater-3.8.3/LICENSE` & `napatrackmater-3.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/PKG-INFO` & `napatrackmater-3.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.3
+Version: 3.8.4
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.8.3/README.md` & `napatrackmater-3.8.4/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.8.4/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.8.4/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater/Trackmate.py` & `napatrackmater-3.8.4/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1197,5709 +1197,5739 @@
 00004ac0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
 00004ad0: 7461 7267 6574 5f63 656c 6c20 3d20 6e65  target_cell = ne
 00004ae0: 7874 5f74 6172 6765 745f 6365 6c6c 735b  xt_target_cells[
 00004af0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
 00004b00: 2020 2020 2020 2020 7768 696c 6520 6e65          while ne
 00004b10: 7874 5f74 6172 6765 745f 6365 6c6c 206e  xt_target_cell n
 00004b20: 6f74 2069 6e20 736f 7274 6564 5f72 6f6f  ot in sorted_roo
-00004b30: 745f 7370 6c69 7473 206f 7220 6e65 7874  t_splits or next
-00004b40: 5f74 6172 6765 745f 6365 6c6c 206e 6f74  _target_cell not
-00004b50: 2069 6e20 726f 6f74 5f6c 6561 663a 0d0a   in root_leaf:..
-00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b70: 2020 2020 2020 2020 7365 6c66 2e67 656e          self.gen
-00004b80: 6572 6174 696f 6e5f 6469 6374 5b6e 6578  eration_dict[nex
-00004b90: 745f 7461 7267 6574 5f63 656c 6c5d 203d  t_target_cell] =
-00004ba0: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2020 2020 7365 6c66 2e74 7261 636b 6c65      self.trackle
-00004bd0: 745f 6469 6374 5b6e 6578 745f 7461 7267  t_dict[next_targ
-00004be0: 6574 5f63 656c 6c5d 203d 2074 7261 636b  et_cell] = track
-00004bf0: 6c65 745f 636f 756e 740d 0a20 2020 2020  let_count..     
-00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 2020 2069 6620 6e65 7874 5f74 6172 6765     if next_targe
-00004c20: 745f 6365 6c6c 2069 6e20 7365 6c66 2e65  t_cell in self.e
-00004c30: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00004c40: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
-00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c60: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
-00004c70: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
-00004c80: 7267 6574 5f6c 6f6f 6b75 705b 6e65 7874  rget_lookup[next
-00004c90: 5f74 6172 6765 745f 6365 6c6c 5d0d 0a20  _target_cell].. 
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cb0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00004cc0: 7461 7267 6574 5f63 656c 6c20 3d20 6e65  target_cell = ne
-00004cd0: 7874 5f74 6172 6765 745f 6365 6c6c 735b  xt_target_cells[
-00004ce0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00004cf0: 2020 2020 2020 2020 6e65 7874 5f69 7465          next_ite
-00004d00: 725f 6365 6c6c 732e 6170 7065 6e64 285b  r_cells.append([
-00004d10: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
-00004d20: 2c20 7472 6163 6b6c 6574 5f63 6f75 6e74  , tracklet_count
-00004d30: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
-00004d40: 200d 0a20 2020 2020 2020 2020 2020 2066   ..            f
-00004d50: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00004d60: 6e28 6e65 7874 5f69 7465 725f 6365 6c6c  n(next_iter_cell
-00004d70: 7329 293a 0d0a 2020 2020 2020 2020 2020  s)):..          
-00004d80: 2020 2020 2020 6e65 7874 5f74 6172 6765        next_targe
-00004d90: 745f 6365 6c6c 2c20 7472 6163 6b6c 6574  t_cell, tracklet
-00004da0: 5f63 6f75 6e74 5f63 656c 6c20 3d20 6e65  _count_cell = ne
-00004db0: 7874 5f69 7465 725f 6365 6c6c 735b 695d  xt_iter_cells[i]
-00004dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004dd0: 2020 7365 6c66 2e67 656e 6572 6174 696f    self.generatio
-00004de0: 6e5f 6469 6374 5b6e 6578 745f 7461 7267  n_dict[next_targ
-00004df0: 6574 5f63 656c 6c5d 203d 2067 656e 5f63  et_cell] = gen_c
-00004e00: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-00004e10: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-00004e20: 6c65 745f 6469 6374 5b6e 6578 745f 7461  let_dict[next_ta
-00004e30: 7267 6574 5f63 656c 6c5d 203d 2074 7261  rget_cell] = tra
-00004e40: 636b 6c65 745f 636f 756e 745f 6365 6c6c  cklet_count_cell
-00004e50: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00004e60: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00004e70: 2020 6966 206c 656e 286e 6578 745f 6974    if len(next_it
-00004e80: 6572 5f63 656c 6c73 2920 3e20 303a 0d0a  er_cells) > 0:..
-00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ea0: 6e65 7874 5f67 656e 5f63 6f75 6e74 203d  next_gen_count =
-00004eb0: 2067 656e 5f63 6f75 6e74 202b 2031 0d0a   gen_count + 1..
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00004ee0: 656e 286e 6578 745f 6974 6572 5f63 656c  en(next_iter_cel
-00004ef0: 6c73 2929 3a0d 0a20 2020 2020 2020 2020  ls)):..         
-00004f00: 2020 2020 2020 2020 2020 7472 6163 6b6c            trackl
-00004f10: 6574 5f63 6f75 6e74 202b 3d20 310d 0a20  et_count += 1.. 
-00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f30: 2020 6e65 7874 5f74 6172 6765 745f 6365    next_target_ce
-00004f40: 6c6c 2c20 7472 6163 6b6c 6574 5f63 6f75  ll, tracklet_cou
-00004f50: 6e74 5f63 656c 6c20 3d20 6e65 7874 5f69  nt_cell = next_i
-00004f60: 7465 725f 6365 6c6c 735b 695d 0d0a 2020  ter_cells[i]..  
-00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f80: 2069 6620 6e65 7874 5f74 6172 6765 745f   if next_target_
-00004f90: 6365 6c6c 2069 6e20 7365 6c66 2e65 6467  cell in self.edg
-00004fa0: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
-00004fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004fc0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00004fd0: 6365 6c6c 7320 3d20 7365 6c66 2e65 6467  cells = self.edg
-00004fe0: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
-00004ff0: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
-00005000: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00005010: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00005020: 6974 6572 6174 655f 6469 7669 6469 6e67  iterate_dividing
-00005030: 5f72 6563 7572 7369 7665 2872 6f6f 745f  _recursive(root_
-00005040: 6c65 6166 2c20 7461 7267 6574 5f63 656c  leaf, target_cel
-00005050: 6c73 2c20 736f 7274 6564 5f72 6f6f 745f  ls, sorted_root_
-00005060: 7370 6c69 7473 2c20 6e65 7874 5f67 656e  splits, next_gen
-00005070: 5f63 6f75 6e74 2c20 7472 6163 6b6c 6574  _count, tracklet
-00005080: 5f63 6f75 6e74 2920 2020 2020 200d 0a20  _count)      .. 
-00005090: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000050a0: 2064 6566 205f 6974 6572 6174 655f 6469   def _iterate_di
-000050b0: 7669 6469 6e67 2873 656c 662c 2072 6f6f  viding(self, roo
-000050c0: 745f 726f 6f74 2c20 726f 6f74 5f6c 6561  t_root, root_lea
-000050d0: 662c 2072 6f6f 745f 7370 6c69 7473 293a  f, root_splits):
-000050e0: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
-000050f0: 6e5f 636f 756e 7420 3d20 300d 0a20 2020  n_count = 0..   
-00005100: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-00005110: 745f 636f 756e 7420 3d20 300d 0a20 2020  t_count = 0..   
-00005120: 2020 2020 2020 2020 2066 6f72 2072 6f6f           for roo
-00005130: 745f 616c 6c20 696e 2072 6f6f 745f 726f  t_all in root_ro
-00005140: 6f74 3a0d 0a20 2020 2020 2020 2020 2020  ot:..           
-00005150: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-00005160: 6e65 7261 7469 6f6e 5f64 6963 745b 726f  neration_dict[ro
-00005170: 6f74 5f61 6c6c 5d20 3d20 6765 6e5f 636f  ot_all] = gen_co
-00005180: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-00005190: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-000051a0: 6163 6b6c 6574 5f64 6963 745b 726f 6f74  acklet_dict[root
-000051b0: 5f61 6c6c 5d20 3d20 7472 6163 6b6c 6574  _all] = tracklet
-000051c0: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
-000051d0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-000051e0: 6f6f 745f 616c 6c20 696e 2073 656c 662e  oot_all in self.
-000051f0: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00005200: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
-00005210: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00005220: 7267 6574 5f63 656c 6c20 3d20 7365 6c66  rget_cell = self
-00005230: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00005240: 6b75 705b 726f 6f74 5f61 6c6c 5d5b 305d  kup[root_all][0]
-00005250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005260: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-00005270: 2074 6172 6765 745f 6365 6c6c 206e 6f74   target_cell not
-00005280: 2069 6e20 726f 6f74 5f73 706c 6974 733a   in root_splits:
-00005290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052b0: 2020 6966 2074 6172 6765 745f 6365 6c6c    if target_cell
-000052c0: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
-000052d0: 7267 6574 5f6c 6f6f 6b75 703a 0d0a 2020  rget_lookup:..  
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005300: 2020 7365 6c66 2e67 656e 6572 6174 696f    self.generatio
-00005310: 6e5f 6469 6374 5b74 6172 6765 745f 6365  n_dict[target_ce
-00005320: 6c6c 5d20 3d20 6765 6e5f 636f 756e 740d  ll] = gen_count.
-00005330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005350: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
-00005360: 6574 5f64 6963 745b 7461 7267 6574 5f63  et_dict[target_c
-00005370: 656c 6c5d 203d 2074 7261 636b 6c65 745f  ell] = tracklet_
-00005380: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053a0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
-000053b0: 745f 6365 6c6c 203d 2073 656c 662e 6564  t_cell = self.ed
-000053c0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-000053d0: 5b74 6172 6765 745f 6365 6c6c 5d5b 305d  [target_cell][0]
-000053e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005400: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
-00005410: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
-00005420: 5f72 6f6f 745f 7370 6c69 7473 203d 2073  _root_splits = s
-00005430: 656c 662e 5f73 6f72 745f 6469 7669 6469  elf._sort_dividi
-00005440: 6e67 5f63 656c 6c73 2872 6f6f 745f 7370  ng_cells(root_sp
-00005450: 6c69 7473 290d 0a20 2020 2020 2020 2020  lits)..         
-00005460: 2020 2067 656e 5f63 6f75 6e74 203d 2030     gen_count = 0
-00005470: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-00005480: 6163 6b6c 6574 5f63 6f75 6e74 203d 2030  acklet_count = 0
-00005490: 0d0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
-000054a0: 7874 5f67 656e 5f63 6f75 6e74 203d 2030  xt_gen_count = 0
-000054b0: 0d0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
-000054c0: 7273 745f 7370 6c69 7420 3d20 736f 7274  rst_split = sort
-000054d0: 6564 5f72 6f6f 745f 7370 6c69 7473 5b30  ed_root_splits[0
-000054e0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-000054f0: 656c 662e 6765 6e65 7261 7469 6f6e 5f64  elf.generation_d
-00005500: 6963 745b 6669 7273 745f 7370 6c69 745d  ict[first_split]
-00005510: 203d 2067 656e 5f63 6f75 6e74 0d0a 2020   = gen_count..  
-00005520: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00005530: 7261 636b 6c65 745f 6469 6374 5b66 6972  racklet_dict[fir
-00005540: 7374 5f73 706c 6974 5d20 3d20 7472 6163  st_split] = trac
-00005550: 6b6c 6574 5f63 6f75 6e74 0d0a 2020 2020  klet_count..    
-00005560: 2020 2020 2020 2020 6966 2066 6972 7374          if first
-00005570: 5f73 706c 6974 2069 6e20 7365 6c66 2e65  _split in self.e
-00005580: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00005590: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
-000055a0: 2020 2020 7461 7267 6574 5f63 656c 6c73      target_cells
-000055b0: 203d 2073 656c 662e 6564 6765 5f74 6172   = self.edge_tar
-000055c0: 6765 745f 6c6f 6f6b 7570 5b66 6972 7374  get_lookup[first
-000055d0: 5f73 706c 6974 5d0d 0a20 2020 2020 2020  _split]..       
-000055e0: 2020 2020 2020 2020 206e 6578 745f 6765           next_ge
-000055f0: 6e5f 636f 756e 7420 2b3d 2031 0d0a 2020  n_count += 1..  
-00005600: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005610: 6c66 2e5f 6974 6572 6174 655f 6469 7669  lf._iterate_divi
-00005620: 6469 6e67 5f72 6563 7572 7369 7665 2872  ding_recursive(r
-00005630: 6f6f 745f 6c65 6166 2c20 7461 7267 6574  oot_leaf, target
-00005640: 5f63 656c 6c73 2c20 736f 7274 6564 5f72  _cells, sorted_r
-00005650: 6f6f 745f 7370 6c69 7473 2c20 6e65 7874  oot_splits, next
-00005660: 5f67 656e 5f63 6f75 6e74 2c20 7472 6163  _gen_count, trac
-00005670: 6b6c 6574 5f63 6f75 6e74 290d 0a20 2020  klet_count)..   
-00005680: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-000056c0: 2064 6566 205f 6974 6572 6174 655f 7370   def _iterate_sp
-000056d0: 6c69 745f 646f 776e 2873 656c 662c 2072  lit_down(self, r
-000056e0: 6f6f 745f 726f 6f74 2c20 726f 6f74 5f6c  oot_root, root_l
-000056f0: 6561 662c 2072 6f6f 745f 7370 6c69 7473  eaf, root_splits
-00005700: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
-00005710: 2020 2020 2020 2069 6620 6c65 6e28 726f         if len(ro
-00005720: 6f74 5f73 706c 6974 7329 203d 3d20 303a  ot_splits) == 0:
-00005730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005740: 2073 656c 662e 5f69 7465 7261 7465 5f6e   self._iterate_n
-00005750: 6f6e 5f64 6976 6964 696e 6728 726f 6f74  on_dividing(root
-00005760: 5f72 6f6f 742c 2072 6f6f 745f 6c65 6166  _root, root_leaf
-00005770: 290d 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
-00005780: 6e28 726f 6f74 5f73 706c 6974 7329 203e  n(root_splits) >
-00005790: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000057a0: 2020 2020 7365 6c66 2e5f 6974 6572 6174      self._iterat
-000057b0: 655f 6469 7669 6469 6e67 2872 6f6f 745f  e_dividing(root_
-000057c0: 726f 6f74 2c20 726f 6f74 5f6c 6561 662c  root, root_leaf,
-000057d0: 2072 6f6f 745f 7370 6c69 7473 2920 2020   root_splits)   
-000057e0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005800: 2020 2020 0d0a 2020 2020 6465 6620 5f67      ..    def _g
-00005810: 6574 5f62 6f75 6e64 6172 795f 6469 7374  et_boundary_dist
-00005820: 2873 656c 662c 2066 7261 6d65 2c20 7465  (self, frame, te
-00005830: 7374 6c6f 6361 7469 6f6e 293a 0d0a 2020  stlocation):..  
-00005840: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00005850: 2069 6620 7365 6c66 2e6d 6173 6b20 6973   if self.mask is
-00005860: 206e 6f74 204e 6f6e 653a 0d0a 0d0a 2020   not None:....  
-00005870: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00005880: 6565 2c20 696e 6469 6365 732c 206d 6173  ee, indices, mas
-00005890: 6b63 656e 7472 6f69 6420 3d20 7365 6c66  kcentroid = self
-000058a0: 2e74 696d 6564 5f6d 6173 6b5b 7374 7228  .timed_mask[str(
-000058b0: 696e 7428 666c 6f61 7428 6672 616d 6529  int(float(frame)
-000058c0: 2929 5d0d 0a20 2020 2020 2020 2020 2020  ))]..           
-000058d0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000058e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000058f0: 2047 6574 2074 6865 206c 6f63 6174 696f   Get the locatio
-00005900: 6e20 616e 6420 6469 7374 616e 6365 2074  n and distance t
-00005910: 6f20 7468 6520 6e65 6172 6573 7420 626f  o the nearest bo
-00005920: 756e 6461 7279 2070 6f69 6e74 0d0a 2020  undary point..  
-00005930: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00005940: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00005950: 2c20 6c6f 6361 7469 6f6e 696e 6465 7820  , locationindex 
-00005960: 3d20 7472 6565 2e71 7565 7279 2874 6573  = tree.query(tes
-00005970: 746c 6f63 6174 696f 6e29 0d0a 2020 2020  tlocation)..    
-00005980: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-00005990: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-000059a0: 206d 6178 2830 2c20 6469 7374 616e 6365   max(0, distance
-000059b0: 5f63 656c 6c5f 6d61 736b 290d 0a20 2020  _cell_mask)..   
-000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059d0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-000059e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059f0: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
-00005a00: 6173 6b20 3d20 300d 0a20 2020 2020 2020  ask = 0..       
-00005a10: 2020 2020 2020 2020 206d 6173 6b63 656e           maskcen
-00005a20: 7472 6f69 6420 3d20 2831 2c31 2c31 290d  troid = (1,1,1).
-00005a30: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00005a40: 6e20 6469 7374 616e 6365 5f63 656c 6c5f  n distance_cell_
-00005a50: 6d61 736b 2c20 6d61 736b 6365 6e74 726f  mask, maskcentro
-00005a60: 6964 2020 2020 2020 2020 0d0a 2020 2020  id        ..    
-00005a70: 2020 2020 200d 0a0d 0a20 2020 2064 6566       ....    def
-00005a80: 205f 7472 6163 6b5f 636f 6d70 7574 6572   _track_computer
-00005a90: 2873 656c 662c 2074 7261 636b 2c20 7472  (self, track, tr
-00005aa0: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
-00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ac0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ae0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00005b10: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b30: 2020 2020 2020 756e 6971 7565 5f74 7261        unique_tra
-00005b40: 636b 6c65 745f 6964 7320 3d20 5b5d 0d0a  cklet_ids = []..
-00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00005b70: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
-00005b80: 7461 7267 6574 5f69 6473 203d 2020 7365  target_ids =  se
-00005b90: 6c66 2e5f 6765 6e65 7261 7465 5f67 656e  lf._generate_gen
-00005ba0: 6572 6174 696f 6e73 2874 7261 636b 290d  erations(track).
-00005bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005bc0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00005bd0: 745f 726f 6f74 2c20 726f 6f74 5f73 706c  t_root, root_spl
-00005be0: 6974 732c 2072 6f6f 745f 6c65 6166 203d  its, root_leaf =
-00005bf0: 2073 656c 662e 5f63 7265 6174 655f 6765   self._create_ge
-00005c00: 6e65 7261 7469 6f6e 7328 616c 6c5f 736f  nerations(all_so
-00005c10: 7572 6365 5f69 6473 2c20 616c 6c5f 7461  urce_ids, all_ta
-00005c20: 7267 6574 5f69 6473 2920 0d0a 2020 2020  rget_ids) ..    
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 2020 2020 2020 7365 6c66 2e5f 6974 6572        self._iter
-00005c70: 6174 655f 7370 6c69 745f 646f 776e 2872  ate_split_down(r
-00005c80: 6f6f 745f 726f 6f74 2c20 726f 6f74 5f6c  oot_root, root_l
-00005c90: 6561 662c 2072 6f6f 745f 7370 6c69 7473  eaf, root_splits
-00005ca0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00005cc0: 756d 6265 725f 6469 7669 6469 6e67 203d  umber_dividing =
-00005cd0: 206c 656e 2872 6f6f 745f 7370 6c69 7473   len(root_splits
-00005ce0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005cf0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005d00: 2044 6574 6572 6d69 6e65 2069 6620 6120   Determine if a 
-00005d10: 7472 6163 6b20 6861 7320 6469 7669 7369  track has divisi
-00005d20: 6f6e 7320 6f72 206e 6f6e 650d 0a20 2020  ons or none..   
+00004b30: 745f 7370 6c69 7473 3a0d 0a20 2020 2020  t_splits:..     
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b50: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00004b60: 6f6e 5f64 6963 745b 6e65 7874 5f74 6172  on_dict[next_tar
+00004b70: 6765 745f 6365 6c6c 5d20 3d20 6765 6e5f  get_cell] = gen_
+00004b80: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004ba0: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
+00004bb0: 745b 6e65 7874 5f74 6172 6765 745f 6365  t[next_target_ce
+00004bc0: 6c6c 5d20 3d20 7472 6163 6b6c 6574 5f63  ll] = tracklet_c
+00004bd0: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+00004be0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004bf0: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
+00004c00: 6c20 696e 2072 6f6f 745f 6c65 6166 3a0d  l in root_leaf:.
+00004c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c30: 7365 6c66 2e67 656e 6572 6174 696f 6e5f  self.generation_
+00004c40: 6469 6374 5b74 6172 6765 745f 6365 6c6c  dict[target_cell
+00004c50: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004c80: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
+00004c90: 5b74 6172 6765 745f 6365 6c6c 5d20 3d20  [target_cell] = 
+00004ca0: 7472 6163 6b6c 6574 5f63 6f75 6e74 0d0a  tracklet_count..
+00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00004cd0: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004cf0: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
+00004d00: 6c20 696e 2073 656c 662e 6564 6765 5f74  l in self.edge_t
+00004d10: 6172 6765 745f 6c6f 6f6b 7570 3a0d 0a20  arget_lookup:.. 
+00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d30: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00004d40: 7461 7267 6574 5f63 656c 6c73 203d 2073  target_cells = s
+00004d50: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
+00004d60: 6c6f 6f6b 7570 5b6e 6578 745f 7461 7267  lookup[next_targ
+00004d70: 6574 5f63 656c 6c5d 0d0a 2020 2020 2020  et_cell]..      
+00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d90: 2020 2020 2020 6e65 7874 5f74 6172 6765        next_targe
+00004da0: 745f 6365 6c6c 203d 206e 6578 745f 7461  t_cell = next_ta
+00004db0: 7267 6574 5f63 656c 6c73 5b30 5d0d 0a20  rget_cells[0].. 
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
+00004de0: 7874 5f74 6172 6765 745f 6365 6c6c 2069  xt_target_cell i
+00004df0: 6e20 726f 6f74 5f6c 6561 663a 0d0a 2020  n root_leaf:..  
+00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004e20: 662e 6765 6e65 7261 7469 6f6e 5f64 6963  f.generation_dic
+00004e30: 745b 7461 7267 6574 5f63 656c 6c5d 203d  t[target_cell] =
+00004e40: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
+00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004e70: 7472 6163 6b6c 6574 5f64 6963 745b 7461  tracklet_dict[ta
+00004e80: 7267 6574 5f63 656c 6c5d 203d 2074 7261  rget_cell] = tra
+00004e90: 636b 6c65 745f 636f 756e 740d 0a20 2020  cklet_count..   
+00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004eb0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00004ec0: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
+00004ed0: 2020 2020 2020 206e 6578 745f 6974 6572         next_iter
+00004ee0: 5f63 656c 6c73 2e61 7070 656e 6428 5b6e  _cells.append([n
+00004ef0: 6578 745f 7461 7267 6574 5f63 656c 6c2c  ext_target_cell,
+00004f00: 2074 7261 636b 6c65 745f 636f 756e 745d   tracklet_count]
+00004f10: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00004f20: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00004f30: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+00004f40: 286e 6578 745f 6974 6572 5f63 656c 6c73  (next_iter_cells
+00004f50: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00004f60: 2020 2020 206e 6578 745f 7461 7267 6574       next_target
+00004f70: 5f63 656c 6c2c 2074 7261 636b 6c65 745f  _cell, tracklet_
+00004f80: 636f 756e 745f 6365 6c6c 203d 206e 6578  count_cell = nex
+00004f90: 745f 6974 6572 5f63 656c 6c73 5b69 5d0d  t_iter_cells[i].
+00004fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004fb0: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
+00004fc0: 5f64 6963 745b 6e65 7874 5f74 6172 6765  _dict[next_targe
+00004fd0: 745f 6365 6c6c 5d20 3d20 6765 6e5f 636f  t_cell] = gen_co
+00004fe0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+00004ff0: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
+00005000: 6574 5f64 6963 745b 6e65 7874 5f74 6172  et_dict[next_tar
+00005010: 6765 745f 6365 6c6c 5d20 3d20 7472 6163  get_cell] = trac
+00005020: 6b6c 6574 5f63 6f75 6e74 5f63 656c 6c20  klet_count_cell 
+00005030: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00005040: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00005050: 2069 6620 6c65 6e28 6e65 7874 5f69 7465   if len(next_ite
+00005060: 725f 6365 6c6c 7329 203e 2030 3a0d 0a20  r_cells) > 0:.. 
+00005070: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00005080: 6578 745f 6765 6e5f 636f 756e 7420 3d20  ext_gen_count = 
+00005090: 6765 6e5f 636f 756e 7420 2b20 310d 0a20  gen_count + 1.. 
+000050a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000050b0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+000050c0: 6e28 6e65 7874 5f69 7465 725f 6365 6c6c  n(next_iter_cell
+000050d0: 7329 293a 0d0a 2020 2020 2020 2020 2020  s)):..          
+000050e0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+000050f0: 745f 636f 756e 7420 2b3d 2031 0d0a 2020  t_count += 1..  
+00005100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005110: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
+00005120: 6c2c 2074 7261 636b 6c65 745f 636f 756e  l, tracklet_coun
+00005130: 745f 6365 6c6c 203d 206e 6578 745f 6974  t_cell = next_it
+00005140: 6572 5f63 656c 6c73 5b69 5d0d 0a20 2020  er_cells[i]..   
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 6966 206e 6578 745f 7461 7267 6574 5f63  if next_target_c
+00005170: 656c 6c20 696e 2073 656c 662e 6564 6765  ell in self.edge
+00005180: 5f74 6172 6765 745f 6c6f 6f6b 7570 3a0d  _target_lookup:.
+00005190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051a0: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
+000051b0: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
+000051c0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b6e  _target_lookup[n
+000051d0: 6578 745f 7461 7267 6574 5f63 656c 6c5d  ext_target_cell]
+000051e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000051f0: 2020 2020 2020 2020 2073 656c 662e 5f69           self._i
+00005200: 7465 7261 7465 5f64 6976 6964 696e 675f  terate_dividing_
+00005210: 7265 6375 7273 6976 6528 726f 6f74 5f6c  recursive(root_l
+00005220: 6561 662c 2074 6172 6765 745f 6365 6c6c  eaf, target_cell
+00005230: 732c 2073 6f72 7465 645f 726f 6f74 5f73  s, sorted_root_s
+00005240: 706c 6974 732c 206e 6578 745f 6765 6e5f  plits, next_gen_
+00005250: 636f 756e 742c 2074 7261 636b 6c65 745f  count, tracklet_
+00005260: 636f 756e 7429 2020 2020 2020 0d0a 2020  count)      ..  
+00005270: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00005280: 6465 6620 5f69 7465 7261 7465 5f64 6976  def _iterate_div
+00005290: 6964 696e 6728 7365 6c66 2c20 726f 6f74  iding(self, root
+000052a0: 5f72 6f6f 742c 2072 6f6f 745f 6c65 6166  _root, root_leaf
+000052b0: 2c20 726f 6f74 5f73 706c 6974 7329 3a0d  , root_splits):.
+000052c0: 0a20 2020 2020 2020 2020 2020 2067 656e  .            gen
+000052d0: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
+000052e0: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
+000052f0: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
+00005300: 2020 2020 2020 2020 666f 7220 726f 6f74          for root
+00005310: 5f61 6c6c 2069 6e20 726f 6f74 5f72 6f6f  _all in root_roo
+00005320: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00005330: 2020 2020 2020 2020 7365 6c66 2e67 656e          self.gen
+00005340: 6572 6174 696f 6e5f 6469 6374 5b72 6f6f  eration_dict[roo
+00005350: 745f 616c 6c5d 203d 2067 656e 5f63 6f75  t_all] = gen_cou
+00005360: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00005370: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00005380: 636b 6c65 745f 6469 6374 5b72 6f6f 745f  cklet_dict[root_
+00005390: 616c 6c5d 203d 2074 7261 636b 6c65 745f  all] = tracklet_
+000053a0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+000053b0: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
+000053c0: 6f74 5f61 6c6c 2069 6e20 7365 6c66 2e65  ot_all in self.e
+000053d0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
+000053e0: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
+000053f0: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00005400: 6765 745f 6365 6c6c 203d 2073 656c 662e  get_cell = self.
+00005410: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00005420: 7570 5b72 6f6f 745f 616c 6c5d 5b30 5d0d  up[root_all][0].
+00005430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005440: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+00005450: 7461 7267 6574 5f63 656c 6c20 6e6f 7420  target_cell not 
+00005460: 696e 2072 6f6f 745f 7370 6c69 7473 3a0d  in root_splits:.
+00005470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005490: 2069 6620 7461 7267 6574 5f63 656c 6c20   if target_cell 
+000054a0: 696e 2073 656c 662e 6564 6765 5f74 6172  in self.edge_tar
+000054b0: 6765 745f 6c6f 6f6b 7570 3a0d 0a20 2020  get_lookup:..   
+000054c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054e0: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
+000054f0: 5f64 6963 745b 7461 7267 6574 5f63 656c  _dict[target_cel
+00005500: 6c5d 203d 2067 656e 5f63 6f75 6e74 0d0a  l] = gen_count..
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005530: 2020 2020 7365 6c66 2e74 7261 636b 6c65      self.trackle
+00005540: 745f 6469 6374 5b74 6172 6765 745f 6365  t_dict[target_ce
+00005550: 6c6c 5d20 3d20 7472 6163 6b6c 6574 5f63  ll] = tracklet_c
+00005560: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00005590: 5f63 656c 6c20 3d20 7365 6c66 2e65 6467  _cell = self.edg
+000055a0: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
+000055b0: 7461 7267 6574 5f63 656c 6c5d 5b30 5d0d  target_cell][0].
+000055c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055e0: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
+000055f0: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
+00005600: 726f 6f74 5f73 706c 6974 7320 3d20 7365  root_splits = se
+00005610: 6c66 2e5f 736f 7274 5f64 6976 6964 696e  lf._sort_dividin
+00005620: 675f 6365 6c6c 7328 726f 6f74 5f73 706c  g_cells(root_spl
+00005630: 6974 7329 0d0a 2020 2020 2020 2020 2020  its)..          
+00005640: 2020 6765 6e5f 636f 756e 7420 3d20 300d    gen_count = 0.
+00005650: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+00005660: 636b 6c65 745f 636f 756e 7420 3d20 300d  cklet_count = 0.
+00005670: 0a20 2020 2020 2020 2020 2020 206e 6578  .            nex
+00005680: 745f 6765 6e5f 636f 756e 7420 3d20 300d  t_gen_count = 0.
+00005690: 0a20 2020 2020 2020 2020 2020 2066 6972  .            fir
+000056a0: 7374 5f73 706c 6974 203d 2073 6f72 7465  st_split = sorte
+000056b0: 645f 726f 6f74 5f73 706c 6974 735b 305d  d_root_splits[0]
+000056c0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000056d0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+000056e0: 6374 5b66 6972 7374 5f73 706c 6974 5d20  ct[first_split] 
+000056f0: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
+00005700: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+00005710: 6163 6b6c 6574 5f64 6963 745b 6669 7273  acklet_dict[firs
+00005720: 745f 7370 6c69 745d 203d 2074 7261 636b  t_split] = track
+00005730: 6c65 745f 636f 756e 740d 0a20 2020 2020  let_count..     
+00005740: 2020 2020 2020 2069 6620 6669 7273 745f         if first_
+00005750: 7370 6c69 7420 696e 2073 656c 662e 6564  split in self.ed
+00005760: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00005770: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005780: 2020 2074 6172 6765 745f 6365 6c6c 7320     target_cells 
+00005790: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
+000057a0: 6574 5f6c 6f6f 6b75 705b 6669 7273 745f  et_lookup[first_
+000057b0: 7370 6c69 745d 0d0a 2020 2020 2020 2020  split]..        
+000057c0: 2020 2020 2020 2020 6e65 7874 5f67 656e          next_gen
+000057d0: 5f63 6f75 6e74 202b 3d20 310d 0a20 2020  _count += 1..   
+000057e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000057f0: 662e 5f69 7465 7261 7465 5f64 6976 6964  f._iterate_divid
+00005800: 696e 675f 7265 6375 7273 6976 6528 726f  ing_recursive(ro
+00005810: 6f74 5f6c 6561 662c 2074 6172 6765 745f  ot_leaf, target_
+00005820: 6365 6c6c 732c 2073 6f72 7465 645f 726f  cells, sorted_ro
+00005830: 6f74 5f73 706c 6974 732c 206e 6578 745f  ot_splits, next_
+00005840: 6765 6e5f 636f 756e 742c 2074 7261 636b  gen_count, track
+00005850: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
+00005860: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005890: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+000058a0: 6465 6620 5f69 7465 7261 7465 5f73 706c  def _iterate_spl
+000058b0: 6974 5f64 6f77 6e28 7365 6c66 2c20 726f  it_down(self, ro
+000058c0: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
+000058d0: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
+000058e0: 3a0d 0a20 2020 2020 2020 2020 0d0a 2020  :..         ..  
+000058f0: 2020 2020 2020 6966 206c 656e 2872 6f6f        if len(roo
+00005900: 745f 7370 6c69 7473 2920 3d3d 2030 3a0d  t_splits) == 0:.
+00005910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005920: 7365 6c66 2e5f 6974 6572 6174 655f 6e6f  self._iterate_no
+00005930: 6e5f 6469 7669 6469 6e67 2872 6f6f 745f  n_dividing(root_
+00005940: 726f 6f74 2c20 726f 6f74 5f6c 6561 6629  root, root_leaf)
+00005950: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00005960: 2872 6f6f 745f 7370 6c69 7473 2920 3e20  (root_splits) > 
+00005970: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00005980: 2020 2073 656c 662e 5f69 7465 7261 7465     self._iterate
+00005990: 5f64 6976 6964 696e 6728 726f 6f74 5f72  _dividing(root_r
+000059a0: 6f6f 742c 2072 6f6f 745f 6c65 6166 2c20  oot, root_leaf, 
+000059b0: 726f 6f74 5f73 706c 6974 7329 2020 2020  root_splits)    
+000059c0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059e0: 2020 200d 0a20 2020 2064 6566 205f 6765     ..    def _ge
+000059f0: 745f 626f 756e 6461 7279 5f64 6973 7428  t_boundary_dist(
+00005a00: 7365 6c66 2c20 6672 616d 652c 2074 6573  self, frame, tes
+00005a10: 746c 6f63 6174 696f 6e29 3a0d 0a20 2020  tlocation):..   
+00005a20: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005a30: 6966 2073 656c 662e 6d61 736b 2069 7320  if self.mask is 
+00005a40: 6e6f 7420 4e6f 6e65 3a0d 0a0d 0a20 2020  not None:....   
+00005a50: 2020 2020 2020 2020 2020 2020 2074 7265               tre
+00005a60: 652c 2069 6e64 6963 6573 2c20 6d61 736b  e, indices, mask
+00005a70: 6365 6e74 726f 6964 203d 2073 656c 662e  centroid = self.
+00005a80: 7469 6d65 645f 6d61 736b 5b73 7472 2869  timed_mask[str(i
+00005a90: 6e74 2866 6c6f 6174 2866 7261 6d65 2929  nt(float(frame))
+00005aa0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
+00005ab0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00005ad0: 4765 7420 7468 6520 6c6f 6361 7469 6f6e  Get the location
+00005ae0: 2061 6e64 2064 6973 7461 6e63 6520 746f   and distance to
+00005af0: 2074 6865 206e 6561 7265 7374 2062 6f75   the nearest bou
+00005b00: 6e64 6172 7920 706f 696e 740d 0a20 2020  ndary point..   
+00005b10: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00005b20: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
+00005b30: 206c 6f63 6174 696f 6e69 6e64 6578 203d   locationindex =
+00005b40: 2074 7265 652e 7175 6572 7928 7465 7374   tree.query(test
+00005b50: 6c6f 6361 7469 6f6e 290d 0a20 2020 2020  location)..     
+00005b60: 2020 2020 2020 2020 2020 2064 6973 7461             dista
+00005b70: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00005b80: 6d61 7828 302c 2064 6973 7461 6e63 655f  max(0, distance_
+00005b90: 6365 6c6c 5f6d 6173 6b29 0d0a 2020 2020  cell_mask)..    
+00005ba0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00005bb0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bd0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00005be0: 736b 203d 2030 0d0a 2020 2020 2020 2020  sk = 0..        
+00005bf0: 2020 2020 2020 2020 6d61 736b 6365 6e74          maskcent
+00005c00: 726f 6964 203d 2028 312c 312c 3129 0d0a  roid = (1,1,1)..
+00005c10: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005c20: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+00005c30: 6173 6b2c 206d 6173 6b63 656e 7472 6f69  ask, maskcentroi
+00005c40: 6420 2020 2020 2020 200d 0a20 2020 2020  d        ..     
+00005c50: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+00005c60: 5f74 7261 636b 5f63 6f6d 7075 7465 7228  _track_computer(
+00005c70: 7365 6c66 2c20 7472 6163 6b2c 2074 7261  self, track, tra
+00005c80: 636b 5f69 6429 3a0d 0a20 2020 2020 2020  ck_id):..       
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00005cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ce0: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
+00005cf0: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d10: 2020 2020 2075 6e69 7175 655f 7472 6163       unique_trac
+00005d20: 6b6c 6574 5f69 6473 203d 205b 5d0d 0a20  klet_ids = [].. 
 00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d40: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00005d50: 726f 6f74 5f73 706c 6974 7329 203e 2030  root_splits) > 0
-00005d60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d80: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00005d90: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
-00005da0: 656c 5b74 7261 636b 5f69 645d 203d 205b  el[track_id] = [
-00005db0: 312c 206e 756d 6265 725f 6469 7669 6469  1, number_dividi
-00005dc0: 6e67 5d0d 0a20 2020 2020 2020 2020 2020  ng]..           
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005de0: 2020 2020 2064 6976 6964 696e 675f 7472       dividing_tr
-00005df0: 616a 6563 746f 7279 203d 2054 7275 650d  ajectory = True.
-00005e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d40: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
+00005d50: 6f75 7263 655f 6964 732c 2061 6c6c 5f74  ource_ids, all_t
+00005d60: 6172 6765 745f 6964 7320 3d20 2073 656c  arget_ids =  sel
+00005d70: 662e 5f67 656e 6572 6174 655f 6765 6e65  f._generate_gene
+00005d80: 7261 7469 6f6e 7328 7472 6163 6b29 0d0a  rations(track)..
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00005db0: 5f72 6f6f 742c 2072 6f6f 745f 7370 6c69  _root, root_spli
+00005dc0: 7473 2c20 726f 6f74 5f6c 6561 6620 3d20  ts, root_leaf = 
+00005dd0: 7365 6c66 2e5f 6372 6561 7465 5f67 656e  self._create_gen
+00005de0: 6572 6174 696f 6e73 2861 6c6c 5f73 6f75  erations(all_sou
+00005df0: 7263 655f 6964 732c 2061 6c6c 5f74 6172  rce_ids, all_tar
+00005e00: 6765 745f 6964 7329 200d 0a20 2020 2020  get_ids) ..     
 00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e20: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
-00005e30: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
-00005e40: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e70: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-00005e80: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
-00005e90: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
-00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005eb0: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
-00005ec0: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
-00005ed0: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
-00005ee0: 636b 4964 733a 2020 2020 200d 0a20 2020  ckIds:     ..   
-00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-00005f20: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
-00005f30: 7428 7472 6163 6b5f 6964 2929 0d0a 2020  t(track_id))..  
-00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
+00005e50: 7465 5f73 706c 6974 5f64 6f77 6e28 726f  te_split_down(ro
+00005e60: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
+00005e70: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
+00005e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005e90: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00005ea0: 6d62 6572 5f64 6976 6964 696e 6720 3d20  mber_dividing = 
+00005eb0: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
+00005ec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005ed0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00005ee0: 4465 7465 726d 696e 6520 6966 2061 2074  Determine if a t
+00005ef0: 7261 636b 2068 6173 2064 6976 6973 696f  rack has divisio
+00005f00: 6e73 206f 7220 6e6f 6e65 0d0a 2020 2020  ns or none..    
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
+00005f30: 6f6f 745f 7370 6c69 7473 2920 3e20 303a  oot_splits) > 0:
+00005f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f80: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005fb0: 756e 6971 7565 5f74 7261 636b 5f6d 6974  unique_track_mit
-00005fc0: 6f73 6973 5f6c 6162 656c 5b74 7261 636b  osis_label[track
-00005fd0: 5f69 645d 203d 205b 302c 2030 5d0d 0a20  _id] = [0, 0].. 
+00005f60: 2020 7365 6c66 2e75 6e69 7175 655f 7472    self.unique_tr
+00005f70: 6163 6b5f 6d69 746f 7369 735f 6c61 6265  ack_mitosis_labe
+00005f80: 6c5b 7472 6163 6b5f 6964 5d20 3d20 5b31  l[track_id] = [1
+00005f90: 2c20 6e75 6d62 6572 5f64 6976 6964 696e  , number_dividin
+00005fa0: 675d 0d0a 2020 2020 2020 2020 2020 2020  g]..            
+00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fc0: 2020 2020 6469 7669 6469 6e67 5f74 7261      dividing_tra
+00005fd0: 6a65 6374 6f72 7920 3d20 5472 7565 0d0a  jectory = True..
 00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006000: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
-00006010: 7279 203d 2046 616c 7365 0d0a 2020 2020  ry = False..    
-00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006030: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00006040: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
-00006050: 2069 6e20 7365 6c66 2e41 6c6c 5472 6163   in self.AllTrac
-00006060: 6b49 6473 3a0d 0a20 2020 2020 2020 2020  kIds:..         
-00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006090: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
-000060a0: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
-000060b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 2020 2069 6620 696e 7428 7472 6163 6b5f     if int(track_
-000060e0: 6964 2920 6e6f 7420 696e 2073 656c 662e  id) not in self.
-000060f0: 4e6f 726d 616c 5472 6163 6b49 6473 3a20  NormalTrackIds: 
-00006100: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
-00006130: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
-00006140: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
-00006150: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006170: 2020 666f 7220 6c65 6166 2069 6e20 726f    for leaf in ro
-00006180: 6f74 5f6c 6561 663a 0d0a 2020 2020 2020  ot_leaf:..      
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-000061b0: 7263 655f 6c65 6166 203d 2073 656c 662e  rce_leaf = self.
-000061c0: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
-000061d0: 7570 5b6c 6561 665d 0d0a 2020 2020 2020  up[leaf]..      
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00006200: 7265 6e74 5f63 656c 6c5f 6964 732e 6170  rent_cell_ids.ap
-00006210: 7065 6e64 286c 6561 6629 200d 0a20 2020  pend(leaf) ..   
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 7365 6c66 2e5f 6469 6374 5f75 7064 6174  self._dict_updat
-00006250: 6528 756e 6971 7565 5f74 7261 636b 6c65  e(unique_trackle
-00006260: 745f 6964 732c 206c 6561 662c 2074 7261  t_ids, leaf, tra
-00006270: 636b 5f69 642c 2073 6f75 7263 655f 6c65  ck_id, source_le
-00006280: 6166 2c20 4e6f 6e65 290d 0a20 2020 2020  af, None)..     
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000062b0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000062c0: 726f 7065 7274 6965 735b 6c65 6166 5d2e  roperties[leaf].
-000062d0: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
-000062e0: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
-000062f0: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
-00006300: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006320: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00006330: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00006340: 735b 6c65 6166 5d2e 7570 6461 7465 287b  s[leaf].update({
-00006350: 7365 6c66 2e6e 756d 6265 725f 6469 7669  self.number_divi
-00006360: 6469 6e67 5f6b 6579 203a 206e 756d 6265  ding_key : numbe
-00006370: 725f 6469 7669 6469 6e67 7d29 0d0a 0d0a  r_dividing})....
-00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000063a0: 736f 7572 6365 5f69 6420 696e 2061 6c6c  source_id in all
-000063b0: 5f73 6f75 7263 655f 6964 733a 0d0a 2020  _source_ids:..  
+00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006000: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
+00006010: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
+00006020: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
+00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006040: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006050: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
+00006060: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
+00006070: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
+00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006090: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
+000060a0: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
+000060b0: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
+000060c0: 6b49 6473 3a20 2020 2020 0d0a 2020 2020  kIds:     ..    
+000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060f0: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
+00006100: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
+00006110: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006140: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006160: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006180: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00006190: 6e69 7175 655f 7472 6163 6b5f 6d69 746f  nique_track_mito
+000061a0: 7369 735f 6c61 6265 6c5b 7472 6163 6b5f  sis_label[track_
+000061b0: 6964 5d20 3d20 5b30 2c20 305d 0d0a 2020  id] = [0, 0]..  
+000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061d0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+000061e0: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
+000061f0: 7920 3d20 4661 6c73 650d 0a20 2020 2020  y = False..     
+00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006210: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00006220: 7428 7472 6163 6b5f 6964 2920 6e6f 7420  t(track_id) not 
+00006230: 696e 2073 656c 662e 416c 6c54 7261 636b  in self.AllTrack
+00006240: 4964 733a 0d0a 2020 2020 2020 2020 2020  Ids:..          
+00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006260: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+00006270: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
+00006280: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
+00006290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062b0: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
+000062c0: 6429 206e 6f74 2069 6e20 7365 6c66 2e4e  d) not in self.N
+000062d0: 6f72 6d61 6c54 7261 636b 4964 733a 2020  ormalTrackIds:  
+000062e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000062f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006300: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
+00006310: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
+00006320: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
+00006330: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2066 6f72 206c 6561 6620 696e 2072 6f6f   for leaf in roo
+00006360: 745f 6c65 6166 3a0d 0a20 2020 2020 2020  t_leaf:..       
+00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006380: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+00006390: 6365 5f6c 6561 6620 3d20 7365 6c66 2e65  ce_leaf = self.e
+000063a0: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
+000063b0: 705b 6c65 6166 5d0d 0a20 2020 2020 2020  p[leaf]..       
 000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063e0: 2020 2020 2020 7461 7267 6574 5f69 6473        target_ids
-000063f0: 203d 2073 656c 662e 6564 6765 5f74 6172   = self.edge_tar
-00006400: 6765 745f 6c6f 6f6b 7570 5b73 6f75 7263  get_lookup[sourc
-00006410: 655f 6964 5d0d 0a20 2020 2020 2020 2020  e_id]..         
-00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006430: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006440: 7572 7265 6e74 5f63 656c 6c5f 6964 732e  urrent_cell_ids.
-00006450: 6170 7065 6e64 2873 6f75 7263 655f 6964  append(source_id
-00006460: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000063d0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000063e0: 656e 745f 6365 6c6c 5f69 6473 2e61 7070  ent_cell_ids.app
+000063f0: 656e 6428 6c65 6166 2920 0d0a 2020 2020  end(leaf) ..    
+00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006420: 656c 662e 5f64 6963 745f 7570 6461 7465  elf._dict_update
+00006430: 2875 6e69 7175 655f 7472 6163 6b6c 6574  (unique_tracklet
+00006440: 5f69 6473 2c20 6c65 6166 2c20 7472 6163  _ids, leaf, trac
+00006450: 6b5f 6964 2c20 736f 7572 6365 5f6c 6561  k_id, source_lea
+00006460: 662c 204e 6f6e 6529 0d0a 2020 2020 2020  f, None)..      
 00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006480: 2020 2020 2020 2020 2020 2023 526f 6f74             #Root
-00006490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000064c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000064d0: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
-000064e0: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
-000064f0: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
-00006500: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-00006510: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006540: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00006550: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
-00006560: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
-00006570: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
-00006580: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
-00006590: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
+00006480: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006490: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000064a0: 6f70 6572 7469 6573 5b6c 6561 665d 2e75  operties[leaf].u
+000064b0: 7064 6174 6528 7b73 656c 662e 6469 7669  pdate({self.divi
+000064c0: 6469 6e67 5f6b 6579 203a 2064 6976 6964  ding_key : divid
+000064d0: 696e 675f 7472 616a 6563 746f 7279 7d29  ing_trajectory})
+000064e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006500: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00006510: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00006520: 5b6c 6561 665d 2e75 7064 6174 6528 7b73  [leaf].update({s
+00006530: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
+00006540: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
+00006550: 5f64 6976 6964 696e 677d 290d 0a0d 0a20  _dividing}).... 
+00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006570: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
+00006580: 6f75 7263 655f 6964 2069 6e20 616c 6c5f  ource_id in all_
+00006590: 736f 7572 6365 5f69 6473 3a0d 0a20 2020  source_ids:..   
 000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065c0: 2069 6620 736f 7572 6365 5f69 6420 6e6f   if source_id no
-000065d0: 7420 696e 2061 6c6c 5f74 6172 6765 745f  t in all_target_
-000065e0: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065c0: 2020 2020 2074 6172 6765 745f 6964 7320       target_ids 
+000065d0: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
+000065e0: 6574 5f6c 6f6f 6b75 705b 736f 7572 6365  et_lookup[source
+000065f0: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
 00006600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006610: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006640: 2020 2020 2020 2020 666f 7220 7461 7267          for targ
-00006650: 6574 5f69 6420 696e 2074 6172 6765 745f  et_id in target_
-00006660: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006610: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00006620: 7272 656e 745f 6365 6c6c 5f69 6473 2e61  rrent_cell_ids.a
+00006630: 7070 656e 6428 736f 7572 6365 5f69 6429  ppend(source_id)
+00006640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006660: 2020 2020 2020 2020 2020 2352 6f6f 740d            #Root.
+00006670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
-000066a0: 6963 745f 7570 6461 7465 2875 6e69 7175  ict_update(uniqu
-000066b0: 655f 7472 6163 6b6c 6574 5f69 6473 2c20  e_tracklet_ids, 
-000066c0: 736f 7572 6365 5f69 642c 2074 7261 636b  source_id, track
-000066d0: 5f69 642c 204e 6f6e 652c 2074 6172 6765  _id, None, targe
-000066e0: 745f 6964 290d 0a20 2020 2020 2020 2020  t_id)..         
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006690: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000066a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000066b0: 7469 6573 5b73 6f75 7263 655f 6964 5d2e  ties[source_id].
+000066c0: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
+000066d0: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
+000066e0: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
+000066f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006710: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00006720: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00006730: 7274 6965 735b 7461 7267 6574 5f69 645d  rties[target_id]
-00006740: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
-00006750: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
-00006760: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-00006770: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00006710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006720: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00006730: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
+00006740: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
+00006750: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
+00006760: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
+00006770: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
 00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067a0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-000067b0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000067c0: 6573 5b74 6172 6765 745f 6964 5d2e 7570  es[target_id].up
-000067d0: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
-000067e0: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
-000067f0: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
-00006800: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+000067a0: 6966 2073 6f75 7263 655f 6964 206e 6f74  if source_id not
+000067b0: 2069 6e20 616c 6c5f 7461 7267 6574 5f69   in all_target_i
+000067c0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006820: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00006830: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006820: 2020 2020 2020 2066 6f72 2074 6172 6765         for targe
+00006830: 745f 6964 2069 6e20 7461 7267 6574 5f69  t_id in target_i
+00006840: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
 00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2023 4e6f 726d 616c 2020 2020 2020 2020   #Normal        
-00006870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 736f 7572 6365 5f73 6f75 7263 655f 6964  source_source_id
-000068b0: 203d 2073 656c 662e 6564 6765 5f73 6f75   = self.edge_sou
-000068c0: 7263 655f 6c6f 6f6b 7570 5b73 6f75 7263  rce_lookup[sourc
-000068d0: 655f 6964 5d0d 0a20 2020 2020 2020 2020  e_id]..         
+00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006870: 2020 2020 2020 2020 7365 6c66 2e5f 6469          self._di
+00006880: 6374 5f75 7064 6174 6528 756e 6971 7565  ct_update(unique
+00006890: 5f74 7261 636b 6c65 745f 6964 732c 2073  _tracklet_ids, s
+000068a0: 6f75 7263 655f 6964 2c20 7472 6163 6b5f  ource_id, track_
+000068b0: 6964 2c20 4e6f 6e65 2c20 7461 7267 6574  id, None, target
+000068c0: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
+000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006900: 2020 2020 2066 6f72 2074 6172 6765 745f       for target_
-00006910: 6964 2069 6e20 7461 7267 6574 5f69 6473  id in target_ids
-00006920: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006950: 2020 2020 2020 2073 656c 662e 5f64 6963         self._dic
-00006960: 745f 7570 6461 7465 2875 6e69 7175 655f  t_update(unique_
-00006970: 7472 6163 6b6c 6574 5f69 6473 2c20 736f  tracklet_ids, so
-00006980: 7572 6365 5f69 642c 2074 7261 636b 5f69  urce_id, track_i
-00006990: 642c 2073 6f75 7263 655f 736f 7572 6365  d, source_source
-000069a0: 5f69 642c 2074 6172 6765 745f 6964 2920  _id, target_id) 
-000069b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000069f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00006a00: 735b 7461 7267 6574 5f69 645d 2e75 7064  s[target_id].upd
-00006a10: 6174 6528 7b73 656c 662e 6469 7669 6469  ate({self.dividi
-00006a20: 6e67 5f6b 6579 203a 2064 6976 6964 696e  ng_key : dividin
-00006a30: 675f 7472 616a 6563 746f 7279 7d29 200d  g_trajectory}) .
-00006a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068f0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00006900: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00006910: 7469 6573 5b74 6172 6765 745f 6964 5d2e  ties[target_id].
+00006920: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
+00006930: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
+00006940: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
+00006950: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006980: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00006990: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000069a0: 735b 7461 7267 6574 5f69 645d 2e75 7064  s[target_id].upd
+000069b0: 6174 6528 7b73 656c 662e 6e75 6d62 6572  ate({self.number
+000069c0: 5f64 6976 6964 696e 675f 6b65 7920 3a20  _dividing_key : 
+000069d0: 6e75 6d62 6572 5f64 6976 6964 696e 677d  number_dividing}
+000069e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00006a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a40: 234e 6f72 6d61 6c20 2020 2020 2020 200d  #Normal        .
+00006a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a70: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00006a80: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00006a90: 5b74 6172 6765 745f 6964 5d2e 7570 6461  [target_id].upda
-00006aa0: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
-00006ab0: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
-00006ac0: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
-00006ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006a80: 6f75 7263 655f 736f 7572 6365 5f69 6420  ource_source_id 
+00006a90: 3d20 7365 6c66 2e65 6467 655f 736f 7572  = self.edge_sour
+00006aa0: 6365 5f6c 6f6f 6b75 705b 736f 7572 6365  ce_lookup[source
+00006ab0: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
+00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ae0: 2020 2020 666f 7220 7461 7267 6574 5f69      for target_i
+00006af0: 6420 696e 2074 6172 6765 745f 6964 733a  d in target_ids:
+00006b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b20: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b40: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2020 2020 2066 6f72 2063 7572 7265 6e74       for current
-00006b70: 5f72 6f6f 7420 696e 2072 6f6f 745f 726f  _root in root_ro
-00006b80: 6f74 3a0d 0a20 2020 2020 2020 2020 2020  ot:..           
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 2020 2020 2020 2020 7365 6c66 2e72 6f6f          self.roo
-00006bb0: 745f 7370 6f74 735b 696e 7428 6375 7272  t_spots[int(curr
-00006bc0: 656e 745f 726f 6f74 295d 203d 2073 656c  ent_root)] = sel
-00006bd0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00006be0: 6f70 6572 7469 6573 5b69 6e74 2863 7572  operties[int(cur
-00006bf0: 7265 6e74 5f72 6f6f 7429 5d0d 0a20 2020  rent_root)]..   
-00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c10: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b30: 2020 2020 2020 7365 6c66 2e5f 6469 6374        self._dict
+00006b40: 5f75 7064 6174 6528 756e 6971 7565 5f74  _update(unique_t
+00006b50: 7261 636b 6c65 745f 6964 732c 2073 6f75  racklet_ids, sou
+00006b60: 7263 655f 6964 2c20 7472 6163 6b5f 6964  rce_id, track_id
+00006b70: 2c20 736f 7572 6365 5f73 6f75 7263 655f  , source_source_
+00006b80: 6964 2c20 7461 7267 6574 5f69 6429 200d  id, target_id) .
+00006b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bc0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00006bd0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00006be0: 5b74 6172 6765 745f 6964 5d2e 7570 6461  [target_id].upda
+00006bf0: 7465 287b 7365 6c66 2e64 6976 6964 696e  te({self.dividin
+00006c00: 675f 6b65 7920 3a20 6469 7669 6469 6e67  g_key : dividing
+00006c10: 5f74 7261 6a65 6374 6f72 797d 2920 0d0a  _trajectory}) ..
 00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c30: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00006c40: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-00006c50: 5b69 6e74 2874 7261 636b 5f69 6429 5d20  [int(track_id)] 
-00006c60: 3d20 6375 7272 656e 745f 6365 6c6c 5f69  = current_cell_i
-00006c70: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
-00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c90: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00006ca0: 656e 2863 7572 7265 6e74 5f63 656c 6c5f  en(current_cell_
-00006cb0: 6964 7329 293a 0d0a 2020 2020 2020 2020  ids)):..        
+00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c50: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00006c60: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00006c70: 7461 7267 6574 5f69 645d 2e75 7064 6174  target_id].updat
+00006c80: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
+00006c90: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
+00006ca0: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
+00006cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006cd0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d00: 2020 2020 2020 6b20 3d20 696e 7428 6375        k = int(cu
-00006d10: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
-00006d20: 5d29 2020 2020 0d0a 2020 2020 2020 2020  ])    ..        
+00006d00: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d20: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00006d50: 6469 6374 5f76 616c 7565 7320 3d20 7365  dict_values = se
-00006d60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00006d70: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
-00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006da0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dc0: 2020 2020 2020 2074 203d 2069 6e74 2866         t = int(f
-00006dd0: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00006de0: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
-00006df0: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
+00006d40: 2020 2020 666f 7220 6375 7272 656e 745f      for current_
+00006d50: 726f 6f74 2069 6e20 726f 6f74 5f72 6f6f  root in root_roo
+00006d60: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d80: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
+00006d90: 5f73 706f 7473 5b69 6e74 2863 7572 7265  _spots[int(curre
+00006da0: 6e74 5f72 6f6f 7429 5d20 3d20 7365 6c66  nt_root)] = self
+00006db0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00006dc0: 7065 7274 6965 735b 696e 7428 6375 7272  perties[int(curr
+00006dd0: 656e 745f 726f 6f74 295d 0d0a 2020 2020  ent_root)]..    
+00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006df0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e10: 2020 2020 2020 2020 2020 2020 2020 7a20                z 
-00006e20: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00006e30: 5f76 616c 7565 735b 7365 6c66 2e7a 706f  _values[self.zpo
-00006e40: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00006e70: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00006e80: 745f 7661 6c75 6573 5b73 656c 662e 7970  t_values[self.yp
-00006e90: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00006e10: 2020 2020 2020 7365 6c66 2e61 6c6c 5f63        self.all_c
+00006e20: 7572 7265 6e74 5f63 656c 6c5f 6964 735b  urrent_cell_ids[
+00006e30: 696e 7428 7472 6163 6b5f 6964 295d 203d  int(track_id)] =
+00006e40: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
+00006e50: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00006e60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00006e70: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00006e80: 6e28 6375 7272 656e 745f 6365 6c6c 5f69  n(current_cell_i
+00006e90: 6473 2929 3a0d 0a20 2020 2020 2020 2020  ds)):..         
 00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ec0: 7820 3d20 666c 6f61 7428 616c 6c5f 6469  x = float(all_di
-00006ed0: 6374 5f76 616c 7565 735b 7365 6c66 2e78  ct_values[self.x
-00006ee0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f10: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f30: 2020 2020 2020 2020 2020 2020 2020 7370                sp
-00006f40: 6f74 5f63 656e 7472 6f69 6420 3d20 2872  ot_centroid = (r
-00006f50: 6f75 6e64 287a 292f 7365 6c66 2e7a 6361  ound(z)/self.zca
-00006f60: 6c69 6272 6174 696f 6e2c 2072 6f75 6e64  libration, round
-00006f70: 2879 292f 7365 6c66 2e79 6361 6c69 6272  (y)/self.ycalibr
-00006f80: 6174 696f 6e2c 2072 6f75 6e64 2878 292f  ation, round(x)/
-00006f90: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00006fa0: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 2020 2020 2020 6672 616d 655f 7370          frame_sp
-00006fd0: 6f74 5f63 656e 7472 6f69 6420 3d20 2874  ot_centroid = (t
-00006fe0: 2c72 6f75 6e64 287a 292f 7365 6c66 2e7a  ,round(z)/self.z
-00006ff0: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-00007000: 6e64 2879 292f 7365 6c66 2e79 6361 6c69  nd(y)/self.ycali
-00007010: 6272 6174 696f 6e2c 2072 6f75 6e64 2878  bration, round(x
-00007020: 292f 7365 6c66 2e78 6361 6c69 6272 6174  )/self.xcalibrat
-00007030: 696f 6e29 0d0a 0d0a 2020 2020 2020 2020  ion)....        
-00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007050: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007060: 2e75 6e69 7175 655f 7370 6f74 5f63 656e  .unique_spot_cen
-00007070: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
-00007080: 5f63 656e 7472 6f69 645d 203d 206b 0d0a  _centroid] = k..
-00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000070c0: 7472 6163 6b5f 6365 6e74 726f 6964 5b66  track_centroid[f
-000070d0: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
-000070e0: 6964 5d20 3d20 7472 6163 6b5f 6964 0d0a  id] = track_id..
-000070f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00006ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ee0: 2020 2020 206b 203d 2069 6e74 2863 7572       k = int(cur
+00006ef0: 7265 6e74 5f63 656c 6c5f 6964 735b 695d  rent_cell_ids[i]
+00006f00: 2920 2020 200d 0a20 2020 2020 2020 2020  )    ..         
+00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f20: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00006f30: 6963 745f 7661 6c75 6573 203d 2073 656c  ict_values = sel
+00006f40: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00006f50: 6f70 6572 7469 6573 5b6b 5d0d 0a20 2020  operties[k]..   
+00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
+00006fb0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+00006fc0: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
+00006fd0: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
+00006fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ff0: 2020 2020 2020 2020 2020 2020 207a 203d               z =
+00007000: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+00007010: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
+00007020: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007040: 2020 2020 2020 2020 2020 2020 2020 7920                y 
+00007050: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+00007060: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
+00007070: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007090: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+000070a0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+000070b0: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
+000070c0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
 00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 2020 2020 6966 2073 7472 2874 2920        if str(t) 
-00007120: 696e 2073 656c 662e 5f74 696d 6564 5f63  in self._timed_c
-00007130: 656e 7472 6f69 643a 0d0a 2020 2020 2020  entroid:..      
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007160: 2020 2020 2074 7265 652c 2073 706f 745f       tree, spot_
-00007170: 6365 6e74 726f 6964 7320 3d20 7365 6c66  centroids = self
-00007180: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
-00007190: 5b73 7472 2874 295d 0d0a 2020 2020 2020  [str(t)]..      
-000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071c0: 2020 2020 2073 706f 745f 6365 6e74 726f       spot_centro
-000071d0: 6964 732e 6170 7065 6e64 2873 706f 745f  ids.append(spot_
-000071e0: 6365 6e74 726f 6964 290d 0a20 2020 2020  centroid)..     
-000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007210: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-00007220: 7469 616c 2e63 4b44 5472 6565 2873 706f  tial.cKDTree(spo
-00007230: 745f 6365 6e74 726f 6964 7329 0d0a 2020  t_centroids)..  
-00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-00007270: 696d 6564 5f63 656e 7472 6f69 645b 7374  imed_centroid[st
-00007280: 7228 7429 5d20 3d20 7472 6565 2c20 7370  r(t)] = tree, sp
-00007290: 6f74 5f63 656e 7472 6f69 6473 200d 0a20  ot_centroids .. 
-000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072c0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007110: 2020 2020 2020 2020 2020 2020 2073 706f               spo
+00007120: 745f 6365 6e74 726f 6964 203d 2028 726f  t_centroid = (ro
+00007130: 756e 6428 7a29 2f73 656c 662e 7a63 616c  und(z)/self.zcal
+00007140: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
+00007150: 7929 2f73 656c 662e 7963 616c 6962 7261  y)/self.ycalibra
+00007160: 7469 6f6e 2c20 726f 756e 6428 7829 2f73  tion, round(x)/s
+00007170: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00007180: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071a0: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
+000071b0: 745f 6365 6e74 726f 6964 203d 2028 742c  t_centroid = (t,
+000071c0: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
+000071d0: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
+000071e0: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
+000071f0: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
+00007200: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
+00007210: 6f6e 290d 0a0d 0a20 2020 2020 2020 2020  on)....         
+00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007230: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007240: 756e 6971 7565 5f73 706f 745f 6365 6e74  unique_spot_cent
+00007250: 726f 6964 5b66 7261 6d65 5f73 706f 745f  roid[frame_spot_
+00007260: 6365 6e74 726f 6964 5d20 3d20 6b0d 0a20  centroid] = k.. 
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007290: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
+000072a0: 7261 636b 5f63 656e 7472 6f69 645b 6672  rack_centroid[fr
+000072b0: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+000072c0: 645d 203d 2074 7261 636b 5f69 640d 0a0d  d] = track_id...
+000072d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000072e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072f0: 2020 2020 2073 706f 745f 6365 6e74 726f       spot_centro
-00007300: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072f0: 2020 2020 2069 6620 7374 7228 7429 2069       if str(t) i
+00007300: 6e20 7365 6c66 2e5f 7469 6d65 645f 6365  n self._timed_ce
+00007310: 6e74 726f 6964 3a0d 0a20 2020 2020 2020  ntroid:..       
 00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007330: 2020 2020 2073 706f 745f 6365 6e74 726f       spot_centro
-00007340: 6964 732e 6170 7065 6e64 2873 706f 745f  ids.append(spot_
-00007350: 6365 6e74 726f 6964 290d 0a20 2020 2020  centroid)..     
-00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-00007390: 7469 616c 2e63 4b44 5472 6565 2873 706f  tial.cKDTree(spo
-000073a0: 745f 6365 6e74 726f 6964 7329 0d0a 2020  t_centroids)..  
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073d0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-000073e0: 696d 6564 5f63 656e 7472 6f69 645b 7374  imed_centroid[st
-000073f0: 7228 7429 5d20 3d20 7472 6565 2c20 7370  r(t)] = tree, sp
-00007400: 6f74 5f63 656e 7472 6f69 6473 0d0a 2020  ot_centroids..  
-00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007420: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00007430: 2020 6465 6620 5f6d 6173 7465 725f 7472    def _master_tr
-00007440: 6163 6b5f 636f 6d70 7574 6572 2873 656c  ack_computer(sel
-00007450: 662c 2074 7261 636b 2c20 7472 6163 6b5f  f, track, track_
-00007460: 6964 293a 0d0a 2020 2020 2020 2020 2020  id):..          
-00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007480: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007340: 2020 2020 7472 6565 2c20 7370 6f74 5f63      tree, spot_c
+00007350: 656e 7472 6f69 6473 203d 2073 656c 662e  entroids = self.
+00007360: 5f74 696d 6564 5f63 656e 7472 6f69 645b  _timed_centroid[
+00007370: 7374 7228 7429 5d0d 0a20 2020 2020 2020  str(t)]..       
+00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073a0: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
+000073b0: 6473 2e61 7070 656e 6428 7370 6f74 5f63  ds.append(spot_c
+000073c0: 656e 7472 6f69 6429 0d0a 2020 2020 2020  entroid)..      
+000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073f0: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
+00007400: 6961 6c2e 634b 4454 7265 6528 7370 6f74  ial.cKDTree(spot
+00007410: 5f63 656e 7472 6f69 6473 290d 0a20 2020  _centroids)..   
+00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007440: 2020 2020 2020 2020 7365 6c66 2e5f 7469          self._ti
+00007450: 6d65 645f 6365 6e74 726f 6964 5b73 7472  med_centroid[str
+00007460: 2874 295d 203d 2074 7265 652c 2073 706f  (t)] = tree, spo
+00007470: 745f 6365 6e74 726f 6964 7320 0d0a 2020  t_centroids ..  
+00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000074b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000074c0: 7572 7265 6e74 5f63 656c 6c5f 6964 7320  urrent_cell_ids 
-000074d0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00007500: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00007510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007520: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00007530: 5f73 6f75 7263 655f 6964 732c 2061 6c6c  _source_ids, all
-00007540: 5f74 6172 6765 745f 6964 7320 3d20 2073  _target_ids =  s
-00007550: 656c 662e 5f67 656e 6572 6174 655f 6765  elf._generate_ge
-00007560: 6e65 7261 7469 6f6e 7328 7472 6163 6b29  nerations(track)
-00007570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007580: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00007590: 6f74 5f72 6f6f 742c 2072 6f6f 745f 7370  ot_root, root_sp
-000075a0: 6c69 7473 2c20 726f 6f74 5f6c 6561 6620  lits, root_leaf 
-000075b0: 3d20 7365 6c66 2e5f 6372 6561 7465 5f67  = self._create_g
-000075c0: 656e 6572 6174 696f 6e73 2861 6c6c 5f73  enerations(all_s
-000075d0: 6f75 7263 655f 6964 732c 2061 6c6c 5f74  ource_ids, all_t
-000075e0: 6172 6765 745f 6964 7329 200d 0a20 2020  arget_ids) ..   
+000074a0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074d0: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
+000074e0: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007510: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
+00007520: 6473 2e61 7070 656e 6428 7370 6f74 5f63  ds.append(spot_c
+00007530: 656e 7472 6f69 6429 0d0a 2020 2020 2020  entroid)..      
+00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007560: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
+00007570: 6961 6c2e 634b 4454 7265 6528 7370 6f74  ial.cKDTree(spot
+00007580: 5f63 656e 7472 6f69 6473 290d 0a20 2020  _centroids)..   
+00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075b0: 2020 2020 2020 2020 7365 6c66 2e5f 7469          self._ti
+000075c0: 6d65 645f 6365 6e74 726f 6964 5b73 7472  med_centroid[str
+000075d0: 2874 295d 203d 2074 7265 652c 2073 706f  (t)] = tree, spo
+000075e0: 745f 6365 6e74 726f 6964 730d 0a20 2020  t_centroids..   
 000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 2020 2020 2020 2020 2073 656c 662e 5f69           self._i
-00007610: 7465 7261 7465 5f73 706c 6974 5f64 6f77  terate_split_dow
-00007620: 6e28 726f 6f74 5f72 6f6f 742c 2072 6f6f  n(root_root, roo
-00007630: 745f 6c65 6166 2c20 726f 6f74 5f73 706c  t_leaf, root_spl
-00007640: 6974 7329 0d0a 2020 2020 2020 2020 2020  its)..          
+00007600: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00007610: 2064 6566 205f 6d61 7374 6572 5f74 7261   def _master_tra
+00007620: 636b 5f63 6f6d 7075 7465 7228 7365 6c66  ck_computer(self
+00007630: 2c20 7472 6163 6b2c 2074 7261 636b 5f69  , track, track_i
+00007640: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
 00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007660: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007680: 2320 4465 7465 726d 696e 6520 6966 2061  # Determine if a
-00007690: 2074 7261 636b 2068 6173 2064 6976 6973   track has divis
-000076a0: 696f 6e73 206f 7220 6e6f 6e65 0d0a 2020  ions or none..  
-000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076c0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-000076d0: 5f64 6976 6964 696e 6720 3d20 6c65 6e28  _dividing = len(
-000076e0: 726f 6f74 5f73 706c 6974 7329 0d0a 2020  root_splits)..  
+00007680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007690: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000076a0: 7272 656e 745f 6365 6c6c 5f69 6473 203d  rrent_cell_ids =
+000076b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000076e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00007710: 2872 6f6f 745f 7370 6c69 7473 2920 3e20  (root_splits) > 
-00007720: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00007750: 7472 6163 6b5f 6d69 746f 7369 735f 6c61  track_mitosis_la
-00007760: 6265 6c5b 7472 6163 6b5f 6964 5d20 3d20  bel[track_id] = 
-00007770: 5b31 2c20 6e75 6d62 6572 5f64 6976 6964  [1, number_divid
-00007780: 696e 675d 0d0a 2020 2020 2020 2020 2020  ing]..          
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 6469 7669 6469 6e67 5f74        dividing_t
-000077b0: 7261 6a65 6374 6f72 7920 3d20 5472 7565  rajectory = True
-000077c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007700: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00007710: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
+00007720: 7461 7267 6574 5f69 6473 203d 2020 7365  target_ids =  se
+00007730: 6c66 2e5f 6765 6e65 7261 7465 5f67 656e  lf._generate_gen
+00007740: 6572 6174 696f 6e73 2874 7261 636b 290d  erations(track).
+00007750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007760: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00007770: 745f 726f 6f74 2c20 726f 6f74 5f73 706c  t_root, root_spl
+00007780: 6974 732c 2072 6f6f 745f 6c65 6166 203d  its, root_leaf =
+00007790: 2073 656c 662e 5f63 7265 6174 655f 6765   self._create_ge
+000077a0: 6e65 7261 7469 6f6e 7328 616c 6c5f 736f  nerations(all_so
+000077b0: 7572 6365 5f69 6473 2c20 616c 6c5f 7461  urce_ids, all_ta
+000077c0: 7267 6574 5f69 6473 2920 0d0a 2020 2020  rget_ids) ..    
 000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077e0: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
-000077f0: 6429 206e 6f74 2069 6e20 7365 6c66 2e41  d) not in self.A
-00007800: 6c6c 5472 6163 6b49 6473 3a0d 0a20 2020  llTrackIds:..   
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-00007840: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
-00007850: 636b 5f69 6429 290d 0a20 2020 2020 2020  ck_id))..       
-00007860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007870: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
-00007880: 7472 6163 6b5f 6964 2920 6e6f 7420 696e  track_id) not in
-00007890: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-000078a0: 6163 6b49 6473 3a20 2020 2020 0d0a 2020  ackIds:     ..  
-000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078d0: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
-000078e0: 7261 636b 4964 732e 6170 7065 6e64 2869  rackIds.append(i
-000078f0: 6e74 2874 7261 636b 5f69 6429 290d 0a20  nt(track_id)).. 
-00007900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077e0: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
+000077f0: 6572 6174 655f 7370 6c69 745f 646f 776e  erate_split_down
+00007800: 2872 6f6f 745f 726f 6f74 2c20 726f 6f74  (root_root, root
+00007810: 5f6c 6561 662c 2072 6f6f 745f 7370 6c69  _leaf, root_spli
+00007820: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00007850: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00007860: 2044 6574 6572 6d69 6e65 2069 6620 6120   Determine if a 
+00007870: 7472 6163 6b20 6861 7320 6469 7669 7369  track has divisi
+00007880: 6f6e 7320 6f72 206e 6f6e 650d 0a20 2020  ons or none..   
+00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078a0: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+000078b0: 6469 7669 6469 6e67 203d 206c 656e 2872  dividing = len(r
+000078c0: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
+000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078e0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+000078f0: 726f 6f74 5f73 706c 6974 7329 203e 2030  root_splits) > 0
+00007900: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007970: 2e75 6e69 7175 655f 7472 6163 6b5f 6d69  .unique_track_mi
-00007980: 746f 7369 735f 6c61 6265 6c5b 7472 6163  tosis_label[trac
-00007990: 6b5f 6964 5d20 3d20 5b30 2c20 305d 0d0a  k_id] = [0, 0]..
-000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007920: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
+00007930: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
+00007940: 656c 5b74 7261 636b 5f69 645d 203d 205b  el[track_id] = [
+00007950: 312c 206e 756d 6265 725f 6469 7669 6469  1, number_dividi
+00007960: 6e67 5d0d 0a20 2020 2020 2020 2020 2020  ng]..           
+00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007980: 2020 2020 2064 6976 6964 696e 675f 7472       dividing_tr
+00007990: 616a 6563 746f 7279 203d 2054 7275 650d  ajectory = True.
+000079a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
-000079d0: 6f72 7920 3d20 4661 6c73 650d 0a20 2020  ory = False..   
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00007a00: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
-00007a10: 7420 696e 2073 656c 662e 416c 6c54 7261  t in self.AllTra
-00007a20: 636b 4964 733a 0d0a 2020 2020 2020 2020  ckIds:..        
-00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007a50: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
-00007a60: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
-00007a70: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2020 6966 2069 6e74 2874 7261 636b      if int(track
-00007aa0: 5f69 6429 206e 6f74 2069 6e20 7365 6c66  _id) not in self
-00007ab0: 2e4e 6f72 6d61 6c54 7261 636b 4964 733a  .NormalTrackIds:
-00007ac0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2020 2020 2020 2020 7365 6c66 2e4e            self.N
-00007af0: 6f72 6d61 6c54 7261 636b 4964 732e 6170  ormalTrackIds.ap
-00007b00: 7065 6e64 2869 6e74 2874 7261 636b 5f69  pend(int(track_i
-00007b10: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
-00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 2020 2066 6f72 206c 6561 6620 696e 2072     for leaf in r
-00007b40: 6f6f 745f 6c65 6166 3a0d 0a20 2020 2020  oot_leaf:..     
-00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007b70: 6c66 2e5f 7365 636f 6e64 5f63 6861 6e6e  lf._second_chann
-00007b80: 656c 5f75 7064 6174 6528 6c65 6166 2c20  el_update(leaf, 
-00007b90: 7472 6163 6b5f 6964 290d 0a20 2020 2020  track_id)..     
-00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bb0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00007bc0: 7272 656e 745f 6365 6c6c 5f69 6473 2e61  rrent_cell_ids.a
-00007bd0: 7070 656e 6428 6c65 6166 2920 0d0a 2020  ppend(leaf) ..  
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00007c10: 745f 7072 6f70 6572 7469 6573 5b6c 6561  t_properties[lea
-00007c20: 665d 2e75 7064 6174 6528 7b73 656c 662e  f].update({self.
-00007c30: 6469 7669 6469 6e67 5f6b 6579 203a 2064  dividing_key : d
-00007c40: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
-00007c50: 7279 7d29 0d0a 2020 2020 2020 2020 2020  ry})..          
+000079c0: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
+000079d0: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
+000079e0: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
+000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
+00007a20: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+00007a30: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
+00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a50: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
+00007a60: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
+00007a70: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
+00007a80: 636b 4964 733a 2020 2020 200d 0a20 2020  ckIds:     ..   
+00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ab0: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
+00007ac0: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
+00007ad0: 7428 7472 6163 6b5f 6964 2929 0d0a 2020  t(track_id))..  
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b20: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007b50: 756e 6971 7565 5f74 7261 636b 5f6d 6974  unique_track_mit
+00007b60: 6f73 6973 5f6c 6162 656c 5b74 7261 636b  osis_label[track
+00007b70: 5f69 645d 203d 205b 302c 2030 5d0d 0a20  _id] = [0, 0].. 
+00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00007ba0: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
+00007bb0: 7279 203d 2046 616c 7365 0d0a 2020 2020  ry = False..    
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00007be0: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
+00007bf0: 2069 6e20 7365 6c66 2e41 6c6c 5472 6163   in self.AllTrac
+00007c00: 6b49 6473 3a0d 0a20 2020 2020 2020 2020  kIds:..         
+00007c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007c30: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
+00007c40: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
+00007c50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00007c80: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00007c90: 7469 6573 5b6c 6561 665d 2e75 7064 6174  ties[leaf].updat
-00007ca0: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
-00007cb0: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
-00007cc0: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
-00007cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007ce0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00007cf0: 2073 6f75 7263 655f 6964 2069 6e20 616c   source_id in al
-00007d00: 6c5f 736f 7572 6365 5f69 6473 3a0d 0a20  l_source_ids:.. 
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
-00007d40: 6861 6e6e 656c 5f75 7064 6174 6528 736f  hannel_update(so
-00007d50: 7572 6365 5f69 642c 2074 7261 636b 5f69  urce_id, track_i
-00007d60: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d80: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00007d90: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00007da0: 6573 5b73 6f75 7263 655f 6964 5d2e 7570  es[source_id].up
-00007db0: 6461 7465 287b 7365 6c66 2e64 6976 6964  date({self.divid
-00007dc0: 696e 675f 6b65 7920 3a20 6469 7669 6469  ing_key : dividi
-00007dd0: 6e67 5f74 7261 6a65 6374 6f72 797d 290d  ng_trajectory}).
-00007de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e00: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00007e10: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00007e20: 736f 7572 6365 5f69 645d 2e75 7064 6174  source_id].updat
-00007e30: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
-00007e40: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
-00007e50: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
-00007e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e80: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
-00007e90: 5f69 6473 2e61 7070 656e 6428 736f 7572  _ids.append(sour
-00007ea0: 6365 5f69 6429 0d0a 2020 2020 2020 2020  ce_id)..        
+00007c70: 2020 2069 6620 696e 7428 7472 6163 6b5f     if int(track_
+00007c80: 6964 2920 6e6f 7420 696e 2073 656c 662e  id) not in self.
+00007c90: 4e6f 726d 616c 5472 6163 6b49 6473 3a20  NormalTrackIds: 
+00007ca0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cc0: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
+00007cd0: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
+00007ce0: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
+00007cf0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d10: 2020 666f 7220 6c65 6166 2069 6e20 726f    for leaf in ro
+00007d20: 6f74 5f6c 6561 663a 0d0a 2020 2020 2020  ot_leaf:..      
+00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007d50: 662e 5f73 6563 6f6e 645f 6368 616e 6e65  f._second_channe
+00007d60: 6c5f 7570 6461 7465 286c 6561 662c 2074  l_update(leaf, t
+00007d70: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
+00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d90: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00007da0: 7265 6e74 5f63 656c 6c5f 6964 732e 6170  rent_cell_ids.ap
+00007db0: 7065 6e64 286c 6561 6629 200d 0a20 2020  pend(leaf) ..   
+00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007de0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00007df0: 5f70 726f 7065 7274 6965 735b 6c65 6166  _properties[leaf
+00007e00: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
+00007e10: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
+00007e20: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
+00007e30: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
+00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e50: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00007e60: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00007e70: 6965 735b 6c65 6166 5d2e 7570 6461 7465  ies[leaf].update
+00007e80: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
+00007e90: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
+00007ea0: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
 00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ed0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ef0: 2020 2020 2020 2020 666f 7220 6375 7272          for curr
-00007f00: 656e 745f 726f 6f74 2069 6e20 726f 6f74  ent_root in root
-00007f10: 5f72 6f6f 743a 0d0a 2020 2020 2020 2020  _root:..        
-00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007f40: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
-00007f50: 7570 6461 7465 2863 7572 7265 6e74 5f72  update(current_r
-00007f60: 6f6f 742c 2074 7261 636b 5f69 6429 0d0a  oot, track_id)..
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f90: 2020 2073 656c 662e 726f 6f74 5f73 706f     self.root_spo
-00007fa0: 7473 5b69 6e74 2863 7572 7265 6e74 5f72  ts[int(current_r
-00007fb0: 6f6f 7429 5d20 3d20 7365 6c66 2e75 6e69  oot)] = self.uni
-00007fc0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00007fd0: 6965 735b 696e 7428 6375 7272 656e 745f  ies[int(current_
-00007fe0: 726f 6f74 295d 0d0a 2020 2020 2020 2020  root)]..        
-00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008000: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008010: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00008020: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
-00008030: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
-00008040: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
-00008050: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-00008060: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
-00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008080: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00008090: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000080a0: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
-000080b0: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
-000080c0: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
-000080d0: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
-000080e0: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00008110: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008120: 656c 662e 616c 6c5f 6375 7272 656e 745f  elf.all_current_
-00008130: 6365 6c6c 5f69 6473 5b69 6e74 2874 7261  cell_ids[int(tra
-00008140: 636b 5f69 6429 5d20 3d20 6375 7272 656e  ck_id)] = curren
-00008150: 745f 6365 6c6c 5f69 6473 0d0a 2020 2020  t_cell_ids..    
+00007ec0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00007ed0: 736f 7572 6365 5f69 6420 696e 2061 6c6c  source_id in all
+00007ee0: 5f73 6f75 7263 655f 6964 733a 0d0a 2020  _source_ids:..  
+00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
+00007f20: 616e 6e65 6c5f 7570 6461 7465 2873 6f75  annel_update(sou
+00007f30: 7263 655f 6964 2c20 7472 6163 6b5f 6964  rce_id, track_id
+00007f40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f60: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00007f70: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00007f80: 735b 736f 7572 6365 5f69 645d 2e75 7064  s[source_id].upd
+00007f90: 6174 6528 7b73 656c 662e 6469 7669 6469  ate({self.dividi
+00007fa0: 6e67 5f6b 6579 203a 2064 6976 6964 696e  ng_key : dividin
+00007fb0: 675f 7472 616a 6563 746f 7279 7d29 0d0a  g_trajectory})..
+00007fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fe0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00007ff0: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
+00008000: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
+00008010: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
+00008020: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
+00008030: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
+00008040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008060: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+00008070: 6964 732e 6170 7065 6e64 2873 6f75 7263  ids.append(sourc
+00008080: 655f 6964 290d 0a20 2020 2020 2020 2020  e_id)..         
+00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080b0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080d0: 2020 2020 2020 2066 6f72 2063 7572 7265         for curre
+000080e0: 6e74 5f72 6f6f 7420 696e 2072 6f6f 745f  nt_root in root_
+000080f0: 726f 6f74 3a0d 0a20 2020 2020 2020 2020  root:..         
+00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008110: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00008120: 7365 636f 6e64 5f63 6861 6e6e 656c 5f75  second_channel_u
+00008130: 7064 6174 6528 6375 7272 656e 745f 726f  pdate(current_ro
+00008140: 6f74 2c20 7472 6163 6b5f 6964 290d 0a20  ot, track_id).. 
+00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008170: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008190: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-000081a0: 6e67 6528 6c65 6e28 6375 7272 656e 745f  nge(len(current_
-000081b0: 6365 6c6c 5f69 6473 2929 3a0d 0a20 2020  cell_ids)):..   
-000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 7365 6c66 2e72 6f6f 745f 7370 6f74    self.root_spot
+00008180: 735b 696e 7428 6375 7272 656e 745f 726f  s[int(current_ro
+00008190: 6f74 295d 203d 2073 656c 662e 756e 6971  ot)] = self.uniq
+000081a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000081b0: 6573 5b69 6e74 2863 7572 7265 6e74 5f72  es[int(current_r
+000081c0: 6f6f 7429 5d0d 0a20 2020 2020 2020 2020  oot)]..         
 000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008200: 2020 2020 2020 2020 2020 206b 203d 2069             k = i
-00008210: 6e74 2863 7572 7265 6e74 5f63 656c 6c5f  nt(current_cell_
-00008220: 6964 735b 695d 2920 2020 0d0a 2020 2020  ids[i])   ..    
-00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008270: 2020 2020 2020 616c 6c5f 6469 6374 5f76        all_dict_v
-00008280: 616c 7565 7320 3d20 7365 6c66 2e75 6e69  alues = self.uni
-00008290: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000082a0: 6965 735b 6b5d 0d0a 2020 2020 2020 2020  ies[k]..        
-000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000081e0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+000081f0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00008200: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
+00008210: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
+00008220: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
+00008230: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
+00008240: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008260: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00008270: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00008280: 6573 5b73 6f75 7263 655f 6964 5d2e 7570  es[source_id].up
+00008290: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
+000082a0: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
+000082b0: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
+000082c0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
 000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008310: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
-00008320: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00008330: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
-00008340: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
-00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008360: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-00008370: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00008380: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
-00008390: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+000082e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000082f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008300: 6c66 2e61 6c6c 5f63 7572 7265 6e74 5f63  lf.all_current_c
+00008310: 656c 6c5f 6964 735b 696e 7428 7472 6163  ell_ids[int(trac
+00008320: 6b5f 6964 295d 203d 2063 7572 7265 6e74  k_id)] = current
+00008330: 5f63 656c 6c5f 6964 730d 0a20 2020 2020  _cell_ids..     
+00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008350: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008370: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00008380: 6765 286c 656e 2863 7572 7265 6e74 5f63  ge(len(current_c
+00008390: 656c 6c5f 6964 7329 293a 0d0a 2020 2020  ell_ids)):..    
 000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-000083c0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-000083d0: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
-000083e0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008400: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00008410: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00008420: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
-00008430: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+000083b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
+000083f0: 7428 6375 7272 656e 745f 6365 6c6c 5f69  t(current_cell_i
+00008400: 6473 5b69 5d29 2020 200d 0a20 2020 2020  ds[i])   ..     
+00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008420: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00008430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008460: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 2020 2020 2020 2020 6672 616d 655f 7370          frame_sp
-00008490: 6f74 5f63 656e 7472 6f69 6420 3d20 2874  ot_centroid = (t
-000084a0: 2c72 6f75 6e64 287a 292f 7365 6c66 2e7a  ,round(z)/self.z
-000084b0: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-000084c0: 6e64 2879 292f 7365 6c66 2e79 6361 6c69  nd(y)/self.ycali
-000084d0: 6272 6174 696f 6e2c 2072 6f75 6e64 2878  bration, round(x
-000084e0: 292f 7365 6c66 2e78 6361 6c69 6272 6174  )/self.xcalibrat
-000084f0: 696f 6e29 200d 0a0d 0a20 2020 2020 2020  ion) ....       
-00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008510: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008520: 662e 756e 6971 7565 5f73 706f 745f 6365  f.unique_spot_ce
-00008530: 6e74 726f 6964 5b66 7261 6d65 5f73 706f  ntroid[frame_spo
-00008540: 745f 6365 6e74 726f 6964 5d20 3d20 6b0d  t_centroid] = k.
-00008550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008570: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00008580: 5f74 7261 636b 5f63 656e 7472 6f69 645b  _track_centroid[
-00008590: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-000085a0: 6f69 645d 203d 2074 7261 636b 5f69 640d  oid] = track_id.
-000085b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2020 2020 0d0a 2020 2020 6465 6620 5f73      ..    def _s
-000085e0: 6563 6f6e 645f 6368 616e 6e65 6c5f 7570  econd_channel_up
-000085f0: 6461 7465 2873 656c 662c 2063 656c 6c5f  date(self, cell_
-00008600: 6964 2c20 7472 6163 6b5f 6964 293a 0d0a  id, track_id):..
-00008610: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00008620: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00008630: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
-00008640: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-00008650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008660: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00008670: 2020 2020 6672 616d 6520 3d20 7365 6c66      frame = self
-00008680: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00008690: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000086a0: 5f69 6429 5d5b 7365 6c66 2e66 7261 6d65  _id)][self.frame
-000086b0: 6964 5f6b 6579 5d0d 0a20 2020 2020 2020  id_key]..       
-000086c0: 2020 2020 2020 2020 207a 203d 2073 656c           z = sel
-000086d0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000086e0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-000086f0: 6c5f 6964 295d 5b73 656c 662e 7a70 6f73  l_id)][self.zpos
-00008700: 6964 5f6b 6579 5d2f 7365 6c66 2e7a 6361  id_key]/self.zca
-00008710: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00008720: 2020 2020 2020 2020 2020 2079 203d 2073             y = s
-00008730: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00008740: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00008750: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
-00008760: 6f73 6964 5f6b 6579 5d2f 7365 6c66 2e79  osid_key]/self.y
-00008770: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00008780: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-00008790: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000087a0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000087b0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-000087c0: 7870 6f73 6964 5f6b 6579 5d2f 7365 6c66  xposid_key]/self
-000087d0: 2e78 6361 6c69 6272 6174 696f 6e0d 0a20  .xcalibration.. 
-000087e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000087f0: 656c 662e 5f73 6563 6f6e 645f 6368 616e  elf._second_chan
-00008800: 6e65 6c5f 7370 6f74 7328 6672 616d 652c  nel_spots(frame,
-00008810: 207a 2c20 792c 2078 2c20 6365 6c6c 5f69   z, y, x, cell_i
-00008820: 642c 2074 7261 636b 5f69 6429 0d0a 2020  d, track_id)..  
-00008830: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-00008840: 5f66 696e 616c 5f74 7261 636b 7328 7365  _final_tracks(se
-00008850: 6c66 2c20 7472 6163 6b5f 6964 293a 0d0a  lf, track_id):..
-00008860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008870: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00008880: 7272 656e 745f 6365 6c6c 5f69 6473 203d  rrent_cell_ids =
-00008890: 2073 656c 662e 616c 6c5f 6375 7272 656e   self.all_curren
-000088a0: 745f 6365 6c6c 5f69 6473 5b69 6e74 2874  t_cell_ids[int(t
-000088b0: 7261 636b 5f69 6429 5d0d 0a20 2020 2020  rack_id)]..     
-000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088d0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-000088e0: 7261 636b 6c65 7473 203d 207b 7d0d 0a20  racklets = {}.. 
-000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008900: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00008910: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-00008920: 7065 7274 6965 7320 3d20 7b7d 0d0a 2020  perties = {}..  
-00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008940: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008960: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00008970: 2072 616e 6765 286c 656e 2863 7572 7265   range(len(curre
-00008980: 6e74 5f63 656c 6c5f 6964 7329 293a 0d0a  nt_cell_ids)):..
-00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089d0: 2020 2020 2020 2020 2020 2020 2020 6b20                k 
-000089e0: 3d20 696e 7428 6375 7272 656e 745f 6365  = int(current_ce
-000089f0: 6c6c 5f69 6473 5b69 5d29 2020 2020 0d0a  ll_ids[i])    ..
-00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 2020 2020 616c 6c5f 6469 6374 5f76 616c      all_dict_val
-00008a30: 7565 7320 3d20 7365 6c66 2e75 6e69 7175  ues = self.uniqu
-00008a40: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00008a50: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
-00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a70: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00008a80: 5f69 6420 3d20 7374 7228 616c 6c5f 6469  _id = str(all_di
-00008a90: 6374 5f76 616c 7565 735b 7365 6c66 2e75  ct_values[self.u
-00008aa0: 6e69 7175 6569 645f 6b65 795d 290d 0a20  niqueid_key]).. 
-00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-00008ae0: 5f69 6420 3d20 7374 7228 616c 6c5f 6469  _id = str(all_di
-00008af0: 6374 5f76 616c 7565 735b 7365 6c66 2e74  ct_values[self.t
-00008b00: 7261 636b 6964 5f6b 6579 5d29 0d0a 2020  rackid_key])..  
+00008450: 2020 2020 2061 6c6c 5f64 6963 745f 7661       all_dict_va
+00008460: 6c75 6573 203d 2073 656c 662e 756e 6971  lues = self.uniq
+00008470: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00008480: 6573 5b6b 5d0d 0a20 2020 2020 2020 2020  es[k]..         
+00008490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084c0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000084d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 2020 2074 203d 2069 6e74 2866 6c6f       t = int(flo
+00008500: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00008510: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
+00008520: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
+00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008540: 2020 2020 2020 2020 2020 2020 7a20 3d20              z = 
+00008550: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+00008560: 616c 7565 735b 7365 6c66 2e7a 706f 7369  alues[self.zposi
+00008570: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00008580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008590: 2020 2020 2020 2020 2020 2020 2079 203d               y =
+000085a0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+000085b0: 7661 6c75 6573 5b73 656c 662e 7970 6f73  values[self.ypos
+000085c0: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2020 2020 2020 2020 2020 2020 2020 7820                x 
+000085f0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+00008600: 5f76 616c 7565 735b 7365 6c66 2e78 706f  _values[self.xpo
+00008610: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008630: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00008640: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00008650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008660: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
+00008670: 745f 6365 6e74 726f 6964 203d 2028 742c  t_centroid = (t,
+00008680: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
+00008690: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
+000086a0: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
+000086b0: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
+000086c0: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
+000086d0: 6f6e 2920 0d0a 0d0a 2020 2020 2020 2020  on) ....        
+000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008700: 2e75 6e69 7175 655f 7370 6f74 5f63 656e  .unique_spot_cen
+00008710: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
+00008720: 5f63 656e 7472 6f69 645d 203d 206b 0d0a  _centroid] = k..
+00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00008760: 7472 6163 6b5f 6365 6e74 726f 6964 5b66  track_centroid[f
+00008770: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
+00008780: 6964 5d20 3d20 7472 6163 6b5f 6964 0d0a  id] = track_id..
+00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087b0: 2020 200d 0a20 2020 2064 6566 205f 7365     ..    def _se
+000087c0: 636f 6e64 5f63 6861 6e6e 656c 5f75 7064  cond_channel_upd
+000087d0: 6174 6528 7365 6c66 2c20 6365 6c6c 5f69  ate(self, cell_i
+000087e0: 642c 2074 7261 636b 5f69 6429 3a0d 0a20  d, track_id):.. 
+000087f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00008800: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00008810: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
+00008820: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
+00008830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008840: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00008850: 2020 2066 7261 6d65 203d 2073 656c 662e     frame = self.
+00008860: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00008870: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00008880: 6964 295d 5b73 656c 662e 6672 616d 6569  id)][self.framei
+00008890: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
+000088a0: 2020 2020 2020 2020 7a20 3d20 7365 6c66          z = self
+000088b0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000088c0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+000088d0: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
+000088e0: 645f 6b65 795d 2f73 656c 662e 7a63 616c  d_key]/self.zcal
+000088f0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00008900: 2020 2020 2020 2020 2020 7920 3d20 7365            y = se
+00008910: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00008920: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00008930: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
+00008940: 7369 645f 6b65 795d 2f73 656c 662e 7963  sid_key]/self.yc
+00008950: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00008960: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+00008970: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00008980: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00008990: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
+000089a0: 706f 7369 645f 6b65 795d 2f73 656c 662e  posid_key]/self.
+000089b0: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
+000089c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000089d0: 6c66 2e5f 7365 636f 6e64 5f63 6861 6e6e  lf._second_chann
+000089e0: 656c 5f73 706f 7473 2866 7261 6d65 2c20  el_spots(frame, 
+000089f0: 7a2c 2079 2c20 782c 2063 656c 6c5f 6964  z, y, x, cell_id
+00008a00: 2c20 7472 6163 6b5f 6964 290d 0a20 2020  , track_id)..   
+00008a10: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
+00008a20: 6669 6e61 6c5f 7472 6163 6b73 2873 656c  final_tracks(sel
+00008a30: 662c 2074 7261 636b 5f69 6429 3a0d 0a0d  f, track_id):...
+00008a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008a50: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00008a60: 7265 6e74 5f63 656c 6c5f 6964 7320 3d20  rent_cell_ids = 
+00008a70: 7365 6c66 2e61 6c6c 5f63 7572 7265 6e74  self.all_current
+00008a80: 5f63 656c 6c5f 6964 735b 696e 7428 7472  _cell_ids[int(tr
+00008a90: 6163 6b5f 6964 295d 0d0a 2020 2020 2020  ack_id)]..      
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ab0: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
+00008ac0: 6163 6b6c 6574 7320 3d20 7b7d 0d0a 2020  acklets = {}..  
+00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ae0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00008af0: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+00008b00: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
 00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b30: 2020 7420 3d20 696e 7428 666c 6f61 7428    t = int(float(
-00008b40: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00008b50: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00008b60: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
+00008b20: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b40: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00008b50: 7261 6e67 6528 6c65 6e28 6375 7272 656e  range(len(curren
+00008b60: 745f 6365 6c6c 5f69 6473 2929 3a0d 0a20  t_cell_ids)):.. 
 00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b80: 2020 2020 2020 2020 207a 203d 2066 6c6f           z = flo
-00008b90: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00008ba0: 6573 5b73 656c 662e 7a70 6f73 6964 5f6b  es[self.zposid_k
-00008bb0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bd0: 2020 2020 2020 2020 2020 7920 3d20 666c            y = fl
-00008be0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00008bf0: 7565 735b 7365 6c66 2e79 706f 7369 645f  ues[self.yposid_
-00008c00: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00008c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c20: 2020 2020 2020 2020 2020 2078 203d 2066             x = f
-00008c30: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00008c40: 6c75 6573 5b73 656c 662e 7870 6f73 6964  lues[self.xposid
-00008c50: 5f6b 6579 5d29 0d0a 0d0a 2020 2020 2020  _key])....      
-00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c70: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00008c80: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
-00008c90: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008ca0: 7473 5f70 726f 7065 7274 6965 7320 3d20  ts_properties = 
-00008cb0: 7365 6c66 2e5f 7472 6163 6b6c 6574 5f61  self._tracklet_a
-00008cc0: 6e64 5f70 726f 7065 7274 6965 7328 616c  nd_properties(al
-00008cd0: 6c5f 6469 6374 5f76 616c 7565 732c 2074  l_dict_values, t
-00008ce0: 2c20 7a2c 2079 2c20 782c 206b 2c20 6375  , z, y, x, k, cu
-00008cf0: 7272 656e 745f 7472 6163 6b5f 6964 2c20  rrent_track_id, 
-00008d00: 756e 6971 7565 5f69 642c 2063 7572 7265  unique_id, curre
-00008d10: 6e74 5f74 7261 636b 6c65 7473 2c20 6375  nt_tracklets, cu
-00008d20: 7272 656e 745f 7472 6163 6b6c 6574 735f  rrent_tracklets_
-00008d30: 7072 6f70 6572 7469 6573 290d 0a20 2020  properties)..   
-00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bb0: 2020 2020 2020 2020 2020 2020 206b 203d               k =
+00008bc0: 2069 6e74 2863 7572 7265 6e74 5f63 656c   int(current_cel
+00008bd0: 6c5f 6964 735b 695d 2920 2020 200d 0a20  l_ids[i])    .. 
+00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c00: 2020 2061 6c6c 5f64 6963 745f 7661 6c75     all_dict_valu
+00008c10: 6573 203d 2073 656c 662e 756e 6971 7565  es = self.unique
+00008c20: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00008c30: 5b6b 5d0d 0a20 2020 2020 2020 2020 2020  [k]..           
+00008c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c50: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
+00008c60: 6964 203d 2073 7472 2861 6c6c 5f64 6963  id = str(all_dic
+00008c70: 745f 7661 6c75 6573 5b73 656c 662e 756e  t_values[self.un
+00008c80: 6971 7565 6964 5f6b 6579 5d29 0d0a 2020  iqueid_key])..  
+00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cb0: 2020 6375 7272 656e 745f 7472 6163 6b5f    current_track_
+00008cc0: 6964 203d 2073 7472 2861 6c6c 5f64 6963  id = str(all_dic
+00008cd0: 745f 7661 6c75 6573 5b73 656c 662e 7472  t_values[self.tr
+00008ce0: 6163 6b69 645f 6b65 795d 290d 0a20 2020  ackid_key])..   
+00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d10: 2074 203d 2069 6e74 2866 6c6f 6174 2861   t = int(float(a
+00008d20: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+00008d30: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+00008d40: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
 00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d60: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d80: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008d90: 7473 203d 206e 702e 6173 6172 7261 7928  ts = np.asarray(
-00008da0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00008db0: 735b 7374 7228 7472 6163 6b5f 6964 295d  s[str(track_id)]
-00008dc0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00008dd0: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008df0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008e00: 7473 5f70 726f 7065 7274 6965 7320 3d20  ts_properties = 
-00008e10: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00008e20: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-00008e30: 7065 7274 6965 735b 7374 7228 7472 6163  perties[str(trac
-00008e40: 6b5f 6964 295d 2c20 6474 7970 653d 6e70  k_id)], dtype=np
-00008e50: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
-00008e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e90: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00008ea0: 5f74 7261 636b 735b 7472 6163 6b5f 6964  _tracks[track_id
-00008eb0: 5d20 3d20 6375 7272 656e 745f 7472 6163  ] = current_trac
-00008ec0: 6b6c 6574 7320 2020 2020 0d0a 2020 2020  klets     ..    
-00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ee0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00008ef0: 7175 655f 7472 6163 6b5f 7072 6f70 6572  que_track_proper
-00008f00: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
-00008f10: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00008f20: 7473 5f70 726f 7065 7274 6965 7320 2020  ts_properties   
-00008f30: 200d 0a0d 0a20 2020 2064 6566 205f 7472   ....    def _tr
-00008f40: 6163 6b6c 6574 5f61 6e64 5f70 726f 7065  acklet_and_prope
-00008f50: 7274 6965 7328 7365 6c66 2c20 616c 6c5f  rties(self, all_
-00008f60: 6469 6374 5f76 616c 7565 732c 2074 2c20  dict_values, t, 
-00008f70: 7a2c 2079 2c20 782c 206b 2c20 6375 7272  z, y, x, k, curr
-00008f80: 656e 745f 7472 6163 6b5f 6964 2c20 756e  ent_track_id, un
-00008f90: 6971 7565 5f69 642c 2063 7572 7265 6e74  ique_id, current
-00008fa0: 5f74 7261 636b 6c65 7473 2c20 6375 7272  _tracklets, curr
-00008fb0: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
-00008fc0: 6f70 6572 7469 6573 293a 0d0a 2020 2020  operties):..    
-00008fd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ff0: 2020 2020 2020 2020 2020 2020 2067 656e               gen
-00009000: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
-00009010: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009020: 7365 6c66 2e67 656e 6572 6174 696f 6e69  self.generationi
-00009030: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
+00008d60: 2020 2020 2020 2020 7a20 3d20 666c 6f61          z = floa
+00008d70: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+00008d80: 735b 7365 6c66 2e7a 706f 7369 645f 6b65  s[self.zposid_ke
+00008d90: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008db0: 2020 2020 2020 2020 2079 203d 2066 6c6f           y = flo
+00008dc0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00008dd0: 6573 5b73 656c 662e 7970 6f73 6964 5f6b  es[self.yposid_k
+00008de0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e00: 2020 2020 2020 2020 2020 7820 3d20 666c            x = fl
+00008e10: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+00008e20: 7565 735b 7365 6c66 2e78 706f 7369 645f  ues[self.xposid_
+00008e30: 6b65 795d 290d 0a0d 0a20 2020 2020 2020  key])....       
+00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e50: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00008e60: 7265 6e74 5f74 7261 636b 6c65 7473 2c20  rent_tracklets, 
+00008e70: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00008e80: 735f 7072 6f70 6572 7469 6573 203d 2073  s_properties = s
+00008e90: 656c 662e 5f74 7261 636b 6c65 745f 616e  elf._tracklet_an
+00008ea0: 645f 7072 6f70 6572 7469 6573 2861 6c6c  d_properties(all
+00008eb0: 5f64 6963 745f 7661 6c75 6573 2c20 742c  _dict_values, t,
+00008ec0: 207a 2c20 792c 2078 2c20 6b2c 2063 7572   z, y, x, k, cur
+00008ed0: 7265 6e74 5f74 7261 636b 5f69 642c 2075  rent_track_id, u
+00008ee0: 6e69 7175 655f 6964 2c20 6375 7272 656e  nique_id, curren
+00008ef0: 745f 7472 6163 6b6c 6574 732c 2063 7572  t_tracklets, cur
+00008f00: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
+00008f10: 726f 7065 7274 6965 7329 0d0a 2020 2020  roperties)..    
+00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00008f70: 7320 3d20 6e70 2e61 7361 7272 6179 2863  s = np.asarray(c
+00008f80: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00008f90: 5b73 7472 2874 7261 636b 5f69 6429 5d2c  [str(track_id)],
+00008fa0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00008fb0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fd0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00008fe0: 735f 7072 6f70 6572 7469 6573 203d 206e  s_properties = n
+00008ff0: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+00009000: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+00009010: 6572 7469 6573 5b73 7472 2874 7261 636b  erties[str(track
+00009020: 5f69 6429 5d2c 2064 7479 7065 3d6e 702e  _id)], dtype=np.
+00009030: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
 00009040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009050: 2020 2020 2020 2020 2020 2020 2020 7370                sp
-00009060: 6565 6420 3d20 666c 6f61 7428 616c 6c5f  eed = float(all_
-00009070: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00009080: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
-00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090b0: 2020 6163 6365 6c65 7261 7469 6f6e 203d    acceleration =
-000090c0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-000090d0: 7661 6c75 6573 5b73 656c 662e 6163 6365  values[self.acce
-000090e0: 6c65 7261 7469 6f6e 5f6b 6579 5d29 0d0a  leration_key])..
-000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
-00009120: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00009130: 745f 7661 6c75 6573 5b73 656c 662e 6d6f  t_values[self.mo
-00009140: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 5d29  tion_angle_key])
-00009150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009170: 2020 2020 2020 7261 6469 616c 5f61 6e67        radial_ang
-00009180: 6c65 203d 2066 6c6f 6174 2861 6c6c 5f64  le = float(all_d
-00009190: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-000091a0: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
-000091b0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00009050: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00009060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009070: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00009080: 7472 6163 6b73 5b74 7261 636b 5f69 645d  tracks[track_id]
+00009090: 203d 2063 7572 7265 6e74 5f74 7261 636b   = current_track
+000090a0: 6c65 7473 2020 2020 200d 0a20 2020 2020  lets     ..     
+000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090c0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000090d0: 7565 5f74 7261 636b 5f70 726f 7065 7274  ue_track_propert
+000090e0: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
+000090f0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00009100: 735f 7072 6f70 6572 7469 6573 2020 2020  s_properties    
+00009110: 0d0a 0d0a 2020 2020 6465 6620 5f74 7261  ....    def _tra
+00009120: 636b 6c65 745f 616e 645f 7072 6f70 6572  cklet_and_proper
+00009130: 7469 6573 2873 656c 662c 2061 6c6c 5f64  ties(self, all_d
+00009140: 6963 745f 7661 6c75 6573 2c20 742c 207a  ict_values, t, z
+00009150: 2c20 792c 2078 2c20 6b2c 2063 7572 7265  , y, x, k, curre
+00009160: 6e74 5f74 7261 636b 5f69 642c 2075 6e69  nt_track_id, uni
+00009170: 7175 655f 6964 2c20 6375 7272 656e 745f  que_id, current_
+00009180: 7472 6163 6b6c 6574 732c 2063 7572 7265  tracklets, curre
+00009190: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
+000091a0: 7065 7274 6965 7329 3a0d 0a20 2020 2020  perties):..     
+000091b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091d0: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
-000091e0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-000091f0: 7661 6c75 6573 5b73 656c 662e 7261 6469  values[self.radi
-00009200: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
-00009210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009220: 2020 2020 2020 2020 2020 2020 2020 766f                vo
-00009230: 6c75 6d65 5f70 6978 656c 7320 3d20 696e  lume_pixels = in
-00009240: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
-00009250: 5f76 616c 7565 735b 7365 6c66 2e71 7561  _values[self.qua
-00009260: 6c69 7479 5f6b 6579 5d29 290d 0a20 2020  lity_key]))..   
+000091d0: 2020 2020 2020 2020 2020 2020 6765 6e5f              gen_
+000091e0: 6964 203d 2069 6e74 2866 6c6f 6174 2861  id = int(float(a
+000091f0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+00009200: 656c 662e 6765 6e65 7261 7469 6f6e 6964  elf.generationid
+00009210: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
+00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009230: 2020 2020 2020 2020 2020 2020 2073 7065               spe
+00009240: 6564 203d 2066 6c6f 6174 2861 6c6c 5f64  ed = float(all_d
+00009250: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00009260: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
 00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009290: 2074 6f74 616c 5f69 6e74 656e 7369 7479   total_intensity
-000092a0: 203d 2020 666c 6f61 7428 616c 6c5f 6469   =  float(all_di
-000092b0: 6374 5f76 616c 7565 735b 7365 6c66 2e74  ct_values[self.t
-000092c0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
-000092d0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00009290: 2061 6363 656c 6572 6174 696f 6e20 3d20   acceleration = 
+000092a0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+000092b0: 616c 7565 735b 7365 6c66 2e61 6363 656c  alues[self.accel
+000092c0: 6572 6174 696f 6e5f 6b65 795d 290d 0a20  eration_key]).. 
+000092d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00009320: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00009330: 6b20 3d20 666c 6f61 7428 616c 6c5f 6469  k = float(all_di
-00009340: 6374 5f76 616c 7565 735b 7365 6c66 2e64  ct_values[self.d
-00009350: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00009360: 6b5f 6b65 795d 290d 0a0d 0a20 2020 2020  k_key])....     
-00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009380: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009390: 6620 7365 6c66 2e73 7572 6661 6365 5f61  f self.surface_a
-000093a0: 7265 615f 6b65 7920 696e 2061 6c6c 5f64  rea_key in all_d
-000093b0: 6963 745f 7661 6c75 6573 2e6b 6579 7328  ict_values.keys(
-000093c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093e0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000093f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009410: 2020 2020 2020 2020 2020 2020 6563 6365              ecce
-00009420: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00009430: 7273 7420 3d20 666c 6f61 7428 616c 6c5f  rst = float(all_
-00009440: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00009450: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
-00009460: 6d70 5f66 6972 7374 6b65 795d 290d 0a20  mp_firstkey]).. 
-00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009490: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
-000094a0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-000094b0: 6e64 203d 2066 6c6f 6174 2861 6c6c 5f64  nd = float(all_d
-000094c0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-000094d0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-000094e0: 705f 7365 636f 6e64 6b65 795d 290d 0a20  p_secondkey]).. 
-000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
-00009520: 655f 6172 6561 203d 2066 6c6f 6174 2861  e_area = float(a
-00009530: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009540: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
-00009550: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009580: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
-00009590: 6b20 3d20 666c 6f61 7428 616c 6c5f 6469  k = float(all_di
-000095a0: 6374 5f76 616c 7565 735b 7365 6c66 2e63  ct_values[self.c
-000095b0: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
-000095c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000092f0: 2020 206d 6f74 696f 6e5f 616e 676c 6520     motion_angle 
+00009300: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+00009310: 5f76 616c 7565 735b 7365 6c66 2e6d 6f74  _values[self.mot
+00009320: 696f 6e5f 616e 676c 655f 6b65 795d 290d  ion_angle_key]).
+00009330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009350: 2020 2020 2072 6164 6961 6c5f 616e 676c       radial_angl
+00009360: 6520 3d20 666c 6f61 7428 616c 6c5f 6469  e = float(all_di
+00009370: 6374 5f76 616c 7565 735b 7365 6c66 2e72  ct_values[self.r
+00009380: 6164 6961 6c5f 616e 676c 655f 6b65 795d  adial_angle_key]
+00009390: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000093a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093b0: 2020 2020 2020 2072 6164 6975 7320 3d20         radius = 
+000093c0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+000093d0: 616c 7565 735b 7365 6c66 2e72 6164 6975  alues[self.radiu
+000093e0: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
+000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009400: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
+00009410: 756d 655f 7069 7865 6c73 203d 2069 6e74  ume_pixels = int
+00009420: 2866 6c6f 6174 2861 6c6c 5f64 6963 745f  (float(all_dict_
+00009430: 7661 6c75 6573 5b73 656c 662e 7175 616c  values[self.qual
+00009440: 6974 795f 6b65 795d 2929 0d0a 2020 2020  ity_key]))..    
+00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009470: 746f 7461 6c5f 696e 7465 6e73 6974 7920  total_intensity 
+00009480: 3d20 2066 6c6f 6174 2861 6c6c 5f64 6963  =  float(all_dic
+00009490: 745f 7661 6c75 6573 5b73 656c 662e 746f  t_values[self.to
+000094a0: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
+000094b0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000094c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00009500: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00009510: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+00009520: 745f 7661 6c75 6573 5b73 656c 662e 6469  t_values[self.di
+00009530: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00009540: 5f6b 6579 5d29 0d0a 0d0a 2020 2020 2020  _key])....      
+00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009560: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00009570: 2073 656c 662e 7375 7266 6163 655f 6172   self.surface_ar
+00009580: 6561 5f6b 6579 2069 6e20 616c 6c5f 6469  ea_key in all_di
+00009590: 6374 5f76 616c 7565 732e 6b65 7973 2829  ct_values.keys()
+000095a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095e0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000095f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009640: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
+00009600: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00009610: 7374 203d 2066 6c6f 6174 2861 6c6c 5f64  st = float(all_d
+00009620: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00009630: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00009640: 705f 6669 7273 746b 6579 5d29 0d0a 2020  p_firstkey])..  
 00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009670: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-00009680: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00009690: 203d 202d 310d 0a20 2020 2020 2020 2020   = -1..         
-000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096c0: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
-000096d0: 636f 6d70 5f73 6563 6f6e 6420 3d20 2d31  comp_second = -1
-000096e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009700: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00009710: 7266 6163 655f 6172 6561 203d 202d 310d  rface_area = -1.
-00009720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00009750: 6c5f 6178 6973 5f6d 6173 6b20 3d20 2d31  l_axis_mask = -1
-00009760: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009780: 2020 2020 2020 2020 2020 2020 2066 7261               fra
-00009790: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
-000097a0: 203d 2028 742c 726f 756e 6428 7a29 2f73   = (t,round(z)/s
-000097b0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-000097c0: 2c20 726f 756e 6428 7929 2f73 656c 662e  , round(y)/self.
-000097d0: 7963 616c 6962 7261 7469 6f6e 2c20 726f  ycalibration, ro
-000097e0: 756e 6428 7829 2f73 656c 662e 7863 616c  und(x)/self.xcal
-000097f0: 6962 7261 7469 6f6e 2920 0d0a 2020 2020  ibration) ..    
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009680: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+00009690: 6420 3d20 666c 6f61 7428 616c 6c5f 6469  d = float(all_di
+000096a0: 6374 5f76 616c 7565 735b 7365 6c66 2e65  ct_values[self.e
+000096b0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+000096c0: 5f73 6563 6f6e 646b 6579 5d29 0d0a 2020  _secondkey])..  
+000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096f0: 2020 2020 2020 2020 2073 7572 6661 6365           surface
+00009700: 5f61 7265 6120 3d20 666c 6f61 7428 616c  _area = float(al
+00009710: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00009720: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+00009730: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009760: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
+00009770: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+00009780: 745f 7661 6c75 6573 5b73 656c 662e 6365  t_values[self.ce
+00009790: 6c6c 6178 6973 5f6d 6173 6b5f 6b65 795d  llaxis_mask_key]
+000097a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000097b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00009800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00009830: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
-00009840: 7370 6f74 5f63 656e 7472 6f69 645d 203d  spot_centroid] =
-00009850: 206b 0d0a 0d0a 2020 2020 2020 2020 2020   k....          
-00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009870: 2020 2020 2020 2020 2020 6966 2063 7572            if cur
-00009880: 7265 6e74 5f74 7261 636b 5f69 6420 696e  rent_track_id in
-00009890: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-000098a0: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098c0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-000098d0: 636b 6c65 745f 6172 7261 7920 3d20 6375  cklet_array = cu
-000098e0: 7272 656e 745f 7472 6163 6b6c 6574 735b  rrent_tracklets[
-000098f0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
-00009900: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00009820: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009850: 2020 2020 2020 2020 6563 6365 6e74 7269          eccentri
+00009860: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
+00009870: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
+00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098a0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
+000098b0: 6f6d 705f 7365 636f 6e64 203d 202d 310d  omp_second = -1.
+000098c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098e0: 2020 2020 2020 2020 2020 2020 2073 7572               sur
+000098f0: 6661 6365 5f61 7265 6120 3d20 2d31 0d0a  face_area = -1..
+00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009920: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00009930: 6e74 5f74 7261 636b 6c65 745f 6172 7261  nt_tracklet_arra
-00009940: 7920 3d20 6e70 2e61 7272 6179 285b 696e  y = np.array([in
-00009950: 7428 666c 6f61 7428 756e 6971 7565 5f69  t(float(unique_i
-00009960: 6429 292c 2074 2c20 7a2f 7365 6c66 2e7a  d)), t, z/self.z
-00009970: 6361 6c69 6272 6174 696f 6e2c 2079 2f73  calibration, y/s
-00009980: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00009990: 2c20 782f 7365 6c66 2e78 6361 6c69 6272  , x/self.xcalibr
-000099a0: 6174 696f 6e5d 290d 0a20 2020 2020 2020  ation])..       
-000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-000099e0: 7473 5b63 7572 7265 6e74 5f74 7261 636b  ts[current_track
-000099f0: 5f69 645d 203d 206e 702e 7673 7461 636b  _id] = np.vstack
-00009a00: 2828 7472 6163 6b6c 6574 5f61 7272 6179  ((tracklet_array
-00009a10: 2c20 6375 7272 656e 745f 7472 6163 6b6c  , current_trackl
-00009a20: 6574 5f61 7272 6179 2929 0d0a 0d0a 2020  et_array))....  
-00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+00009930: 5f61 7869 735f 6d61 736b 203d 202d 3120  _axis_mask = -1 
+00009940: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009960: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+00009970: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
+00009980: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
+00009990: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+000099a0: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
+000099b0: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
+000099c0: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
+000099d0: 6272 6174 696f 6e29 200d 0a20 2020 2020  bration) ..     
+000099e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009a00: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00009a10: 6365 6e74 726f 6964 5b66 7261 6d65 5f73  centroid[frame_s
+00009a20: 706f 745f 6365 6e74 726f 6964 5d20 3d20  pot_centroid] = 
+00009a30: 6b0d 0a0d 0a20 2020 2020 2020 2020 2020  k....           
 00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a50: 2020 2020 2020 7661 6c75 655f 6172 7261        value_arra
-00009a60: 7920 3d20 6375 7272 656e 745f 7472 6163  y = current_trac
-00009a70: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
-00009a80: 5b63 7572 7265 6e74 5f74 7261 636b 5f69  [current_track_i
-00009a90: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00009ac0: 656e 745f 7661 6c75 655f 6172 7261 7920  ent_value_array 
-00009ad0: 3d20 6e70 2e61 7272 6179 285b 742c 2069  = np.array([t, i
-00009ae0: 6e74 2866 6c6f 6174 2875 6e69 7175 655f  nt(float(unique_
-00009af0: 6964 2929 2c20 6765 6e5f 6964 2c20 7261  id)), gen_id, ra
-00009b00: 6469 7573 2c20 766f 6c75 6d65 5f70 6978  dius, volume_pix
-00009b10: 656c 732c 2065 6363 656e 7472 6963 6974  els, eccentricit
-00009b20: 795f 636f 6d70 5f66 6972 7374 2c20 6563  y_comp_first, ec
-00009b30: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00009b40: 7365 636f 6e64 2c20 7375 7266 6163 655f  second, surface_
-00009b50: 6172 6561 2c20 746f 7461 6c5f 696e 7465  area, total_inte
-00009b60: 6e73 6974 792c 2073 7065 6564 2c20 6d6f  nsity, speed, mo
-00009b70: 7469 6f6e 5f61 6e67 6c65 2c20 6163 6365  tion_angle, acce
-00009b80: 6c65 7261 7469 6f6e 2c20 6469 7374 616e  leration, distan
-00009b90: 6365 5f63 656c 6c5f 6d61 736b 2c20 7261  ce_cell_mask, ra
-00009ba0: 6469 616c 5f61 6e67 6c65 2c20 6365 6c6c  dial_angle, cell
-00009bb0: 5f61 7869 735f 6d61 736b 5d29 0d0a 2020  _axis_mask])..  
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009be0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00009c20: 735f 7072 6f70 6572 7469 6573 5b63 7572  s_properties[cur
-00009c30: 7265 6e74 5f74 7261 636b 5f69 645d 203d  rent_track_id] =
-00009c40: 206e 702e 7673 7461 636b 2828 7661 6c75   np.vstack((valu
-00009c50: 655f 6172 7261 792c 2063 7572 7265 6e74  e_array, current
-00009c60: 5f76 616c 7565 5f61 7272 6179 2929 0d0a  _value_array))..
-00009c70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009a50: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
+00009a60: 656e 745f 7472 6163 6b5f 6964 2069 6e20  ent_track_id in 
+00009a70: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00009a80: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00009ab0: 6b6c 6574 5f61 7272 6179 203d 2063 7572  klet_array = cur
+00009ac0: 7265 6e74 5f74 7261 636b 6c65 7473 5b63  rent_tracklets[c
+00009ad0: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
+00009ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b00: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00009b10: 745f 7472 6163 6b6c 6574 5f61 7272 6179  t_tracklet_array
+00009b20: 203d 206e 702e 6172 7261 7928 5b69 6e74   = np.array([int
+00009b30: 2866 6c6f 6174 2875 6e69 7175 655f 6964  (float(unique_id
+00009b40: 2929 2c20 742c 207a 2f73 656c 662e 7a63  )), t, z/self.zc
+00009b50: 616c 6962 7261 7469 6f6e 2c20 792f 7365  alibration, y/se
+00009b60: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
+00009b70: 2078 2f73 656c 662e 7863 616c 6962 7261   x/self.xcalibra
+00009b80: 7469 6f6e 5d29 0d0a 2020 2020 2020 2020  tion])..        
+00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bb0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00009bc0: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
+00009bd0: 6964 5d20 3d20 6e70 2e76 7374 6163 6b28  id] = np.vstack(
+00009be0: 2874 7261 636b 6c65 745f 6172 7261 792c  (tracklet_array,
+00009bf0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00009c00: 745f 6172 7261 7929 290d 0a0d 0a20 2020  t_array))....   
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c30: 2020 2020 2076 616c 7565 5f61 7272 6179       value_array
+00009c40: 203d 2063 7572 7265 6e74 5f74 7261 636b   = current_track
+00009c50: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
+00009c60: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+00009c70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
 00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c90: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-00009cd0: 636b 6c65 745f 6172 7261 7920 3d20 6e70  cklet_array = np
-00009ce0: 2e61 7272 6179 285b 696e 7428 666c 6f61  .array([int(floa
-00009cf0: 7428 756e 6971 7565 5f69 6429 292c 2074  t(unique_id)), t
-00009d00: 2c20 7a2f 7365 6c66 2e7a 6361 6c69 6272  , z/self.zcalibr
-00009d10: 6174 696f 6e2c 2079 2f73 656c 662e 7963  ation, y/self.yc
-00009d20: 616c 6962 7261 7469 6f6e 2c20 782f 7365  alibration, x/se
-00009d30: 6c66 2e78 6361 6c69 6272 6174 696f 6e5d  lf.xcalibration]
-00009d40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00009d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d60: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00009d70: 6e74 5f74 7261 636b 6c65 7473 5b63 7572  nt_tracklets[cur
-00009d80: 7265 6e74 5f74 7261 636b 5f69 645d 203d  rent_track_id] =
-00009d90: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00009da0: 745f 6172 7261 7920 0d0a 0d0a 2020 2020  t_array ....    
+00009c90: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00009ca0: 6e74 5f76 616c 7565 5f61 7272 6179 203d  nt_value_array =
+00009cb0: 206e 702e 6172 7261 7928 5b74 2c20 696e   np.array([t, in
+00009cc0: 7428 666c 6f61 7428 756e 6971 7565 5f69  t(float(unique_i
+00009cd0: 6429 292c 2067 656e 5f69 642c 2072 6164  d)), gen_id, rad
+00009ce0: 6975 732c 2076 6f6c 756d 655f 7069 7865  ius, volume_pixe
+00009cf0: 6c73 2c20 6563 6365 6e74 7269 6369 7479  ls, eccentricity
+00009d00: 5f63 6f6d 705f 6669 7273 742c 2065 6363  _comp_first, ecc
+00009d10: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00009d20: 6563 6f6e 642c 2073 7572 6661 6365 5f61  econd, surface_a
+00009d30: 7265 612c 2074 6f74 616c 5f69 6e74 656e  rea, total_inten
+00009d40: 7369 7479 2c20 7370 6565 642c 206d 6f74  sity, speed, mot
+00009d50: 696f 6e5f 616e 676c 652c 2061 6363 656c  ion_angle, accel
+00009d60: 6572 6174 696f 6e2c 2064 6973 7461 6e63  eration, distanc
+00009d70: 655f 6365 6c6c 5f6d 6173 6b2c 2072 6164  e_cell_mask, rad
+00009d80: 6961 6c5f 616e 676c 652c 2063 656c 6c5f  ial_angle, cell_
+00009d90: 6178 6973 5f6d 6173 6b5d 290d 0a20 2020  axis_mask])..   
+00009da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 2020 2020 6375 7272 656e 745f 7661 6c75      current_valu
-00009de0: 655f 6172 7261 7920 3d20 6e70 2e61 7272  e_array = np.arr
-00009df0: 6179 285b 742c 2069 6e74 2866 6c6f 6174  ay([t, int(float
-00009e00: 2875 6e69 7175 655f 6964 2929 2c20 6765  (unique_id)), ge
-00009e10: 6e5f 6964 2c20 7261 6469 7573 2c20 766f  n_id, radius, vo
-00009e20: 6c75 6d65 5f70 6978 656c 732c 2020 6563  lume_pixels,  ec
-00009e30: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00009e40: 6669 7273 742c 2065 6363 656e 7472 6963  first, eccentric
-00009e50: 6974 795f 636f 6d70 5f73 6563 6f6e 642c  ity_comp_second,
-00009e60: 2073 7572 6661 6365 5f61 7265 612c 2020   surface_area,  
-00009e70: 746f 7461 6c5f 696e 7465 6e73 6974 792c  total_intensity,
-00009e80: 2073 7065 6564 2c20 6d6f 7469 6f6e 5f61   speed, motion_a
-00009e90: 6e67 6c65 2c20 6163 6365 6c65 7261 7469  ngle, accelerati
-00009ea0: 6f6e 2c20 6469 7374 616e 6365 5f63 656c  on, distance_cel
-00009eb0: 6c5f 6d61 736b 2c20 7261 6469 616c 5f61  l_mask, radial_a
-00009ec0: 6e67 6c65 2c20 6365 6c6c 5f61 7869 735f  ngle, cell_axis_
-00009ed0: 6d61 736b 205d 290d 0a20 2020 2020 2020  mask ])..       
-00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f00: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00009f10: 7473 5f70 726f 7065 7274 6965 735b 6375  ts_properties[cu
-00009f20: 7272 656e 745f 7472 6163 6b5f 6964 5d20  rrent_track_id] 
-00009f30: 3d20 6375 7272 656e 745f 7661 6c75 655f  = current_value_
-00009f40: 6172 7261 790d 0a0d 0a20 2020 2020 2020  array....       
-00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f60: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00009f70: 7572 6e20 6375 7272 656e 745f 7472 6163  urn current_trac
-00009f80: 6b6c 6574 732c 2063 7572 7265 6e74 5f74  klets, current_t
-00009f90: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00009fa0: 6965 7320 2020 2020 0d0a 0d0a 2020 2020  ies     ....    
-00009fb0: 6465 6620 5f6d 6173 7465 725f 7370 6f74  def _master_spot
-00009fc0: 5f63 6f6d 7075 7465 7228 7365 6c66 2c20  _computer(self, 
-00009fd0: 6672 616d 6529 3a0d 0a20 2020 2020 2020  frame):..       
-00009fe0: 2020 200d 0a20 2020 2020 2020 2020 2066     ..          f
-00009ff0: 6f72 2053 706f 746f 626a 6563 7420 696e  or Spotobject in
-0000a000: 2066 7261 6d65 2e66 696e 6461 6c6c 2827   frame.findall('
-0000a010: 5370 6f74 2729 3a0d 0a20 2020 2020 2020  Spot'):..       
-0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a040: 2020 2020 2020 2020 2020 6365 6c6c 5f69            cell_i
-0000a050: 6420 3d20 696e 7428 5370 6f74 6f62 6a65  d = int(Spotobje
-0000a060: 6374 2e67 6574 2873 656c 662e 7370 6f74  ct.get(self.spot
-0000a070: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
-0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a0a0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000a0b0: 662e 756e 6971 7565 6964 5f6b 6579 2069  f.uniqueid_key i
-0000a0c0: 6e20 5370 6f74 6f62 6a65 6374 2e6b 6579  n Spotobject.key
-0000a0d0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-0000a0e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 7261 6469 7573 203d 2066 6c6f 6174 2853  radius = float(S
-0000a120: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000a130: 6c66 2e72 6164 6975 735f 6b65 7929 290d  lf.radius_key)).
-0000a140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a160: 2071 7561 6c69 7479 203d 2066 6c6f 6174   quality = float
-0000a170: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000a180: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-0000a190: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1b0: 2020 2020 746f 7461 6c5f 696e 7465 6e73      total_intens
-0000a1c0: 6974 7920 3d20 666c 6f61 7428 5370 6f74  ity = float(Spot
-0000a1d0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000a1e0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000a1f0: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a210: 2020 2020 2020 206d 6561 6e5f 696e 7465         mean_inte
-0000a220: 6e73 6974 7920 3d20 666c 6f61 7428 5370  nsity = float(Sp
-0000a230: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000a240: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
-0000a250: 5f6b 6579 2929 0d0a 0d0a 2020 2020 2020  _key))....      
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a270: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000a280: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000a290: 7274 6965 735b 6365 6c6c 5f69 645d 203d  rties[cell_id] =
-0000a2a0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
-0000a2d0: 6c69 645f 6b65 793a 2069 6e74 2866 6c6f  lid_key: int(flo
-0000a2e0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000a2f0: 7428 7365 6c66 2e73 706f 7469 645f 6b65  t(self.spotid_ke
-0000a300: 7929 2929 2c20 0d0a 2020 2020 2020 2020  y))), ..        
-0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a330: 2e66 7261 6d65 6964 5f6b 6579 203a 2069  .frameid_key : i
-0000a340: 6e74 2866 6c6f 6174 2853 706f 746f 626a  nt(float(Spotobj
-0000a350: 6563 742e 6765 7428 7365 6c66 2e66 7261  ect.get(self.fra
-0000a360: 6d65 6964 5f6b 6579 2929 292c 0d0a 2020  meid_key))),..  
-0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009dc0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009df0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00009e00: 5f70 726f 7065 7274 6965 735b 6375 7272  _properties[curr
+00009e10: 656e 745f 7472 6163 6b5f 6964 5d20 3d20  ent_track_id] = 
+00009e20: 6e70 2e76 7374 6163 6b28 2876 616c 7565  np.vstack((value
+00009e30: 5f61 7272 6179 2c20 6375 7272 656e 745f  _array, current_
+00009e40: 7661 6c75 655f 6172 7261 7929 290d 0a0d  value_array))...
+00009e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e70: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ea0: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00009eb0: 6b6c 6574 5f61 7272 6179 203d 206e 702e  klet_array = np.
+00009ec0: 6172 7261 7928 5b69 6e74 2866 6c6f 6174  array([int(float
+00009ed0: 2875 6e69 7175 655f 6964 2929 2c20 742c  (unique_id)), t,
+00009ee0: 207a 2f73 656c 662e 7a63 616c 6962 7261   z/self.zcalibra
+00009ef0: 7469 6f6e 2c20 792f 7365 6c66 2e79 6361  tion, y/self.yca
+00009f00: 6c69 6272 6174 696f 6e2c 2078 2f73 656c  libration, x/sel
+00009f10: 662e 7863 616c 6962 7261 7469 6f6e 5d29  f.xcalibration])
+00009f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f40: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00009f50: 745f 7472 6163 6b6c 6574 735b 6375 7272  t_tracklets[curr
+00009f60: 656e 745f 7472 6163 6b5f 6964 5d20 3d20  ent_track_id] = 
+00009f70: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00009f80: 5f61 7272 6179 200d 0a0d 0a20 2020 2020  _array ....     
+00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fb0: 2020 2063 7572 7265 6e74 5f76 616c 7565     current_value
+00009fc0: 5f61 7272 6179 203d 206e 702e 6172 7261  _array = np.arra
+00009fd0: 7928 5b74 2c20 696e 7428 666c 6f61 7428  y([t, int(float(
+00009fe0: 756e 6971 7565 5f69 6429 292c 2067 656e  unique_id)), gen
+00009ff0: 5f69 642c 2072 6164 6975 732c 2076 6f6c  _id, radius, vol
+0000a000: 756d 655f 7069 7865 6c73 2c20 2065 6363  ume_pixels,  ecc
+0000a010: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+0000a020: 6972 7374 2c20 6563 6365 6e74 7269 6369  irst, eccentrici
+0000a030: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
+0000a040: 7375 7266 6163 655f 6172 6561 2c20 2074  surface_area,  t
+0000a050: 6f74 616c 5f69 6e74 656e 7369 7479 2c20  otal_intensity, 
+0000a060: 7370 6565 642c 206d 6f74 696f 6e5f 616e  speed, motion_an
+0000a070: 676c 652c 2061 6363 656c 6572 6174 696f  gle, acceleratio
+0000a080: 6e2c 2064 6973 7461 6e63 655f 6365 6c6c  n, distance_cell
+0000a090: 5f6d 6173 6b2c 2072 6164 6961 6c5f 616e  _mask, radial_an
+0000a0a0: 676c 652c 2063 656c 6c5f 6178 6973 5f6d  gle, cell_axis_m
+0000a0b0: 6173 6b20 5d29 0d0a 2020 2020 2020 2020  ask ])..        
+0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0e0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+0000a0f0: 735f 7072 6f70 6572 7469 6573 5b63 7572  s_properties[cur
+0000a100: 7265 6e74 5f74 7261 636b 5f69 645d 203d  rent_track_id] =
+0000a110: 2063 7572 7265 6e74 5f76 616c 7565 5f61   current_value_a
+0000a120: 7272 6179 0d0a 0d0a 2020 2020 2020 2020  rray....        
+0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a140: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a150: 726e 2063 7572 7265 6e74 5f74 7261 636b  rn current_track
+0000a160: 6c65 7473 2c20 6375 7272 656e 745f 7472  lets, current_tr
+0000a170: 6163 6b6c 6574 735f 7072 6f70 6572 7469  acklets_properti
+0000a180: 6573 2020 2020 200d 0a0d 0a20 2020 2064  es     ....    d
+0000a190: 6566 205f 6d61 7374 6572 5f73 706f 745f  ef _master_spot_
+0000a1a0: 636f 6d70 7574 6572 2873 656c 662c 2066  computer(self, f
+0000a1b0: 7261 6d65 293a 0d0a 2020 2020 2020 2020  rame):..        
+0000a1c0: 2020 0d0a 2020 2020 2020 2020 2020 666f    ..          fo
+0000a1d0: 7220 5370 6f74 6f62 6a65 6374 2069 6e20  r Spotobject in 
+0000a1e0: 6672 616d 652e 6669 6e64 616c 6c28 2753  frame.findall('S
+0000a1f0: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
+0000a200: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000a210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a220: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
+0000a230: 203d 2069 6e74 2853 706f 746f 626a 6563   = int(Spotobjec
+0000a240: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
+0000a250: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
+0000a260: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000a270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a280: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000a290: 2e75 6e69 7175 6569 645f 6b65 7920 696e  .uniqueid_key in
+0000a2a0: 2053 706f 746f 626a 6563 742e 6b65 7973   Spotobject.keys
+0000a2b0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+0000a2c0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a2f0: 6164 6975 7320 3d20 666c 6f61 7428 5370  adius = float(Sp
+0000a300: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000a310: 662e 7261 6469 7573 5f6b 6579 2929 0d0a  f.radius_key))..
+0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a340: 7175 616c 6974 7920 3d20 666c 6f61 7428  quality = float(
+0000a350: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000a360: 656c 662e 7175 616c 6974 795f 6b65 7929  elf.quality_key)
+0000a370: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a390: 2020 7365 6c66 2e7a 706f 7369 645f 6b65    self.zposid_ke
-0000a3a0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000a3b0: 6a65 6374 2e67 6574 2873 656c 662e 7a70  ject.get(self.zp
-0000a3c0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
-0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a390: 2020 2074 6f74 616c 5f69 6e74 656e 7369     total_intensi
+0000a3a0: 7479 203d 2066 6c6f 6174 2853 706f 746f  ty = float(Spoto
+0000a3b0: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
+0000a3c0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+0000a3d0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
 0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3f0: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
-0000a400: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000a410: 6563 742e 6765 7428 7365 6c66 2e79 706f  ect.get(self.ypo
-0000a420: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
-0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3f0: 2020 2020 2020 6d65 616e 5f69 6e74 656e        mean_inten
+0000a400: 7369 7479 203d 2066 6c6f 6174 2853 706f  sity = float(Spo
+0000a410: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000a420: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
+0000a430: 6b65 7929 290d 0a0d 0a20 2020 2020 2020  key))....       
 0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a450: 7365 6c66 2e78 706f 7369 645f 6b65 7920  self.xposid_key 
-0000a460: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
-0000a470: 6374 2e67 6574 2873 656c 662e 7870 6f73  ct.get(self.xpos
-0000a480: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000a450: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000a460: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000a470: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
+0000a480: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
 0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a4b0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000a4c0: 6974 795f 6b65 7920 3a20 746f 7461 6c5f  ity_key : total_
-0000a4d0: 696e 7465 6e73 6974 792c 0d0a 2020 2020  intensity,..    
-0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
+0000a4b0: 6964 5f6b 6579 3a20 696e 7428 666c 6f61  id_key: int(floa
+0000a4c0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000a4d0: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
+0000a4e0: 2929 292c 200d 0a20 2020 2020 2020 2020  ))), ..         
 0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000a510: 6974 795f 6b65 7920 3a20 6d65 616e 5f69  ity_key : mean_i
-0000a520: 6e74 656e 7369 7479 2c0d 0a20 2020 2020  ntensity,..     
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a550: 656c 662e 7261 6469 7573 5f6b 6579 203a  elf.radius_key :
-0000a560: 2072 6164 6975 732c 0d0a 2020 2020 2020   radius,..      
-0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a580: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a590: 6c66 2e71 7561 6c69 7479 5f6b 6579 203a  lf.quality_key :
-0000a5a0: 2071 7561 6c69 7479 2c0d 0a20 2020 2020   quality,..     
+0000a500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a510: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
+0000a520: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
+0000a530: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
+0000a540: 6569 645f 6b65 7929 2929 2c0d 0a20 2020  eid_key))),..   
+0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
+0000a580: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000a590: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
+0000a5a0: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
 0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a5d0: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
-0000a5e0: 6c5f 6d61 736b 5f6b 6579 3a20 2866 6c6f  l_mask_key: (flo
-0000a5f0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000a600: 7428 7365 6c66 2e64 6973 7461 6e63 655f  t(self.distance_
-0000a610: 6365 6c6c 5f6d 6173 6b5f 6b65 7929 2929  cell_mask_key)))
-0000a620: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a640: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-0000a650: 7565 6964 5f6b 6579 203a 2073 7472 2853  ueid_key : str(S
-0000a660: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000a670: 6c66 2e75 6e69 7175 6569 645f 6b65 7929  lf.uniqueid_key)
-0000a680: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6a0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-0000a6b0: 636b 6c65 7469 645f 6b65 7920 3a20 7374  ckletid_key : st
-0000a6c0: 7228 5370 6f74 6f62 6a65 6374 2e67 6574  r(Spotobject.get
-0000a6d0: 2873 656c 662e 7472 6163 6b6c 6574 6964  (self.trackletid
-0000a6e0: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
-0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a710: 662e 6765 6e65 7261 7469 6f6e 6964 5f6b  f.generationid_k
-0000a720: 6579 203a 2073 7472 2853 706f 746f 626a  ey : str(Spotobj
-0000a730: 6563 742e 6765 7428 7365 6c66 2e67 656e  ect.get(self.gen
-0000a740: 6572 6174 696f 6e69 645f 6b65 7929 292c  erationid_key)),
-0000a750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a770: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-0000a780: 6964 5f6b 6579 203a 2073 7472 2853 706f  id_key : str(Spo
-0000a790: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000a7a0: 2e74 7261 636b 6964 5f6b 6579 2929 2c0d  .trackid_key)),.
-0000a7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7d0: 2020 2020 2073 656c 662e 6d6f 7469 6f6e       self.motion
-0000a7e0: 5f61 6e67 6c65 5f6b 6579 203a 2028 666c  _angle_key : (fl
-0000a7f0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000a800: 6574 2873 656c 662e 6d6f 7469 6f6e 5f61  et(self.motion_a
-0000a810: 6e67 6c65 5f6b 6579 2929 292c 0d0a 2020  ngle_key))),..  
-0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 2020 7365 6c66 2e73 7065 6564 5f6b 6579    self.speed_key
-0000a850: 203a 2028 666c 6f61 7428 5370 6f74 6f62   : (float(Spotob
-0000a860: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
-0000a870: 6565 645f 6b65 7929 2929 2c0d 0a20 2020  eed_key))),..   
-0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8a0: 2073 656c 662e 6163 6365 6c65 7261 7469   self.accelerati
-0000a8b0: 6f6e 5f6b 6579 203a 2028 666c 6f61 7428  on_key : (float(
-0000a8c0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000a8d0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-0000a8e0: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a900: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a910: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
-0000a920: 6b65 793a 2066 6c6f 6174 2853 706f 746f  key: float(Spoto
-0000a930: 626a 6563 742e 6765 7428 7365 6c66 2e72  bject.get(self.r
-0000a940: 6164 6961 6c5f 616e 676c 655f 6b65 7929  adial_angle_key)
-0000a950: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a970: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
-0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a990: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0000a9a0: 7572 6661 6365 5f61 7265 615f 6b65 7920  urface_area_key 
-0000a9b0: 696e 2053 706f 746f 626a 6563 742e 6b65  in Spotobject.ke
-0000a9c0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-0000a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a9f0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000aa00: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-0000aa10: 6964 295d 2e75 7064 6174 6528 7b0d 0a20  id)].update({.. 
-0000aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5d0: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
+0000a5e0: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
+0000a5f0: 6374 2e67 6574 2873 656c 662e 7970 6f73  ct.get(self.ypos
+0000a600: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a620: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a630: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
+0000a640: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000a650: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
+0000a660: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a690: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000a6a0: 7479 5f6b 6579 203a 2074 6f74 616c 5f69  ty_key : total_i
+0000a6b0: 6e74 656e 7369 7479 2c0d 0a20 2020 2020  ntensity,..     
+0000a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a6e0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000a6f0: 7479 5f6b 6579 203a 206d 6561 6e5f 696e  ty_key : mean_in
+0000a700: 7465 6e73 6974 792c 0d0a 2020 2020 2020  tensity,..      
+0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a720: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a730: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
+0000a740: 7261 6469 7573 2c0d 0a20 2020 2020 2020  radius,..       
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a760: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a770: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+0000a780: 7175 616c 6974 792c 0d0a 2020 2020 2020  quality,..      
+0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a7b0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+0000a7c0: 5f6d 6173 6b5f 6b65 793a 2028 666c 6f61  _mask_key: (floa
+0000a7d0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000a7e0: 2873 656c 662e 6469 7374 616e 6365 5f63  (self.distance_c
+0000a7f0: 656c 6c5f 6d61 736b 5f6b 6579 2929 292c  ell_mask_key))),
+0000a800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a820: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000a830: 6569 645f 6b65 7920 3a20 7374 7228 5370  eid_key : str(Sp
+0000a840: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000a850: 662e 756e 6971 7565 6964 5f6b 6579 2929  f.uniqueid_key))
+0000a860: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a880: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000a890: 6b6c 6574 6964 5f6b 6579 203a 2073 7472  kletid_key : str
+0000a8a0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000a8b0: 7365 6c66 2e74 7261 636b 6c65 7469 645f  self.trackletid_
+0000a8c0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a8f0: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
+0000a900: 7920 3a20 7374 7228 5370 6f74 6f62 6a65  y : str(Spotobje
+0000a910: 6374 2e67 6574 2873 656c 662e 6765 6e65  ct.get(self.gene
+0000a920: 7261 7469 6f6e 6964 5f6b 6579 2929 2c0d  rationid_key)),.
+0000a930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a950: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
+0000a960: 645f 6b65 7920 3a20 7374 7228 5370 6f74  d_key : str(Spot
+0000a970: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000a980: 7472 6163 6b69 645f 6b65 7929 292c 0d0a  trackid_key)),..
+0000a990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9b0: 2020 2020 7365 6c66 2e6d 6f74 696f 6e5f      self.motion_
+0000a9c0: 616e 676c 655f 6b65 7920 3a20 2866 6c6f  angle_key : (flo
+0000a9d0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000a9e0: 7428 7365 6c66 2e6d 6f74 696f 6e5f 616e  t(self.motion_an
+0000a9f0: 676c 655f 6b65 7929 2929 2c0d 0a20 2020  gle_key))),..   
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 2073 656c 662e 7370 6565 645f 6b65 7920   self.speed_key 
+0000aa30: 3a20 2866 6c6f 6174 2853 706f 746f 626a  : (float(Spotobj
+0000aa40: 6563 742e 6765 7428 7365 6c66 2e73 7065  ect.get(self.spe
+0000aa50: 6564 5f6b 6579 2929 292c 0d0a 2020 2020  ed_key))),..    
 0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa70: 2020 2020 2020 2073 656c 662e 6563 6365         self.ecce
-0000aa80: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-0000aa90: 7273 746b 6579 203a 2066 6c6f 6174 2853  rstkey : float(S
+0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa80: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+0000aa90: 6e5f 6b65 7920 3a20 2866 6c6f 6174 2853  n_key : (float(S
 0000aaa0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000aab0: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
-0000aac0: 636f 6d70 5f66 6972 7374 6b65 7929 292c  comp_firstkey)),
-0000aad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab20: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000ab30: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-0000ab40: 5f73 6563 6f6e 646b 6579 203a 2066 6c6f  _secondkey : flo
-0000ab50: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000ab60: 7428 7365 6c66 2e65 6363 656e 7472 6963  t(self.eccentric
-0000ab70: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
-0000ab80: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
-0000ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aab0: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+0000aac0: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
+0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000aaf0: 662e 7261 6469 616c 5f61 6e67 6c65 5f6b  f.radial_angle_k
+0000ab00: 6579 3a20 666c 6f61 7428 5370 6f74 6f62  ey: float(Spotob
+0000ab10: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
+0000ab20: 6469 616c 5f61 6e67 6c65 5f6b 6579 2929  dial_angle_key))
+0000ab30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab50: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab70: 2020 2020 2020 6966 2073 656c 662e 7375        if self.su
+0000ab80: 7266 6163 655f 6172 6561 5f6b 6579 2069  rface_area_key i
+0000ab90: 6e20 5370 6f74 6f62 6a65 6374 2e6b 6579  n Spotobject.key
+0000aba0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
 0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000abe0: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
-0000abf0: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
-0000ac00: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000ac10: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
-0000ac20: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000abc0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000abd0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000abe0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+0000abf0: 6429 5d2e 7570 6461 7465 287b 0d0a 2020  d)].update({..  
+0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ac80: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
-0000ac90: 5f6b 6579 3a20 666c 6f61 7428 5370 6f74  _key: float(Spot
-0000aca0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000acb0: 6365 6c6c 6178 6973 5f6d 6173 6b5f 6b65  cellaxis_mask_ke
-0000acc0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000ac50: 2020 2020 2020 7365 6c66 2e65 6363 656e        self.eccen
+0000ac60: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+0000ac70: 7374 6b65 7920 3a20 666c 6f61 7428 5370  stkey : float(Sp
+0000ac80: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000ac90: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+0000aca0: 6f6d 705f 6669 7273 746b 6579 2929 2c0d  omp_firstkey)),.
+0000acb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad20: 207d 290d 0a20 2020 2020 2020 2020 2020   })..           
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000ad80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ad00: 2020 2020 2020 2020 2073 656c 662e 6563           self.ec
+0000ad10: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+0000ad20: 7365 636f 6e64 6b65 7920 3a20 666c 6f61  secondkey : floa
+0000ad30: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000ad40: 2873 656c 662e 6563 6365 6e74 7269 6369  (self.eccentrici
+0000ad50: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
+0000ad60: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ada0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000adb0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000adc0: 6966 2073 656c 662e 756e 6971 7565 6964  if self.uniqueid
-0000add0: 5f6b 6579 206e 6f74 2069 6e20 5370 6f74  _key not in Spot
-0000ade0: 6f62 6a65 6374 2e6b 6579 7328 293a 0d0a  object.keys():..
-0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000adc0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+0000add0: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
+0000ade0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000adf0: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
+0000ae00: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
 0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ae60: 6465 7465 6374 6f72 6368 616e 6e65 6c20  detectorchannel 
-0000ae70: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
-0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aea0: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
-0000aeb0: 5f49 4e54 454e 5349 5459 203d 2053 706f  _INTENSITY = Spo
-0000aec0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000aed0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
-0000aee0: 5f63 6832 5f6b 6579 290d 0a20 2020 2020  _ch2_key)..     
+0000ae50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ae60: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
+0000ae70: 6b65 793a 2066 6c6f 6174 2853 706f 746f  key: float(Spoto
+0000ae80: 626a 6563 742e 6765 7428 7365 6c66 2e63  bject.get(self.c
+0000ae90: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
+0000aea0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af10: 2020 2020 2020 2020 2020 2020 2020 204d                 M
-0000af20: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
-0000af30: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000af40: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-0000af50: 7479 5f63 6832 5f6b 6579 290d 0a20 2020  ty_ch2_key)..   
+0000af00: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af50: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af80: 2020 2020 2020 2020 2065 6c73 653a 2020           else:  
-0000af90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afc0: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
-0000afd0: 4c5f 494e 5445 4e53 4954 5920 3d20 5370  L_INTENSITY = Sp
-0000afe0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000aff0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000b000: 795f 6368 315f 6b65 7929 0d0a 2020 2020  y_ch1_key)..    
+0000af80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000af90: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0000afa0: 6620 7365 6c66 2e75 6e69 7175 6569 645f  f self.uniqueid_
+0000afb0: 6b65 7920 6e6f 7420 696e 2053 706f 746f  key not in Spoto
+0000afc0: 626a 6563 742e 6b65 7973 2829 3a0d 0a20  bject.keys():.. 
+0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b040: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
-0000b050: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
-0000b060: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000b070: 6974 795f 6368 315f 6b65 7929 0d0a 2020  ity_ch1_key)..  
-0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0a0: 2020 2020 2020 2020 2020 5241 4449 5553            RADIUS
-0000b0b0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000b0c0: 6563 742e 6765 7428 7365 6c66 2e72 6164  ect.get(self.rad
-0000b0d0: 6975 735f 6b65 7929 290d 0a20 2020 2020  ius_key))..     
+0000b030: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+0000b040: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
+0000b050: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b080: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000b090: 494e 5445 4e53 4954 5920 3d20 5370 6f74  INTENSITY = Spot
+0000b0a0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000b0b0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+0000b0c0: 6368 325f 6b65 7929 0d0a 2020 2020 2020  ch2_key)..      
+0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b100: 2020 2020 2020 2051 5541 4c49 5459 203d         QUALITY =
-0000b110: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000b120: 742e 6765 7428 7365 6c66 2e71 7561 6c69  t.get(self.quali
-0000b130: 7479 5f6b 6579 2929 2020 2020 200d 0a20  ty_key))     .. 
+0000b0f0: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
+0000b100: 414e 5f49 4e54 454e 5349 5459 203d 2053  AN_INTENSITY = S
+0000b110: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b120: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000b130: 795f 6368 325f 6b65 7929 0d0a 2020 2020  y_ch2_key)..    
 0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b160: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
-0000b170: 5f49 4e54 454e 5349 5459 203d 2066 6c6f  _INTENSITY = flo
-0000b180: 6174 2854 4f54 414c 5f49 4e54 454e 5349  at(TOTAL_INTENSI
-0000b190: 5459 290d 0a20 2020 2020 2020 2020 2020  TY)..           
-0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
-0000b1d0: 3d20 666c 6f61 7428 4d45 414e 5f49 4e54  = float(MEAN_INT
-0000b1e0: 454e 5349 5459 290d 0a20 2020 2020 2020  ENSITY)..       
+0000b160: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
+0000b170: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1a0: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
+0000b1b0: 5f49 4e54 454e 5349 5459 203d 2053 706f  _INTENSITY = Spo
+0000b1c0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b1d0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000b1e0: 5f63 6831 5f6b 6579 290d 0a20 2020 2020  _ch1_key)..     
 0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b210: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000b220: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000b230: 5b63 656c 6c5f 6964 5d20 3d20 7b0d 0a20  [cell_id] = {.. 
-0000b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b260: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b270: 6365 6c6c 6964 5f6b 6579 3a20 696e 7428  cellid_key: int(
-0000b280: 6365 6c6c 5f69 6429 2c20 0d0a 2020 2020  cell_id), ..    
-0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2b0: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
-0000b2c0: 6d65 6964 5f6b 6579 203a 2069 6e74 2866  meid_key : int(f
-0000b2d0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b2e0: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
-0000b2f0: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
-0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b320: 2020 2020 2020 7365 6c66 2e7a 706f 7369        self.zposi
-0000b330: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
-0000b340: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b350: 662e 7a70 6f73 6964 5f6b 6579 2929 2c0d  f.zposid_key)),.
-0000b360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b380: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b390: 662e 7970 6f73 6964 5f6b 6579 203a 2066  f.yposid_key : f
-0000b3a0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b3b0: 6765 7428 7365 6c66 2e79 706f 7369 645f  get(self.yposid_
-0000b3c0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000b210: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000b220: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000b230: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000b240: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000b250: 7479 5f63 6831 5f6b 6579 290d 0a20 2020  ty_ch1_key)..   
+0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b280: 2020 2020 2020 2020 2052 4144 4955 5320           RADIUS 
+0000b290: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000b2a0: 6374 2e67 6574 2873 656c 662e 7261 6469  ct.get(self.radi
+0000b2b0: 7573 5f6b 6579 2929 0d0a 2020 2020 2020  us_key))..      
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2e0: 2020 2020 2020 5155 414c 4954 5920 3d20        QUALITY = 
+0000b2f0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000b300: 2e67 6574 2873 656c 662e 7175 616c 6974  .get(self.qualit
+0000b310: 795f 6b65 7929 2920 2020 2020 0d0a 2020  y_key))     ..  
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000b350: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000b360: 7428 544f 5441 4c5f 494e 5445 4e53 4954  t(TOTAL_INTENSIT
+0000b370: 5929 0d0a 2020 2020 2020 2020 2020 2020  Y)..            
+0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3a0: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000b3b0: 2066 6c6f 6174 284d 4541 4e5f 494e 5445   float(MEAN_INTE
+0000b3c0: 4e53 4954 5929 0d0a 2020 2020 2020 2020  NSITY)..        
 0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3f0: 2020 2020 7365 6c66 2e78 706f 7369 645f      self.xposid_
-0000b400: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-0000b410: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b420: 7870 6f73 6964 5f6b 6579 2929 2c0d 0a20  xposid_key)),.. 
+0000b3f0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000b400: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000b410: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
+0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b460: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000b470: 6b65 7920 3a20 544f 5441 4c5f 494e 5445  key : TOTAL_INTE
-0000b480: 4e53 4954 592c 0d0a 2020 2020 2020 2020  NSITY,..        
-0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4b0: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
-0000b4c0: 7465 6e73 6974 795f 6b65 7920 3a20 4d45  tensity_key : ME
-0000b4d0: 414e 5f49 4e54 454e 5349 5459 2c0d 0a20  AN_INTENSITY,.. 
+0000b440: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000b450: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
+0000b460: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b490: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+0000b4a0: 6569 645f 6b65 7920 3a20 696e 7428 666c  eid_key : int(fl
+0000b4b0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000b4c0: 6574 2873 656c 662e 6672 616d 6569 645f  et(self.frameid_
+0000b4d0: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
 0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b510: 7261 6469 7573 5f6b 6579 203a 2052 4144  radius_key : RAD
-0000b520: 4955 532c 0d0a 2020 2020 2020 2020 2020  IUS,..          
-0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b500: 2020 2020 2073 656c 662e 7a70 6f73 6964       self.zposid
+0000b510: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000b520: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b530: 2e7a 706f 7369 645f 6b65 7929 292c 0d0a  .zposid_key)),..
 0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
-0000b560: 6579 203a 2051 5541 4c49 5459 0d0a 2020  ey : QUALITY..  
-0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b590: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-0000b5a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b5b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000b5c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5e0: 2020 2020 200d 0a0d 0a20 2020 2064 6566       ....    def
-0000b5f0: 205f 7370 6f74 5f63 6f6d 7075 7465 7228   _spot_computer(
-0000b600: 7365 6c66 2c20 6672 616d 6529 3a0d 0a0d  self, frame):...
-0000b610: 0a20 2020 2020 2020 2020 2066 6f72 2053  .          for S
-0000b620: 706f 746f 626a 6563 7420 696e 2066 7261  potobject in fra
-0000b630: 6d65 2e66 696e 6461 6c6c 2827 5370 6f74  me.findall('Spot
-0000b640: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000b650: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-0000b660: 7265 6174 6520 6f62 6a65 6374 2077 6974  reate object wit
-0000b670: 6820 756e 6971 7565 2063 656c 6c20 4944  h unique cell ID
-0000b680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b690: 2020 2020 2020 2020 2020 6365 6c6c 5f69            cell_i
-0000b6a0: 6420 3d20 696e 7428 5370 6f74 6f62 6a65  d = int(Spotobje
-0000b6b0: 6374 2e67 6574 2873 656c 662e 7370 6f74  ct.get(self.spot
-0000b6c0: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
+0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b570: 2e79 706f 7369 645f 6b65 7920 3a20 666c  .yposid_key : fl
+0000b580: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000b590: 6574 2873 656c 662e 7970 6f73 6964 5f6b  et(self.yposid_k
+0000b5a0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5d0: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+0000b5e0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000b5f0: 626a 6563 742e 6765 7428 7365 6c66 2e78  bject.get(self.x
+0000b600: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b630: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000b640: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+0000b650: 6579 203a 2054 4f54 414c 5f49 4e54 454e  ey : TOTAL_INTEN
+0000b660: 5349 5459 2c0d 0a20 2020 2020 2020 2020  SITY,..         
+0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
+0000b6a0: 656e 7369 7479 5f6b 6579 203a 204d 4541  ensity_key : MEA
+0000b6b0: 4e5f 494e 5445 4e53 4954 592c 0d0a 2020  N_INTENSITY,..  
+0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6e0: 2020 2320 4765 7420 7468 6520 545a 5958    # Get the TZYX
-0000b6f0: 206c 6f63 6174 696f 6e20 6f66 2074 6865   location of the
-0000b700: 2063 656c 6c73 2069 6e20 7468 6174 2066   cells in that f
-0000b710: 7261 6d65 0d0a 2020 2020 2020 2020 2020  rame..          
-0000b720: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000b730: 2073 656c 662e 6465 7465 6374 6f72 6368   self.detectorch
-0000b740: 616e 6e65 6c20 3d3d 2031 3a0d 0a20 2020  annel == 1:..   
+0000b6e0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000b6f0: 6164 6975 735f 6b65 7920 3a20 5241 4449  adius_key : RADI
+0000b700: 5553 2c0d 0a20 2020 2020 2020 2020 2020  US,..           
+0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b730: 2073 656c 662e 7175 616c 6974 795f 6b65   self.quality_ke
+0000b740: 7920 3a20 5155 414c 4954 590d 0a20 2020  y : QUALITY..   
 0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000b770: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b780: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000b790: 6974 795f 6368 325f 6b65 7929 2069 7320  ity_ch2_key) is 
-0000b7a0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b770: 2020 2020 207d 0d0a 2020 2020 2020 200d       }..       .
+0000b780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b790: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000b7a0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7d0: 2020 2054 4f54 414c 5f49 4e54 454e 5349     TOTAL_INTENSI
-0000b7e0: 5459 203d 2066 6c6f 6174 2853 706f 746f  TY = float(Spoto
-0000b7f0: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
-0000b800: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
-0000b810: 6832 5f6b 6579 2929 0d0a 2020 2020 2020  h2_key))..      
-0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b840: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
-0000b850: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000b860: 6563 742e 6765 7428 7365 6c66 2e6d 6561  ect.get(self.mea
-0000b870: 6e5f 696e 7465 6e73 6974 795f 6368 325f  n_intensity_ch2_
-0000b880: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000b7c0: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+0000b7d0: 5f73 706f 745f 636f 6d70 7574 6572 2873  _spot_computer(s
+0000b7e0: 656c 662c 2066 7261 6d65 293a 0d0a 0d0a  elf, frame):....
+0000b7f0: 2020 2020 2020 2020 2020 666f 7220 5370            for Sp
+0000b800: 6f74 6f62 6a65 6374 2069 6e20 6672 616d  otobject in fram
+0000b810: 652e 6669 6e64 616c 6c28 2753 706f 7427  e.findall('Spot'
+0000b820: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000b830: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+0000b840: 6561 7465 206f 626a 6563 7420 7769 7468  eate object with
+0000b850: 2075 6e69 7175 6520 6365 6c6c 2049 440d   unique cell ID.
+0000b860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b870: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
+0000b880: 203d 2069 6e74 2853 706f 746f 626a 6563   = int(Spotobjec
+0000b890: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
+0000b8a0: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
 0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8d0: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
-0000b8e0: 5349 5459 203d 202d 310d 0a20 2020 2020  SITY = -1..     
-0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b910: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
-0000b920: 203d 202d 3120 2020 2020 2020 0d0a 2020   = -1       ..  
+0000b8c0: 2023 2047 6574 2074 6865 2054 5a59 5820   # Get the TZYX 
+0000b8d0: 6c6f 6361 7469 6f6e 206f 6620 7468 6520  location of the 
+0000b8e0: 6365 6c6c 7320 696e 2074 6861 7420 6672  cells in that fr
+0000b8f0: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
+0000b900: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000b910: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
+0000b920: 6e6e 656c 203d 3d20 313a 0d0a 2020 2020  nnel == 1:..    
 0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 2020 2020 2020 656c 7365 3a20 2020 2020        else:     
-0000b950: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b970: 2020 2020 2069 6620 5370 6f74 6f62 6a65       if Spotobje
-0000b980: 6374 2e67 6574 2873 656c 662e 746f 7461  ct.get(self.tota
-0000b990: 6c5f 696e 7465 6e73 6974 795f 6368 315f  l_intensity_ch1_
-0000b9a0: 6b65 7929 2069 7320 6e6f 7420 4e6f 6e65  key) is not None
-0000b9b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9d0: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
-0000b9e0: 5f49 4e54 454e 5349 5459 203d 2066 6c6f  _INTENSITY = flo
-0000b9f0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000ba00: 7428 7365 6c66 2e74 6f74 616c 5f69 6e74  t(self.total_int
-0000ba10: 656e 7369 7479 5f63 6831 5f6b 6579 2929  ensity_ch1_key))
-0000ba20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba40: 2020 2020 2020 2020 2020 4d45 414e 5f49            MEAN_I
-0000ba50: 4e54 454e 5349 5459 203d 2066 6c6f 6174  NTENSITY = float
-0000ba60: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000ba70: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000ba80: 6974 795f 6368 315f 6b65 7929 290d 0a20  ity_ch1_key)).. 
+0000b940: 2020 2020 2020 2020 2020 2020 6966 2053              if S
+0000b950: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b960: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000b970: 7479 5f63 6832 5f6b 6579 2920 6973 206e  ty_ch2_key) is n
+0000b980: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9b0: 2020 544f 5441 4c5f 494e 5445 4e53 4954    TOTAL_INTENSIT
+0000b9c0: 5920 3d20 666c 6f61 7428 5370 6f74 6f62  Y = float(Spotob
+0000b9d0: 6a65 6374 2e67 6574 2873 656c 662e 746f  ject.get(self.to
+0000b9e0: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
+0000b9f0: 325f 6b65 7929 290d 0a20 2020 2020 2020  2_key))..       
+0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba20: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000ba30: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000ba40: 6374 2e67 6574 2873 656c 662e 6d65 616e  ct.get(self.mean
+0000ba50: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
+0000ba60: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba80: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
 0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baa0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000bab0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bad0: 2020 2020 2020 2020 2020 2020 2020 544f                TO
-0000bae0: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
-0000baf0: 2d31 0d0a 2020 2020 2020 2020 2020 2020  -1..            
-0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb10: 2020 2020 2020 2020 2020 2020 4d45 414e              MEAN
-0000bb20: 5f49 4e54 454e 5349 5459 203d 202d 3120  _INTENSITY = -1 
-0000bb30: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bab0: 2020 2020 544f 5441 4c5f 494e 5445 4e53      TOTAL_INTENS
+0000bac0: 4954 5920 3d20 2d31 0d0a 2020 2020 2020  ITY = -1..      
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baf0: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000bb00: 3d20 2d31 2020 2020 2020 200d 0a20 2020  = -1       ..   
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2020 2065 6c73 653a 2020 2020 2020       else:      
+0000bb30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb70: 2020 2020 2020 5241 4449 5553 203d 2066        RADIUS = f
-0000bb80: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000bb90: 6765 7428 7365 6c66 2e72 6164 6975 735f  get(self.radius_
-0000bba0: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2051                 Q
-0000bbc0: 5541 4c49 5459 203d 2066 6c6f 6174 2853  UALITY = float(S
-0000bbd0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000bbe0: 6c66 2e71 7561 6c69 7479 5f6b 6579 2929  lf.quality_key))
-0000bbf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bc00: 2020 2020 2020 2020 2020 7465 7374 6c6f            testlo
-0000bc10: 6361 7469 6f6e 203d 2028 666c 6f61 7428  cation = (float(
-0000bc20: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000bc30: 656c 662e 7a70 6f73 6964 5f6b 6579 2929  elf.zposid_key))
-0000bc40: 2c20 666c 6f61 7428 5370 6f74 6f62 6a65  , float(Spotobje
-0000bc50: 6374 2e67 6574 2873 656c 662e 7970 6f73  ct.get(self.ypos
-0000bc60: 6964 5f6b 6579 2929 2c20 2066 6c6f 6174  id_key)),  float
-0000bc70: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000bc80: 7365 6c66 2e78 706f 7369 645f 6b65 7929  self.xposid_key)
-0000bc90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000bca0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-0000bcb0: 6520 3d20 5370 6f74 6f62 6a65 6374 2e67  e = Spotobject.g
-0000bcc0: 6574 2873 656c 662e 6672 616d 6569 645f  et(self.frameid_
-0000bcd0: 6b65 7929 0d0a 2020 2020 2020 2020 2020  key)..          
-0000bce0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0000bcf0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000bd00: 2c20 6d61 736b 6365 6e74 726f 6964 203d  , maskcentroid =
-0000bd10: 2073 656c 662e 5f67 6574 5f62 6f75 6e64   self._get_bound
-0000bd20: 6172 795f 6469 7374 2866 7261 6d65 2c20  ary_dist(frame, 
-0000bd30: 7465 7374 6c6f 6361 7469 6f6e 290d 0a20  testlocation).. 
+0000bb50: 2020 2020 6966 2053 706f 746f 626a 6563      if Spotobjec
+0000bb60: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
+0000bb70: 5f69 6e74 656e 7369 7479 5f63 6831 5f6b  _intensity_ch1_k
+0000bb80: 6579 2920 6973 206e 6f74 204e 6f6e 653a  ey) is not None:
+0000bb90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbb0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000bbc0: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000bbd0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000bbe0: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
+0000bbf0: 6e73 6974 795f 6368 315f 6b65 7929 290d  nsity_ch1_key)).
+0000bc00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc20: 2020 2020 2020 2020 204d 4541 4e5f 494e           MEAN_IN
+0000bc30: 5445 4e53 4954 5920 3d20 666c 6f61 7428  TENSITY = float(
+0000bc40: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000bc50: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000bc60: 7479 5f63 6831 5f6b 6579 2929 0d0a 2020  ty_ch1_key))..  
+0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc80: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000bc90: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcb0: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
+0000bcc0: 414c 5f49 4e54 454e 5349 5459 203d 202d  AL_INTENSITY = -
+0000bcd0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcf0: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
+0000bd00: 494e 5445 4e53 4954 5920 3d20 2d31 2020  INTENSITY = -1  
+0000bd10: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-0000bd80: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000bd90: 6c5f 6964 5d20 3d20 7b0d 0a20 2020 2020  l_id] = {..     
-0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
-0000bdc0: 6964 5f6b 6579 3a20 696e 7428 6365 6c6c  id_key: int(cell
-0000bdd0: 5f69 6429 2c20 0d0a 2020 2020 2020 2020  _id), ..        
-0000bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdf0: 2020 2020 7365 6c66 2e66 7261 6d65 6964      self.frameid
-0000be00: 5f6b 6579 203a 2069 6e74 2866 6c6f 6174  _key : int(float
-0000be10: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000be20: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-0000be30: 2929 292c 0d0a 2020 2020 2020 2020 2020  ))),..          
-0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be50: 2020 7365 6c66 2e7a 706f 7369 645f 6b65    self.zposid_ke
-0000be60: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000be70: 6a65 6374 2e67 6574 2873 656c 662e 7a70  ject.get(self.zp
-0000be80: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
-0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bea0: 2020 2020 2020 2020 2073 656c 662e 7970           self.yp
-0000beb0: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
-0000bec0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000bed0: 7365 6c66 2e79 706f 7369 645f 6b65 7929  self.yposid_key)
-0000bee0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf00: 7365 6c66 2e78 706f 7369 645f 6b65 7920  self.xposid_key 
-0000bf10: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
-0000bf20: 6374 2e67 6574 2873 656c 662e 7870 6f73  ct.get(self.xpos
-0000bf30: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000bd50: 2020 2020 2052 4144 4955 5320 3d20 666c       RADIUS = fl
+0000bd60: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000bd70: 6574 2873 656c 662e 7261 6469 7573 5f6b  et(self.radius_k
+0000bd80: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000bd90: 2020 2020 2020 2020 2020 2020 2020 5155                QU
+0000bda0: 414c 4954 5920 3d20 666c 6f61 7428 5370  ALITY = float(Sp
+0000bdb0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000bdc0: 662e 7175 616c 6974 795f 6b65 7929 290d  f.quality_key)).
+0000bdd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bde0: 2020 2020 2020 2020 2074 6573 746c 6f63           testloc
+0000bdf0: 6174 696f 6e20 3d20 2866 6c6f 6174 2853  ation = (float(S
+0000be00: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000be10: 6c66 2e7a 706f 7369 645f 6b65 7929 292c  lf.zposid_key)),
+0000be20: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000be30: 742e 6765 7428 7365 6c66 2e79 706f 7369  t.get(self.yposi
+0000be40: 645f 6b65 7929 292c 2020 666c 6f61 7428  d_key)),  float(
+0000be50: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000be60: 656c 662e 7870 6f73 6964 5f6b 6579 2929  elf.xposid_key))
+0000be70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000be80: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+0000be90: 203d 2053 706f 746f 626a 6563 742e 6765   = Spotobject.ge
+0000bea0: 7428 7365 6c66 2e66 7261 6d65 6964 5f6b  t(self.frameid_k
+0000beb0: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
+0000bec0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+0000bed0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
+0000bee0: 206d 6173 6b63 656e 7472 6f69 6420 3d20   maskcentroid = 
+0000bef0: 7365 6c66 2e5f 6765 745f 626f 756e 6461  self._get_bounda
+0000bf00: 7279 5f64 6973 7428 6672 616d 652c 2074  ry_dist(frame, t
+0000bf10: 6573 746c 6f63 6174 696f 6e29 0d0a 2020  estlocation)..  
+0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf50: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-0000bf60: 6c5f 696e 7465 6e73 6974 795f 6b65 7920  l_intensity_key 
-0000bf70: 3a20 544f 5441 4c5f 494e 5445 4e53 4954  : TOTAL_INTENSIT
-0000bf80: 592c 0d0a 2020 2020 2020 2020 2020 2020  Y,..            
-0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfa0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000bfb0: 6974 795f 6b65 7920 3a20 4d45 414e 5f49  ity_key : MEAN_I
-0000bfc0: 4e54 454e 5349 5459 2c0d 0a20 2020 2020  NTENSITY,..     
-0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfe0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-0000bff0: 7573 5f6b 6579 203a 2052 4144 4955 532c  us_key : RADIUS,
-0000c000: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c010: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c020: 6c66 2e71 7561 6c69 7479 5f6b 6579 203a  lf.quality_key :
-0000c030: 2051 5541 4c49 5459 2c0d 0a20 2020 2020   QUALITY,..     
-0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c050: 2020 2020 2020 2073 656c 662e 6469 7374         self.dist
-0000c060: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
-0000c070: 6579 3a20 666c 6f61 7428 6469 7374 616e  ey: float(distan
-0000c080: 6365 5f63 656c 6c5f 6d61 736b 292c 0d0a  ce_cell_mask),..
-0000c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c0b0: 2e6d 6173 6b63 656e 7472 6f69 645f 7a5f  .maskcentroid_z_
-0000c0c0: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
-0000c0d0: 656e 7472 6f69 645b 305d 292c 0d0a 2020  entroid[0]),..  
-0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000c100: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
-0000c110: 793a 2066 6c6f 6174 286d 6173 6b63 656e  y: float(maskcen
-0000c120: 7472 6f69 645b 315d 292c 0d0a 2020 2020  troid[1]),..    
-0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c140: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-0000c150: 6b63 656e 7472 6f69 645f 785f 6b65 793a  kcentroid_x_key:
-0000c160: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
-0000c170: 6f69 645b 325d 2920 0d0a 2020 2020 2020  oid[2]) ..      
-0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c190: 2020 7d0d 0a20 2020 2020 2020 0d0a 2020    }..       ..  
-0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000c1c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000c1d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c200: 2020 2020 0d0a 0d0a 2020 2020 0d0a 2020      ....    ..  
-0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
-0000c230: 6620 5f67 6574 5f6d 6173 7465 725f 786d  f _get_master_xm
-0000c240: 6c5f 6461 7461 2873 656c 6629 3a0d 0a20  l_data(self):.. 
-0000c250: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000c260: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
-0000c270: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-0000c280: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000c290: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-0000c2a0: 616e 6e65 6c5f 786d 6c5f 636f 6e74 656e  annel_xml_conten
-0000c2b0: 7420 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  t = self.xml_con
-0000c2c0: 7465 6e74 0d0a 2020 2020 2020 2020 2020  tent..          
-0000c2d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c2e0: 2e78 6d6c 5f74 7265 6520 3d20 6574 2e70  .xml_tree = et.p
-0000c2f0: 6172 7365 2873 656c 662e 786d 6c5f 7061  arse(self.xml_pa
-0000c300: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
-0000c310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c320: 786d 6c5f 726f 6f74 203d 2073 656c 662e  xml_root = self.
-0000c330: 786d 6c5f 7472 6565 2e67 6574 726f 6f74  xml_tree.getroot
-0000c340: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000c350: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000c360: 6861 6e6e 656c 5f78 6d6c 5f6e 616d 6520  hannel_xml_name 
-0000c370: 3d20 2773 6563 6f6e 645f 6368 616e 6e65  = 'second_channe
-0000c380: 6c5f 2720 2b20 6f73 2e70 6174 682e 7370  l_' + os.path.sp
-0000c390: 6c69 7465 7874 286f 732e 7061 7468 2e62  litext(os.path.b
-0000c3a0: 6173 656e 616d 6528 7365 6c66 2e78 6d6c  asename(self.xml
-0000c3b0: 5f70 6174 6829 295b 305d 202b 2027 2e78  _path))[0] + '.x
-0000c3c0: 6d6c 270d 0a20 2020 2020 2020 2020 2020  ml'..           
-0000c3d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c3e0: 6368 616e 6e65 6c5f 786d 6c5f 7061 7468  channel_xml_path
-0000c3f0: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-0000c400: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
-0000c410: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000c420: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-0000c430: 7265 6174 655f 6368 616e 6e65 6c5f 7472  reate_channel_tr
-0000c440: 6565 2829 0d0a 0d0a 2020 2020 2020 2020  ee()....        
-0000c450: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-0000c460: 6f62 6a65 6374 7320 3d20 7b7d 0d0a 2020  objects = {}..  
-0000c470: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000c480: 6e69 7175 655f 7072 6f70 6572 7469 6573  nique_properties
-0000c490: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-0000c4a0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-0000c4b0: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
-0000c4c0: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
-0000c4d0: 696e 6754 7261 636b 4964 7320 3d20 5b5d  ingTrackIds = []
-0000c4e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000c4f0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000c500: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000c510: 2020 2020 7365 6c66 2e61 6c6c 5f74 7261      self.all_tra
-0000c520: 636b 5f70 726f 7065 7274 6965 7320 3d20  ck_properties = 
-0000c530: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000c540: 7365 6c66 2e73 706c 6974 5f70 6f69 6e74  self.split_point
-0000c550: 735f 7469 6d65 7320 3d20 5b5d 0d0a 0d0a  s_times = []....
-0000c560: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000c570: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000c580: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-0000c590: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000c5a0: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000c5b0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000c5c0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000c5d0: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000c5e0: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
-0000c5f0: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000c600: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000c610: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-0000c620: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-0000c630: 6170 7065 6e64 2873 656c 662e 5472 6163  append(self.Trac
-0000c640: 6b69 6442 6f78 290d 0a20 2020 2020 2020  kidBox)..       
-0000c650: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
-0000c660: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
-0000c670: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
-0000c680: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0000c690: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-0000c6a0: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
-0000c6b0: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
-0000c6c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000c6d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c6e0: 2020 2020 2073 656c 662e 5370 6f74 6f62       self.Spotob
-0000c6f0: 6a65 6374 7320 3d20 7365 6c66 2e78 6d6c  jects = self.xml
-0000c700: 5f63 6f6e 7465 6e74 2e66 696e 6428 274d  _content.find('M
-0000c710: 6f64 656c 2729 2e66 696e 6428 2741 6c6c  odel').find('All
-0000c720: 5370 6f74 7327 290d 0a20 2020 2020 2020  Spots')..       
-0000c730: 2020 2020 2023 2045 7874 7261 6374 2074       # Extract t
-0000c740: 6865 2074 7261 636b 7320 6672 6f6d 2078  he tracks from x
-0000c750: 6d6c 0d0a 2020 2020 2020 2020 2020 2020  ml..            
-0000c760: 7365 6c66 2e74 7261 636b 7320 3d20 7365  self.tracks = se
-0000c770: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000c780: 696e 6428 224d 6f64 656c 2229 2e66 696e  ind("Model").fin
-0000c790: 6428 2241 6c6c 5472 6163 6b73 2229 0d0a  d("AllTracks")..
-0000c7a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c7b0: 2e73 6574 7469 6e67 7320 3d20 7365 6c66  .settings = self
-0000c7c0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000c7d0: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
-0000c7e0: 6e64 2822 496d 6167 6544 6174 6122 290d  nd("ImageData").
-0000c7f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c800: 662e 7863 616c 6962 7261 7469 6f6e 203d  f.xcalibration =
-0000c810: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
-0000c820: 696e 6773 2e67 6574 2822 7069 7865 6c77  ings.get("pixelw
-0000c830: 6964 7468 2229 290d 0a20 2020 2020 2020  idth"))..       
-0000c840: 2020 2020 2073 656c 662e 7963 616c 6962       self.ycalib
-0000c850: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
-0000c860: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000c870: 2822 7069 7865 6c68 6569 6768 7422 2929  ("pixelheight"))
-0000c880: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000c890: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
-0000c8a0: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
-0000c8b0: 7469 6e67 732e 6765 7428 2276 6f78 656c  tings.get("voxel
-0000c8c0: 6465 7074 6822 2929 0d0a 2020 2020 2020  depth"))..      
-0000c8d0: 2020 2020 2020 7365 6c66 2e74 6361 6c69        self.tcali
-0000c8e0: 6272 6174 696f 6e20 3d20 696e 7428 666c  bration = int(fl
-0000c8f0: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
-0000c900: 732e 6765 7428 2274 696d 6569 6e74 6572  s.get("timeinter
-0000c910: 7661 6c22 2929 290d 0a20 2020 2020 2020  val")))..       
-0000c920: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
-0000c930: 6f72 7365 7474 696e 6773 203d 2073 656c  orsettings = sel
-0000c940: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-0000c950: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
-0000c960: 696e 6428 2244 6574 6563 746f 7253 6574  ind("DetectorSet
-0000c970: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
-0000c980: 2020 2020 2073 656c 662e 6261 7369 6373       self.basics
-0000c990: 6574 7469 6e67 7320 3d20 7365 6c66 2e78  ettings = self.x
-0000c9a0: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
-0000c9b0: 2253 6574 7469 6e67 7322 292e 6669 6e64  "Settings").find
-0000c9c0: 2822 4261 7369 6353 6574 7469 6e67 7322  ("BasicSettings"
-0000c9d0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0000c9e0: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
-0000c9f0: 6e65 6c20 3d20 696e 7428 666c 6f61 7428  nel = int(float(
-0000ca00: 7365 6c66 2e64 6574 6563 746f 7273 6574  self.detectorset
-0000ca10: 7469 6e67 732e 6765 7428 2254 4152 4745  tings.get("TARGE
-0000ca20: 545f 4348 414e 4e45 4c22 2929 290d 0a20  T_CHANNEL"))).. 
-0000ca30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ca40: 7473 7461 7274 203d 2069 6e74 2866 6c6f  tstart = int(flo
-0000ca50: 6174 2873 656c 662e 6261 7369 6373 6574  at(self.basicset
-0000ca60: 7469 6e67 732e 6765 7428 2274 7374 6172  tings.get("tstar
-0000ca70: 7422 2929 290d 0a20 2020 2020 2020 2020  t")))..         
-0000ca80: 2020 2073 656c 662e 7465 6e64 203d 2069     self.tend = i
-0000ca90: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
-0000caa0: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
-0000cab0: 2274 656e 6422 2929 2920 2020 2020 200d  "tend")))      .
-0000cac0: 0a0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
-0000cad0: 7269 6e74 2827 4974 6572 6174 696e 6720  rint('Iterating 
-0000cae0: 6f76 6572 2073 706f 7473 2069 6e20 6672  over spots in fr
-0000caf0: 616d 6527 290d 0a20 2020 2020 2020 2020  ame')..         
-0000cb00: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-0000cb10: 300d 0a20 2020 2020 2020 2020 2020 2066  0..            f
-0000cb20: 7574 7572 6573 203d 205b 5d0d 0a0d 0a20  utures = [].... 
-0000cb30: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000cb40: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-0000cb50: 6573 2e54 6872 6561 6450 6f6f 6c45 7865  es.ThreadPoolExe
-0000cb60: 6375 746f 7228 6d61 785f 776f 726b 6572  cutor(max_worker
-0000cb70: 7320 3d20 6f73 2e63 7075 5f63 6f75 6e74  s = os.cpu_count
-0000cb80: 2829 2920 6173 2065 7865 6375 746f 723a  ()) as executor:
-0000cb90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cba0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000cbb0: 2020 2020 666f 7220 6672 616d 6520 696e      for frame in
-0000cbc0: 2073 656c 662e 5370 6f74 6f62 6a65 6374   self.Spotobject
-0000cbd0: 732e 6669 6e64 616c 6c28 2753 706f 7473  s.findall('Spots
-0000cbe0: 496e 4672 616d 6527 293a 0d0a 2020 2020  InFrame'):..    
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc00: 2020 2020 2020 2020 6675 7475 7265 732e          futures.
-0000cc10: 6170 7065 6e64 2865 7865 6375 746f 722e  append(executor.
-0000cc20: 7375 626d 6974 2873 656c 662e 5f6d 6173  submit(self._mas
-0000cc30: 7465 725f 7370 6f74 5f63 6f6d 7075 7465  ter_spot_compute
-0000cc40: 722c 2066 7261 6d65 2929 0d0a 2020 2020  r, frame))..    
-0000cc50: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000cc60: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000cc70: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc90: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000cca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccc0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000ccd0: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
-0000cce0: 6563 7469 6e67 2053 706f 7473 220d 0a20  ecting Spots".. 
-0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000cd10: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000cd20: 2e72 616e 6765 203d 2028 0d0a 2020 2020  .range = (..    
-0000cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd50: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2020 2020 2020 2020 6c65 6e28 6675 7475          len(futu
-0000cd80: 7265 7329 2c0d 0a20 2020 2020 2020 2020  res),..         
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cda0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdc0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000cdd0: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
-0000cde0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-0000cdf0: 2020 2020 2020 666f 7220 7220 696e 2063        for r in c
-0000ce00: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-0000ce10: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
-0000ce20: 7574 7572 6573 293a 0d0a 2020 2020 2020  utures):..      
-0000ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000ce50: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
-0000ce60: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce80: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000ce90: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000cea0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ced0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000cee0: 7661 6c75 6520 3d20 2073 656c 662e 636f  value =  self.co
-0000cef0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf10: 2020 2020 2072 2e72 6573 756c 7428 2920       r.result() 
-0000cf20: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-0000cf30: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000cf40: 2070 7269 6e74 2866 2749 7465 7261 7469   print(f'Iterati
-0000cf50: 6e67 206f 7665 7220 7472 6163 6b73 207b  ng over tracks {
-0000cf60: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
-0000cf70: 645f 7472 6163 6b5f 6964 7329 7d27 2920  d_track_ids)}') 
-0000cf80: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-0000cf90: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-0000cfa0: 2020 2020 2020 2020 2020 2066 7574 7572             futur
-0000cfb0: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-0000cfc0: 2020 2020 2077 6974 6820 636f 6e63 7572       with concur
-0000cfd0: 7265 6e74 2e66 7574 7572 6573 2e54 6872  rent.futures.Thr
-0000cfe0: 6561 6450 6f6f 6c45 7865 6375 746f 7228  eadPoolExecutor(
-0000cff0: 6d61 785f 776f 726b 6572 7320 3d20 6f73  max_workers = os
-0000d000: 2e63 7075 5f63 6f75 6e74 2829 2920 6173  .cpu_count()) as
-0000d010: 2065 7865 6375 746f 723a 0d0a 2020 2020   executor:..    
-0000d020: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000d030: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000d040: 7220 7472 6163 6b20 696e 2073 656c 662e  r track in self.
-0000d050: 7472 6163 6b73 2e66 696e 6461 6c6c 2827  tracks.findall('
-0000d060: 5472 6163 6b27 293a 0d0a 2020 2020 2020  Track'):..      
-0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d080: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d090: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-0000d0a0: 6b5f 6964 203d 2069 6e74 2874 7261 636b  k_id = int(track
-0000d0b0: 2e67 6574 2873 656c 662e 7472 6163 6b69  .get(self.tracki
-0000d0c0: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
-0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0e0: 2069 6620 7472 6163 6b5f 6964 2069 6e20   if track_id in 
-0000d0f0: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-0000d100: 6163 6b5f 6964 733a 0d0a 2020 2020 2020  ack_ids:..      
-0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2020 2020 2020 2020 2020 6675 7475 7265            future
-0000d130: 732e 6170 7065 6e64 2865 7865 6375 746f  s.append(executo
-0000d140: 722e 7375 626d 6974 2873 656c 662e 5f6d  r.submit(self._m
-0000d150: 6173 7465 725f 7472 6163 6b5f 636f 6d70  aster_track_comp
-0000d160: 7574 6572 2c20 7472 6163 6b2c 2074 7261  uter, track, tra
-0000d170: 636b 5f69 6429 290d 0a20 2020 2020 2020  ck_id))..       
-0000d180: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000d190: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-0000d1a0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d1f0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000d200: 6c61 6265 6c20 3d20 2243 6f6c 6c65 6374  label = "Collect
-0000d210: 696e 6720 5472 6163 6b73 220d 0a20 2020  ing Tracks"..   
-0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d230: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000d240: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-0000d250: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-0000d280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
-0000d2b0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-0000d2c0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2e0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0000bf50: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+0000bf60: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000bf70: 5f69 645d 203d 207b 0d0a 2020 2020 2020  _id] = {..      
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf90: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
+0000bfa0: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
+0000bfb0: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
+0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfd0: 2020 2073 656c 662e 6672 616d 6569 645f     self.frameid_
+0000bfe0: 6b65 7920 3a20 696e 7428 666c 6f61 7428  key : int(float(
+0000bff0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c000: 656c 662e 6672 616d 6569 645f 6b65 7929  elf.frameid_key)
+0000c010: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c030: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
+0000c040: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000c050: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
+0000c060: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c080: 2020 2020 2020 2020 7365 6c66 2e79 706f          self.ypo
+0000c090: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+0000c0a0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c0b0: 656c 662e 7970 6f73 6964 5f6b 6579 2929  elf.yposid_key))
+0000c0c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c0e0: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
+0000c0f0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000c100: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
+0000c110: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c130: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+0000c140: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
+0000c150: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
+0000c160: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c180: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000c190: 7479 5f6b 6579 203a 204d 4541 4e5f 494e  ty_key : MEAN_IN
+0000c1a0: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
+0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1c0: 2020 2020 2020 7365 6c66 2e72 6164 6975        self.radiu
+0000c1d0: 735f 6b65 7920 3a20 5241 4449 5553 2c0d  s_key : RADIUS,.
+0000c1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c200: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+0000c210: 5155 414c 4954 592c 0d0a 2020 2020 2020  QUALITY,..      
+0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c230: 2020 2020 2020 7365 6c66 2e64 6973 7461        self.dista
+0000c240: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+0000c250: 793a 2066 6c6f 6174 2864 6973 7461 6e63  y: float(distanc
+0000c260: 655f 6365 6c6c 5f6d 6173 6b29 2c0d 0a20  e_cell_mask),.. 
+0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c280: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c290: 6d61 736b 6365 6e74 726f 6964 5f7a 5f6b  maskcentroid_z_k
+0000c2a0: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+0000c2b0: 6e74 726f 6964 5b30 5d29 2c0d 0a20 2020  ntroid[0]),..   
+0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2d0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000c2e0: 736b 6365 6e74 726f 6964 5f79 5f6b 6579  skcentroid_y_key
+0000c2f0: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+0000c300: 726f 6964 5b31 5d29 2c0d 0a20 2020 2020  roid[1]),..     
+0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c320: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
+0000c330: 6365 6e74 726f 6964 5f78 5f6b 6579 3a20  centroid_x_key: 
+0000c340: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
+0000c350: 6964 5b32 5d29 200d 0a20 2020 2020 2020  id[2]) ..       
+0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c370: 207d 0d0a 2020 2020 2020 200d 0a20 2020   }..       ..   
+0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c390: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000c3a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000c3b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3e0: 2020 200d 0a0d 0a20 2020 200d 0a20 2020     ....    ..   
+0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 2020 2020 200d 0a0d 0a20 2020 2064 6566       ....    def
+0000c410: 205f 6765 745f 6d61 7374 6572 5f78 6d6c   _get_master_xml
+0000c420: 5f64 6174 6128 7365 6c66 293a 0d0a 2020  _data(self):..  
+0000c430: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000c440: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
+0000c450: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
+0000c460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c470: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+0000c480: 6e6e 656c 5f78 6d6c 5f63 6f6e 7465 6e74  nnel_xml_content
+0000c490: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
+0000c4a0: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
+0000c4b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c4c0: 786d 6c5f 7472 6565 203d 2065 742e 7061  xml_tree = et.pa
+0000c4d0: 7273 6528 7365 6c66 2e78 6d6c 5f70 6174  rse(self.xml_pat
+0000c4e0: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+0000c4f0: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
+0000c500: 6d6c 5f72 6f6f 7420 3d20 7365 6c66 2e78  ml_root = self.x
+0000c510: 6d6c 5f74 7265 652e 6765 7472 6f6f 7428  ml_tree.getroot(
+0000c520: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000c530: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+0000c540: 616e 6e65 6c5f 786d 6c5f 6e61 6d65 203d  annel_xml_name =
+0000c550: 2027 7365 636f 6e64 5f63 6861 6e6e 656c   'second_channel
+0000c560: 5f27 202b 206f 732e 7061 7468 2e73 706c  _' + os.path.spl
+0000c570: 6974 6578 7428 6f73 2e70 6174 682e 6261  itext(os.path.ba
+0000c580: 7365 6e61 6d65 2873 656c 662e 786d 6c5f  sename(self.xml_
+0000c590: 7061 7468 2929 5b30 5d20 2b20 272e 786d  path))[0] + '.xm
+0000c5a0: 6c27 0d0a 2020 2020 2020 2020 2020 2020  l'..            
+0000c5b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000c5c0: 6861 6e6e 656c 5f78 6d6c 5f70 6174 6820  hannel_xml_path 
+0000c5d0: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
+0000c5e0: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
+0000c5f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c600: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+0000c610: 6561 7465 5f63 6861 6e6e 656c 5f74 7265  eate_channel_tre
+0000c620: 6528 290d 0a0d 0a20 2020 2020 2020 2020  e()....         
+0000c630: 2020 2073 656c 662e 756e 6971 7565 5f6f     self.unique_o
+0000c640: 626a 6563 7473 203d 207b 7d0d 0a20 2020  bjects = {}..   
+0000c650: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000c660: 6971 7565 5f70 726f 7065 7274 6965 7320  ique_properties 
+0000c670: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+0000c680: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+0000c690: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+0000c6a0: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+0000c6b0: 6e67 5472 6163 6b49 6473 203d 205b 5d0d  ngTrackIds = [].
+0000c6c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c6d0: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
+0000c6e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000c6f0: 2020 2073 656c 662e 616c 6c5f 7472 6163     self.all_trac
+0000c700: 6b5f 7072 6f70 6572 7469 6573 203d 205b  k_properties = [
+0000c710: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+0000c720: 656c 662e 7370 6c69 745f 706f 696e 7473  elf.split_points
+0000c730: 5f74 696d 6573 203d 205b 5d0d 0a0d 0a20  _times = [].... 
+0000c740: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000c750: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000c760: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
+0000c770: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
+0000c780: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+0000c790: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
+0000c7a0: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
+0000c7b0: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+0000c7c0: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
+0000c7d0: 636b 4964 732e 6170 7065 6e64 284e 6f6e  ckIds.append(Non
+0000c7e0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+0000c7f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000c800: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
+0000c810: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
+0000c820: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
+0000c830: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000c840: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
+0000c850: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
+0000c860: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000c870: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+0000c880: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
+0000c890: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
+0000c8a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000c8b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000c8c0: 2020 2020 7365 6c66 2e53 706f 746f 626a      self.Spotobj
+0000c8d0: 6563 7473 203d 2073 656c 662e 786d 6c5f  ects = self.xml_
+0000c8e0: 636f 6e74 656e 742e 6669 6e64 2827 4d6f  content.find('Mo
+0000c8f0: 6465 6c27 292e 6669 6e64 2827 416c 6c53  del').find('AllS
+0000c900: 706f 7473 2729 0d0a 2020 2020 2020 2020  pots')..        
+0000c910: 2020 2020 2320 4578 7472 6163 7420 7468      # Extract th
+0000c920: 6520 7472 6163 6b73 2066 726f 6d20 786d  e tracks from xm
+0000c930: 6c0d 0a20 2020 2020 2020 2020 2020 2073  l..            s
+0000c940: 656c 662e 7472 6163 6b73 203d 2073 656c  elf.tracks = sel
+0000c950: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000c960: 6e64 2822 4d6f 6465 6c22 292e 6669 6e64  nd("Model").find
+0000c970: 2822 416c 6c54 7261 636b 7322 290d 0a20  ("AllTracks").. 
+0000c980: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c990: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
+0000c9a0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000c9b0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
+0000c9c0: 6428 2249 6d61 6765 4461 7461 2229 0d0a  d("ImageData")..
+0000c9d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c9e0: 2e78 6361 6c69 6272 6174 696f 6e20 3d20  .xcalibration = 
+0000c9f0: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
+0000ca00: 6e67 732e 6765 7428 2270 6978 656c 7769  ngs.get("pixelwi
+0000ca10: 6474 6822 2929 0d0a 2020 2020 2020 2020  dth"))..        
+0000ca20: 2020 2020 7365 6c66 2e79 6361 6c69 6272      self.ycalibr
+0000ca30: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
+0000ca40: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
+0000ca50: 2270 6978 656c 6865 6967 6874 2229 290d  "pixelheight")).
+0000ca60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ca70: 662e 7a63 616c 6962 7261 7469 6f6e 203d  f.zcalibration =
+0000ca80: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
+0000ca90: 696e 6773 2e67 6574 2822 766f 7865 6c64  ings.get("voxeld
+0000caa0: 6570 7468 2229 290d 0a20 2020 2020 2020  epth"))..       
+0000cab0: 2020 2020 2073 656c 662e 7463 616c 6962       self.tcalib
+0000cac0: 7261 7469 6f6e 203d 2069 6e74 2866 6c6f  ration = int(flo
+0000cad0: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000cae0: 2e67 6574 2822 7469 6d65 696e 7465 7276  .get("timeinterv
+0000caf0: 616c 2229 2929 0d0a 2020 2020 2020 2020  al")))..        
+0000cb00: 2020 2020 7365 6c66 2e64 6574 6563 746f      self.detecto
+0000cb10: 7273 6574 7469 6e67 7320 3d20 7365 6c66  rsettings = self
+0000cb20: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
+0000cb30: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
+0000cb40: 6e64 2822 4465 7465 6374 6f72 5365 7474  nd("DetectorSett
+0000cb50: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
+0000cb60: 2020 2020 7365 6c66 2e62 6173 6963 7365      self.basicse
+0000cb70: 7474 696e 6773 203d 2073 656c 662e 786d  ttings = self.xm
+0000cb80: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
+0000cb90: 5365 7474 696e 6773 2229 2e66 696e 6428  Settings").find(
+0000cba0: 2242 6173 6963 5365 7474 696e 6773 2229  "BasicSettings")
+0000cbb0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000cbc0: 6c66 2e64 6574 6563 746f 7263 6861 6e6e  lf.detectorchann
+0000cbd0: 656c 203d 2069 6e74 2866 6c6f 6174 2873  el = int(float(s
+0000cbe0: 656c 662e 6465 7465 6374 6f72 7365 7474  elf.detectorsett
+0000cbf0: 696e 6773 2e67 6574 2822 5441 5247 4554  ings.get("TARGET
+0000cc00: 5f43 4841 4e4e 454c 2229 2929 0d0a 2020  _CHANNEL")))..  
+0000cc10: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000cc20: 7374 6172 7420 3d20 696e 7428 666c 6f61  start = int(floa
+0000cc30: 7428 7365 6c66 2e62 6173 6963 7365 7474  t(self.basicsett
+0000cc40: 696e 6773 2e67 6574 2822 7473 7461 7274  ings.get("tstart
+0000cc50: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
+0000cc60: 2020 7365 6c66 2e74 656e 6420 3d20 696e    self.tend = in
+0000cc70: 7428 666c 6f61 7428 7365 6c66 2e62 6173  t(float(self.bas
+0000cc80: 6963 7365 7474 696e 6773 2e67 6574 2822  icsettings.get("
+0000cc90: 7465 6e64 2229 2929 2020 2020 2020 0d0a  tend")))      ..
+0000cca0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000ccb0: 696e 7428 2749 7465 7261 7469 6e67 206f  int('Iterating o
+0000ccc0: 7665 7220 7370 6f74 7320 696e 2066 7261  ver spots in fra
+0000ccd0: 6d65 2729 0d0a 2020 2020 2020 2020 2020  me')..          
+0000cce0: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
+0000ccf0: 0d0a 2020 2020 2020 2020 2020 2020 6675  ..            fu
+0000cd00: 7475 7265 7320 3d20 5b5d 0d0a 0d0a 2020  tures = []....  
+0000cd10: 2020 2020 2020 2020 2020 7769 7468 2063            with c
+0000cd20: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+0000cd30: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
+0000cd40: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
+0000cd50: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
+0000cd60: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
+0000cd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000cd90: 2020 2066 6f72 2066 7261 6d65 2069 6e20     for frame in 
+0000cda0: 7365 6c66 2e53 706f 746f 626a 6563 7473  self.Spotobjects
+0000cdb0: 2e66 696e 6461 6c6c 2827 5370 6f74 7349  .findall('SpotsI
+0000cdc0: 6e46 7261 6d65 2729 3a0d 0a20 2020 2020  nFrame'):..     
+0000cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cde0: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
+0000cdf0: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
+0000ce00: 7562 6d69 7428 7365 6c66 2e5f 6d61 7374  ubmit(self._mast
+0000ce10: 6572 5f73 706f 745f 636f 6d70 7574 6572  er_spot_computer
+0000ce20: 2c20 6672 616d 6529 290d 0a20 2020 2020  , frame))..     
+0000ce30: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000ce40: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
+0000ce50: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000ce60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce70: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cea0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000ceb0: 722e 6c61 6265 6c20 3d20 2243 6f6c 6c65  r.label = "Colle
+0000cec0: 6374 696e 6720 5370 6f74 7322 0d0a 2020  cting Spots"..  
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cee0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cef0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000cf00: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
+0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf20: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0000cf30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf50: 2020 2020 2020 206c 656e 2866 7574 7572         len(futur
+0000cf60: 6573 292c 0d0a 2020 2020 2020 2020 2020  es),..          
+0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf80: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfa0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000cfb0: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+0000cfc0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000cfd0: 2020 2020 2066 6f72 2072 2069 6e20 636f       for r in co
+0000cfe0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+0000cff0: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
+0000d000: 7475 7265 7329 3a0d 0a20 2020 2020 2020  tures):..       
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000d030: 756e 7420 3d20 7365 6c66 2e63 6f75 6e74  unt = self.count
+0000d040: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000d070: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000d080: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d0b0: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+0000d0c0: 616c 7565 203d 2020 7365 6c66 2e63 6f75  alue =  self.cou
+0000d0d0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0f0: 2020 2020 722e 7265 7375 6c74 2829 2020      r.result()  
+0000d100: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000d110: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d120: 7072 696e 7428 6627 4974 6572 6174 696e  print(f'Iteratin
+0000d130: 6720 6f76 6572 2074 7261 636b 7320 7b6c  g over tracks {l
+0000d140: 656e 2873 656c 662e 6669 6c74 6572 6564  en(self.filtered
+0000d150: 5f74 7261 636b 5f69 6473 297d 2729 2020  _track_ids)}')  
+0000d160: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d170: 6c66 2e63 6f75 6e74 203d 2030 0d0a 2020  lf.count = 0..  
+0000d180: 2020 2020 2020 2020 2020 6675 7475 7265            future
+0000d190: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000d1a0: 2020 2020 7769 7468 2063 6f6e 6375 7272      with concurr
+0000d1b0: 656e 742e 6675 7475 7265 732e 5468 7265  ent.futures.Thre
+0000d1c0: 6164 506f 6f6c 4578 6563 7574 6f72 286d  adPoolExecutor(m
+0000d1d0: 6178 5f77 6f72 6b65 7273 203d 206f 732e  ax_workers = os.
+0000d1e0: 6370 755f 636f 756e 7428 2929 2061 7320  cpu_count()) as 
+0000d1f0: 6578 6563 7574 6f72 3a0d 0a20 2020 2020  executor:..     
+0000d200: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000d210: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000d220: 2074 7261 636b 2069 6e20 7365 6c66 2e74   track in self.t
+0000d230: 7261 636b 732e 6669 6e64 616c 6c28 2754  racks.findall('T
+0000d240: 7261 636b 2729 3a0d 0a20 2020 2020 2020  rack'):..       
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d260: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000d270: 2020 2020 2020 2020 2020 2074 7261 636b             track
+0000d280: 5f69 6420 3d20 696e 7428 7472 6163 6b2e  _id = int(track.
+0000d290: 6765 7428 7365 6c66 2e74 7261 636b 6964  get(self.trackid
+0000d2a0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2c0: 6966 2074 7261 636b 5f69 6420 696e 2073  if track_id in s
+0000d2d0: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000d2e0: 636b 5f69 6473 3a0d 0a20 2020 2020 2020  ck_ids:..       
 0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d300: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000d310: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
-0000d320: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-0000d330: 2020 2020 2020 666f 7220 7220 696e 2063        for r in c
-0000d340: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-0000d350: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
-0000d360: 7574 7572 6573 293a 0d0a 2020 2020 2020  utures):..      
-0000d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d380: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000d390: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
-0000d3a0: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
+0000d300: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+0000d310: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
+0000d320: 2e73 7562 6d69 7428 7365 6c66 2e5f 6d61  .submit(self._ma
+0000d330: 7374 6572 5f74 7261 636b 5f63 6f6d 7075  ster_track_compu
+0000d340: 7465 722c 2074 7261 636b 2c20 7472 6163  ter, track, trac
+0000d350: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
+0000d360: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d370: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000d380: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 0000d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3c0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000d3d0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000d3e0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d400: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d410: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000d420: 7661 6c75 6520 3d20 7365 6c66 2e63 6f75  value = self.cou
-0000d430: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+0000d3c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d3d0: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+0000d3e0: 6162 656c 203d 2022 436f 6c6c 6563 7469  abel = "Collecti
+0000d3f0: 6e67 2054 7261 636b 7322 0d0a 2020 2020  ng Tracks"..    
+0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d420: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
+0000d430: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
 0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d450: 2020 2020 722e 7265 7375 6c74 2829 0d0a      r.result()..
-0000d460: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000d470: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000d480: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
-0000d490: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-0000d4a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d4b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4d0: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
-0000d4e0: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
-0000d4f0: 786d 6c28 290d 0a20 2020 2020 2020 2020  xml()..         
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0000d520: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-0000d530: 6c66 2e67 7261 7068 5f73 706c 6974 2e69  lf.graph_split.i
-0000d540: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+0000d450: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
+0000d460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d480: 2020 2020 206c 656e 2873 656c 662e 6669       len(self.fi
+0000d490: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+0000d4a0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4c0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4e0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000d4f0: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
+0000d500: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+0000d510: 2020 2020 2066 6f72 2072 2069 6e20 636f       for r in co
+0000d520: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+0000d530: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
+0000d540: 7475 7265 7329 3a0d 0a20 2020 2020 2020  tures):..       
 0000d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d560: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d580: 2020 6461 7567 6874 6572 5f74 7261 636b    daughter_track
-0000d590: 5f69 6420 3d20 2069 6e74 2866 6c6f 6174  _id =  int(float
-0000d5a0: 2873 7472 2873 656c 662e 756e 6971 7565  (str(self.unique
-0000d5b0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000d5c0: 5b69 6e74 2866 6c6f 6174 286b 2929 5d5b  [int(float(k))][
-0000d5d0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
-0000d5e0: 795d 2929 290d 0a20 2020 2020 2020 2020  y])))..         
-0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d600: 2020 2070 6172 656e 745f 7472 6163 6b5f     parent_track_
-0000d610: 6964 203d 2069 6e74 2866 6c6f 6174 2873  id = int(float(s
-0000d620: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
-0000d630: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-0000d640: 6e74 2866 6c6f 6174 2876 2929 5d5b 7365  nt(float(v))][se
-0000d650: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
-0000d660: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d680: 2073 656c 662e 6772 6170 685f 7472 6163   self.graph_trac
-0000d690: 6b73 5b64 6175 6768 7465 725f 7472 6163  ks[daughter_trac
-0000d6a0: 6b5f 6964 5d20 3d20 7061 7265 6e74 5f74  k_id] = parent_t
-0000d6b0: 7261 636b 5f69 640d 0a0d 0a20 2020 2020  rack_id....     
-0000d6c0: 2020 2020 2020 2070 7269 6e74 2827 6765         print('ge
-0000d6d0: 7474 696e 6720 6174 7472 6962 7574 6573  tting attributes
-0000d6e0: 2729 2020 2020 2020 2020 2020 2020 2020  ')              
-0000d6f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d700: 7365 6c66 2e5f 6765 745f 6174 7472 6962  self._get_attrib
-0000d710: 7574 6573 2829 0d0a 2020 2020 2020 2020  utes()..        
-0000d720: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000d730: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
-0000d740: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000d750: 2074 7261 636b 5f69 6420 696e 2073 656c   track_id in sel
-0000d760: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
-0000d770: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
-0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d790: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000d7a0: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000d7b0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d560: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000d570: 756e 7420 3d20 7365 6c66 2e63 6f75 6e74  unt = self.count
+0000d580: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
+0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5a0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000d5b0: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000d5c0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d5f0: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+0000d600: 616c 7565 203d 2073 656c 662e 636f 756e  alue = self.coun
+0000d610: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d630: 2020 2072 2e72 6573 756c 7428 290d 0a20     r.result().. 
+0000d640: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000d650: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000d660: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
+0000d670: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a20  ge is not None: 
+0000d680: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000d690: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6b0: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
+0000d6c0: 7365 636f 6e64 5f63 6861 6e6e 656c 5f78  second_channel_x
+0000d6d0: 6d6c 2829 0d0a 2020 2020 2020 2020 2020  ml()..          
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000d700: 666f 7220 286b 2c76 2920 696e 2073 656c  for (k,v) in sel
+0000d710: 662e 6772 6170 685f 7370 6c69 742e 6974  f.graph_split.it
+0000d720: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d760: 2064 6175 6768 7465 725f 7472 6163 6b5f   daughter_track_
+0000d770: 6964 203d 2020 696e 7428 666c 6f61 7428  id =  int(float(
+0000d780: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
+0000d790: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000d7a0: 696e 7428 666c 6f61 7428 6b29 295d 5b73  int(float(k))][s
+0000d7b0: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000d7c0: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
 0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7e0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000d7f0: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
-0000d800: 224a 7573 7420 6f6e 6520 6d6f 7265 2074  "Just one more t
-0000d810: 6869 6e67 220d 0a20 2020 2020 2020 2020  hing"..         
-0000d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d830: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d840: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000d850: 2e72 616e 6765 203d 2028 0d0a 2020 2020  .range = (..    
-0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d880: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
-0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8c0: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
-0000d8d0: 645f 7472 6163 6b5f 6964 7329 2c0d 0a20  d_track_ids),.. 
-0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d900: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d930: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000d940: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
-0000d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 2020 7061 7265 6e74 5f74 7261 636b 5f69    parent_track_i
+0000d7f0: 6420 3d20 696e 7428 666c 6f61 7428 7374  d = int(float(st
+0000d800: 7228 7365 6c66 2e75 6e69 7175 655f 7370  r(self.unique_sp
+0000d810: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+0000d820: 7428 666c 6f61 7428 7629 295d 5b73 656c  t(float(v))][sel
+0000d830: 662e 756e 6971 7565 6964 5f6b 6579 5d29  f.uniqueid_key])
+0000d840: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d860: 7365 6c66 2e67 7261 7068 5f74 7261 636b  self.graph_track
+0000d870: 735b 6461 7567 6874 6572 5f74 7261 636b  s[daughter_track
+0000d880: 5f69 645d 203d 2070 6172 656e 745f 7472  _id] = parent_tr
+0000d890: 6163 6b5f 6964 0d0a 0d0a 2020 2020 2020  ack_id....      
+0000d8a0: 2020 2020 2020 7072 696e 7428 2767 6574        print('get
+0000d8b0: 7469 6e67 2061 7474 7269 6275 7465 7327  ting attributes'
+0000d8c0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+0000d8d0: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
+0000d8e0: 656c 662e 5f67 6574 5f61 7474 7269 6275  elf._get_attribu
+0000d8f0: 7465 7328 290d 0a20 2020 2020 2020 2020  tes()..         
+0000d900: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d910: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
+0000d920: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d930: 7472 6163 6b5f 6964 2069 6e20 7365 6c66  track_id in self
+0000d940: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+0000d950: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
 0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d970: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000d980: 6e74 203d 2073 656c 662e 636f 756e 7420  nt = self.count 
-0000d990: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
+0000d970: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000d980: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000d990: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
 0000d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000d9c0: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
-0000d9d0: 616c 7565 203d 2073 656c 662e 636f 756e  alue = self.coun
-0000d9e0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da00: 2020 2020 2020 2073 656c 662e 5f66 696e         self._fin
-0000da10: 616c 5f74 7261 636b 7328 7472 6163 6b5f  al_tracks(track_
-0000da20: 6964 2920 0d0a 0d0a 2020 2020 2020 2020  id) ....        
-0000da30: 2020 2020 6966 2073 656c 662e 666f 7572      if self.four
-0000da40: 6965 723a 0d0a 2020 2020 2020 2020 2020  ier:..          
-0000da50: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-0000da60: 636f 6d70 7574 696e 6720 466f 7572 6965  computing Fourie
-0000da70: 7227 290d 0a20 2020 2020 2020 2020 2020  r')..           
-0000da80: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-0000da90: 6d70 7574 655f 7068 656e 6f74 7970 6573  mpute_phenotypes
-0000daa0: 2829 2020 2020 2020 2020 2020 2020 2020  ()              
-0000dab0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000dac0: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
-0000dad0: 6d70 6f72 616c 5f70 6c6f 7473 5f74 7261  mporal_plots_tra
-0000dae0: 636b 6d61 7465 2829 2020 2020 2020 2020  ckmate()        
-0000daf0: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f63  ......    def _c
-0000db00: 7265 6174 655f 7365 636f 6e64 5f63 6861  reate_second_cha
-0000db10: 6e6e 656c 5f78 6d6c 2873 656c 6629 3a0d  nnel_xml(self):.
-0000db20: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
+0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9c0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000d9d0: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
+0000d9e0: 4a75 7374 206f 6e65 206d 6f72 6520 7468  Just one more th
+0000d9f0: 696e 6722 0d0a 2020 2020 2020 2020 2020  ing"..          
+0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000da20: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000da30: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
+0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da60: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
+0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da90: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000daa0: 656e 2873 656c 662e 6669 6c74 6572 6564  en(self.filtered
+0000dab0: 5f74 7261 636b 5f69 6473 292c 0d0a 2020  _track_ids),..  
+0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dae0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db10: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000db20: 7373 5f62 6172 2e73 686f 7728 290d 0a20  ss_bar.show().. 
 0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 7072 696e 7428 2754 7261 6e73 6665    print('Transfe
-0000db50: 7272 696e 6720 584d 4c27 2920 2020 0d0a  rring XML')   ..
-0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db70: 2020 2020 6368 616e 6e65 6c5f 6669 6c74      channel_filt
-0000db80: 6572 6564 5f74 7261 636b 7320 3d20 5b5d  ered_tracks = []
-0000db90: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbb0: 2020 666f 7220 5370 6f74 6f62 6a65 6374    for Spotobject
-0000dbc0: 2069 6e20 7365 6c66 2e78 6d6c 5f72 6f6f   in self.xml_roo
-0000dbd0: 742e 6974 6572 2827 5370 6f74 2729 3a0d  t.iter('Spot'):.
-0000dbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dbf0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-0000dc00: 6c5f 6964 203d 2069 6e74 2853 706f 746f  l_id = int(Spoto
-0000dc10: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
-0000dc20: 706f 7469 645f 6b65 7929 290d 0a20 2020  potid_key))..   
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc40: 2020 2020 2020 2020 2069 6620 6365 6c6c           if cell
-0000dc50: 5f69 6420 696e 2073 656c 662e 6368 616e  _id in self.chan
-0000dc60: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000dc70: 7072 6f70 6572 7469 6573 2e6b 6579 7328  properties.keys(
-0000dc80: 293a 2020 2020 2020 2020 0d0a 2020 2020  ):        ..    
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dca0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000dcd0: 775f 706f 7369 7469 6f6e 7820 3d20 2073  w_positionx =  s
-0000dce0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-0000dcf0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000dd00: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
-0000dd10: 2e78 706f 7369 645f 6b65 795d 0d0a 2020  .xposid_key]..  
-0000dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd40: 2020 6e65 775f 706f 7369 7469 6f6e 7920    new_positiony 
-0000dd50: 3d20 2073 656c 662e 6368 616e 6e65 6c5f  =  self.channel_
-0000dd60: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000dd70: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
-0000dd80: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-0000dd90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddb0: 2020 2020 2020 6e65 775f 706f 7369 7469        new_positi
-0000ddc0: 6f6e 7a20 3d20 2073 656c 662e 6368 616e  onz =  self.chan
-0000ddd0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000dde0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-0000ddf0: 6964 5d5b 7365 6c66 2e7a 706f 7369 645f  id][self.zposid_
-0000de00: 6b65 795d 0d0a 0d0a 2020 2020 2020 2020  key]....        
+0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db50: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+0000db60: 7420 3d20 7365 6c66 2e63 6f75 6e74 202b  t = self.count +
+0000db70: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dba0: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
+0000dbb0: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
+0000dbc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbe0: 2020 2020 2020 7365 6c66 2e5f 6669 6e61        self._fina
+0000dbf0: 6c5f 7472 6163 6b73 2874 7261 636b 5f69  l_tracks(track_i
+0000dc00: 6429 200d 0a0d 0a20 2020 2020 2020 2020  d) ....         
+0000dc10: 2020 2069 6620 7365 6c66 2e66 6f75 7269     if self.fouri
+0000dc20: 6572 3a0d 0a20 2020 2020 2020 2020 2020  er:..           
+0000dc30: 2020 2020 2020 2020 7072 696e 7428 2763          print('c
+0000dc40: 6f6d 7075 7469 6e67 2046 6f75 7269 6572  omputing Fourier
+0000dc50: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+0000dc60: 2020 2020 2020 2073 656c 662e 5f63 6f6d         self._com
+0000dc70: 7075 7465 5f70 6865 6e6f 7479 7065 7328  pute_phenotypes(
+0000dc80: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+0000dc90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000dca0: 2020 2020 2020 2073 656c 662e 5f74 656d         self._tem
+0000dcb0: 706f 7261 6c5f 706c 6f74 735f 7472 6163  poral_plots_trac
+0000dcc0: 6b6d 6174 6528 2920 2020 2020 2020 200d  kmate()        .
+0000dcd0: 0a0d 0a0d 0a20 2020 2064 6566 205f 6372  .....    def _cr
+0000dce0: 6561 7465 5f73 6563 6f6e 645f 6368 616e  eate_second_chan
+0000dcf0: 6e65 6c5f 786d 6c28 7365 6c66 293a 0d0a  nel_xml(self):..
+0000dd00: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd20: 2070 7269 6e74 2827 5472 616e 7366 6572   print('Transfer
+0000dd30: 7269 6e67 2058 4d4c 2729 2020 200d 0a20  ring XML')   .. 
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd50: 2020 2063 6861 6e6e 656c 5f66 696c 7465     channel_filte
+0000dd60: 7265 645f 7472 6163 6b73 203d 205b 5d20  red_tracks = [] 
+0000dd70: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd90: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
+0000dda0: 696e 2073 656c 662e 786d 6c5f 726f 6f74  in self.xml_root
+0000ddb0: 2e69 7465 7228 2753 706f 7427 293a 0d0a  .iter('Spot'):..
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddd0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+0000dde0: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
+0000ddf0: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
+0000de00: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
 0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de20: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000de30: 746f 7461 6c5f 696e 7465 6e73 6974 7920  total_intensity 
-0000de40: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f75  = self.channel_u
-0000de50: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000de60: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
-0000de70: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000de80: 6974 795f 6b65 795d 0d0a 2020 2020 2020  ity_key]..      
+0000de20: 2020 2020 2020 2020 6966 2063 656c 6c5f          if cell_
+0000de30: 6964 2069 6e20 7365 6c66 2e63 6861 6e6e  id in self.chann
+0000de40: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000de50: 726f 7065 7274 6965 732e 6b65 7973 2829  roperties.keys()
+0000de60: 3a20 2020 2020 2020 200d 0a20 2020 2020  :        ..     
+0000de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dea0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000deb0: 775f 6d65 616e 5f69 6e74 656e 7369 7479  w_mean_intensity
-0000dec0: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
-0000ded0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000dee0: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
-0000def0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000df00: 6974 795f 6b65 795d 0d0a 0d0a 2020 2020  ity_key]....    
+0000dea0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000deb0: 5f70 6f73 6974 696f 6e78 203d 2020 7365  _positionx =  se
+0000dec0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000ded0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000dee0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000def0: 7870 6f73 6964 5f6b 6579 5d0d 0a20 2020  xposid_key]..   
+0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df30: 6e65 775f 7261 6469 7573 203d 2073 656c  new_radius = sel
-0000df40: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000df50: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000df60: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e72  [cell_id][self.r
-0000df70: 6164 6975 735f 6b65 795d 0d0a 2020 2020  adius_key]..    
+0000df20: 206e 6577 5f70 6f73 6974 696f 6e79 203d   new_positiony =
+0000df30: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+0000df40: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000df50: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
+0000df60: 656c 662e 7970 6f73 6964 5f6b 6579 5d0d  elf.yposid_key].
+0000df70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000df80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfa0: 6e65 775f 7175 616c 6974 7920 3d20 7365  new_quality = se
-0000dfb0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-0000dfc0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000dfd0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
-0000dfe0: 7175 616c 6974 795f 6b65 795d 0d0a 2020  quality_key]..  
+0000df90: 2020 2020 206e 6577 5f70 6f73 6974 696f       new_positio
+0000dfa0: 6e7a 203d 2020 7365 6c66 2e63 6861 6e6e  nz =  self.chann
+0000dfb0: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000dfc0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+0000dfd0: 645d 5b73 656c 662e 7a70 6f73 6964 5f6b  d][self.zposid_k
+0000dfe0: 6579 5d0d 0a0d 0a20 2020 2020 2020 2020  ey]....         
 0000dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e010: 2020 6e65 775f 6469 7374 616e 6365 5f63    new_distance_c
-0000e020: 656c 6c5f 6d61 736b 203d 2073 656c 662e  ell_mask = self.
-0000e030: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000e040: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000e050: 656c 6c5f 6964 5d5b 7365 6c66 2e64 6973  ell_id][self.dis
-0000e060: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-0000e070: 6b65 795d 0d0a 0d0a 2020 2020 2020 2020  key]....        
-0000e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e090: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000e0a0: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000e0b0: 7870 6f73 6964 5f6b 6579 2c20 7374 7228  xposid_key, str(
-0000e0c0: 6e65 775f 706f 7369 7469 6f6e 7829 2920  new_positionx)) 
-0000e0d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0f0: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
-0000e100: 6a65 6374 2e73 6574 2873 656c 662e 7970  ject.set(self.yp
-0000e110: 6f73 6964 5f6b 6579 2c20 7374 7228 6e65  osid_key, str(ne
-0000e120: 775f 706f 7369 7469 6f6e 7929 290d 0a20  w_positiony)).. 
-0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e150: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
-0000e160: 7428 7365 6c66 2e7a 706f 7369 645f 6b65  t(self.zposid_ke
-0000e170: 792c 2073 7472 286e 6577 5f70 6f73 6974  y, str(new_posit
-0000e180: 696f 6e7a 2929 0d0a 0d0a 2020 2020 2020  ionz))....      
-0000e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1a0: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-0000e1b0: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
-0000e1c0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000e1d0: 795f 6b65 792c 2073 7472 286e 6577 5f74  y_key, str(new_t
-0000e1e0: 6f74 616c 5f69 6e74 656e 7369 7479 2929  otal_intensity))
-0000e1f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e210: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
-0000e220: 626a 6563 742e 7365 7428 7365 6c66 2e6d  bject.set(self.m
-0000e230: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
-0000e240: 792c 2073 7472 286e 6577 5f6d 6561 6e5f  y, str(new_mean_
-0000e250: 696e 7465 6e73 6974 7929 290d 0a20 2020  intensity))..   
+0000e000: 2020 2020 2020 2020 2020 206e 6577 5f74             new_t
+0000e010: 6f74 616c 5f69 6e74 656e 7369 7479 203d  otal_intensity =
+0000e020: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+0000e030: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000e040: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
+0000e050: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000e060: 7479 5f6b 6579 5d0d 0a20 2020 2020 2020  ty_key]..       
+0000e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e080: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000e090: 5f6d 6561 6e5f 696e 7465 6e73 6974 7920  _mean_intensity 
+0000e0a0: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f75  = self.channel_u
+0000e0b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000e0c0: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
+0000e0d0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000e0e0: 7479 5f6b 6579 5d0d 0a0d 0a20 2020 2020  ty_key]....     
+0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e100: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e110: 6577 5f72 6164 6975 7320 3d20 7365 6c66  ew_radius = self
+0000e120: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000e130: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000e140: 6365 6c6c 5f69 645d 5b73 656c 662e 7261  cell_id][self.ra
+0000e150: 6469 7573 5f6b 6579 5d0d 0a20 2020 2020  dius_key]..     
+0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e170: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e180: 6577 5f71 7561 6c69 7479 203d 2073 656c  ew_quality = sel
+0000e190: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000e1a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000e1b0: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e71  [cell_id][self.q
+0000e1c0: 7561 6c69 7479 5f6b 6579 5d0d 0a20 2020  uality_key]..   
+0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 206e 6577 5f64 6973 7461 6e63 655f 6365   new_distance_ce
+0000e200: 6c6c 5f6d 6173 6b20 3d20 7365 6c66 2e63  ll_mask = self.c
+0000e210: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+0000e220: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000e230: 6c6c 5f69 645d 5b73 656c 662e 6469 7374  ll_id][self.dist
+0000e240: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+0000e250: 6579 5d0d 0a0d 0a20 2020 2020 2020 2020  ey]....         
 0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e280: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
-0000e290: 7365 6c66 2e72 6164 6975 735f 6b65 792c  self.radius_key,
-0000e2a0: 2073 7472 286e 6577 5f72 6164 6975 7329   str(new_radius)
-0000e2b0: 2920 2020 2020 0d0a 2020 2020 2020 2020  )     ..        
+0000e270: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000e280: 626a 6563 742e 7365 7428 7365 6c66 2e78  bject.set(self.x
+0000e290: 706f 7369 645f 6b65 792c 2073 7472 286e  posid_key, str(n
+0000e2a0: 6577 5f70 6f73 6974 696f 6e78 2929 2020  ew_positionx))  
+0000e2b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2d0: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000e2e0: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000e2f0: 7175 616c 6974 795f 6b65 792c 2073 7472  quality_key, str
-0000e300: 286e 6577 5f71 7561 6c69 7479 2929 0d0a  (new_quality))..
+0000e2d0: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
+0000e2e0: 6563 742e 7365 7428 7365 6c66 2e79 706f  ect.set(self.ypo
+0000e2f0: 7369 645f 6b65 792c 2073 7472 286e 6577  sid_key, str(new
+0000e300: 5f70 6f73 6974 696f 6e79 2929 0d0a 2020  _positiony))..  
 0000e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e330: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000e340: 6574 2873 656c 662e 6469 7374 616e 6365  et(self.distance
-0000e350: 5f63 656c 6c5f 6d61 736b 5f6b 6579 2c20  _cell_mask_key, 
-0000e360: 7374 7228 6e65 775f 6469 7374 616e 6365  str(new_distance
-0000e370: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
-0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3a0: 2020 7472 6163 6b5f 6964 203d 2073 656c    track_id = sel
-0000e3b0: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000e3c0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000e3d0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-0000e3e0: 656c 662e 7472 6163 6b69 645f 6b65 795d  elf.trackid_key]
-0000e3f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e410: 2020 2020 2020 6368 616e 6e65 6c5f 6669        channel_fi
-0000e420: 6c74 6572 6564 5f74 7261 636b 732e 6170  ltered_tracks.ap
-0000e430: 7065 6e64 2874 7261 636b 5f69 6429 0d0a  pend(track_id)..
+0000e330: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+0000e340: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
+0000e350: 2c20 7374 7228 6e65 775f 706f 7369 7469  , str(new_positi
+0000e360: 6f6e 7a29 290d 0a0d 0a20 2020 2020 2020  onz))....       
+0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e380: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000e390: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000e3a0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000e3b0: 5f6b 6579 2c20 7374 7228 6e65 775f 746f  _key, str(new_to
+0000e3c0: 7461 6c5f 696e 7465 6e73 6974 7929 2920  tal_intensity)) 
+0000e3d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3f0: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
+0000e400: 6a65 6374 2e73 6574 2873 656c 662e 6d65  ject.set(self.me
+0000e410: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
+0000e420: 2c20 7374 7228 6e65 775f 6d65 616e 5f69  , str(new_mean_i
+0000e430: 6e74 656e 7369 7479 2929 0d0a 2020 2020  ntensity))..    
 0000e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000e470: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
-0000e480: 6d6c 5f74 7265 652e 7772 6974 6528 6f73  ml_tree.write(os
-0000e490: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
-0000e4a0: 6368 616e 6e65 6c5f 786d 6c5f 7061 7468  channel_xml_path
-0000e4b0: 2c20 7365 6c66 2e63 6861 6e6e 656c 5f78  , self.channel_x
-0000e4c0: 6d6c 5f6e 616d 6529 2920 0d0a 0d0a 2020  ml_name)) ....  
-0000e4d0: 2020 6465 6620 5f67 6574 5f78 6d6c 5f64    def _get_xml_d
-0000e4e0: 6174 6128 7365 6c66 293a 0d0a 0d0a 2020  ata(self):....  
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000e500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e510: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
-0000e520: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
-0000e530: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e550: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000e560: 5f63 6f6e 7465 6e74 203d 2073 656c 662e  _content = self.
-0000e570: 786d 6c5f 636f 6e74 656e 740d 0a20 2020  xml_content..   
-0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e590: 2020 2073 656c 662e 786d 6c5f 7472 6565     self.xml_tree
-0000e5a0: 203d 2065 742e 7061 7273 6528 7365 6c66   = et.parse(self
-0000e5b0: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
-0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5d0: 2020 7365 6c66 2e78 6d6c 5f72 6f6f 7420    self.xml_root 
-0000e5e0: 3d20 7365 6c66 2e78 6d6c 5f74 7265 652e  = self.xml_tree.
-0000e5f0: 6765 7472 6f6f 7428 290d 0a20 2020 2020  getroot()..     
-0000e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e610: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
-0000e620: 6c5f 6e61 6d65 203d 2027 7365 636f 6e64  l_name = 'second
-0000e630: 5f63 6861 6e6e 656c 5f27 202b 206f 732e  _channel_' + os.
-0000e640: 7061 7468 2e73 706c 6974 6578 7428 6f73  path.splitext(os
-0000e650: 2e70 6174 682e 6261 7365 6e61 6d65 2873  .path.basename(s
-0000e660: 656c 662e 786d 6c5f 7061 7468 2929 5b30  elf.xml_path))[0
-0000e670: 5d20 2b20 272e 786d 6c27 0d0a 2020 2020  ] + '.xml'..    
-0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e690: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
-0000e6a0: 6d6c 5f70 6174 6820 3d20 6f73 2e70 6174  ml_path = os.pat
-0000e6b0: 682e 6469 726e 616d 6528 7365 6c66 2e78  h.dirname(self.x
-0000e6c0: 6d6c 5f70 6174 6829 0d0a 2020 2020 2020  ml_path)..      
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6e0: 7365 6c66 2e5f 6372 6561 7465 5f63 6861  self._create_cha
-0000e6f0: 6e6e 656c 5f74 7265 6528 290d 0a20 2020  nnel_tree()..   
-0000e700: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e710: 7365 6c66 2e61 7574 6f65 6e63 6f64 6572  self.autoencoder
-0000e720: 5f6d 6f64 656c 2069 7320 6e6f 7420 4e6f  _model is not No
-0000e730: 6e65 2061 6e64 2073 656c 662e 7365 675f  ne and self.seg_
-0000e740: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
-0000e750: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000e760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e770: 6d61 7374 6572 5f78 6d6c 5f63 6f6e 7465  master_xml_conte
-0000e780: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
-0000e790: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e7b0: 6c66 2e6d 6173 7465 725f 786d 6c5f 7472  lf.master_xml_tr
-0000e7c0: 6565 203d 2065 742e 7061 7273 6528 7365  ee = et.parse(se
-0000e7d0: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
+0000e460: 5370 6f74 6f62 6a65 6374 2e73 6574 2873  Spotobject.set(s
+0000e470: 656c 662e 7261 6469 7573 5f6b 6579 2c20  elf.radius_key, 
+0000e480: 7374 7228 6e65 775f 7261 6469 7573 2929  str(new_radius))
+0000e490: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4b0: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000e4c0: 626a 6563 742e 7365 7428 7365 6c66 2e71  bject.set(self.q
+0000e4d0: 7561 6c69 7479 5f6b 6579 2c20 7374 7228  uality_key, str(
+0000e4e0: 6e65 775f 7175 616c 6974 7929 290d 0a20  new_quality)).. 
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e510: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
+0000e520: 7428 7365 6c66 2e64 6973 7461 6e63 655f  t(self.distance_
+0000e530: 6365 6c6c 5f6d 6173 6b5f 6b65 792c 2073  cell_mask_key, s
+0000e540: 7472 286e 6577 5f64 6973 7461 6e63 655f  tr(new_distance_
+0000e550: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e580: 2074 7261 636b 5f69 6420 3d20 7365 6c66   track_id = self
+0000e590: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000e5a0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000e5b0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+0000e5c0: 6c66 2e74 7261 636b 6964 5f6b 6579 5d0d  lf.trackid_key].
+0000e5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5f0: 2020 2020 2063 6861 6e6e 656c 5f66 696c       channel_fil
+0000e600: 7465 7265 645f 7472 6163 6b73 2e61 7070  tered_tracks.app
+0000e610: 656e 6428 7472 6163 6b5f 6964 290d 0a20  end(track_id).. 
+0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e640: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000e650: 2020 2020 2020 2020 2073 656c 662e 786d           self.xm
+0000e660: 6c5f 7472 6565 2e77 7269 7465 286f 732e  l_tree.write(os.
+0000e670: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
+0000e680: 6861 6e6e 656c 5f78 6d6c 5f70 6174 682c  hannel_xml_path,
+0000e690: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+0000e6a0: 6c5f 6e61 6d65 2929 200d 0a0d 0a20 2020  l_name)) ....   
+0000e6b0: 2064 6566 205f 6765 745f 786d 6c5f 6461   def _get_xml_da
+0000e6c0: 7461 2873 656c 6629 3a0d 0a0d 0a20 2020  ta(self):....   
+0000e6d0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+0000e6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e6f0: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
+0000e700: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
+0000e710: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000e720: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e730: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
+0000e740: 636f 6e74 656e 7420 3d20 7365 6c66 2e78  content = self.x
+0000e750: 6d6c 5f63 6f6e 7465 6e74 0d0a 2020 2020  ml_content..    
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 7365 6c66 2e78 6d6c 5f74 7265 6520    self.xml_tree 
+0000e780: 3d20 6574 2e70 6172 7365 2873 656c 662e  = et.parse(self.
+0000e790: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
+0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7b0: 2073 656c 662e 786d 6c5f 726f 6f74 203d   self.xml_root =
+0000e7c0: 2073 656c 662e 786d 6c5f 7472 6565 2e67   self.xml_tree.g
+0000e7d0: 6574 726f 6f74 2829 0d0a 2020 2020 2020  etroot()..      
 0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7f0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
-0000e800: 5f78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  _xml_root = self
-0000e810: 2e6d 6173 7465 725f 786d 6c5f 7472 6565  .master_xml_tree
-0000e820: 2e67 6574 726f 6f74 2829 0d0a 2020 2020  .getroot()..    
-0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e840: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
-0000e850: 6d6c 5f6e 616d 6520 3d20 276d 6173 7465  ml_name = 'maste
-0000e860: 725f 2720 2b20 7365 6c66 2e6d 6173 7465  r_' + self.maste
-0000e870: 725f 6578 7472 615f 6e61 6d65 2020 2b20  r_extra_name  + 
-0000e880: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
-0000e890: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
-0000e8a0: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
-0000e8b0: 295b 305d 202b 2027 2e78 6d6c 270d 0a20  )[0] + '.xml'.. 
-0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8d0: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
-0000e8e0: 725f 786d 6c5f 7061 7468 203d 206f 732e  r_xml_path = os.
-0000e8f0: 7061 7468 2e64 6972 6e61 6d65 2873 656c  path.dirname(sel
-0000e900: 662e 786d 6c5f 7061 7468 2920 2020 2020  f.xml_path)     
-0000e910: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000e920: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000e930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e940: 2e75 6e69 7175 655f 6f62 6a65 6374 7320  .unique_objects 
-0000e950: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-0000e960: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-0000e970: 655f 7072 6f70 6572 7469 6573 203d 207b  e_properties = {
-0000e980: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-0000e990: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-0000e9a0: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
-0000e9b0: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
-0000e9c0: 6976 6964 696e 6754 7261 636b 4964 7320  ividingTrackIds 
-0000e9d0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000e9e0: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
-0000e9f0: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
-0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea10: 7365 6c66 2e61 6c6c 5f74 7261 636b 5f70  self.all_track_p
-0000ea20: 726f 7065 7274 6965 7320 3d20 5b5d 0d0a  roperties = []..
-0000ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea40: 7365 6c66 2e73 706c 6974 5f70 6f69 6e74  self.split_point
-0000ea50: 735f 7469 6d65 7320 3d20 5b5d 0d0a 0d0a  s_times = []....
-0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ea80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000ea90: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
-0000eaa0: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
-0000eab0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000eac0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000ead0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000eae0: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000eaf0: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
-0000eb00: 616c 5472 6163 6b49 6473 2e61 7070 656e  alTrackIds.appen
-0000eb10: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
-0000eb20: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000eb30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000eb40: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
-0000eb50: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
-0000eb60: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
-0000eb70: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
-0000eb80: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
-0000eb90: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
-0000eba0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0000ebb0: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
-0000ebc0: 7261 636b 4964 732e 6170 7065 6e64 2873  rackIds.append(s
-0000ebd0: 656c 662e 5472 6163 6b69 6442 6f78 290d  elf.TrackidBox).
-0000ebe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ebf0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000ec00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000ec10: 2020 2020 2073 656c 662e 5370 6f74 6f62       self.Spotob
-0000ec20: 6a65 6374 7320 3d20 7365 6c66 2e78 6d6c  jects = self.xml
-0000ec30: 5f63 6f6e 7465 6e74 2e66 696e 6428 274d  _content.find('M
-0000ec40: 6f64 656c 2729 2e66 696e 6428 2741 6c6c  odel').find('All
-0000ec50: 5370 6f74 7327 290d 0a20 2020 2020 2020  Spots')..       
-0000ec60: 2020 2020 2020 2020 2023 2045 7874 7261           # Extra
-0000ec70: 6374 2074 6865 2074 7261 636b 7320 6672  ct the tracks fr
-0000ec80: 6f6d 2078 6d6c 0d0a 2020 2020 2020 2020  om xml..        
-0000ec90: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-0000eca0: 636b 7320 3d20 7365 6c66 2e78 6d6c 5f63  cks = self.xml_c
-0000ecb0: 6f6e 7465 6e74 2e66 696e 6428 224d 6f64  ontent.find("Mod
-0000ecc0: 656c 2229 2e66 696e 6428 2241 6c6c 5472  el").find("AllTr
-0000ecd0: 6163 6b73 2229 0d0a 2020 2020 2020 2020  acks")..        
-0000ece0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000ecf0: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
-0000ed00: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
-0000ed10: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
-0000ed20: 496d 6167 6544 6174 6122 290d 0a20 2020  ImageData")..   
-0000ed30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ed40: 662e 7863 616c 6962 7261 7469 6f6e 203d  f.xcalibration =
-0000ed50: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
-0000ed60: 696e 6773 2e67 6574 2822 7069 7865 6c77  ings.get("pixelw
-0000ed70: 6964 7468 2229 290d 0a20 2020 2020 2020  idth"))..       
-0000ed80: 2020 2020 2020 2020 2073 656c 662e 7963           self.yc
-0000ed90: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
-0000eda0: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
-0000edb0: 2e67 6574 2822 7069 7865 6c68 6569 6768  .get("pixelheigh
-0000edc0: 7422 2929 0d0a 2020 2020 2020 2020 2020  t"))..          
-0000edd0: 2020 2020 2020 7365 6c66 2e7a 6361 6c69        self.zcali
-0000ede0: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
-0000edf0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
-0000ee00: 7428 2276 6f78 656c 6465 7074 6822 2929  t("voxeldepth"))
-0000ee10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ee20: 2020 7365 6c66 2e74 6361 6c69 6272 6174    self.tcalibrat
-0000ee30: 696f 6e20 3d20 696e 7428 666c 6f61 7428  ion = int(float(
-0000ee40: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
-0000ee50: 7428 2274 696d 6569 6e74 6572 7661 6c22  t("timeinterval"
-0000ee60: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000ee70: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
-0000ee80: 6f72 7365 7474 696e 6773 203d 2073 656c  orsettings = sel
-0000ee90: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-0000eea0: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
-0000eeb0: 696e 6428 2244 6574 6563 746f 7253 6574  ind("DetectorSet
-0000eec0: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
-0000eed0: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
-0000eee0: 7369 6373 6574 7469 6e67 7320 3d20 7365  sicsettings = se
-0000eef0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000ef00: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
-0000ef10: 6669 6e64 2822 4261 7369 6353 6574 7469  find("BasicSetti
-0000ef20: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
-0000ef30: 2020 2020 2020 2073 656c 662e 6465 7465         self.dete
-0000ef40: 6374 6f72 6368 616e 6e65 6c20 3d20 696e  ctorchannel = in
-0000ef50: 7428 666c 6f61 7428 7365 6c66 2e64 6574  t(float(self.det
-0000ef60: 6563 746f 7273 6574 7469 6e67 732e 6765  ectorsettings.ge
-0000ef70: 7428 2254 4152 4745 545f 4348 414e 4e45  t("TARGET_CHANNE
-0000ef80: 4c22 2929 290d 0a20 2020 2020 2020 2020  L")))..         
-0000ef90: 2020 2020 2020 2073 656c 662e 7473 7461         self.tsta
-0000efa0: 7274 203d 2069 6e74 2866 6c6f 6174 2873  rt = int(float(s
-0000efb0: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
-0000efc0: 732e 6765 7428 2274 7374 6172 7422 2929  s.get("tstart"))
-0000efd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000efe0: 2020 2073 656c 662e 7465 6e64 203d 2069     self.tend = i
-0000eff0: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
-0000f000: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
-0000f010: 2274 656e 6422 2929 290d 0a20 2020 2020  "tend")))..     
-0000f020: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f030: 5f67 6574 5f62 6f75 6e64 6172 795f 706f  _get_boundary_po
-0000f040: 696e 7473 2829 0d0a 2020 2020 2020 2020  ints()..        
-0000f050: 2020 2020 2020 2020 7072 696e 7428 2749          print('I
-0000f060: 7465 7261 7469 6e67 206f 7665 7220 7370  terating over sp
-0000f070: 6f74 7320 696e 2066 7261 6d65 2729 0d0a  ots in frame')..
-0000f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f090: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
-0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0b0: 6675 7475 7265 7320 3d20 5b5d 0d0a 0d0a  futures = []....
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0d0: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
-0000f0e0: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
-0000f0f0: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
-0000f100: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
-0000f110: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
-0000f120: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
-0000f130: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f150: 2066 6f72 2066 7261 6d65 2069 6e20 7365   for frame in se
-0000f160: 6c66 2e53 706f 746f 626a 6563 7473 2e66  lf.Spotobjects.f
-0000f170: 696e 6461 6c6c 2827 5370 6f74 7349 6e46  indall('SpotsInF
-0000f180: 7261 6d65 2729 3a0d 0a20 2020 2020 2020  rame'):..       
-0000f190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1a0: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
-0000f1b0: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
-0000f1c0: 626d 6974 2873 656c 662e 5f73 706f 745f  bmit(self._spot_
-0000f1d0: 636f 6d70 7574 6572 2c20 6672 616d 6529  computer, frame)
-0000f1e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f1f0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000f200: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000f210: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f230: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f260: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000f270: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
-0000f280: 6563 7469 6e67 2053 706f 7473 220d 0a20  ecting Spots".. 
-0000f290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2b0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000f2c0: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
-0000f2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2f0: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
-0000f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f320: 2020 2020 6c65 6e28 6675 7475 7265 7329      len(futures)
-0000f330: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f350: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f370: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f380: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000f390: 7368 6f77 2829 0d0a 0d0a 2020 2020 2020  show()....      
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000f3b0: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
-0000f3c0: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
-0000f3d0: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
-0000f3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f400: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000f410: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
-0000f420: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+0000e7f0: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
+0000e800: 5f6e 616d 6520 3d20 2773 6563 6f6e 645f  _name = 'second_
+0000e810: 6368 616e 6e65 6c5f 2720 2b20 6f73 2e70  channel_' + os.p
+0000e820: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
+0000e830: 7061 7468 2e62 6173 656e 616d 6528 7365  path.basename(se
+0000e840: 6c66 2e78 6d6c 5f70 6174 6829 295b 305d  lf.xml_path))[0]
+0000e850: 202b 2027 2e78 6d6c 270d 0a20 2020 2020   + '.xml'..     
+0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e870: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+0000e880: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
+0000e890: 2e64 6972 6e61 6d65 2873 656c 662e 786d  .dirname(self.xm
+0000e8a0: 6c5f 7061 7468 290d 0a20 2020 2020 2020  l_path)..       
+0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e8c0: 656c 662e 5f63 7265 6174 655f 6368 616e  elf._create_chan
+0000e8d0: 6e65 6c5f 7472 6565 2829 0d0a 2020 2020  nel_tree()..    
+0000e8e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000e8f0: 656c 662e 6175 746f 656e 636f 6465 725f  elf.autoencoder_
+0000e900: 6d6f 6465 6c20 6973 206e 6f74 204e 6f6e  model is not Non
+0000e910: 6520 616e 6420 7365 6c66 2e73 6567 5f69  e and self.seg_i
+0000e920: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+0000e930: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000e940: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000e950: 6173 7465 725f 786d 6c5f 636f 6e74 656e  aster_xml_conten
+0000e960: 7420 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  t = self.xml_con
+0000e970: 7465 6e74 0d0a 2020 2020 2020 2020 2020  tent..          
+0000e980: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e990: 662e 6d61 7374 6572 5f78 6d6c 5f74 7265  f.master_xml_tre
+0000e9a0: 6520 3d20 6574 2e70 6172 7365 2873 656c  e = et.parse(sel
+0000e9b0: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
+0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9d0: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
+0000e9e0: 786d 6c5f 726f 6f74 203d 2073 656c 662e  xml_root = self.
+0000e9f0: 6d61 7374 6572 5f78 6d6c 5f74 7265 652e  master_xml_tree.
+0000ea00: 6765 7472 6f6f 7428 290d 0a20 2020 2020  getroot()..     
+0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea20: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
+0000ea30: 6c5f 6e61 6d65 203d 2027 6d61 7374 6572  l_name = 'master
+0000ea40: 5f27 202b 2073 656c 662e 6d61 7374 6572  _' + self.master
+0000ea50: 5f65 7874 7261 5f6e 616d 6520 202b 206f  _extra_name  + o
+0000ea60: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
+0000ea70: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
+0000ea80: 2873 656c 662e 786d 6c5f 7061 7468 2929  (self.xml_path))
+0000ea90: 5b30 5d20 2b20 272e 786d 6c27 0d0a 2020  [0] + '.xml'..  
+0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eab0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+0000eac0: 5f78 6d6c 5f70 6174 6820 3d20 6f73 2e70  _xml_path = os.p
+0000ead0: 6174 682e 6469 726e 616d 6528 7365 6c66  ath.dirname(self
+0000eae0: 2e78 6d6c 5f70 6174 6829 2020 2020 2020  .xml_path)      
+0000eaf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000eb00: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000eb10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000eb20: 756e 6971 7565 5f6f 626a 6563 7473 203d  unique_objects =
+0000eb30: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+0000eb40: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+0000eb50: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+0000eb60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000eb70: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+0000eb80: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+0000eb90: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
+0000eba0: 7669 6469 6e67 5472 6163 6b49 6473 203d  vidingTrackIds =
+0000ebb0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000ebc0: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
+0000ebd0: 5472 6163 6b49 6473 203d 205b 5d0d 0a20  TrackIds = [].. 
+0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ebf0: 656c 662e 616c 6c5f 7472 6163 6b5f 7072  elf.all_track_pr
+0000ec00: 6f70 6572 7469 6573 203d 205b 5d0d 0a20  operties = [].. 
+0000ec10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ec20: 656c 662e 7370 6c69 745f 706f 696e 7473  elf.split_points
+0000ec30: 5f74 696d 6573 203d 205b 5d0d 0a0d 0a20  _times = [].... 
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000ec50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ec60: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000ec70: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+0000ec80: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
+0000ec90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000eca0: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
+0000ecb0: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
+0000ecc0: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+0000ecd0: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000ece0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000ecf0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000ed00: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000ed10: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+0000ed20: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
+0000ed30: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
+0000ed40: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000ed50: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000ed60: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
+0000ed70: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
+0000ed80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ed90: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
+0000eda0: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
+0000edb0: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
+0000edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ede0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000edf0: 2020 2020 7365 6c66 2e53 706f 746f 626a      self.Spotobj
+0000ee00: 6563 7473 203d 2073 656c 662e 786d 6c5f  ects = self.xml_
+0000ee10: 636f 6e74 656e 742e 6669 6e64 2827 4d6f  content.find('Mo
+0000ee20: 6465 6c27 292e 6669 6e64 2827 416c 6c53  del').find('AllS
+0000ee30: 706f 7473 2729 0d0a 2020 2020 2020 2020  pots')..        
+0000ee40: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
+0000ee50: 7420 7468 6520 7472 6163 6b73 2066 726f  t the tracks fro
+0000ee60: 6d20 786d 6c0d 0a20 2020 2020 2020 2020  m xml..         
+0000ee70: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000ee80: 6b73 203d 2073 656c 662e 786d 6c5f 636f  ks = self.xml_co
+0000ee90: 6e74 656e 742e 6669 6e64 2822 4d6f 6465  ntent.find("Mode
+0000eea0: 6c22 292e 6669 6e64 2822 416c 6c54 7261  l").find("AllTra
+0000eeb0: 636b 7322 290d 0a20 2020 2020 2020 2020  cks")..         
+0000eec0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000eed0: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
+0000eee0: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
+0000eef0: 7474 696e 6773 2229 2e66 696e 6428 2249  ttings").find("I
+0000ef00: 6d61 6765 4461 7461 2229 0d0a 2020 2020  mageData")..    
+0000ef10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ef20: 2e78 6361 6c69 6272 6174 696f 6e20 3d20  .xcalibration = 
+0000ef30: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
+0000ef40: 6e67 732e 6765 7428 2270 6978 656c 7769  ngs.get("pixelwi
+0000ef50: 6474 6822 2929 0d0a 2020 2020 2020 2020  dth"))..        
+0000ef60: 2020 2020 2020 2020 7365 6c66 2e79 6361          self.yca
+0000ef70: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
+0000ef80: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000ef90: 6765 7428 2270 6978 656c 6865 6967 6874  get("pixelheight
+0000efa0: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+0000efb0: 2020 2020 2073 656c 662e 7a63 616c 6962       self.zcalib
+0000efc0: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
+0000efd0: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000efe0: 2822 766f 7865 6c64 6570 7468 2229 290d  ("voxeldepth")).
+0000eff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f000: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
+0000f010: 6f6e 203d 2069 6e74 2866 6c6f 6174 2873  on = int(float(s
+0000f020: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000f030: 2822 7469 6d65 696e 7465 7276 616c 2229  ("timeinterval")
+0000f040: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000f050: 2020 2020 7365 6c66 2e64 6574 6563 746f      self.detecto
+0000f060: 7273 6574 7469 6e67 7320 3d20 7365 6c66  rsettings = self
+0000f070: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
+0000f080: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
+0000f090: 6e64 2822 4465 7465 6374 6f72 5365 7474  nd("DetectorSett
+0000f0a0: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
+0000f0b0: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
+0000f0c0: 6963 7365 7474 696e 6773 203d 2073 656c  icsettings = sel
+0000f0d0: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000f0e0: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000f0f0: 696e 6428 2242 6173 6963 5365 7474 696e  ind("BasicSettin
+0000f100: 6773 2229 0d0a 2020 2020 2020 2020 2020  gs")..          
+0000f110: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
+0000f120: 746f 7263 6861 6e6e 656c 203d 2069 6e74  torchannel = int
+0000f130: 2866 6c6f 6174 2873 656c 662e 6465 7465  (float(self.dete
+0000f140: 6374 6f72 7365 7474 696e 6773 2e67 6574  ctorsettings.get
+0000f150: 2822 5441 5247 4554 5f43 4841 4e4e 454c  ("TARGET_CHANNEL
+0000f160: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
+0000f170: 2020 2020 2020 7365 6c66 2e74 7374 6172        self.tstar
+0000f180: 7420 3d20 696e 7428 666c 6f61 7428 7365  t = int(float(se
+0000f190: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
+0000f1a0: 2e67 6574 2822 7473 7461 7274 2229 2929  .get("tstart")))
+0000f1b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f1c0: 2020 7365 6c66 2e74 656e 6420 3d20 696e    self.tend = in
+0000f1d0: 7428 666c 6f61 7428 7365 6c66 2e62 6173  t(float(self.bas
+0000f1e0: 6963 7365 7474 696e 6773 2e67 6574 2822  icsettings.get("
+0000f1f0: 7465 6e64 2229 2929 0d0a 2020 2020 2020  tend")))..      
+0000f200: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000f210: 6765 745f 626f 756e 6461 7279 5f70 6f69  get_boundary_poi
+0000f220: 6e74 7328 290d 0a20 2020 2020 2020 2020  nts()..         
+0000f230: 2020 2020 2020 2070 7269 6e74 2827 4974         print('It
+0000f240: 6572 6174 696e 6720 6f76 6572 2073 706f  erating over spo
+0000f250: 7473 2069 6e20 6672 616d 6527 290d 0a20  ts in frame').. 
+0000f260: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f270: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
+0000f280: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f290: 7574 7572 6573 203d 205b 5d0d 0a0d 0a20  utures = [].... 
+0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000f2b0: 6974 6820 636f 6e63 7572 7265 6e74 2e66  ith concurrent.f
+0000f2c0: 7574 7572 6573 2e54 6872 6561 6450 6f6f  utures.ThreadPoo
+0000f2d0: 6c45 7865 6375 746f 7228 6d61 785f 776f  lExecutor(max_wo
+0000f2e0: 726b 6572 7320 3d20 6f73 2e63 7075 5f63  rkers = os.cpu_c
+0000f2f0: 6f75 6e74 2829 2920 6173 2065 7865 6375  ount()) as execu
+0000f300: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
+0000f310: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f330: 666f 7220 6672 616d 6520 696e 2073 656c  for frame in sel
+0000f340: 662e 5370 6f74 6f62 6a65 6374 732e 6669  f.Spotobjects.fi
+0000f350: 6e64 616c 6c28 2753 706f 7473 496e 4672  ndall('SpotsInFr
+0000f360: 616d 6527 293a 0d0a 2020 2020 2020 2020  ame'):..        
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f380: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
+0000f390: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
+0000f3a0: 6d69 7428 7365 6c66 2e5f 7370 6f74 5f63  mit(self._spot_c
+0000f3b0: 6f6d 7075 7465 722c 2066 7261 6d65 2929  omputer, frame))
+0000f3c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f3d0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000f3e0: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000f3f0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f410: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f440: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000f450: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000f460: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000f440: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000f450: 722e 6c61 6265 6c20 3d20 2243 6f6c 6c65  r.label = "Colle
+0000f460: 6374 696e 6720 5370 6f74 7322 0d0a 2020  cting Spots"..  
 0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f490: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000f4a0: 722e 7661 6c75 6520 3d20 2073 656c 662e  r.value =  self.
-0000f4b0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+0000f490: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000f4a0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4d0: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
-0000f4e0: 756c 7428 290d 0a0d 0a20 2020 2020 2020  ult()....       
-0000f4f0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-0000f500: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
-0000f510: 7472 6163 6b73 207b 6c65 6e28 7365 6c66  tracks {len(self
-0000f520: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
-0000f530: 6964 7329 7d27 2920 200d 0a20 2020 2020  ids)}')  ..     
-0000f540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f550: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
-0000f560: 2020 2020 2020 2020 2020 2066 7574 7572             futur
-0000f570: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-0000f580: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-0000f590: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-0000f5a0: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
-0000f5b0: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
-0000f5c0: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
-0000f5d0: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
-0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000f600: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
-0000f610: 6163 6b20 696e 2073 656c 662e 7472 6163  ack in self.trac
-0000f620: 6b73 2e66 696e 6461 6c6c 2827 5472 6163  ks.findall('Trac
-0000f630: 6b27 293a 0d0a 2020 2020 2020 2020 2020  k'):..          
-0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f650: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f670: 7472 6163 6b5f 6964 203d 2069 6e74 2874  track_id = int(t
-0000f680: 7261 636b 2e67 6574 2873 656c 662e 7472  rack.get(self.tr
-0000f690: 6163 6b69 645f 6b65 7929 290d 0a20 2020  ackid_key))..   
+0000f4d0: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
+0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f500: 2020 206c 656e 2866 7574 7572 6573 292c     len(futures),
+0000f510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f530: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f550: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f560: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
+0000f570: 686f 7728 290d 0a0d 0a20 2020 2020 2020  how()....       
+0000f580: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f590: 2072 2069 6e20 636f 6e63 7572 7265 6e74   r in concurrent
+0000f5a0: 2e66 7574 7572 6573 2e61 735f 636f 6d70  .futures.as_comp
+0000f5b0: 6c65 7465 6428 6675 7475 7265 7329 3a0d  leted(futures):.
+0000f5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5e0: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000f5f0: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+0000f600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f620: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000f630: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000f640: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f660: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f670: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000f680: 2e76 616c 7565 203d 2020 7365 6c66 2e63  .value =  self.c
+0000f690: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
 0000f6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6b0: 2020 2020 2020 2020 2069 6620 7472 6163           if trac
-0000f6c0: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
-0000f6d0: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
-0000f6e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 2020 2020 6675 7475 7265 732e 6170 7065      futures.appe
-0000f710: 6e64 2865 7865 6375 746f 722e 7375 626d  nd(executor.subm
-0000f720: 6974 2873 656c 662e 5f74 7261 636b 5f63  it(self._track_c
-0000f730: 6f6d 7075 7465 722c 2074 7261 636b 2c20  omputer, track, 
-0000f740: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
-0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f760: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-0000f770: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-0000f780: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7c0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000f7d0: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-0000f7e0: 6c20 3d20 2243 6f6c 6c65 6374 696e 6720  l = "Collecting 
-0000f7f0: 5472 6163 6b73 220d 0a20 2020 2020 2020  Tracks"..       
-0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f820: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-0000f830: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f880: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000f890: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
-0000f8a0: 7472 6163 6b5f 6964 7329 2c0d 0a20 2020  track_ids),..   
-0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8d0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8f0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000f900: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
-0000f910: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-0000f920: 2020 2020 2020 666f 7220 7220 696e 2063        for r in c
-0000f930: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-0000f940: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
-0000f950: 7574 7572 6573 293a 0d0a 2020 2020 2020  utures):..      
-0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f970: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f980: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000f990: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f9c0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-0000f9d0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-0000f9e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa00: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000fa10: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
-0000fa20: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
+0000f6b0: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
+0000f6c0: 6c74 2829 0d0a 0d0a 2020 2020 2020 2020  lt()....        
+0000f6d0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+0000f6e0: 4974 6572 6174 696e 6720 6f76 6572 2074  Iterating over t
+0000f6f0: 7261 636b 7320 7b6c 656e 2873 656c 662e  racks {len(self.
+0000f700: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+0000f710: 6473 297d 2729 2020 0d0a 2020 2020 2020  ds)}')  ..      
+0000f720: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000f730: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+0000f740: 2020 2020 2020 2020 2020 6675 7475 7265            future
+0000f750: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000f760: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
+0000f770: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
+0000f780: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
+0000f790: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
+0000f7a0: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
+0000f7b0: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
+0000f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f7e0: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
+0000f7f0: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
+0000f800: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
+0000f810: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+0000f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f830: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f840: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000f850: 7261 636b 5f69 6420 3d20 696e 7428 7472  rack_id = int(tr
+0000f860: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
+0000f870: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
+0000f880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f890: 2020 2020 2020 2020 6966 2074 7261 636b          if track
+0000f8a0: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
+0000f8b0: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
+0000f8c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8e0: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
+0000f8f0: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
+0000f900: 7428 7365 6c66 2e5f 7472 6163 6b5f 636f  t(self._track_co
+0000f910: 6d70 7574 6572 2c20 7472 6163 6b2c 2074  mputer, track, t
+0000f920: 7261 636b 5f69 6429 290d 0a20 2020 2020  rack_id))..     
+0000f930: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f940: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000f950: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000f960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f980: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9a0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000f9b0: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+0000f9c0: 203d 2022 436f 6c6c 6563 7469 6e67 2054   = "Collecting T
+0000f9d0: 7261 636b 7322 0d0a 2020 2020 2020 2020  racks"..        
+0000f9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fa00: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
+0000fa10: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa50: 2020 2072 2e72 6573 756c 7428 290d 0a20     r.result().. 
-0000fa60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000fa70: 6620 7365 6c66 2e63 6861 6e6e 656c 5f73  f self.channel_s
-0000fa80: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
-0000fa90: 4e6f 6e65 3a20 200d 0a20 2020 2020 2020  None:  ..       
+0000fa40: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa60: 2020 2020 2020 2020 2020 2020 206c 656e               len
+0000fa70: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
+0000fa80: 7261 636b 5f69 6473 292c 0d0a 2020 2020  rack_ids),..    
+0000fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fab0: 7365 6c66 2e5f 6372 6561 7465 5f73 6563  self._create_sec
-0000fac0: 6f6e 645f 6368 616e 6e65 6c5f 786d 6c28  ond_channel_xml(
-0000fad0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fae0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-0000faf0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-0000fb00: 2069 6e20 7365 6c66 2e67 7261 7068 5f73   in self.graph_s
-0000fb10: 706c 6974 2e69 7465 6d73 2829 3a0d 0a20  plit.items():.. 
-0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb30: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000fab0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fad0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000fae0: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
+0000faf0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+0000fb00: 2020 2020 2066 6f72 2072 2069 6e20 636f       for r in co
+0000fb10: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+0000fb20: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
+0000fb30: 7475 7265 7329 3a0d 0a20 2020 2020 2020  tures):..       
 0000fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb50: 2020 2020 2020 2020 6461 7567 6874 6572          daughter
-0000fb60: 5f74 7261 636b 5f69 6420 3d20 2069 6e74  _track_id =  int
-0000fb70: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
-0000fb80: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000fb90: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
-0000fba0: 286b 2929 5d5b 7365 6c66 2e75 6e69 7175  (k))][self.uniqu
-0000fbb0: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
-0000fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbd0: 2020 2020 2020 2020 2070 6172 656e 745f           parent_
-0000fbe0: 7472 6163 6b5f 6964 203d 2069 6e74 2866  track_id = int(f
-0000fbf0: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
-0000fc00: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000fc10: 7469 6573 5b69 6e74 2866 6c6f 6174 2876  ties[int(float(v
-0000fc20: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
-0000fc30: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
-0000fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc50: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
-0000fc60: 685f 7472 6163 6b73 5b64 6175 6768 7465  h_tracks[daughte
-0000fc70: 725f 7472 6163 6b5f 6964 5d20 3d20 7061  r_track_id] = pa
-0000fc80: 7265 6e74 5f74 7261 636b 5f69 640d 0a20  rent_track_id.. 
-0000fc90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fca0: 656c 662e 5f67 6574 5f61 7474 7269 6275  elf._get_attribu
-0000fcb0: 7465 7328 290d 0a20 2020 2020 2020 2020  tes()..         
-0000fcc0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-0000fcd0: 7574 6f65 6e63 6f64 6572 5f6d 6f64 656c  utoencoder_model
-0000fce0: 2061 6e64 2073 656c 662e 7365 675f 696d   and self.seg_im
-0000fcf0: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-0000fd00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fd10: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-0000fd20: 4765 7474 696e 6720 6175 746f 656e 636f  Getting autoenco
-0000fd30: 6465 7220 636c 6f75 6473 2729 0d0a 2020  der clouds')..  
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 2020 2020 2073 656c 662e 5f61 7373 6967       self._assig
-0000fd60: 6e5f 636c 7573 7465 725f 636c 6173 7328  n_cluster_class(
-0000fd70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fd80: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000fd90: 2743 7265 6174 696e 6720 6d61 7374 6572  'Creating master
-0000fda0: 2078 6d6c 2729 0d0a 2020 2020 2020 2020   xml')..        
-0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fdc0: 656c 662e 5f63 7265 6174 655f 6d61 7374  elf._create_mast
-0000fdd0: 6572 5f78 6d6c 2829 0d0a 2020 2020 2020  er_xml()..      
-0000fde0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000fdf0: 6f75 6e74 203d 2030 200d 0a20 2020 2020  ount = 0 ..     
-0000fe00: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-0000fe10: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
-0000fe20: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000fe30: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-0000fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe50: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000fe60: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-0000fe70: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fea0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000feb0: 735f 6261 722e 6c61 6265 6c20 3d20 224a  s_bar.label = "J
-0000fec0: 7573 7420 6f6e 6520 6d6f 7265 2074 6869  ust one more thi
-0000fed0: 6e67 220d 0a20 2020 2020 2020 2020 2020  ng"..           
-0000fee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fef0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ff00: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-0000ff10: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
+0000fb50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fb60: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
+0000fb70: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+0000fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000fba0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000fbb0: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+0000fbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbe0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000fbf0: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
+0000fc00: 3d20 7365 6c66 2e63 6f75 6e74 0d0a 2020  = self.count..  
+0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc30: 2020 722e 7265 7375 6c74 2829 0d0a 2020    r.result()..  
+0000fc40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000fc50: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+0000fc60: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+0000fc70: 6f6e 653a 2020 0d0a 2020 2020 2020 2020  one:  ..        
+0000fc80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fc90: 656c 662e 5f63 7265 6174 655f 7365 636f  elf._create_seco
+0000fca0: 6e64 5f63 6861 6e6e 656c 5f78 6d6c 2829  nd_channel_xml()
+0000fcb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fcc0: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000fcd0: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
+0000fce0: 696e 2073 656c 662e 6772 6170 685f 7370  in self.graph_sp
+0000fcf0: 6c69 742e 6974 656d 7328 293a 0d0a 2020  lit.items():..  
+0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd10: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd30: 2020 2020 2020 2064 6175 6768 7465 725f         daughter_
+0000fd40: 7472 6163 6b5f 6964 203d 2020 696e 7428  track_id =  int(
+0000fd50: 666c 6f61 7428 7374 7228 7365 6c66 2e75  float(str(self.u
+0000fd60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000fd70: 7274 6965 735b 696e 7428 666c 6f61 7428  rties[int(float(
+0000fd80: 6b29 295d 5b73 656c 662e 756e 6971 7565  k))][self.unique
+0000fd90: 6964 5f6b 6579 5d29 2929 0d0a 2020 2020  id_key])))..    
+0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdb0: 2020 2020 2020 2020 7061 7265 6e74 5f74          parent_t
+0000fdc0: 7261 636b 5f69 6420 3d20 696e 7428 666c  rack_id = int(fl
+0000fdd0: 6f61 7428 7374 7228 7365 6c66 2e75 6e69  oat(str(self.uni
+0000fde0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000fdf0: 6965 735b 696e 7428 666c 6f61 7428 7629  ies[int(float(v)
+0000fe00: 295d 5b73 656c 662e 756e 6971 7565 6964  )][self.uniqueid
+0000fe10: 5f6b 6579 5d29 2929 0d0a 2020 2020 2020  _key])))..      
+0000fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe30: 2020 2020 2020 7365 6c66 2e67 7261 7068        self.graph
+0000fe40: 5f74 7261 636b 735b 6461 7567 6874 6572  _tracks[daughter
+0000fe50: 5f74 7261 636b 5f69 645d 203d 2070 6172  _track_id] = par
+0000fe60: 656e 745f 7472 6163 6b5f 6964 0d0a 2020  ent_track_id..  
+0000fe70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fe80: 6c66 2e5f 6765 745f 6174 7472 6962 7574  lf._get_attribut
+0000fe90: 6573 2829 0d0a 2020 2020 2020 2020 2020  es()..          
+0000fea0: 2020 2020 2020 6966 2073 656c 662e 6175        if self.au
+0000feb0: 746f 656e 636f 6465 725f 6d6f 6465 6c20  toencoder_model 
+0000fec0: 616e 6420 7365 6c66 2e73 6567 5f69 6d61  and self.seg_ima
+0000fed0: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
+0000fee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fef0: 2020 2020 2020 2020 7072 696e 7428 2747          print('G
+0000ff00: 6574 7469 6e67 2061 7574 6f65 6e63 6f64  etting autoencod
+0000ff10: 6572 2063 6c6f 7564 7327 290d 0a20 2020  er clouds')..   
 0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff40: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
-0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff70: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000ff80: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
-0000ff90: 7472 6163 6b5f 6964 7329 2c0d 0a20 2020  track_ids),..   
-0000ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffc0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fff0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-00010000: 735f 6261 722e 7368 6f77 2829 0d0a 2020  s_bar.show()..  
-00010010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff30: 2020 2020 7365 6c66 2e5f 6173 7369 676e      self._assign
+0000ff40: 5f63 6c75 7374 6572 5f63 6c61 7373 2829  _cluster_class()
+0000ff50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ff60: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+0000ff70: 4372 6561 7469 6e67 206d 6173 7465 7220  Creating master 
+0000ff80: 786d 6c27 290d 0a20 2020 2020 2020 2020  xml')..         
+0000ff90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ffa0: 6c66 2e5f 6372 6561 7465 5f6d 6173 7465  lf._create_maste
+0000ffb0: 725f 786d 6c28 290d 0a20 2020 2020 2020  r_xml()..       
+0000ffc0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000ffd0: 756e 7420 3d20 3020 0d0a 2020 2020 2020  unt = 0 ..      
+0000ffe0: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
+0000fff0: 6163 6b5f 6964 2069 6e20 7365 6c66 2e66  ack_id in self.f
+00010000: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+00010010: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
 00010020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010030: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-00010040: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
-00010050: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+00010030: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010040: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+00010050: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
 00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010080: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
-00010090: 7565 203d 2073 656c 662e 636f 756e 740d  ue = self.count.
-000100a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000100b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100c0: 2020 2020 2073 656c 662e 5f66 696e 616c       self._final
-000100d0: 5f74 7261 636b 7328 7472 6163 6b5f 6964  _tracks(track_id
-000100e0: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-000100f0: 2020 2020 2020 6966 2073 656c 662e 666f        if self.fo
-00010100: 7572 6965 723a 0d0a 2020 2020 2020 2020  urier:..        
-00010110: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00010120: 2827 636f 6d70 7574 696e 6720 466f 7572  ('computing Four
-00010130: 6965 7227 290d 0a20 2020 2020 2020 2020  ier')..         
-00010140: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00010150: 636f 6d70 7574 655f 7068 656e 6f74 7970  compute_phenotyp
-00010160: 6573 2829 2020 2020 2020 2020 2020 2020  es()            
-00010170: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00010180: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010190: 6c66 2e5f 7465 6d70 6f72 616c 5f70 6c6f  lf._temporal_plo
-000101a0: 7473 5f74 7261 636b 6d61 7465 2829 0d0a  ts_trackmate()..
+00010070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010080: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+00010090: 5f62 6172 2e6c 6162 656c 203d 2022 4a75  _bar.label = "Ju
+000100a0: 7374 206f 6e65 206d 6f72 6520 7468 696e  st one more thin
+000100b0: 6722 0d0a 2020 2020 2020 2020 2020 2020  g"..            
+000100c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000100e0: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
+000100f0: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
+00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010120: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
+00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010150: 2020 2020 2020 2020 2020 2020 206c 656e               len
+00010160: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
+00010170: 7261 636b 5f69 6473 292c 0d0a 2020 2020  rack_ids),..    
+00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101a0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
 000101b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101c0: 0d0a 0d0a 2020 2020 6465 6620 5f63 7265  ....    def _cre
-000101d0: 6174 655f 6d61 7374 6572 5f78 6d6c 2873  ate_master_xml(s
-000101e0: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-000101f0: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
-00010200: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
-00010210: 746f 626a 6563 7420 696e 2073 656c 662e  tobject in self.
-00010220: 6d61 7374 6572 5f78 6d6c 5f72 6f6f 742e  master_xml_root.
-00010230: 6974 6572 2827 5370 6f74 2729 3a0d 0a20  iter('Spot'):.. 
+000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101d0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+000101e0: 5f62 6172 2e73 686f 7728 290d 0a20 2020  _bar.show()..   
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010210: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+00010220: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+00010230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010250: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00010260: 656c 6c5f 6964 203d 2069 6e74 2853 706f  ell_id = int(Spo
-00010270: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-00010280: 2e73 706f 7469 645f 6b65 7929 290d 0a20  .spotid_key)).. 
+00010250: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00010260: 726f 6772 6573 735f 6261 722e 7661 6c75  rogress_bar.valu
+00010270: 6520 3d20 7365 6c66 2e63 6f75 6e74 0d0a  e = self.count..
+00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000102b0: 6620 6365 6c6c 5f69 6420 696e 2073 656c  f cell_id in sel
-000102c0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000102d0: 6f70 6572 7469 6573 2e6b 6579 7328 293a  operties.keys():
-000102e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010330: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
-00010340: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00010350: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
-00010360: 6b65 7973 2829 3a0d 0a0d 0a20 2020 2020  keys():....     
-00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
-000103a0: 2e73 6574 286b 2c20 7374 7228 7365 6c66  .set(k, str(self
-000103b0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000103c0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-000103d0: 5b6b 5d29 2920 2020 0d0a 0d0a 2020 2020  [k]))   ....    
-000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010400: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00010410: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
-00010420: 5f74 7265 652e 7772 6974 6528 6f73 2e70  _tree.write(os.p
-00010430: 6174 682e 6a6f 696e 2873 656c 662e 6d61  ath.join(self.ma
-00010440: 7374 6572 5f78 6d6c 5f70 6174 682c 2073  ster_xml_path, s
-00010450: 656c 662e 6d61 7374 6572 5f78 6d6c 5f6e  elf.master_xml_n
-00010460: 616d 6529 290d 0a20 2020 2020 2020 2020  ame))..         
-00010470: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010490: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
-000104d0: 5f61 7373 6967 6e5f 636c 7573 7465 725f  _assign_cluster_
-000104e0: 636c 6173 7328 7365 6c66 293a 0d0a 2020  class(self):..  
-000104f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00010500: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010510: 656c 662e 6178 6573 203d 2073 656c 662e  elf.axes = self.
-00010520: 6178 6573 2e72 6570 6c61 6365 2822 5422  axes.replace("T"
-00010530: 2c20 2222 290d 0a20 2020 2020 2020 2020  , "")..         
-00010540: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000102a0: 2020 2020 7365 6c66 2e5f 6669 6e61 6c5f      self._final_
+000102b0: 7472 6163 6b73 2874 7261 636b 5f69 6429  tracks(track_id)
+000102c0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+000102d0: 2020 2020 2069 6620 7365 6c66 2e66 6f75       if self.fou
+000102e0: 7269 6572 3a0d 0a20 2020 2020 2020 2020  rier:..         
+000102f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00010300: 2763 6f6d 7075 7469 6e67 2046 6f75 7269  'computing Fouri
+00010310: 6572 2729 0d0a 2020 2020 2020 2020 2020  er')..          
+00010320: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00010330: 6f6d 7075 7465 5f70 6865 6e6f 7479 7065  ompute_phenotype
+00010340: 7328 2920 2020 2020 2020 2020 2020 2020  s()             
+00010350: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00010360: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010370: 662e 5f74 656d 706f 7261 6c5f 706c 6f74  f._temporal_plot
+00010380: 735f 7472 6163 6b6d 6174 6528 290d 0a20  s_trackmate().. 
+00010390: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000103a0: 0a0d 0a20 2020 2064 6566 205f 6372 6561  ...    def _crea
+000103b0: 7465 5f6d 6173 7465 725f 786d 6c28 7365  te_master_xml(se
+000103c0: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
+000103d0: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
+000103e0: 2020 2020 2020 2020 666f 7220 5370 6f74          for Spot
+000103f0: 6f62 6a65 6374 2069 6e20 7365 6c66 2e6d  object in self.m
+00010400: 6173 7465 725f 786d 6c5f 726f 6f74 2e69  aster_xml_root.i
+00010410: 7465 7228 2753 706f 7427 293a 0d0a 2020  ter('Spot'):..  
+00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010430: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00010440: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
+00010450: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+00010460: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
+00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010480: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010490: 2063 656c 6c5f 6964 2069 6e20 7365 6c66   cell_id in self
+000104a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000104b0: 7065 7274 6965 732e 6b65 7973 2829 3a0d  perties.keys():.
+000104c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 2066 6f72 206b 2069 6e20 7365 6c66 2e75   for k in self.u
+00010520: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00010530: 7274 6965 735b 6365 6c6c 5f69 645d 2e6b  rties[cell_id].k
+00010540: 6579 7328 293a 0d0a 0d0a 2020 2020 2020  eys():....      
 00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2066 6f72 2063 6f75 6e74 2c20 7469 6d65   for count, time
-00010570: 5f6b 6579 2069 6e20 656e 756d 6572 6174  _key in enumerat
-00010580: 6528 7365 6c66 2e5f 7469 6d65 645f 6365  e(self._timed_ce
-00010590: 6e74 726f 6964 2e6b 6579 7328 2929 3a0d  ntroid.keys()):.
-000105a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000105b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010570: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
+00010580: 7365 7428 6b2c 2073 7472 2873 656c 662e  set(k, str(self.
+00010590: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000105a0: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+000105b0: 6b5d 2929 2020 200d 0a0d 0a20 2020 2020  k]))   ....     
 000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105d0: 2020 2020 2020 2020 2074 7265 652c 2073           tree, s
-000105e0: 706f 745f 6365 6e74 726f 6964 7320 3d20  pot_centroids = 
-000105f0: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
-00010600: 726f 6964 5b74 696d 655f 6b65 795d 0d0a  roid[time_key]..
-00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010620: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00010630: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-00010640: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010670: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-00010680: 6c61 6265 6c20 3d20 2241 7574 6f65 6e63  label = "Autoenc
-00010690: 6f64 6572 2066 6f72 2072 6566 696e 696e  oder for refinin
-000106a0: 6720 706f 696e 7420 636c 6f75 6473 220d  g point clouds".
-000106b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106d0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-000106e0: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
-000106f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010720: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-00010730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2020 6c65 6e28 7365 6c66 2e5f 7469 6d65    len(self._time
-00010780: 645f 6365 6e74 726f 6964 2e6b 6579 7328  d_centroid.keys(
-00010790: 2929 202b 2031 2c0d 0a20 2020 2020 2020  )) + 1,..       
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105e0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+000105f0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+00010600: 7472 6565 2e77 7269 7465 286f 732e 7061  tree.write(os.pa
+00010610: 7468 2e6a 6f69 6e28 7365 6c66 2e6d 6173  th.join(self.mas
+00010620: 7465 725f 786d 6c5f 7061 7468 2c20 7365  ter_xml_path, se
+00010630: 6c66 2e6d 6173 7465 725f 786d 6c5f 6e61  lf.master_xml_na
+00010640: 6d65 2929 0d0a 2020 2020 2020 2020 2020  me))..          
+00010650: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010670: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106a0: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
+000106b0: 6173 7369 676e 5f63 6c75 7374 6572 5f63  assign_cluster_c
+000106c0: 6c61 7373 2873 656c 6629 3a0d 0a20 2020  lass(self):..   
+000106d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000106e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000106f0: 6c66 2e61 7865 7320 3d20 7365 6c66 2e61  lf.axes = self.a
+00010700: 7865 732e 7265 706c 6163 6528 2254 222c  xes.replace("T",
+00010710: 2022 2229 0d0a 2020 2020 2020 2020 2020   "")..          
+00010720: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010740: 666f 7220 636f 756e 742c 2074 696d 655f  for count, time_
+00010750: 6b65 7920 696e 2065 6e75 6d65 7261 7465  key in enumerate
+00010760: 2873 656c 662e 5f74 696d 6564 5f63 656e  (self._timed_cen
+00010770: 7472 6f69 642e 6b65 7973 2829 293a 0d0a  troid.keys()):..
+00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010790: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107d0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107f0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00010800: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
-00010810: 3d20 2063 6f75 6e74 200d 0a20 2020 2020  =  count ..     
-00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010840: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
-00010850: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2020 636c 7573 7465 725f 6576 616c 203d    cluster_eval =
-00010880: 2043 6c75 7374 6572 696e 6728 7365 6c66   Clustering(self
-00010890: 2e61 6363 656c 6572 6174 6f72 2c20 7365  .accelerator, se
-000108a0: 6c66 2e64 6576 6963 6573 2c20 7365 6c66  lf.devices, self
-000108b0: 2e73 6567 5f69 6d61 6765 5b69 6e74 2874  .seg_image[int(t
-000108c0: 696d 655f 6b65 7929 2c3a 5d2c 2020 7365  ime_key),:],  se
-000108d0: 6c66 2e61 7865 732c 2073 656c 662e 6e75  lf.axes, self.nu
-000108e0: 6d5f 706f 696e 7473 2c20 7365 6c66 2e61  m_points, self.a
-000108f0: 7574 6f65 6e63 6f64 6572 5f6d 6f64 656c  utoencoder_model
-00010900: 2c20 6b65 7920 3d20 7469 6d65 5f6b 6579  , key = time_key
-00010910: 2c20 7072 6f67 7265 7373 5f62 6172 3d73  , progress_bar=s
-00010920: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00010930: 2c20 6261 7463 685f 7369 7a65 203d 2073  , batch_size = s
-00010940: 656c 662e 6261 7463 685f 7369 7a65 2c20  elf.batch_size, 
-00010950: 7363 616c 655f 7a3d 7365 6c66 2e73 6361  scale_z=self.sca
-00010960: 6c65 5f7a 2c20 7363 616c 655f 7879 3d20  le_z, scale_xy= 
-00010970: 7365 6c66 2e73 6361 6c65 5f78 792c 2063  self.scale_xy, c
-00010980: 656e 7465 7220 3d20 7365 6c66 2e63 656e  enter = self.cen
-00010990: 7465 7229 2020 2020 2020 200d 0a20 2020  ter)       ..   
+000107b0: 2020 2020 2020 2020 7472 6565 2c20 7370          tree, sp
+000107c0: 6f74 5f63 656e 7472 6f69 6473 203d 2073  ot_centroids = s
+000107d0: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
+000107e0: 6f69 645b 7469 6d65 5f6b 6579 5d0d 0a20  oid[time_key].. 
+000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010800: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00010810: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+00010820: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010840: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010850: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+00010860: 6162 656c 203d 2022 4175 746f 656e 636f  abel = "Autoenco
+00010870: 6465 7220 666f 7220 7265 6669 6e69 6e67  der for refining
+00010880: 2070 6f69 6e74 2063 6c6f 7564 7322 0d0a   point clouds"..
+00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108b0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+000108c0: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
+000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010900: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
+00010910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010950: 206c 656e 2873 656c 662e 5f74 696d 6564   len(self._timed
+00010960: 5f63 656e 7472 6f69 642e 6b65 7973 2829  _centroid.keys()
+00010970: 2920 2b20 312c 0d0a 2020 2020 2020 2020  ) + 1,..        
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109b0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
-000109c0: 6576 616c 2e5f 6372 6561 7465 5f63 6c75  eval._create_clu
-000109d0: 7374 6572 5f6c 6162 656c 7328 290d 0a20  ster_labels().. 
-000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109f0: 2020 2020 2020 2020 2020 7469 6d65 645f            timed_
-00010a00: 636c 7573 7465 725f 6c61 6265 6c20 3d20  cluster_label = 
-00010a10: 636c 7573 7465 725f 6576 616c 2e74 696d  cluster_eval.tim
-00010a20: 6564 5f63 6c75 7374 6572 5f6c 6162 656c  ed_cluster_label
-00010a30: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010a40: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00010a50: 7470 7574 5f6c 6162 656c 732c 2020 6f75  tput_labels,  ou
-00010a60: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
-00010a70: 7472 6f69 642c 206f 7574 7075 745f 636c  troid, output_cl
-00010a80: 6f75 645f 6563 6365 6e74 7269 6369 7479  oud_eccentricity
-00010a90: 2c20 6f75 7470 7574 5f6c 6172 6765 7374  , output_largest
-00010aa0: 5f65 6967 656e 7665 6374 6f72 2c20 6f75  _eigenvector, ou
-00010ab0: 7470 7574 5f6c 6172 6765 7374 5f65 6967  tput_largest_eig
-00010ac0: 656e 7661 6c75 652c 206f 7574 7075 745f  envalue, output_
-00010ad0: 6469 6d65 6e73 696f 6e73 2c20 6f75 7470  dimensions, outp
-00010ae0: 7574 5f63 6c6f 7564 5f73 7572 6661 6365  ut_cloud_surface
-00010af0: 5f61 7265 6120 3d20 7469 6d65 645f 636c  _area = timed_cl
-00010b00: 7573 7465 725f 6c61 6265 6c5b 7469 6d65  uster_label[time
-00010b10: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b30: 2020 7363 616c 655f 3120 3d20 310d 0a20    scale_1 = 1.. 
-00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b50: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00010b60: 3220 3d20 310d 0a20 2020 2020 2020 2020  2 = 1..         
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00010b90: 286c 656e 286f 7574 7075 745f 636c 7573  (len(output_clus
-00010ba0: 7465 725f 6365 6e74 726f 6964 2929 3a0d  ter_centroid)):.
-00010bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000109b0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109d0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+000109e0: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
+000109f0: 2020 636f 756e 7420 0d0a 2020 2020 2020    count ..      
+00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a10: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00010a20: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
+00010a30: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a50: 2063 6c75 7374 6572 5f65 7661 6c20 3d20   cluster_eval = 
+00010a60: 436c 7573 7465 7269 6e67 2873 656c 662e  Clustering(self.
+00010a70: 6163 6365 6c65 7261 746f 722c 2073 656c  accelerator, sel
+00010a80: 662e 6465 7669 6365 732c 2073 656c 662e  f.devices, self.
+00010a90: 7365 675f 696d 6167 655b 696e 7428 7469  seg_image[int(ti
+00010aa0: 6d65 5f6b 6579 292c 3a5d 2c20 2073 656c  me_key),:],  sel
+00010ab0: 662e 6178 6573 2c20 7365 6c66 2e6e 756d  f.axes, self.num
+00010ac0: 5f70 6f69 6e74 732c 2073 656c 662e 6175  _points, self.au
+00010ad0: 746f 656e 636f 6465 725f 6d6f 6465 6c2c  toencoder_model,
+00010ae0: 206b 6579 203d 2074 696d 655f 6b65 792c   key = time_key,
+00010af0: 2070 726f 6772 6573 735f 6261 723d 7365   progress_bar=se
+00010b00: 6c66 2e70 726f 6772 6573 735f 6261 722c  lf.progress_bar,
+00010b10: 2062 6174 6368 5f73 697a 6520 3d20 7365   batch_size = se
+00010b20: 6c66 2e62 6174 6368 5f73 697a 652c 2073  lf.batch_size, s
+00010b30: 6361 6c65 5f7a 3d73 656c 662e 7363 616c  cale_z=self.scal
+00010b40: 655f 7a2c 2073 6361 6c65 5f78 793d 2073  e_z, scale_xy= s
+00010b50: 656c 662e 7363 616c 655f 7879 2c20 6365  elf.scale_xy, ce
+00010b60: 6e74 6572 203d 2073 656c 662e 6365 6e74  nter = self.cent
+00010b70: 6572 2920 2020 2020 2020 0d0a 2020 2020  er)       ..    
+00010b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b90: 2020 2020 2020 2063 6c75 7374 6572 5f65         cluster_e
+00010ba0: 7661 6c2e 5f63 7265 6174 655f 636c 7573  val._create_clus
+00010bb0: 7465 725f 6c61 6265 6c73 2829 0d0a 2020  ter_labels()..  
 00010bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bd0: 2020 2020 2063 656e 7472 6f69 6420 3d20       centroid = 
-00010be0: 6f75 7470 7574 5f63 6c75 7374 6572 5f63  output_cluster_c
-00010bf0: 656e 7472 6f69 645b 695d 0d0a 2020 2020  entroid[i]..    
-00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c20: 7175 616c 6974 7920 3d20 6f75 7470 7574  quality = output
-00010c30: 5f6c 6172 6765 7374 5f65 6967 656e 7661  _largest_eigenva
-00010c40: 6c75 655b 695d 0d0a 2020 2020 2020 2020  lue[i]..        
-00010c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c60: 2020 2020 2020 2020 2020 2020 6563 6365              ecce
-00010c70: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00010c80: 7273 7479 7a20 3d20 6f75 7470 7574 5f63  rstyz = output_c
-00010c90: 6c6f 7564 5f65 6363 656e 7472 6963 6974  loud_eccentricit
-00010ca0: 795b 695d 0d0a 2020 2020 2020 2020 2020  y[i]..          
-00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cc0: 2020 2020 2020 2020 2020 6573 7365 6e74            essent
-00010cd0: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
-00010ce0: 203d 206f 7574 7075 745f 6469 6d65 6e73   = output_dimens
-00010cf0: 696f 6e73 5b69 5d20 0d0a 2020 2020 2020  ions[i] ..      
+00010bd0: 2020 2020 2020 2020 2074 696d 6564 5f63           timed_c
+00010be0: 6c75 7374 6572 5f6c 6162 656c 203d 2063  luster_label = c
+00010bf0: 6c75 7374 6572 5f65 7661 6c2e 7469 6d65  luster_eval.time
+00010c00: 645f 636c 7573 7465 725f 6c61 6265 6c20  d_cluster_label 
+00010c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010c20: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00010c30: 7075 745f 6c61 6265 6c73 2c20 206f 7574  put_labels,  out
+00010c40: 7075 745f 636c 7573 7465 725f 6365 6e74  put_cluster_cent
+00010c50: 726f 6964 2c20 6f75 7470 7574 5f63 6c6f  roid, output_clo
+00010c60: 7564 5f65 6363 656e 7472 6963 6974 792c  ud_eccentricity,
+00010c70: 206f 7574 7075 745f 6c61 7267 6573 745f   output_largest_
+00010c80: 6569 6765 6e76 6563 746f 722c 206f 7574  eigenvector, out
+00010c90: 7075 745f 6c61 7267 6573 745f 6569 6765  put_largest_eige
+00010ca0: 6e76 616c 7565 2c20 6f75 7470 7574 5f64  nvalue, output_d
+00010cb0: 696d 656e 7369 6f6e 732c 206f 7574 7075  imensions, outpu
+00010cc0: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
+00010cd0: 6172 6561 203d 2074 696d 6564 5f63 6c75  area = timed_clu
+00010ce0: 7374 6572 5f6c 6162 656c 5b74 696d 655f  ster_label[time_
+00010cf0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
 00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010d20: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-00010d30: 6d65 6e73 696f 6e5b 305d 203d 3d20 323a  mension[0] == 2:
-00010d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010d10: 2073 6361 6c65 5f31 203d 2031 0d0a 2020   scale_1 = 1..  
+00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d30: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
+00010d40: 203d 2031 0d0a 2020 2020 2020 2020 2020   = 1..          
 00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 2020 2020 2020 2020 2020 2020 2073 6361               sca
-00010d70: 6c65 5f31 203d 2073 656c 662e 7a63 616c  le_1 = self.zcal
-00010d80: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00010d60: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00010d70: 6c65 6e28 6f75 7470 7574 5f63 6c75 7374  len(output_clust
+00010d80: 6572 5f63 656e 7472 6f69 6429 293a 0d0a  er_centroid)):..
 00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010db0: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
-00010dc0: 6369 7479 5f64 696d 656e 7369 6f6e 5b31  city_dimension[1
-00010dd0: 5d20 3d3d 2031 3a0d 0a20 2020 2020 2020  ] == 1:..       
+00010db0: 2020 2020 6365 6e74 726f 6964 203d 206f      centroid = o
+00010dc0: 7574 7075 745f 636c 7573 7465 725f 6365  utput_cluster_ce
+00010dd0: 6e74 726f 6964 5b69 5d0d 0a20 2020 2020  ntroid[i]..     
 00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e00: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-00010e10: 5f32 203d 2073 656c 662e 7963 616c 6962  _2 = self.ycalib
-00010e20: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+00010e00: 7561 6c69 7479 203d 206f 7574 7075 745f  uality = output_
+00010e10: 6c61 7267 6573 745f 6569 6765 6e76 616c  largest_eigenval
+00010e20: 7565 5b69 5d0d 0a20 2020 2020 2020 2020  ue[i]..         
 00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010e50: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-00010e60: 6d65 6e73 696f 6e5b 305d 203d 3d20 323a  mension[0] == 2:
-00010e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e90: 2020 2020 2020 2020 2020 2020 2073 6361               sca
-00010ea0: 6c65 5f31 203d 2073 656c 662e 7a63 616c  le_1 = self.zcal
-00010eb0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ee0: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
-00010ef0: 6369 7479 5f64 696d 656e 7369 6f6e 5b31  city_dimension[1
-00010f00: 5d20 3d3d 2030 3a0d 0a20 2020 2020 2020  ] == 0:..       
-00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f30: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-00010f40: 5f32 203d 2073 656c 662e 7863 616c 6962  _2 = self.xcalib
-00010f50: 7261 7469 6f6e 2020 200d 0a0d 0a20 2020  ration   ....   
-00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
+00010e50: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00010e60: 7374 797a 203d 206f 7574 7075 745f 636c  styz = output_cl
+00010e70: 6f75 645f 6563 6365 6e74 7269 6369 7479  oud_eccentricity
+00010e80: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
+00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ea0: 2020 2020 2020 2020 2065 7373 656e 7472           essentr
+00010eb0: 6963 6974 795f 6469 6d65 6e73 696f 6e20  icity_dimension 
+00010ec0: 3d20 6f75 7470 7574 5f64 696d 656e 7369  = output_dimensi
+00010ed0: 6f6e 735b 695d 200d 0a20 2020 2020 2020  ons[i] ..       
+00010ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ef0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010f00: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
+00010f10: 656e 7369 6f6e 5b30 5d20 3d3d 2032 3a0d  ension[0] == 2:.
+00010f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f40: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00010f50: 655f 3120 3d20 7365 6c66 2e7a 6361 6c69  e_1 = self.zcali
+00010f60: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
 00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f80: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-00010f90: 5f64 696d 656e 7369 6f6e 5b30 5d20 3d3d  _dimension[0] ==
-00010fa0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f90: 2020 2020 6966 2065 7373 656e 7472 6963      if essentric
+00010fa0: 6974 795f 6469 6d65 6e73 696f 6e5b 315d  ity_dimension[1]
+00010fb0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
 00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fd0: 7363 616c 655f 3120 3d20 7365 6c66 2e79  scale_1 = self.y
-00010fe0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011010: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
-00011020: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
-00011030: 6e5b 315d 203d 3d20 303a 0d0a 2020 2020  n[1] == 0:..    
-00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011060: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00011070: 616c 655f 3220 3d20 7365 6c66 2e78 6361  ale_2 = self.xca
-00011080: 6c69 6272 6174 696f 6e20 200d 0a0d 0a20  libration  .... 
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fe0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00010ff0: 3220 3d20 7365 6c66 2e79 6361 6c69 6272  2 = self.ycalibr
+00011000: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011030: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
+00011040: 656e 7369 6f6e 5b30 5d20 3d3d 2032 3a0d  ension[0] == 2:.
+00011050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011070: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00011080: 655f 3120 3d20 7365 6c66 2e7a 6361 6c69  e_1 = self.zcali
+00011090: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
 000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
-000110c0: 7479 5f64 696d 656e 7369 6f6e 5b30 5d20  ty_dimension[0] 
-000110d0: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110c0: 2020 2020 6966 2065 7373 656e 7472 6963      if essentric
+000110d0: 6974 795f 6469 6d65 6e73 696f 6e5b 315d  ity_dimension[1]
+000110e0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
 000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011100: 2020 7363 616c 655f 3120 3d20 7365 6c66    scale_1 = self
-00011110: 2e79 6361 6c69 6272 6174 696f 6e0d 0a20  .ycalibration.. 
-00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011140: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00011150: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00011160: 696f 6e5b 315d 203d 3d20 323a 0d0a 2020  ion[1] == 2:..  
-00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011110: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00011120: 3220 3d20 7365 6c66 2e78 6361 6c69 6272  2 = self.xcalibr
+00011130: 6174 696f 6e20 2020 0d0a 0d0a 2020 2020  ation   ....    
+00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011160: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
+00011170: 6469 6d65 6e73 696f 6e5b 305d 203d 3d20  dimension[0] == 
+00011180: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
 00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 7363 616c 655f 3220 3d20 7365 6c66 2e7a  scale_2 = self.z
-000111b0: 6361 6c69 6272 6174 696f 6e20 2020 2020  calibration     
-000111c0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+000111a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000111b0: 6361 6c65 5f31 203d 2073 656c 662e 7963  cale_1 = self.yc
+000111c0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
 000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111f0: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
-00011200: 795f 6469 6d65 6e73 696f 6e5b 305d 203d  y_dimension[0] =
-00011210: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+000111f0: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
+00011200: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
+00011210: 5b31 5d20 3d3d 2030 3a0d 0a20 2020 2020  [1] == 0:..     
 00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011240: 2073 6361 6c65 5f31 203d 2073 656c 662e   scale_1 = self.
-00011250: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
-00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011240: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00011250: 6c65 5f32 203d 2073 656c 662e 7863 616c  le_2 = self.xcal
+00011260: 6962 7261 7469 6f6e 2020 0d0a 0d0a 2020  ibration  ....  
 00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011280: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
-00011290: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
-000112a0: 6f6e 5b31 5d20 3d3d 2031 3a0d 0a20 2020  on[1] == 1:..   
-000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011290: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+000112a0: 795f 6469 6d65 6e73 696f 6e5b 305d 203d  y_dimension[0] =
+000112b0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
 000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000112e0: 6361 6c65 5f32 203d 2073 656c 662e 7963  cale_2 = self.yc
-000112f0: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
+000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112e0: 2073 6361 6c65 5f31 203d 2073 656c 662e   scale_1 = self.
+000112f0: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
 00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
-00011330: 795f 6469 6d65 6e73 696f 6e5b 305d 203d  y_dimension[0] =
-00011340: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+00011320: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
+00011330: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
+00011340: 6f6e 5b31 5d20 3d3d 2032 3a0d 0a20 2020  on[1] == 2:..   
 00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011370: 2073 6361 6c65 5f31 203d 2073 656c 662e   scale_1 = self.
-00011380: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
-00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
-000113c0: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
-000113d0: 6f6e 5b31 5d20 3d3d 2032 3a0d 0a20 2020  on[1] == 2:..   
-000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011400: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011410: 6361 6c65 5f32 203d 2073 656c 662e 7a63  cale_2 = self.zc
-00011420: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011370: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011380: 6361 6c65 5f32 203d 2073 656c 662e 7a63  cale_2 = self.zc
+00011390: 616c 6962 7261 7469 6f6e 2020 2020 2020  alibration      
+000113a0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113d0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+000113e0: 5f64 696d 656e 7369 6f6e 5b30 5d20 3d3d  _dimension[0] ==
+000113f0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011420: 7363 616c 655f 3120 3d20 7365 6c66 2e78  scale_1 = self.x
+00011430: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
 00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011490: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00011460: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
+00011470: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
+00011480: 6e5b 315d 203d 3d20 313a 0d0a 2020 2020  n[1] == 1:..    
+00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000114c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114e0: 2020 2020 2063 656c 6c5f 6178 6973 203d       cell_axis =
-000114f0: 206f 7574 7075 745f 6c61 7267 6573 745f   output_largest_
-00011500: 6569 6765 6e76 6563 746f 725b 695d 0d0a  eigenvector[i]..
-00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011530: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
-00011540: 203d 206f 7574 7075 745f 636c 6f75 645f   = output_cloud_
-00011550: 7375 7266 6163 655f 6172 6561 5b69 5d20  surface_area[i] 
-00011560: 2a20 7365 6c66 2e7a 6361 6c69 6272 6174  * self.zcalibrat
-00011570: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
-00011580: 6272 6174 696f 6e20 2a20 7365 6c66 2e78  bration * self.x
-00011590: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115c0: 2064 6973 742c 2069 6e64 6578 203d 2074   dist, index = t
-000115d0: 7265 652e 7175 6572 7928 6365 6e74 726f  ree.query(centro
-000115e0: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
-000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011600: 2020 2020 2020 2020 2072 6164 6975 7320           radius 
-00011610: 3d20 7175 616c 6974 7920 2a20 6d61 7468  = quality * math
-00011620: 2e70 6f77 2873 656c 662e 7a63 616c 6962  .pow(self.zcalib
-00011630: 7261 7469 6f6e 202a 2073 656c 662e 7863  ration * self.xc
-00011640: 616c 6962 7261 7469 6f6e 202a 2073 656c  alibration * sel
-00011650: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
-00011660: 312e 302f 332e 3029 0d0a 2020 2020 2020  1.0/3.0)..      
-00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011680: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011690: 2064 6973 7420 3c20 7175 616c 6974 793a   dist < quality:
-000116a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000114b0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+000114c0: 616c 655f 3220 3d20 7365 6c66 2e79 6361  ale_2 = self.yca
+000114d0: 6c69 6272 6174 696f 6e0d 0a0d 0a20 2020  libration....   
+000114e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011500: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+00011510: 5f64 696d 656e 7369 6f6e 5b30 5d20 3d3d  _dimension[0] ==
+00011520: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011550: 7363 616c 655f 3120 3d20 7365 6c66 2e78  scale_1 = self.x
+00011560: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
+00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011590: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
+000115a0: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
+000115b0: 6e5b 315d 203d 3d20 323a 0d0a 2020 2020  n[1] == 2:..    
+000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115e0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+000115f0: 616c 655f 3220 3d20 7365 6c66 2e7a 6361  ale_2 = self.zca
+00011600: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+00011610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011670: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011690: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000116a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116c0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-000116d0: 6f73 6573 745f 6365 6e74 726f 6964 203d  osest_centroid =
-000116e0: 2073 706f 745f 6365 6e74 726f 6964 735b   spot_centroids[
-000116f0: 696e 6465 785d 0d0a 2020 2020 2020 2020  index]..        
+000116c0: 2020 2020 6365 6c6c 5f61 7869 7320 3d20      cell_axis = 
+000116d0: 6f75 7470 7574 5f6c 6172 6765 7374 5f65  output_largest_e
+000116e0: 6967 656e 7665 6374 6f72 5b69 5d0d 0a20  igenvector[i].. 
+000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011720: 2020 2020 6672 616d 655f 7370 6f74 5f63      frame_spot_c
-00011730: 656e 7472 6f69 6420 3d20 2869 6e74 2874  entroid = (int(t
-00011740: 696d 655f 6b65 7929 2c63 6c6f 7365 7374  ime_key),closest
-00011750: 5f63 656e 7472 6f69 645b 305d 2c20 636c  _centroid[0], cl
-00011760: 6f73 6573 745f 6365 6e74 726f 6964 5b31  osest_centroid[1
-00011770: 5d2c 2063 6c6f 7365 7374 5f63 656e 7472  ], closest_centr
-00011780: 6f69 645b 325d 290d 0a20 2020 2020 2020  oid[2])..       
+00011710: 2020 2073 7572 6661 6365 5f61 7265 6120     surface_area 
+00011720: 3d20 6f75 7470 7574 5f63 6c6f 7564 5f73  = output_cloud_s
+00011730: 7572 6661 6365 5f61 7265 615b 695d 202a  urface_area[i] *
+00011740: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+00011750: 6f6e 202a 2073 656c 662e 7963 616c 6962  on * self.ycalib
+00011760: 7261 7469 6f6e 202a 2073 656c 662e 7863  ration * self.xc
+00011770: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00011780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117b0: 2020 2020 2063 6c6f 7365 7374 5f63 656c       closest_cel
-000117c0: 6c5f 6964 203d 2073 656c 662e 756e 6971  l_id = self.uniq
-000117d0: 7565 5f73 706f 745f 6365 6e74 726f 6964  ue_spot_centroid
-000117e0: 5b66 7261 6d65 5f73 706f 745f 6365 6e74  [frame_spot_cent
-000117f0: 726f 6964 5d0d 0a20 2020 2020 2020 2020  roid]..         
-00011800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011820: 2020 206d 6173 6b5f 7665 6374 6f72 203d     mask_vector =
-00011830: 205b 2066 6c6f 6174 2873 656c 662e 756e   [ float(self.un
-00011840: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011850: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00011860: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
-00011870: 6d61 736b 6365 6e74 726f 6964 5f78 5f6b  maskcentroid_x_k
-00011880: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
-00011890: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000118a0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-000118b0: 6573 745f 6365 6c6c 5f69 6429 5d5b 7365  est_cell_id)][se
-000118c0: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-000118d0: 795f 6b65 795d 292c 2066 6c6f 6174 2873  y_key]), float(s
-000118e0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000118f0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00011900: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-00011910: 5b73 656c 662e 6d61 736b 6365 6e74 726f  [self.maskcentro
-00011920: 6964 5f7a 5f6b 6579 5d29 205d 0d0a 2020  id_z_key]) ]..  
-00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011950: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
-00011960: 7869 735f 6d61 736b 203d 2061 6e67 756c  xis_mask = angul
-00011970: 6172 5f63 6861 6e67 6528 6365 6c6c 5f61  ar_change(cell_a
-00011980: 7869 732c 206d 6173 6b5f 7665 6374 6f72  xis, mask_vector
-00011990: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000119c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000119f0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00011a00: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00011a10: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-00011a20: 7064 6174 6528 7b73 656c 662e 6365 6c6c  pdate({self.cell
-00011a30: 6178 6973 5f6d 6173 6b5f 6b65 7920 3a20  axis_mask_key : 
-00011a40: 6365 6c6c 5f61 7869 735f 6d61 736b 7d29  cell_axis_mask})
-00011a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a70: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011a80: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00011a90: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00011aa0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00011ab0: 295d 5b73 656c 662e 7261 6469 7573 5f6b  )][self.radius_k
-00011ac0: 6579 5d20 3e20 303a 0d0a 2020 2020 2020  ey] > 0:..      
-00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011af0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011b00: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00011b10: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00011b20: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
-00011b30: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-00011b40: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00011b50: 6972 7374 6b65 7920 3a20 6563 6365 6e74  irstkey : eccent
-00011b60: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00011b70: 7479 7a5b 305d 202a 2073 6361 6c65 5f31  tyz[0] * scale_1
-00011b80: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117a0: 6469 7374 2c20 696e 6465 7820 3d20 7472  dist, index = tr
+000117b0: 6565 2e71 7565 7279 2863 656e 7472 6f69  ee.query(centroi
+000117c0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+000117d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117e0: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
+000117f0: 2071 7561 6c69 7479 202a 206d 6174 682e   quality * math.
+00011800: 706f 7728 7365 6c66 2e7a 6361 6c69 6272  pow(self.zcalibr
+00011810: 6174 696f 6e20 2a20 7365 6c66 2e78 6361  ation * self.xca
+00011820: 6c69 6272 6174 696f 6e20 2a20 7365 6c66  libration * self
+00011830: 2e79 6361 6c69 6272 6174 696f 6e2c 2031  .ycalibration, 1
+00011840: 2e30 2f33 2e30 290d 0a20 2020 2020 2020  .0/3.0)..       
+00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011860: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011870: 6469 7374 203c 2071 7561 6c69 7479 3a0d  dist < quality:.
+00011880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118a0: 2020 2020 2020 2020 2020 2020 2063 6c6f               clo
+000118b0: 7365 7374 5f63 656e 7472 6f69 6420 3d20  sest_centroid = 
+000118c0: 7370 6f74 5f63 656e 7472 6f69 6473 5b69  spot_centroids[i
+000118d0: 6e64 6578 5d0d 0a20 2020 2020 2020 2020  ndex]..         
+000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011900: 2020 2066 7261 6d65 5f73 706f 745f 6365     frame_spot_ce
+00011910: 6e74 726f 6964 203d 2028 696e 7428 7469  ntroid = (int(ti
+00011920: 6d65 5f6b 6579 292c 636c 6f73 6573 745f  me_key),closest_
+00011930: 6365 6e74 726f 6964 5b30 5d2c 2063 6c6f  centroid[0], clo
+00011940: 7365 7374 5f63 656e 7472 6f69 645b 315d  sest_centroid[1]
+00011950: 2c20 636c 6f73 6573 745f 6365 6e74 726f  , closest_centro
+00011960: 6964 5b32 5d29 0d0a 2020 2020 2020 2020  id[2])..        
+00011970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011990: 2020 2020 636c 6f73 6573 745f 6365 6c6c      closest_cell
+000119a0: 5f69 6420 3d20 7365 6c66 2e75 6e69 7175  _id = self.uniqu
+000119b0: 655f 7370 6f74 5f63 656e 7472 6f69 645b  e_spot_centroid[
+000119c0: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
+000119d0: 6f69 645d 0d0a 2020 2020 2020 2020 2020  oid]..          
+000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a00: 2020 6d61 736b 5f76 6563 746f 7220 3d20    mask_vector = 
+00011a10: 5b20 666c 6f61 7428 7365 6c66 2e75 6e69  [ float(self.uni
+00011a20: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011a30: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00011a40: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00011a50: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
+00011a60: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
+00011a70: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00011a80: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+00011a90: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
+00011aa0: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
+00011ab0: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
+00011ac0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00011ad0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00011ae0: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
+00011af0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00011b00: 645f 7a5f 6b65 795d 2920 5d0d 0a20 2020  d_z_key]) ]..   
+00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b30: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
+00011b40: 6973 5f6d 6173 6b20 3d20 616e 6775 6c61  is_mask = angula
+00011b50: 725f 6368 616e 6765 2863 656c 6c5f 6178  r_change(cell_ax
+00011b60: 6973 2c20 6d61 736b 5f76 6563 746f 7229  is, mask_vector)
+00011b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b90: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 00011ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bb0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00011bc0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00011bd0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00011be0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00011bf0: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
-00011c00: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
-00011c10: 6579 203a 2065 6363 656e 7472 6963 6974  ey : eccentricit
-00011c20: 795f 636f 6d70 5f66 6972 7374 797a 5b31  y_comp_firstyz[1
-00011c30: 5d20 2a20 7363 616c 655f 327d 290d 0a20  ] * scale_2}).. 
+00011bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011bd0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00011be0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00011bf0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00011c00: 6461 7465 287b 7365 6c66 2e63 656c 6c61  date({self.cella
+00011c10: 7869 735f 6d61 736b 5f6b 6579 203a 2063  xis_mask_key : c
+00011c20: 656c 6c5f 6178 6973 5f6d 6173 6b7d 290d  ell_axis_mask}).
+00011c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c70: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00011c80: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00011c90: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-00011ca0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00011cb0: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
-00011cc0: 6579 203a 2073 7572 6661 6365 5f61 7265  ey : surface_are
-00011cd0: 617d 290d 0a20 2020 2020 2020 2020 2020  a})..           
-00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d00: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00011d10: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011d20: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00011d30: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
-00011d40: 6528 7b73 656c 662e 7175 616c 6974 795f  e({self.quality_
-00011d50: 6b65 7920 3a20 7175 616c 6974 797d 290d  key : quality}).
-00011d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011c50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011c60: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00011c70: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00011c80: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00011c90: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
+00011ca0: 795d 203e 2030 3a0d 0a20 2020 2020 2020  y] > 0:..       
+00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011ce0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00011cf0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00011d00: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+00011d10: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
+00011d20: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00011d30: 7273 746b 6579 203a 2065 6363 656e 7472  rstkey : eccentr
+00011d40: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+00011d50: 797a 5b30 5d20 2a20 7363 616c 655f 317d  yz[0] * scale_1}
+00011d60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d90: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00011da0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011db0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00011dc0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00011dd0: 656c 662e 7261 6469 7573 5f6b 6579 203a  elf.radius_key :
-00011de0: 2072 6164 6975 7320 7d29 0d0a 2020 2020   radius })..    
-00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00011d90: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00011da0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00011db0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00011dc0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00011dd0: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
+00011de0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
+00011df0: 7920 3a20 6563 6365 6e74 7269 6369 7479  y : eccentricity
+00011e00: 5f63 6f6d 705f 6669 7273 7479 7a5b 315d  _comp_firstyz[1]
+00011e10: 202a 2073 6361 6c65 5f32 7d29 0d0a 2020   * scale_2})..  
 00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e50: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e80: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00011e90: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00011ea0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00011eb0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00011ec0: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
-00011ed0: 6974 795f 636f 6d70 5f66 6972 7374 6b65  ity_comp_firstke
-00011ee0: 7920 3a20 2d31 7d29 0d0a 2020 2020 2020  y : -1})..      
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011f20: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00011f30: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00011f40: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
-00011f50: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-00011f60: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00011f70: 6563 6f6e 646b 6579 203a 202d 317d 290d  econdkey : -1}).
-00011f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fb0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00011fc0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011fd0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00011fe0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00011ff0: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
-00012000: 5f6b 6579 203a 202d 317d 290d 0a20 2020  _key : -1})..   
+00011e50: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00011e60: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00011e70: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00011e80: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00011e90: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
+00011ea0: 7920 3a20 7375 7266 6163 655f 6172 6561  y : surface_area
+00011eb0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ee0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00011ef0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011f00: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00011f10: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00011f20: 287b 7365 6c66 2e71 7561 6c69 7479 5f6b  ({self.quality_k
+00011f30: 6579 203a 2071 7561 6c69 7479 7d29 0d0a  ey : quality})..
+00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00011f80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00011f90: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
+00011fa0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00011fb0: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
+00011fc0: 7261 6469 7573 207d 290d 0a20 2020 2020  radius })..     
+00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ff0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012040: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00012050: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00012060: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00012070: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00012080: 7175 616c 6974 795f 6b65 7920 3a20 2d31  quality_key : -1
-00012090: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120c0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000120d0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000120e0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-000120f0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00012100: 287b 7365 6c66 2e72 6164 6975 735f 6b65  ({self.radius_ke
-00012110: 7920 3a20 2d31 207d 290d 0a20 2020 2020  y : -1 })..     
-00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012140: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00012150: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
+00012030: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012060: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00012070: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00012080: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00012090: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000120a0: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
+000120b0: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
+000120c0: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
+000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012100: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00012110: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00012120: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+00012130: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
+00012140: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+00012150: 636f 6e64 6b65 7920 3a20 2d31 7d29 0d0a  condkey : -1})..
 00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012170: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012190: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-000121a0: 7629 2069 6e20 7365 6c66 2e72 6f6f 745f  v) in self.root_
-000121b0: 7370 6f74 732e 6974 656d 7328 293a 0d0a  spots.items():..
-000121c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 2020 7365 6c66 2e72 6f6f 745f 7370 6f74    self.root_spot
-000121f0: 735b 6b5d 203d 2073 656c 662e 756e 6971  s[k] = self.uniq
-00012200: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012210: 6573 5b6b 5d20 2020 2020 2020 2020 0d0a  es[k]         ..
-00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012230: 0d0a 2020 2020 6465 6620 5f63 6f6d 7075  ..    def _compu
-00012240: 7465 5f70 6865 6e6f 7479 7065 7328 7365  te_phenotypes(se
-00012250: 6c66 293a 0d0a 0d0a 2020 2020 2020 2020  lf):....        
-00012260: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
-00012270: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
-00012280: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
-00012290: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000122a0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000122b0: 6163 6b5f 6964 203d 206b 0d0a 2020 2020  ack_id = k..    
-000122c0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-000122d0: 6b6c 6574 5f70 726f 7065 7274 6965 7320  klet_properties 
-000122e0: 3d20 7365 6c66 2e75 6e69 7175 655f 7472  = self.unique_tr
-000122f0: 6163 6b5f 7072 6f70 6572 7469 6573 5b6b  ack_properties[k
-00012300: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012310: 2020 2074 7261 636b 7320 3d20 7365 6c66     tracks = self
-00012320: 2e75 6e69 7175 655f 7472 6163 6b73 5b6b  .unique_tracks[k
-00012330: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012340: 2020 205a 203d 2074 7261 636b 735b 3a2c     Z = tracks[:,
-00012350: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-00012360: 2020 2020 5920 3d20 7472 6163 6b73 5b3a      Y = tracks[:
-00012370: 2c33 5d0d 0a20 2020 2020 2020 2020 2020  ,3]..           
-00012380: 2020 2020 2058 203d 2074 7261 636b 735b       X = tracks[
-00012390: 3a2c 345d 0d0a 2020 2020 2020 2020 2020  :,4]..          
-000123a0: 2020 2020 2020 7469 6d65 203d 2074 7261        time = tra
-000123b0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000123c0: 5b3a 2c30 5d0d 0a20 2020 2020 2020 2020  [:,0]..         
-000123d0: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
-000123e0: 7320 3d20 7472 6163 6b6c 6574 5f70 726f  s = tracklet_pro
-000123f0: 7065 7274 6965 735b 3a2c 315d 0d0a 2020  perties[:,1]..  
-00012400: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00012410: 6971 7565 5f69 6473 5f73 6574 203d 2073  ique_ids_set = s
-00012420: 6574 2875 6e69 7175 655f 6964 7329 0d0a  et(unique_ids)..
-00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012440: 6765 6e65 7261 7469 6f6e 5f69 6473 203d  generation_ids =
-00012450: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00012460: 7469 6573 5b3a 2c32 5d0d 0a20 2020 2020  ties[:,2]..     
-00012470: 2020 2020 2020 2020 2020 2072 6164 6975             radiu
-00012480: 7320 3d20 7472 6163 6b6c 6574 5f70 726f  s = tracklet_pro
-00012490: 7065 7274 6965 735b 3a2c 335d 0d0a 2020  perties[:,3]..  
-000124a0: 2020 2020 2020 2020 2020 2020 2020 766f                vo
-000124b0: 6c75 6d65 203d 2074 7261 636b 6c65 745f  lume = tracklet_
-000124c0: 7072 6f70 6572 7469 6573 5b3a 2c34 5d0d  properties[:,4].
-000124d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000124e0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
-000124f0: 6d70 5f66 6972 7374 203d 2074 7261 636b  mp_first = track
-00012500: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00012510: 2c35 5d0d 0a20 2020 2020 2020 2020 2020  ,5]..           
-00012520: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
-00012530: 795f 636f 6d70 5f73 6563 6f6e 6420 3d20  y_comp_second = 
-00012540: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00012550: 6965 735b 3a2c 365d 0d0a 2020 2020 2020  ies[:,6]..      
-00012560: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
-00012570: 655f 6172 6561 203d 2074 7261 636b 6c65  e_area = trackle
-00012580: 745f 7072 6f70 6572 7469 6573 5b3a 2c37  t_properties[:,7
-00012590: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000125a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000125b0: 2020 2020 696e 7465 6e73 6974 7920 3d20      intensity = 
-000125c0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-000125d0: 6965 735b 3a2c 385d 0d0a 2020 2020 2020  ies[:,8]..      
-000125e0: 2020 2020 2020 2020 2020 7370 6565 6420            speed 
-000125f0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012600: 7274 6965 735b 3a2c 395d 0d0a 2020 2020  rties[:,9]..    
-00012610: 2020 2020 2020 2020 2020 2020 6d6f 7469              moti
-00012620: 6f6e 5f61 6e67 6c65 203d 2074 7261 636b  on_angle = track
-00012630: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00012640: 2c31 305d 0d0a 2020 2020 2020 2020 2020  ,10]..          
-00012650: 2020 2020 2020 6163 6365 6c65 7261 7469        accelerati
-00012660: 6f6e 203d 2074 7261 636b 6c65 745f 7072  on = tracklet_pr
-00012670: 6f70 6572 7469 6573 5b3a 2c31 315d 0d0a  operties[:,11]..
-00012680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012690: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000126a0: 736b 203d 2074 7261 636b 6c65 745f 7072  sk = tracklet_pr
-000126b0: 6f70 6572 7469 6573 5b3a 2c31 325d 0d0a  operties[:,12]..
-000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126d0: 7261 6469 616c 5f61 6e67 6c65 203d 2074  radial_angle = t
-000126e0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-000126f0: 6573 5b3a 2c31 335d 0d0a 2020 2020 2020  es[:,13]..      
-00012700: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
-00012710: 7869 735f 6d61 736b 203d 2074 7261 636b  xis_mask = track
-00012720: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00012730: 2c31 345d 0d0a 0d0a 0d0a 2020 2020 2020  ,14]......      
-00012740: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00012750: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-00012760: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
-00012770: 735f 7472 6163 6b6c 6574 203d 207b 7d0d  s_tracklet = {}.
-00012780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012790: 2075 6e69 7175 655f 636c 7573 7465 725f   unique_cluster_
-000127a0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-000127b0: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
-000127c0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000127d0: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
-000127e0: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
-000127f0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00012800: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00012810: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
-00012820: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
-00012830: 7b7d 0d0a 0d0a 2020 2020 2020 2020 2020  {}....          
-00012840: 2020 2020 2020 756e 6971 7565 5f73 6861        unique_sha
-00012850: 7065 5f70 726f 7065 7274 6965 735f 7472  pe_properties_tr
-00012860: 6163 6b6c 6574 203d 207b 7d0d 0a20 2020  acklet = {}..   
-00012870: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-00012880: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
-00012890: 6572 7469 6573 5f74 7261 636b 6c65 7420  erties_tracklet 
-000128a0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-000128b0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000128c0: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
-000128d0: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
-000128e0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-000128f0: 2020 2073 656c 662e 756e 6971 7565 5f64     self.unique_d
-00012900: 796e 616d 6963 5f70 726f 7065 7274 6965  ynamic_propertie
-00012910: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
-00012920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012930: 2020 6578 7061 6e64 6564 5f74 696d 6520    expanded_time 
-00012940: 3d20 6e70 2e7a 6572 6f73 2873 656c 662e  = np.zeros(self.
-00012950: 7465 6e64 202d 2073 656c 662e 7473 7461  tend - self.tsta
-00012960: 7274 202b 2031 290d 0a20 2020 2020 2020  rt + 1)..       
-00012970: 2020 2020 2020 2020 2070 6f69 6e74 5f73           point_s
-00012980: 616d 706c 6520 3d20 6578 7061 6e64 6564  ample = expanded
-00012990: 5f74 696d 652e 7368 6170 655b 305d 0d0a  _time.shape[0]..
-000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129b0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-000129c0: 656e 2865 7870 616e 6465 645f 7469 6d65  en(expanded_time
-000129d0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-000129e0: 2020 2020 2020 2020 2020 2020 6578 7061              expa
-000129f0: 6e64 6564 5f74 696d 655b 695d 203d 2069  nded_time[i] = i
-00012a00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00012a10: 2020 2066 6f72 2063 7572 7265 6e74 5f75     for current_u
-00012a20: 6e69 7175 655f 6964 2069 6e20 756e 6971  nique_id in uniq
-00012a30: 7565 5f69 6473 5f73 6574 3a0d 0a20 2020  ue_ids_set:..   
-00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012a60: 2020 2020 2065 7870 616e 6465 645f 696e       expanded_in
-00012a70: 7465 6e73 6974 7920 3d20 6e70 2e7a 6572  tensity = np.zer
-00012a80: 6f73 2873 656c 662e 7465 6e64 202d 2073  os(self.tend - s
-00012a90: 656c 662e 7473 7461 7274 202b 2031 290d  elf.tstart + 1).
-00012aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ab0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00012ac0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012ae0: 7272 656e 745f 7469 6d65 203d 205b 5d0d  rrent_time = [].
-00012af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012b00: 2020 2020 6375 7272 656e 745f 7a20 3d20      current_z = 
-00012b10: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012b20: 2020 2020 2020 2063 7572 7265 6e74 5f79         current_y
-00012b30: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012b40: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012b50: 745f 7820 3d20 5b5d 0d0a 2020 2020 2020  t_x = []..      
-00012b60: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012b70: 7265 6e74 5f69 6e74 656e 7369 7479 203d  rent_intensity =
-00012b80: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012b90: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012ba0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 6375 7272 656e 745f 766f 6c75 6d65 203d  current_volume =
-00012bd0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012be0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012bf0: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
-00012c00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012c10: 7572 7265 6e74 5f6d 6f74 696f 6e5f 616e  urrent_motion_an
-00012c20: 676c 6520 3d20 5b5d 0d0a 2020 2020 2020  gle = []..      
-00012c30: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012c40: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
-00012c50: 6e20 3d20 5b5d 0d0a 2020 2020 2020 2020  n = []..        
-00012c60: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012c70: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
-00012c80: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012ca0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00012cb0: 6974 795f 636f 6d70 5f66 6972 7374 203d  ity_comp_first =
-00012cc0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012cd0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012ce0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00012cf0: 705f 7365 636f 6e64 203d 205b 5d0d 0a20  p_second = [].. 
-00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d10: 2020 6375 7272 656e 745f 7375 7266 6163    current_surfac
-00012d20: 655f 6172 6561 203d 205b 5d0d 0a0d 0a20  e_area = [].... 
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2020 6375 7272 656e 745f 7261 6469 616c    current_radial
-00012d50: 5f61 6e67 6c65 203d 205b 5d0d 0a20 2020  _angle = []..   
-00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d70: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
-00012d80: 735f 6d61 736b 203d 205b 5d20 0d0a 2020  s_mask = [] ..  
-00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00012db0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-00012dc0: 616e 6765 2874 696d 652e 7368 6170 655b  ange(time.shape[
-00012dd0: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
-00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012df0: 6966 2063 7572 7265 6e74 5f75 6e69 7175  if current_uniqu
-00012e00: 655f 6964 203d 3d20 756e 6971 7565 5f69  e_id == unique_i
-00012e10: 6473 5b6a 5d3a 0d0a 2020 2020 2020 2020  ds[j]:..        
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012e40: 5f74 696d 652e 6170 7065 6e64 2874 696d  _time.append(tim
-00012e50: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e70: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012e80: 7a2e 6170 7065 6e64 285a 5b6a 5d29 0d0a  z.append(Z[j])..
-00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012eb0: 2063 7572 7265 6e74 5f79 2e61 7070 656e   current_y.appen
-00012ec0: 6428 595b 6a5d 290d 0a20 2020 2020 2020  d(Y[j])..       
-00012ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ee0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012ef0: 745f 782e 6170 7065 6e64 2858 5b6a 5d29  t_x.append(X[j])
-00012f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012190: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000121a0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000121b0: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
+000121c0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+000121d0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+000121e0: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
+000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012220: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00012230: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00012240: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00012250: 5d2e 7570 6461 7465 287b 7365 6c66 2e71  ].update({self.q
+00012260: 7561 6c69 7479 5f6b 6579 203a 202d 317d  uality_key : -1}
+00012270: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122a0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000122b0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000122c0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+000122d0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000122e0: 7b73 656c 662e 7261 6469 7573 5f6b 6579  {self.radius_key
+000122f0: 203a 202d 3120 7d29 0d0a 2020 2020 2020   : -1 })..      
+00012300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012320: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+00012330: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
+00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012350: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012370: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+00012380: 2920 696e 2073 656c 662e 726f 6f74 5f73  ) in self.root_s
+00012390: 706f 7473 2e69 7465 6d73 2829 3a0d 0a20  pots.items():.. 
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123c0: 2073 656c 662e 726f 6f74 5f73 706f 7473   self.root_spots
+000123d0: 5b6b 5d20 3d20 7365 6c66 2e75 6e69 7175  [k] = self.uniqu
+000123e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000123f0: 735b 6b5d 2020 2020 2020 2020 200d 0a20  s[k]         .. 
+00012400: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00012410: 0a20 2020 2064 6566 205f 636f 6d70 7574  .    def _comput
+00012420: 655f 7068 656e 6f74 7970 6573 2873 656c  e_phenotypes(sel
+00012430: 6629 3a0d 0a0d 0a20 2020 2020 2020 2020  f):....         
+00012440: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+00012450: 6c66 2e75 6e69 7175 655f 7472 6163 6b73  lf.unique_tracks
+00012460: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00012470: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012480: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00012490: 636b 5f69 6420 3d20 6b0d 0a20 2020 2020  ck_id = k..     
+000124a0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+000124b0: 6c65 745f 7072 6f70 6572 7469 6573 203d  let_properties =
+000124c0: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+000124d0: 636b 5f70 726f 7065 7274 6965 735b 6b5d  ck_properties[k]
+000124e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000124f0: 2020 7472 6163 6b73 203d 2073 656c 662e    tracks = self.
+00012500: 756e 6971 7565 5f74 7261 636b 735b 6b5d  unique_tracks[k]
+00012510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012520: 2020 5a20 3d20 7472 6163 6b73 5b3a 2c32    Z = tracks[:,2
+00012530: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012540: 2020 2059 203d 2074 7261 636b 735b 3a2c     Y = tracks[:,
+00012550: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
+00012560: 2020 2020 5820 3d20 7472 6163 6b73 5b3a      X = tracks[:
+00012570: 2c34 5d0d 0a20 2020 2020 2020 2020 2020  ,4]..           
+00012580: 2020 2020 2074 696d 6520 3d20 7472 6163       time = trac
+00012590: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+000125a0: 3a2c 305d 0d0a 2020 2020 2020 2020 2020  :,0]..          
+000125b0: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
+000125c0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+000125d0: 6572 7469 6573 5b3a 2c31 5d0d 0a20 2020  erties[:,1]..   
+000125e0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+000125f0: 7175 655f 6964 735f 7365 7420 3d20 7365  que_ids_set = se
+00012600: 7428 756e 6971 7565 5f69 6473 290d 0a20  t(unique_ids).. 
+00012610: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00012620: 656e 6572 6174 696f 6e5f 6964 7320 3d20  eneration_ids = 
+00012630: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00012640: 6965 735b 3a2c 325d 0d0a 2020 2020 2020  ies[:,2]..      
+00012650: 2020 2020 2020 2020 2020 7261 6469 7573            radius
+00012660: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00012670: 6572 7469 6573 5b3a 2c33 5d0d 0a20 2020  erties[:,3]..   
+00012680: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
+00012690: 756d 6520 3d20 7472 6163 6b6c 6574 5f70  ume = tracklet_p
+000126a0: 726f 7065 7274 6965 735b 3a2c 345d 0d0a  roperties[:,4]..
+000126b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126c0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+000126d0: 705f 6669 7273 7420 3d20 7472 6163 6b6c  p_first = trackl
+000126e0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000126f0: 355d 0d0a 2020 2020 2020 2020 2020 2020  5]..            
+00012700: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+00012710: 5f63 6f6d 705f 7365 636f 6e64 203d 2074  _comp_second = t
+00012720: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012730: 6573 5b3a 2c36 5d0d 0a20 2020 2020 2020  es[:,6]..       
+00012740: 2020 2020 2020 2020 2073 7572 6661 6365           surface
+00012750: 5f61 7265 6120 3d20 7472 6163 6b6c 6574  _area = tracklet
+00012760: 5f70 726f 7065 7274 6965 735b 3a2c 375d  _properties[:,7]
+00012770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012780: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012790: 2020 2069 6e74 656e 7369 7479 203d 2074     intensity = t
+000127a0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+000127b0: 6573 5b3a 2c38 5d0d 0a20 2020 2020 2020  es[:,8]..       
+000127c0: 2020 2020 2020 2020 2073 7065 6564 203d           speed =
+000127d0: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+000127e0: 7469 6573 5b3a 2c39 5d0d 0a20 2020 2020  ties[:,9]..     
+000127f0: 2020 2020 2020 2020 2020 206d 6f74 696f             motio
+00012800: 6e5f 616e 676c 6520 3d20 7472 6163 6b6c  n_angle = trackl
+00012810: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00012820: 3130 5d0d 0a20 2020 2020 2020 2020 2020  10]..           
+00012830: 2020 2020 2061 6363 656c 6572 6174 696f       acceleratio
+00012840: 6e20 3d20 7472 6163 6b6c 6574 5f70 726f  n = tracklet_pro
+00012850: 7065 7274 6965 735b 3a2c 3131 5d0d 0a20  perties[:,11].. 
+00012860: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00012870: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00012880: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
+00012890: 7065 7274 6965 735b 3a2c 3132 5d0d 0a20  perties[:,12].. 
+000128a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000128b0: 6164 6961 6c5f 616e 676c 6520 3d20 7472  adial_angle = tr
+000128c0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+000128d0: 735b 3a2c 3133 5d0d 0a20 2020 2020 2020  s[:,13]..       
+000128e0: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
+000128f0: 6973 5f6d 6173 6b20 3d20 7472 6163 6b6c  is_mask = trackl
+00012900: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00012910: 3134 5d0d 0a0d 0a0d 0a20 2020 2020 2020  14]......       
+00012920: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00012930: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00012940: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
+00012950: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
+00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012970: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
+00012980: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00012990: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
+000129a0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000129b0: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
+000129c0: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
+000129d0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+000129e0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000129f0: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
+00012a00: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
+00012a10: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
+00012a20: 2020 2020 2075 6e69 7175 655f 7368 6170       unique_shap
+00012a30: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
+00012a40: 636b 6c65 7420 3d20 7b7d 0d0a 2020 2020  cklet = {}..    
+00012a50: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+00012a60: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
+00012a70: 7274 6965 735f 7472 6163 6b6c 6574 203d  rties_tracklet =
+00012a80: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00012a90: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00012aa0: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+00012ab0: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
+00012ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012ad0: 2020 7365 6c66 2e75 6e69 7175 655f 6479    self.unique_dy
+00012ae0: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
+00012af0: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
+00012b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b10: 2065 7870 616e 6465 645f 7469 6d65 203d   expanded_time =
+00012b20: 206e 702e 7a65 726f 7328 7365 6c66 2e74   np.zeros(self.t
+00012b30: 656e 6420 2d20 7365 6c66 2e74 7374 6172  end - self.tstar
+00012b40: 7420 2b20 3129 0d0a 2020 2020 2020 2020  t + 1)..        
+00012b50: 2020 2020 2020 2020 706f 696e 745f 7361          point_sa
+00012b60: 6d70 6c65 203d 2065 7870 616e 6465 645f  mple = expanded_
+00012b70: 7469 6d65 2e73 6861 7065 5b30 5d0d 0a20  time.shape[0].. 
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00012b90: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00012ba0: 6e28 6578 7061 6e64 6564 5f74 696d 6529  n(expanded_time)
+00012bb0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00012bc0: 2020 2020 2020 2020 2020 2065 7870 616e             expan
+00012bd0: 6465 645f 7469 6d65 5b69 5d20 3d20 6920  ded_time[i] = i 
+00012be0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012bf0: 2020 666f 7220 6375 7272 656e 745f 756e    for current_un
+00012c00: 6971 7565 5f69 6420 696e 2075 6e69 7175  ique_id in uniqu
+00012c10: 655f 6964 735f 7365 743a 0d0a 2020 2020  e_ids_set:..    
+00012c20: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00012c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c40: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
+00012c50: 656e 7369 7479 203d 206e 702e 7a65 726f  ensity = np.zero
+00012c60: 7328 7365 6c66 2e74 656e 6420 2d20 7365  s(self.tend - se
+00012c70: 6c66 2e74 7374 6172 7420 2b20 3129 0d0a  lf.tstart + 1)..
+00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c90: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00012ca0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00012cb0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012cc0: 7265 6e74 5f74 696d 6520 3d20 5b5d 0d0a  rent_time = []..
+00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ce0: 2020 2063 7572 7265 6e74 5f7a 203d 205b     current_z = [
+00012cf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012d00: 2020 2020 2020 6375 7272 656e 745f 7920        current_y 
+00012d10: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012d20: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012d30: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00012d40: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012d50: 656e 745f 696e 7465 6e73 6974 7920 3d20  ent_intensity = 
+00012d60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012d70: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
+00012d80: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012da0: 7572 7265 6e74 5f76 6f6c 756d 6520 3d20  urrent_volume = 
+00012db0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012dc0: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
+00012dd0: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
+00012de0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012df0: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
+00012e00: 6c65 203d 205b 5d0d 0a20 2020 2020 2020  le = []..       
+00012e10: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012e20: 656e 745f 6163 6365 6c65 7261 7469 6f6e  ent_acceleration
+00012e30: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00012e40: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012e50: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
+00012e60: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
+00012e70: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012e80: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00012e90: 7479 5f63 6f6d 705f 6669 7273 7420 3d20  ty_comp_first = 
+00012ea0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012eb0: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
+00012ec0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00012ed0: 5f73 6563 6f6e 6420 3d20 5b5d 0d0a 2020  _second = []..  
+00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ef0: 2063 7572 7265 6e74 5f73 7572 6661 6365   current_surface
+00012f00: 5f61 7265 6120 3d20 5b5d 0d0a 0d0a 2020  _area = []....  
 00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 2020 2065 7870 616e 6465 645f 696e 7465     expanded_inte
-00012f30: 6e73 6974 795b 696e 7428 7469 6d65 5b6a  nsity[int(time[j
-00012f40: 5d29 5d20 3d20 696e 7465 6e73 6974 795b  ])] = intensity[
-00012f50: 6a5d 0d0a 2020 2020 2020 2020 2020 2020  j]..            
-00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f70: 2020 2020 2063 7572 7265 6e74 5f69 6e74       current_int
-00012f80: 656e 7369 7479 2e61 7070 656e 6428 696e  ensity.append(in
-00012f90: 7465 6e73 6974 795b 6a5d 290d 0a20 2020  tensity[j])..   
-00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012fc0: 7272 656e 745f 7261 6469 7573 2e61 7070  rrent_radius.app
-00012fd0: 656e 6428 7261 6469 7573 5b6a 5d29 0d0a  end(radius[j])..
-00012fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 2063 7572 7265 6e74 5f76 6f6c 756d 652e   current_volume.
-00013010: 6170 7065 6e64 2876 6f6c 756d 655b 6a5d  append(volume[j]
-00013020: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013040: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
-00013050: 642e 6170 7065 6e64 2873 7065 6564 5b6a  d.append(speed[j
-00013060: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00012f20: 2063 7572 7265 6e74 5f72 6164 6961 6c5f   current_radial_
+00012f30: 616e 676c 6520 3d20 5b5d 0d0a 2020 2020  angle = []..    
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012f50: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
+00012f60: 5f6d 6173 6b20 3d20 5b5d 200d 0a20 2020  _mask = [] ..   
+00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012f90: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+00012fa0: 6e67 6528 7469 6d65 2e73 6861 7065 5b30  nge(time.shape[0
+00012fb0: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+00012fc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012fd0: 6620 6375 7272 656e 745f 756e 6971 7565  f current_unique
+00012fe0: 5f69 6420 3d3d 2075 6e69 7175 655f 6964  _id == unique_id
+00012ff0: 735b 6a5d 3a0d 0a20 2020 2020 2020 2020  s[j]:..         
+00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013010: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013020: 7469 6d65 2e61 7070 656e 6428 7469 6d65  time.append(time
+00013030: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013050: 2020 2020 2020 2063 7572 7265 6e74 5f7a         current_z
+00013060: 2e61 7070 656e 6428 5a5b 6a5d 290d 0a20  .append(Z[j]).. 
 00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 2020 2063 7572 7265 6e74 5f6d 6f74       current_mot
-00013090: 696f 6e5f 616e 676c 652e 6170 7065 6e64  ion_angle.append
-000130a0: 286d 6f74 696f 6e5f 616e 676c 655b 6a5d  (motion_angle[j]
-000130b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130d0: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
-000130e0: 6c65 7261 7469 6f6e 2e61 7070 656e 6428  leration.append(
-000130f0: 6163 6365 6c65 7261 7469 6f6e 5b6a 5d29  acceleration[j])
-00013100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013120: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
-00013130: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00013140: 7065 6e64 2864 6973 7461 6e63 655f 6365  pend(distance_ce
-00013150: 6c6c 5f6d 6173 6b5b 6a5d 290d 0a20 2020  ll_mask[j])..   
-00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013170: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013180: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-00013190: 7479 5f63 6f6d 705f 6669 7273 742e 6170  ty_comp_first.ap
-000131a0: 7065 6e64 2865 6363 656e 7472 6963 6974  pend(eccentricit
-000131b0: 795f 636f 6d70 5f66 6972 7374 5b6a 5d29  y_comp_first[j])
-000131c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013090: 6375 7272 656e 745f 792e 6170 7065 6e64  current_y.append
+000130a0: 2859 5b6a 5d29 0d0a 2020 2020 2020 2020  (Y[j])..        
+000130b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130c0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000130d0: 5f78 2e61 7070 656e 6428 585b 6a5d 290d  _x.append(X[j]).
+000130e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013100: 2020 6578 7061 6e64 6564 5f69 6e74 656e    expanded_inten
+00013110: 7369 7479 5b69 6e74 2874 696d 655b 6a5d  sity[int(time[j]
+00013120: 295d 203d 2069 6e74 656e 7369 7479 5b6a  )] = intensity[j
+00013130: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013150: 2020 2020 6375 7272 656e 745f 696e 7465      current_inte
+00013160: 6e73 6974 792e 6170 7065 6e64 2869 6e74  nsity.append(int
+00013170: 656e 7369 7479 5b6a 5d29 0d0a 2020 2020  ensity[j])..    
+00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013190: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000131a0: 7265 6e74 5f72 6164 6975 732e 6170 7065  rent_radius.appe
+000131b0: 6e64 2872 6164 6975 735b 6a5d 290d 0a20  nd(radius[j]).. 
+000131c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
-000131f0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00013200: 6f6e 642e 6170 7065 6e64 2865 6363 656e  ond.append(eccen
-00013210: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00013220: 6f6e 645b 6a5d 290d 0a20 2020 2020 2020  ond[j])..       
-00013230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013240: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013250: 745f 7375 7266 6163 655f 6172 6561 2e61  t_surface_area.a
-00013260: 7070 656e 6428 7375 7266 6163 655f 6172  ppend(surface_ar
-00013270: 6561 5b6a 5d29 0d0a 2020 2020 2020 2020  ea[j])..        
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013290: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000132a0: 5f72 6164 6961 6c5f 616e 676c 652e 6170  _radial_angle.ap
-000132b0: 7065 6e64 2872 6164 6961 6c5f 616e 676c  pend(radial_angl
-000132c0: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
-000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132e0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000132f0: 6365 6c6c 5f61 7869 735f 6d61 736b 2e61  cell_axis_mask.a
-00013300: 7070 656e 6428 6365 6c6c 5f61 7869 735f  ppend(cell_axis_
-00013310: 6d61 736b 5b6a 5d29 0d0a 2020 2020 2020  mask[j])..      
-00013320: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013330: 7265 6e74 5f74 696d 6520 3d20 6e70 2e61  rent_time = np.a
-00013340: 7361 7272 6179 2863 7572 7265 6e74 5f74  sarray(current_t
-00013350: 696d 652c 2064 7479 7065 3d6e 702e 666c  ime, dtype=np.fl
-00013360: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00013370: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013380: 6e74 5f69 6e74 656e 7369 7479 203d 206e  nt_intensity = n
-00013390: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-000133a0: 745f 696e 7465 6e73 6974 792c 2064 7479  t_intensity, dty
-000133b0: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-000133c0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-000133d0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000133e0: 5f72 6164 6975 7320 3d20 6e70 2e61 7361  _radius = np.asa
-000133f0: 7272 6179 2863 7572 7265 6e74 5f72 6164  rray(current_rad
-00013400: 6975 732c 2064 7479 7065 3d6e 702e 666c  ius, dtype=np.fl
-00013410: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00013420: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013430: 6e74 5f76 6f6c 756d 6520 3d20 6e70 2e61  nt_volume = np.a
-00013440: 7361 7272 6179 2863 7572 7265 6e74 5f76  sarray(current_v
-00013450: 6f6c 756d 652c 2064 7479 7065 3d6e 702e  olume, dtype=np.
-00013460: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-00013470: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013480: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-00013490: 795f 636f 6d70 5f66 6972 7374 203d 206e  y_comp_first = n
-000134a0: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-000134b0: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
-000134c0: 6f6d 705f 6669 7273 742c 2064 7479 7065  omp_first, dtype
-000134d0: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
-000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134f0: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
-00013500: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-00013510: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
-00013520: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00013530: 6974 795f 636f 6d70 5f73 6563 6f6e 642c  ity_comp_second,
-00013540: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00013550: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00013560: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-00013570: 7572 6661 6365 5f61 7265 6120 3d20 6e70  urface_area = np
-00013580: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013590: 5f73 7572 6661 6365 5f61 7265 612c 2064  _surface_area, d
-000135a0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-000135b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000135c0: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-000135d0: 7065 6564 203d 206e 702e 6173 6172 7261  peed = np.asarra
-000135e0: 7928 6375 7272 656e 745f 7370 6565 642c  y(current_speed,
-000135f0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00013600: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00013610: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
-00013620: 6f74 696f 6e5f 616e 676c 6520 3d20 6e70  otion_angle = np
-00013630: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013640: 5f6d 6f74 696f 6e5f 616e 676c 652c 2064  _motion_angle, d
-00013650: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00013660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013670: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
-00013680: 656c 6572 6174 696f 6e20 3d20 6e70 2e61  eleration = np.a
-00013690: 7361 7272 6179 2863 7572 7265 6e74 5f61  sarray(current_a
-000136a0: 6363 656c 6572 6174 696f 6e2c 2064 7479  cceleration, dty
-000136b0: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+000131e0: 6375 7272 656e 745f 766f 6c75 6d65 2e61  current_volume.a
+000131f0: 7070 656e 6428 766f 6c75 6d65 5b6a 5d29  ppend(volume[j])
+00013200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013220: 2020 2063 7572 7265 6e74 5f73 7065 6564     current_speed
+00013230: 2e61 7070 656e 6428 7370 6565 645b 6a5d  .append(speed[j]
+00013240: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013260: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
+00013270: 6f6e 5f61 6e67 6c65 2e61 7070 656e 6428  on_angle.append(
+00013280: 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a 5d29  motion_angle[j])
+00013290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
+000132c0: 6572 6174 696f 6e2e 6170 7065 6e64 2861  eration.append(a
+000132d0: 6363 656c 6572 6174 696f 6e5b 6a5d 290d  cceleration[j]).
+000132e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013300: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
+00013310: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+00013320: 656e 6428 6469 7374 616e 6365 5f63 656c  end(distance_cel
+00013330: 6c5f 6d61 736b 5b6a 5d29 0d0a 2020 2020  l_mask[j])..    
+00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013350: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013360: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+00013370: 795f 636f 6d70 5f66 6972 7374 2e61 7070  y_comp_first.app
+00013380: 656e 6428 6563 6365 6e74 7269 6369 7479  end(eccentricity
+00013390: 5f63 6f6d 705f 6669 7273 745b 6a5d 290d  _comp_first[j]).
+000133a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133c0: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
+000133d0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+000133e0: 6e64 2e61 7070 656e 6428 6563 6365 6e74  nd.append(eccent
+000133f0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00013400: 6e64 5b6a 5d29 0d0a 2020 2020 2020 2020  nd[j])..        
+00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013420: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013430: 5f73 7572 6661 6365 5f61 7265 612e 6170  _surface_area.ap
+00013440: 7065 6e64 2873 7572 6661 6365 5f61 7265  pend(surface_are
+00013450: 615b 6a5d 290d 0a20 2020 2020 2020 2020  a[j])..         
+00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013470: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013480: 7261 6469 616c 5f61 6e67 6c65 2e61 7070  radial_angle.app
+00013490: 656e 6428 7261 6469 616c 5f61 6e67 6c65  end(radial_angle
+000134a0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134c0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+000134d0: 656c 6c5f 6178 6973 5f6d 6173 6b2e 6170  ell_axis_mask.ap
+000134e0: 7065 6e64 2863 656c 6c5f 6178 6973 5f6d  pend(cell_axis_m
+000134f0: 6173 6b5b 6a5d 290d 0a20 2020 2020 2020  ask[j])..       
+00013500: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013510: 656e 745f 7469 6d65 203d 206e 702e 6173  ent_time = np.as
+00013520: 6172 7261 7928 6375 7272 656e 745f 7469  array(current_ti
+00013530: 6d65 2c20 6474 7970 653d 6e70 2e66 6c6f  me, dtype=np.flo
+00013540: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00013550: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013560: 745f 696e 7465 6e73 6974 7920 3d20 6e70  t_intensity = np
+00013570: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013580: 5f69 6e74 656e 7369 7479 2c20 6474 7970  _intensity, dtyp
+00013590: 653d 6e70 2e66 6c6f 6174 3332 290d 0a0d  e=np.float32)...
+000135a0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+000135b0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000135c0: 7261 6469 7573 203d 206e 702e 6173 6172  radius = np.asar
+000135d0: 7261 7928 6375 7272 656e 745f 7261 6469  ray(current_radi
+000135e0: 7573 2c20 6474 7970 653d 6e70 2e66 6c6f  us, dtype=np.flo
+000135f0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00013600: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013610: 745f 766f 6c75 6d65 203d 206e 702e 6173  t_volume = np.as
+00013620: 6172 7261 7928 6375 7272 656e 745f 766f  array(current_vo
+00013630: 6c75 6d65 2c20 6474 7970 653d 6e70 2e66  lume, dtype=np.f
+00013640: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00013650: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013660: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00013670: 5f63 6f6d 705f 6669 7273 7420 3d20 6e70  _comp_first = np
+00013680: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013690: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+000136a0: 6d70 5f66 6972 7374 2c20 6474 7970 653d  mp_first, dtype=
+000136b0: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
 000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136d0: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
-000136e0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
-000136f0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00013700: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
-00013710: 5f6d 6173 6b2c 2064 7479 7065 3d6e 702e  _mask, dtype=np.
-00013720: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-00013730: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013740: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
-00013750: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
-00013760: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
-00013770: 676c 652c 2064 7479 7065 3d6e 702e 666c  gle, dtype=np.fl
-00013780: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00013790: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000137a0: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
-000137b0: 6b20 3d20 6e70 2e61 7361 7272 6179 2863  k = np.asarray(c
-000137c0: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
-000137d0: 5f6d 6173 6b2c 2064 7479 7065 3d6e 702e  _mask, dtype=np.
-000137e0: 666c 6f61 7433 3229 0d0a 0d0a 0d0a 2020  float32)......  
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00013810: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00013820: 2020 2020 2020 2020 2020 2069 6620 706f             if po
-00013830: 696e 745f 7361 6d70 6c65 203e 2030 3a0d  int_sample > 0:.
+000136d0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+000136e0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+000136f0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00013700: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00013710: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
+00013720: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00013730: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013740: 2020 2020 2020 6375 7272 656e 745f 7375        current_su
+00013750: 7266 6163 655f 6172 6561 203d 206e 702e  rface_area = np.
+00013760: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00013770: 7375 7266 6163 655f 6172 6561 2c20 6474  surface_area, dt
+00013780: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+00013790: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000137a0: 2020 2020 2020 6375 7272 656e 745f 7370        current_sp
+000137b0: 6565 6420 3d20 6e70 2e61 7361 7272 6179  eed = np.asarray
+000137c0: 2863 7572 7265 6e74 5f73 7065 6564 2c20  (current_speed, 
+000137d0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+000137e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000137f0: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
+00013800: 7469 6f6e 5f61 6e67 6c65 203d 206e 702e  tion_angle = np.
+00013810: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00013820: 6d6f 7469 6f6e 5f61 6e67 6c65 2c20 6474  motion_angle, dt
+00013830: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
 00013840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013860: 2078 665f 7361 6d70 6c65 203d 2066 6674   xf_sample = fft
-00013870: 6672 6571 2870 6f69 6e74 5f73 616d 706c  freq(point_sampl
-00013880: 652c 2073 656c 662e 7463 616c 6962 7261  e, self.tcalibra
-00013890: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
+00013850: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
+00013860: 6c65 7261 7469 6f6e 203d 206e 702e 6173  leration = np.as
+00013870: 6172 7261 7928 6375 7272 656e 745f 6163  array(current_ac
+00013880: 6365 6c65 7261 7469 6f6e 2c20 6474 7970  celeration, dtyp
+00013890: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
 000138a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138b0: 2020 2020 2020 2066 6674 7374 7269 705f         fftstrip_
-000138c0: 7361 6d70 6c65 203d 2066 6674 2865 7870  sample = fft(exp
-000138d0: 616e 6465 645f 696e 7465 6e73 6974 7929  anded_intensity)
-000138e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000138f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013900: 2020 6666 7474 6f74 616c 5f73 616d 706c    ffttotal_sampl
-00013910: 6520 3d20 6e70 2e61 6273 2866 6674 7374  e = np.abs(fftst
-00013920: 7269 705f 7361 6d70 6c65 290d 0a20 2020  rip_sample)..   
-00013930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013940: 2020 2020 2020 2020 2020 2020 2078 665f               xf_
-00013950: 7361 6d70 6c65 203d 2078 665f 7361 6d70  sample = xf_samp
-00013960: 6c65 5b30 203a 206c 656e 2878 665f 7361  le[0 : len(xf_sa
-00013970: 6d70 6c65 2920 2f2f 2032 5d0d 0a20 2020  mple) // 2]..   
-00013980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013990: 2020 2020 2020 2020 2020 2020 2066 6674               fft
-000139a0: 746f 7461 6c5f 7361 6d70 6c65 203d 2066  total_sample = f
-000139b0: 6674 746f 7461 6c5f 7361 6d70 6c65 5b30  fttotal_sample[0
-000139c0: 203a 206c 656e 2866 6674 746f 7461 6c5f   : len(ffttotal_
-000139d0: 7361 6d70 6c65 2920 2f2f 2032 5d0d 0a0d  sample) // 2]...
-000139e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000139f0: 2020 2020 756e 6971 7565 5f66 6674 5f70      unique_fft_p
-00013a00: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00013a10: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
-00013a20: 655f 6964 5d20 3d20 6578 7061 6e64 6564  e_id] = expanded
-00013a30: 5f74 696d 652c 2065 7870 616e 6465 645f  _time, expanded_
-00013a40: 696e 7465 6e73 6974 792c 2078 665f 7361  intensity, xf_sa
-00013a50: 6d70 6c65 2c20 6666 7474 6f74 616c 5f73  mple, ffttotal_s
-00013a60: 616d 706c 650d 0a20 2020 2020 2020 2020  ample..         
-00013a70: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00013a80: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
-00013a90: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
-00013aa0: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
-00013ab0: 3d20 2063 7572 7265 6e74 5f74 696d 650d  =  current_time.
+000138b0: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
+000138c0: 6365 5f63 656c 6c5f 6d61 736b 203d 206e  ce_cell_mask = n
+000138d0: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+000138e0: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
+000138f0: 6d61 736b 2c20 6474 7970 653d 6e70 2e66  mask, dtype=np.f
+00013900: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00013910: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013920: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+00013930: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00013940: 7272 656e 745f 7261 6469 616c 5f61 6e67  rrent_radial_ang
+00013950: 6c65 2c20 6474 7970 653d 6e70 2e66 6c6f  le, dtype=np.flo
+00013960: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00013970: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013980: 745f 6365 6c6c 5f61 7869 735f 6d61 736b  t_cell_axis_mask
+00013990: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+000139a0: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
+000139b0: 6d61 736b 2c20 6474 7970 653d 6e70 2e66  mask, dtype=np.f
+000139c0: 6c6f 6174 3332 290d 0a0d 0a0d 0a20 2020  loat32)......   
+000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000139f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00013a00: 2020 2020 2020 2020 2020 6966 2070 6f69            if poi
+00013a10: 6e74 5f73 616d 706c 6520 3e20 303a 0d0a  nt_sample > 0:..
+00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a40: 7866 5f73 616d 706c 6520 3d20 6666 7466  xf_sample = fftf
+00013a50: 7265 7128 706f 696e 745f 7361 6d70 6c65  req(point_sample
+00013a60: 2c20 7365 6c66 2e74 6361 6c69 6272 6174  , self.tcalibrat
+00013a70: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+00013a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a90: 2020 2020 2020 6666 7473 7472 6970 5f73        fftstrip_s
+00013aa0: 616d 706c 6520 3d20 6666 7428 6578 7061  ample = fft(expa
+00013ab0: 6e64 6564 5f69 6e74 656e 7369 7479 290d  nded_intensity).
 00013ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ad0: 2020 2020 756e 6971 7565 5f73 6861 7065      unique_shape
-00013ae0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013af0: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00013b00: 7175 655f 6964 5d20 3d20 6375 7272 656e  que_id] = curren
-00013b10: 745f 7469 6d65 2c20 6375 7272 656e 745f  t_time, current_
-00013b20: 7a2c 2063 7572 7265 6e74 5f79 2c20 6375  z, current_y, cu
-00013b30: 7272 656e 745f 782c 2063 7572 7265 6e74  rrent_x, current
-00013b40: 5f72 6164 6975 732c 2063 7572 7265 6e74  _radius, current
-00013b50: 5f76 6f6c 756d 652c 2063 7572 7265 6e74  _volume, current
-00013b60: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00013b70: 6d70 5f66 6972 7374 2c20 6375 7272 656e  mp_first, curren
-00013b80: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
-00013b90: 6f6d 705f 7365 636f 6e64 2c20 6375 7272  omp_second, curr
-00013ba0: 656e 745f 7375 7266 6163 655f 6172 6561  ent_surface_area
-00013bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013bc0: 2020 2020 2075 6e69 7175 655f 6479 6e61       unique_dyna
-00013bd0: 6d69 635f 7072 6f70 6572 7469 6573 5f74  mic_properties_t
-00013be0: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
-00013bf0: 756e 6971 7565 5f69 645d 203d 2063 7572  unique_id] = cur
-00013c00: 7265 6e74 5f74 696d 652c 2063 7572 7265  rent_time, curre
-00013c10: 6e74 5f73 7065 6564 2c20 6375 7272 656e  nt_speed, curren
-00013c20: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  t_motion_angle, 
-00013c30: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
-00013c40: 7469 6f6e 2c20 6375 7272 656e 745f 6469  tion, current_di
-00013c50: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00013c60: 2c20 6375 7272 656e 745f 7261 6469 616c  , current_radial
-00013c70: 5f61 6e67 6c65 2c20 6375 7272 656e 745f  _angle, current_
-00013c80: 6365 6c6c 5f61 7869 735f 6d61 736b 0d0a  cell_axis_mask..
-00013c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ca0: 2020 2073 656c 662e 756e 6971 7565 5f66     self.unique_f
-00013cb0: 6674 5f70 726f 7065 7274 6965 735b 7472  ft_properties[tr
-00013cc0: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
-00013cd0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00013ce0: 643a 756e 6971 7565 5f66 6674 5f70 726f  d:unique_fft_pro
-00013cf0: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
-00013d00: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
-00013d10: 6964 5d7d 290d 0a20 2020 2020 2020 2020  id]})..         
-00013d20: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00013d30: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
-00013d40: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-00013d50: 645d 2e75 7064 6174 6528 7b63 7572 7265  d].update({curre
-00013d60: 6e74 5f75 6e69 7175 655f 6964 3a75 6e69  nt_unique_id:uni
-00013d70: 7175 655f 636c 7573 7465 725f 7072 6f70  que_cluster_prop
-00013d80: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
-00013d90: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00013da0: 645d 7d29 0d0a 0d0a 2020 2020 2020 2020  d]})....        
-00013db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013dc0: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
-00013dd0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
-00013de0: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
-00013df0: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
-00013e00: 7565 5f73 6861 7065 5f70 726f 7065 7274  ue_shape_propert
-00013e10: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
-00013e20: 7265 6e74 5f75 6e69 7175 655f 6964 5d7d  rent_unique_id]}
-00013e30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013e40: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00013e50: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
-00013e60: 7469 6573 5b74 7261 636b 5f69 645d 2e75  ties[track_id].u
-00013e70: 7064 6174 6528 7b63 7572 7265 6e74 5f75  pdate({current_u
-00013e80: 6e69 7175 655f 6964 3a75 6e69 7175 655f  nique_id:unique_
-00013e90: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
-00013ea0: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
-00013eb0: 656e 745f 756e 6971 7565 5f69 645d 7d29  ent_unique_id]})
-00013ec0: 0d0a 0d0a 2020 2020 6465 6620 5f73 6563  ....    def _sec
-00013ed0: 6f6e 645f 6368 616e 6e65 6c5f 7370 6f74  ond_channel_spot
-00013ee0: 7328 7365 6c66 2c20 6672 616d 652c 207a  s(self, frame, z
-00013ef0: 2c20 792c 2078 2c20 6365 6c6c 5f69 642c  , y, x, cell_id,
-00013f00: 2074 7261 636b 5f69 6429 3a0d 0a20 2020   track_id):..   
-00013f10: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00013f20: 2020 2020 2020 7472 6565 2c20 6365 6e74        tree, cent
-00013f30: 726f 6964 732c 206c 6162 656c 732c 2076  roids, labels, v
-00013f40: 6f6c 756d 652c 2069 6e74 656e 7369 7479  olume, intensity
-00013f50: 5f6d 6561 6e2c 2069 6e74 656e 7369 7479  _mean, intensity
-00013f60: 5f74 6f74 616c 2c20 626f 756e 6469 6e67  _total, bounding
-00013f70: 5f62 6f78 6573 203d 2073 656c 662e 5f74  _boxes = self._t
-00013f80: 696d 6564 5f63 6861 6e6e 656c 5f73 6567  imed_channel_seg
-00013f90: 5f69 6d61 6765 5b73 7472 2869 6e74 2866  _image[str(int(f
-00013fa0: 6c6f 6174 2866 7261 6d65 2929 295d 0d0a  loat(frame)))]..
-00013fb0: 2020 2020 2020 2020 2020 2020 7069 7865              pixe
-00013fc0: 6c74 6573 746c 6f63 6174 696f 6e20 3d20  ltestlocation = 
-00013fd0: 287a 2c79 2c78 290d 0a20 2020 2020 2020  (z,y,x)..       
-00013fe0: 2020 2020 2064 6973 742c 2069 6e64 6578       dist, index
-00013ff0: 203d 2074 7265 652e 7175 6572 7928 7069   = tree.query(pi
-00014000: 7865 6c74 6573 746c 6f63 6174 696f 6e29  xeltestlocation)
-00014010: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-00014020: 2020 6262 6f78 203d 2062 6f75 6e64 696e    bbox = boundin
-00014030: 675f 626f 7865 735b 696e 6465 785d 0d0a  g_boxes[index]..
-00014040: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00014050: 7a20 3d20 6162 7328 6262 6f78 5b30 5d20  z = abs(bbox[0] 
-00014060: 2d20 6262 6f78 5b33 5d29 0d0a 2020 2020  - bbox[3])..    
-00014070: 2020 2020 2020 2020 7369 7a65 7920 3d20          sizey = 
-00014080: 6162 7328 6262 6f78 5b31 5d20 2d20 6262  abs(bbox[1] - bb
-00014090: 6f78 5b34 5d29 0d0a 2020 2020 2020 2020  ox[4])..        
-000140a0: 2020 2020 7369 7a65 7820 3d20 6162 7328      sizex = abs(
-000140b0: 6262 6f78 5b32 5d20 2d20 6262 6f78 5b35  bbox[2] - bbox[5
-000140c0: 5d29 200d 0a20 2020 2020 2020 2020 2020  ]) ..           
-000140d0: 2076 6574 6f5f 766f 6c75 6d65 203d 2073   veto_volume = s
-000140e0: 697a 6578 202a 2073 697a 6579 202a 2073  izex * sizey * s
-000140f0: 697a 657a 0d0a 2020 2020 2020 2020 2020  izez..          
-00014100: 2020 7665 746f 5f72 6164 6975 7320 3d20    veto_radius = 
-00014110: 6d61 7468 2e70 6f77 2833 202a 2076 6574  math.pow(3 * vet
-00014120: 6f5f 766f 6c75 6d65 202f 2028 3420 2a20  o_volume / (4 * 
-00014130: 6d61 7468 2e70 6929 2c20 312e 3020 2f20  math.pi), 1.0 / 
-00014140: 332e 3029 0d0a 0d0a 2020 2020 2020 2020  3.0)....        
-00014150: 2020 2020 6c6f 6361 7469 6f6e 203d 2028      location = (
-00014160: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
-00014170: 5b30 5d20 2a20 7365 6c66 2e7a 6361 6c69  [0] * self.zcali
-00014180: 6272 6174 696f 6e2c 2063 656e 7472 6f69  bration, centroi
-00014190: 6473 5b69 6e64 6578 5d5b 315d 2a73 656c  ds[index][1]*sel
-000141a0: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
-000141b0: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
-000141c0: 5b32 5d2a 7365 6c66 2e78 6361 6c69 6272  [2]*self.xcalibr
-000141d0: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
-000141e0: 2020 2020 5155 414c 4954 5920 3d20 6d61      QUALITY = ma
-000141f0: 7468 2e70 6f77 2876 6f6c 756d 655b 696e  th.pow(volume[in
-00014200: 6465 785d 2c20 312e 302f 332e 3029 0d0a  dex], 1.0/3.0)..
-00014210: 2020 2020 2020 2020 2020 2020 5241 4449              RADI
-00014220: 5553 203d 206d 6174 682e 706f 7728 766f  US = math.pow(vo
-00014230: 6c75 6d65 5b69 6e64 6578 5d20 2a20 7365  lume[index] * se
-00014240: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
-00014250: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
-00014260: 696f 6e20 2a20 7365 6c66 2e7a 6361 6c69  ion * self.zcali
-00014270: 6272 6174 696f 6e2c 2031 2e30 2f33 2e30  bration, 1.0/3.0
-00014280: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-00014290: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
-000142a0: 6d61 736b 2c20 6d61 736b 6365 6e74 726f  mask, maskcentro
-000142b0: 6964 203d 2073 656c 662e 5f67 6574 5f62  id = self._get_b
-000142c0: 6f75 6e64 6172 795f 6469 7374 2866 7261  oundary_dist(fra
-000142d0: 6d65 2c20 6c6f 6361 7469 6f6e 290d 0a20  me, location).. 
-000142e0: 2020 2020 2020 2020 2020 2069 6620 6469             if di
-000142f0: 7374 203c 3d20 3220 2a20 7665 746f 5f72  st <= 2 * veto_r
-00014300: 6164 6975 733a 0d0a 2020 2020 2020 2020  adius:..        
-00014310: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00014320: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-00014330: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-00014340: 5f69 645d 203d 207b 0d0a 2020 2020 2020  _id] = {..      
-00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014360: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
-00014370: 793a 2069 6e74 2863 656c 6c5f 6964 292c  y: int(cell_id),
-00014380: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00014390: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000143a0: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
-000143b0: 7428 6672 616d 6529 2c0d 0a20 2020 2020  t(frame),..     
-000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143d0: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
-000143e0: 6579 203a 2066 6c6f 6174 2863 656e 7472  ey : float(centr
-000143f0: 6f69 6473 5b69 6e64 6578 5d5b 305d 2a20  oids[index][0]* 
-00014400: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00014410: 6e29 2c0d 0a20 2020 2020 2020 2020 2020  n),..           
-00014420: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00014430: 662e 7970 6f73 6964 5f6b 6579 203a 2066  f.yposid_key : f
-00014440: 6c6f 6174 2863 656e 7472 6f69 6473 5b69  loat(centroids[i
-00014450: 6e64 6578 5d5b 315d 2a20 7365 6c66 2e79  ndex][1]* self.y
-00014460: 6361 6c69 6272 6174 696f 6e29 2c0d 0a20  calibration),.. 
-00014470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014480: 2020 2020 2020 2073 656c 662e 7870 6f73         self.xpos
-00014490: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
-000144a0: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-000144b0: 325d 2a20 7365 6c66 2e78 6361 6c69 6272  2]* self.xcalibr
-000144c0: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
-000144d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144e0: 2073 656c 662e 7472 6163 6b69 645f 6b65   self.trackid_ke
-000144f0: 793a 2069 6e74 2874 7261 636b 5f69 6429  y: int(track_id)
-00014500: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00014510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014520: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-00014530: 6b65 7920 3a20 2866 6c6f 6174 2869 6e74  key : (float(int
-00014540: 656e 7369 7479 5f74 6f74 616c 5b69 6e64  ensity_total[ind
-00014550: 6578 5d29 292c 0d0a 2020 2020 2020 2020  ex])),..        
-00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014570: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-00014580: 6974 795f 6b65 7920 3a20 2866 6c6f 6174  ity_key : (float
-00014590: 2869 6e74 656e 7369 7479 5f6d 6561 6e5b  (intensity_mean[
-000145a0: 696e 6465 785d 2929 2c0d 0a20 2020 2020  index])),..     
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145c0: 2020 2073 656c 662e 7261 6469 7573 5f6b     self.radius_k
-000145d0: 6579 203a 2028 666c 6f61 7428 5241 4449  ey : (float(RADI
-000145e0: 5553 2929 2c0d 0a20 2020 2020 2020 2020  US)),..         
-000145f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014600: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
-00014610: 3a20 2866 6c6f 6174 2851 5541 4c49 5459  : (float(QUALITY
-00014620: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-00014630: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00014640: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
-00014650: 6d61 736b 5f6b 6579 3a20 666c 6f61 7428  mask_key: float(
-00014660: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00014670: 736b 292c 0d0a 2020 2020 2020 2020 2020  sk),..          
-00014680: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014690: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-000146a0: 7a5f 6b65 793a 2066 6c6f 6174 286d 6173  z_key: float(mas
-000146b0: 6b63 656e 7472 6f69 645b 305d 292c 0d0a  kcentroid[0]),..
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-000146e0: 6b63 656e 7472 6f69 645f 795f 6b65 793a  kcentroid_y_key:
-000146f0: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
-00014700: 6f69 645b 315d 292c 0d0a 2020 2020 2020  oid[1]),..      
-00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014720: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
-00014730: 6f69 645f 785f 6b65 793a 2066 6c6f 6174  oid_x_key: float
-00014740: 286d 6173 6b63 656e 7472 6f69 645b 325d  (maskcentroid[2]
-00014750: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-00014760: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-00014770: 2020 2020 2065 6c69 6620 6365 6c6c 5f69       elif cell_i
-00014780: 6420 696e 2073 656c 662e 6564 6765 5f73  d in self.edge_s
-00014790: 6f75 7263 655f 6c6f 6f6b 7570 2e6b 6579  ource_lookup.key
-000147a0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-000147b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-000147e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000147f0: 6965 735b 6365 6c6c 5f69 645d 203d 2073  ies[cell_id] = s
-00014800: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014810: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-00014820: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
-00014830: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-00014840: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-00014850: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-00014860: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
-00014870: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-00014880: 7479 5f6b 6579 3a20 2d31 7d29 0d0a 2020  ty_key: -1})..  
-00014890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148a0: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
-000148b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000148c0: 7274 6965 735b 6365 6c6c 5f69 645d 2e75  rties[cell_id].u
-000148d0: 7064 6174 6528 7b73 656c 662e 6d65 616e  pdate({self.mean
-000148e0: 5f69 6e74 656e 7369 7479 5f6b 6579 3a20  _intensity_key: 
-000148f0: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
-00014900: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00014910: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-00014920: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-00014930: 6c6c 5f69 645d 2e75 7064 6174 6528 7b73  ll_id].update({s
-00014940: 656c 662e 7261 6469 7573 5f6b 6579 3a20  elf.radius_key: 
-00014950: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
-00014960: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00014970: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-00014980: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-00014990: 6c6c 5f69 645d 2e75 7064 6174 6528 7b73  ll_id].update({s
-000149a0: 656c 662e 7175 616c 6974 795f 6b65 793a  elf.quality_key:
-000149b0: 202d 317d 290d 0a0d 0a0d 0a0d 0a20 2020   -1})........   
-000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000149e0: 2020 2020 6465 6620 5f64 6963 745f 7570      def _dict_up
-000149f0: 6461 7465 2873 656c 662c 2075 6e69 7175  date(self, uniqu
-00014a00: 655f 7472 6163 6b6c 6574 5f69 6473 3a20  e_tracklet_ids: 
-00014a10: 4c69 7374 2c20 2063 656c 6c5f 6964 3a20  List,  cell_id: 
-00014a20: 696e 742c 2074 7261 636b 5f69 643a 2069  int, track_id: i
-00014a30: 6e74 2c20 736f 7572 6365 5f69 643a 2069  nt, source_id: i
-00014a40: 6e74 2c20 7461 7267 6574 5f69 643a 2069  nt, target_id: i
-00014a50: 6e74 293a 0d0a 0d0a 200d 0a20 2020 2020  nt):.... ..     
-00014a60: 2020 2067 656e 6572 6174 696f 6e5f 6964     generation_id
-00014a70: 203d 2073 656c 662e 6765 6e65 7261 7469   = self.generati
-00014a80: 6f6e 5f64 6963 745b 6365 6c6c 5f69 645d  on_dict[cell_id]
-00014a90: 0d0a 2020 2020 2020 2020 7472 6163 6b6c  ..        trackl
-00014aa0: 6574 5f69 6420 3d20 7365 6c66 2e74 7261  et_id = self.tra
-00014ab0: 636b 6c65 745f 6469 6374 5b63 656c 6c5f  cklet_dict[cell_
-00014ac0: 6964 5d0d 0a0d 0a20 2020 2020 2020 2075  id]....        u
-00014ad0: 6e69 7175 655f 6964 203d 2073 7472 2874  nique_id = str(t
-00014ae0: 7261 636b 5f69 6429 202b 2020 7374 7228  rack_id) +  str(
-00014af0: 6765 6e65 7261 7469 6f6e 5f69 6429 202b  generation_id) +
-00014b00: 2073 7472 2874 7261 636b 6c65 745f 6964   str(tracklet_id
-00014b10: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00014b20: 2020 2020 2076 6563 5f6d 6173 6b20 3d20       vec_mask = 
-00014b30: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
-00014b40: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014b50: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014b60: 5b73 656c 662e 6d61 736b 6365 6e74 726f  [self.maskcentro
-00014b70: 6964 5f78 5f6b 6579 5d29 2c20 666c 6f61  id_x_key]), floa
-00014b80: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00014b90: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014ba0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00014bb0: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
-00014bc0: 6b65 795d 292c 2066 6c6f 6174 2873 656c  key]), float(sel
-00014bd0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014be0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014bf0: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
-00014c00: 6365 6e74 726f 6964 5f7a 5f6b 6579 5d29  centroid_z_key])
-00014c10: 205d 0d0a 0d0a 2020 2020 2020 2020 7665   ]....        ve
-00014c20: 635f 6365 6c6c 203d 205b 666c 6f61 7428  c_cell = [float(
-00014c30: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014c40: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014c50: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-00014c60: 706f 7369 645f 6b65 795d 2920 2c20 0d0a  posid_key]) , ..
-00014c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c80: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00014c90: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00014ca0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014cb0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00014cc0: 2e79 706f 7369 645f 6b65 795d 292c 200d  .yposid_key]), .
-00014cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ce0: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00014cf0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014d00: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014d10: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00014d20: 662e 7a70 6f73 6964 5f6b 6579 5d29 5d0d  f.zposid_key])].
-00014d30: 0a0d 0a20 2020 2020 2020 2061 6e67 6c65  ...        angle
-00014d40: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
-00014d50: 6528 7665 635f 6d61 736b 2c20 7665 635f  e(vec_mask, vec_
-00014d60: 6365 6c6c 290d 0a0d 0a20 2020 2020 2020  cell)....       
-00014d70: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014d80: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014d90: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014da0: 6528 7b73 656c 662e 7261 6469 616c 5f61  e({self.radial_a
-00014db0: 6e67 6c65 5f6b 6579 203a 2061 6e67 6c65  ngle_key : angle
-00014dc0: 7d29 2020 2020 2020 2020 2020 2020 2020  })              
-00014dd0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00014de0: 2020 756e 6971 7565 5f74 7261 636b 6c65    unique_trackle
-00014df0: 745f 6964 732e 6170 7065 6e64 2873 7472  t_ids.append(str
-00014e00: 2875 6e69 7175 655f 6964 2929 0d0a 2020  (unique_id))..  
-00014e10: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014e20: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014e30: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00014e40: 7570 6461 7465 287b 7365 6c66 2e75 6e69  update({self.uni
-00014e50: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
-00014e60: 756e 6971 7565 5f69 6429 7d29 0d0a 2020  unique_id)})..  
-00014e70: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014e80: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014e90: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00014ea0: 7570 6461 7465 287b 7365 6c66 2e74 7261  update({self.tra
-00014eb0: 636b 6c65 7469 645f 6b65 7920 3a20 7374  ckletid_key : st
-00014ec0: 7228 7472 6163 6b6c 6574 5f69 6429 7d29  r(tracklet_id)})
-00014ed0: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00014ee0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014ef0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014f00: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00014f10: 662e 6765 6e65 7261 7469 6f6e 6964 5f6b  f.generationid_k
-00014f20: 6579 203a 2073 7472 2867 656e 6572 6174  ey : str(generat
-00014f30: 696f 6e5f 6964 297d 2920 0d0a 2020 2020  ion_id)}) ..    
-00014f40: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00014f50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014f60: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00014f70: 6461 7465 287b 7365 6c66 2e74 7261 636b  date({self.track
-00014f80: 6964 5f6b 6579 203a 2073 7472 2874 7261  id_key : str(tra
-00014f90: 636b 5f69 6429 7d29 0d0a 2020 2020 2020  ck_id)})..      
-00014fa0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014fb0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014fc0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014fd0: 7465 287b 7365 6c66 2e6d 6f74 696f 6e5f  te({self.motion_
-00014fe0: 616e 676c 655f 6b65 7920 3a20 302e 307d  angle_key : 0.0}
-00014ff0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00015000: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015010: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015020: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00015030: 662e 7370 6565 645f 6b65 7920 3a20 302e  f.speed_key : 0.
-00015040: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
-00015050: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015060: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015070: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00015080: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00015090: 5f6b 6579 203a 2030 2e30 7d29 0d0a 2020  _key : 0.0})..  
-000150a0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000150b0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000150c0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-000150d0: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-000150e0: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-000150f0: 6972 7374 6b65 7920 3a20 2d31 7d29 0d0a  irstkey : -1})..
-00015100: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00015110: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015120: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015130: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
-00015140: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00015150: 5f73 6563 6f6e 646b 6579 203a 202d 317d  _secondkey : -1}
-00015160: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00015170: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015180: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015190: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000151a0: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
-000151b0: 6579 203a 202d 317d 290d 0a20 2020 2020  ey : -1})..     
-000151c0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000151d0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000151e0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-000151f0: 6174 6528 7b73 656c 662e 6365 6c6c 6178  ate({self.cellax
-00015200: 6973 5f6d 6173 6b5f 6b65 7920 3a20 2d31  is_mask_key : -1
-00015210: 7d29 0d0a 0d0a 2020 2020 2020 2020 6966  })....        if
-00015220: 2073 6f75 7263 655f 6964 2069 7320 6e6f   source_id is no
-00015230: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00015240: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015250: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015260: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015270: 7064 6174 6528 7b73 656c 662e 6265 666f  pdate({self.befo
-00015280: 7265 6964 5f6b 6579 203a 2069 6e74 2873  reid_key : int(s
-00015290: 6f75 7263 655f 6964 297d 290d 0a20 2020  ource_id)})..   
-000152a0: 2020 2020 2020 2020 2076 6563 5f31 203d           vec_1 =
-000152b0: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
-000152c0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000152d0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000152e0: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-000152f0: 795d 2920 2d20 666c 6f61 7428 7365 6c66  y]) - float(self
-00015300: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015310: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
-00015320: 6365 5f69 6429 5d5b 7365 6c66 2e78 706f  ce_id)][self.xpo
-00015330: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
-00015340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015350: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-00015360: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015370: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00015380: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
-00015390: 6f73 6964 5f6b 6579 5d29 202d 2066 6c6f  osid_key]) - flo
-000153a0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-000153b0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000153c0: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-000153d0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-000153e0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-000153f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015400: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015410: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015420: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00015430: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-00015440: 2920 2d20 2066 6c6f 6174 2873 656c 662e  ) -  float(self.
-00015450: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015460: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00015470: 655f 6964 295d 5b73 656c 662e 7a70 6f73  e_id)][self.zpos
-00015480: 6964 5f6b 6579 5d29 5d0d 0a20 2020 2020  id_key])]..     
-00015490: 2020 2020 2020 2073 7065 6564 203d 206e         speed = n
-000154a0: 702e 7371 7274 286e 702e 646f 7428 7665  p.sqrt(np.dot(ve
-000154b0: 635f 312c 2076 6563 5f31 2929 2f73 656c  c_1, vec_1))/sel
-000154c0: 662e 7463 616c 6962 7261 7469 6f6e 0d0a  f.tcalibration..
-000154d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000154e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000154f0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015500: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015510: 6c66 2e73 7065 6564 5f6b 6579 203a 2073  lf.speed_key : s
-00015520: 7065 6564 7d29 0d0a 0d0a 2020 2020 2020  peed})....      
-00015530: 2020 2020 2020 6d6f 7469 6f6e 5f61 6e67        motion_ang
-00015540: 6c65 203d 2061 6e67 756c 6172 5f63 6861  le = angular_cha
-00015550: 6e67 6528 7665 635f 6d61 736b 2c20 7665  nge(vec_mask, ve
-00015560: 635f 3129 0d0a 0d0a 2020 2020 2020 2020  c_1)....        
-00015570: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00015580: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015590: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-000155a0: 6461 7465 287b 7365 6c66 2e6d 6f74 696f  date({self.motio
-000155b0: 6e5f 616e 676c 655f 6b65 7920 3a20 6d6f  n_angle_key : mo
-000155c0: 7469 6f6e 5f61 6e67 6c65 7d29 200d 0a0d  tion_angle}) ...
-000155d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000155e0: 736f 7572 6365 5f69 6420 696e 2073 656c  source_id in sel
-000155f0: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
-00015600: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
-00015610: 2020 2020 2020 2020 2020 2070 7265 5f73             pre_s
-00015620: 6f75 7263 655f 6964 203d 2073 656c 662e  ource_id = self.
-00015630: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
-00015640: 7570 5b73 6f75 7263 655f 6964 5d0d 0a20  up[source_id].. 
-00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015660: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00015670: 2020 2020 2020 2020 2076 6563 5f32 203d           vec_2 =
-00015680: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
-00015690: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000156a0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000156b0: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-000156c0: 795d 2920 2d20 3220 2a20 666c 6f61 7428  y]) - 2 * float(
-000156d0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000156e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000156f0: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00015700: 2e78 706f 7369 645f 6b65 795d 2920 2b20  .xposid_key]) + 
-00015710: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015720: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015730: 735b 696e 7428 7072 655f 736f 7572 6365  s[int(pre_source
-00015740: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
-00015750: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
-00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
-00015780: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015790: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-000157a0: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
-000157b0: 6964 5f6b 6579 5d29 202d 2032 202a 2066  id_key]) - 2 * f
-000157c0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-000157d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000157e0: 5b69 6e74 2873 6f75 7263 655f 6964 295d  [int(source_id)]
-000157f0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-00015800: 5d29 202b 2066 6c6f 6174 2873 656c 662e  ]) + float(self.
-00015810: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015820: 6572 7469 6573 5b69 6e74 2870 7265 5f73  erties[int(pre_s
-00015830: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
-00015840: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
-00015850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015860: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00015870: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00015880: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015890: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-000158a0: 2e7a 706f 7369 645f 6b65 795d 2920 2d20  .zposid_key]) - 
-000158b0: 2032 202a 2066 6c6f 6174 2873 656c 662e   2 * float(self.
-000158c0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000158d0: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-000158e0: 655f 6964 295d 5b73 656c 662e 7a70 6f73  e_id)][self.zpos
-000158f0: 6964 5f6b 6579 5d29 202b 2066 6c6f 6174  id_key]) + float
-00015900: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015910: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015920: 2870 7265 5f73 6f75 7263 655f 6964 295d  (pre_source_id)]
-00015930: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
-00015940: 5d29 5d0d 0a20 2020 2020 2020 2020 2020  ])]..           
-00015950: 2020 2020 2020 2020 2061 6363 203d 206e           acc = n
-00015960: 702e 7371 7274 286e 702e 646f 7428 7665  p.sqrt(np.dot(ve
-00015970: 635f 322c 2076 6563 5f32 2929 2f73 656c  c_2, vec_2))/sel
-00015980: 662e 7463 616c 6962 7261 7469 6f6e 0d0a  f.tcalibration..
-00015990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000159b0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000159c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000159d0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-000159e0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-000159f0: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-00015a00: 7920 3a20 6163 637d 290d 0a20 2020 2020  y : acc})..     
-00015a10: 2020 2065 6c69 6620 736f 7572 6365 5f69     elif source_i
-00015a20: 6420 6973 204e 6f6e 653a 0d0a 2020 2020  d is None:..    
-00015a30: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00015a40: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015a50: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015a60: 5d2e 7570 6461 7465 287b 7365 6c66 2e62  ].update({self.b
-00015a70: 6566 6f72 6569 645f 6b65 7920 3a20 4e6f  eforeid_key : No
-00015a80: 6e65 7d29 200d 0a20 2020 2020 2020 2020  ne}) ..         
-00015a90: 2020 200d 0a0d 0a20 2020 2020 2020 2069     ....        i
-00015aa0: 6620 7461 7267 6574 5f69 6420 6973 206e  f target_id is n
-00015ab0: 6f74 204e 6f6e 653a 2020 2020 2020 200d  ot None:       .
-00015ac0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015ad0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015ae0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015af0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00015b00: 656c 662e 6166 7465 7269 645f 6b65 7920  elf.afterid_key 
-00015b10: 3a20 696e 7428 7461 7267 6574 5f69 6429  : int(target_id)
-00015b20: 7d29 200d 0a20 2020 2020 2020 2065 6c69  }) ..        eli
-00015b30: 6620 7461 7267 6574 5f69 6420 6973 204e  f target_id is N
-00015b40: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00015b50: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00015b60: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015b70: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00015b80: 7465 287b 7365 6c66 2e61 6674 6572 6964  te({self.afterid
-00015b90: 5f6b 6579 203a 204e 6f6e 657d 290d 0a20  _key : None}).. 
-00015ba0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00015bb0: 2020 2020 2073 656c 662e 5f73 6563 6f6e       self._secon
-00015bc0: 645f 6368 616e 6e65 6c5f 7570 6461 7465  d_channel_update
-00015bd0: 2863 656c 6c5f 6964 2c20 7472 6163 6b5f  (cell_id, track_
-00015be0: 6964 2920 2020 200d 0a0d 0a0d 0a20 2020  id)    ......   
-00015bf0: 2064 6566 205f 7465 6d70 6f72 616c 5f70   def _temporal_p
-00015c00: 6c6f 7473 5f74 7261 636b 6d61 7465 2873  lots_trackmate(s
-00015c10: 656c 6629 3a0d 0a20 2020 200d 0a20 2020  elf):..    ..   
-00015c20: 200d 0a20 2020 200d 0a20 2020 2020 2020   ..    ..       
-00015c30: 2020 2020 2020 2020 2073 656c 662e 4174           self.At
-00015c40: 7472 203d 207b 7d0d 0a20 2020 2020 2020  tr = {}..       
-00015c50: 2020 2020 2020 2020 2073 7461 7274 7469           startti
-00015c60: 6d65 203d 2069 6e74 286d 696e 2873 656c  me = int(min(sel
-00015c70: 662e 416c 6c56 616c 7565 735b 7365 6c66  f.AllValues[self
-00015c80: 2e66 7261 6d65 6964 5f6b 6579 5d29 290d  .frameid_key])).
-00015c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ca0: 2065 6e64 7469 6d65 203d 2069 6e74 286d   endtime = int(m
-00015cb0: 6178 2873 656c 662e 416c 6c56 616c 7565  ax(self.AllValue
-00015cc0: 735b 7365 6c66 2e66 7261 6d65 6964 5f6b  s[self.frameid_k
-00015cd0: 6579 5d29 290d 0a20 2020 2020 2020 2020  ey]))..         
-00015ce0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00015cf0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00015d00: 696d 6520 3d20 5b5d 0d0a 2020 2020 2020  ime = []..      
-00015d10: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015d20: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00015d30: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
-00015d40: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015d50: 746f 7469 635f 7661 725f 6469 7370 5f7a  totic_var_disp_z
-00015d60: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015d70: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015d80: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00015d90: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
-00015da0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015db0: 6f74 6963 5f76 6172 5f64 6973 705f 7920  otic_var_disp_y 
-00015dc0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00015dd0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015de0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
-00015df0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015e00: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015e10: 7469 635f 7661 725f 6469 7370 5f78 203d  tic_var_disp_x =
-00015e20: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015e30: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015e40: 7469 635f 6d65 616e 5f72 6164 6975 7320  tic_mean_radius 
-00015e50: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015e60: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00015e70: 6963 5f76 6172 5f72 6164 6975 7320 3d20  ic_var_radius = 
-00015e80: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015e90: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00015ea0: 6963 5f6d 6561 6e5f 7370 6565 6420 3d20  ic_mean_speed = 
-00015eb0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00015ec0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00015ed0: 5f76 6172 5f73 7065 6564 203d 205b 5d0d  _var_speed = [].
-00015ee0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015ef0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00015f00: 6d65 616e 5f61 6363 203d 205b 5d0d 0a20  mean_acc = [].. 
-00015f10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015f20: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00015f30: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
-00015f40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015f50: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-00015f60: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ae0: 2066 6674 746f 7461 6c5f 7361 6d70 6c65   ffttotal_sample
+00013af0: 203d 206e 702e 6162 7328 6666 7473 7472   = np.abs(fftstr
+00013b00: 6970 5f73 616d 706c 6529 0d0a 2020 2020  ip_sample)..    
+00013b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b20: 2020 2020 2020 2020 2020 2020 7866 5f73              xf_s
+00013b30: 616d 706c 6520 3d20 7866 5f73 616d 706c  ample = xf_sampl
+00013b40: 655b 3020 3a20 6c65 6e28 7866 5f73 616d  e[0 : len(xf_sam
+00013b50: 706c 6529 202f 2f20 325d 0d0a 2020 2020  ple) // 2]..    
+00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b70: 2020 2020 2020 2020 2020 2020 6666 7474              fftt
+00013b80: 6f74 616c 5f73 616d 706c 6520 3d20 6666  otal_sample = ff
+00013b90: 7474 6f74 616c 5f73 616d 706c 655b 3020  ttotal_sample[0 
+00013ba0: 3a20 6c65 6e28 6666 7474 6f74 616c 5f73  : len(ffttotal_s
+00013bb0: 616d 706c 6529 202f 2f20 325d 0d0a 0d0a  ample) // 2]....
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 2020 2075 6e69 7175 655f 6666 745f 7072     unique_fft_pr
+00013be0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00013bf0: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00013c00: 5f69 645d 203d 2065 7870 616e 6465 645f  _id] = expanded_
+00013c10: 7469 6d65 2c20 6578 7061 6e64 6564 5f69  time, expanded_i
+00013c20: 6e74 656e 7369 7479 2c20 7866 5f73 616d  ntensity, xf_sam
+00013c30: 706c 652c 2066 6674 746f 7461 6c5f 7361  ple, ffttotal_sa
+00013c40: 6d70 6c65 0d0a 2020 2020 2020 2020 2020  mple..          
+00013c50: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
+00013c60: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
+00013c70: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
+00013c80: 656e 745f 756e 6971 7565 5f69 645d 203d  ent_unique_id] =
+00013c90: 2020 6375 7272 656e 745f 7469 6d65 0d0a    current_time..
+00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cb0: 2020 2075 6e69 7175 655f 7368 6170 655f     unique_shape_
+00013cc0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+00013cd0: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
+00013ce0: 7565 5f69 645d 203d 2063 7572 7265 6e74  ue_id] = current
+00013cf0: 5f74 696d 652c 2063 7572 7265 6e74 5f7a  _time, current_z
+00013d00: 2c20 6375 7272 656e 745f 792c 2063 7572  , current_y, cur
+00013d10: 7265 6e74 5f78 2c20 6375 7272 656e 745f  rent_x, current_
+00013d20: 7261 6469 7573 2c20 6375 7272 656e 745f  radius, current_
+00013d30: 766f 6c75 6d65 2c20 6375 7272 656e 745f  volume, current_
+00013d40: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00013d50: 705f 6669 7273 742c 2063 7572 7265 6e74  p_first, current
+00013d60: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00013d70: 6d70 5f73 6563 6f6e 642c 2063 7572 7265  mp_second, curre
+00013d80: 6e74 5f73 7572 6661 6365 5f61 7265 610d  nt_surface_area.
+00013d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013da0: 2020 2020 756e 6971 7565 5f64 796e 616d      unique_dynam
+00013db0: 6963 5f70 726f 7065 7274 6965 735f 7472  ic_properties_tr
+00013dc0: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
+00013dd0: 6e69 7175 655f 6964 5d20 3d20 6375 7272  nique_id] = curr
+00013de0: 656e 745f 7469 6d65 2c20 6375 7272 656e  ent_time, curren
+00013df0: 745f 7370 6565 642c 2063 7572 7265 6e74  t_speed, current
+00013e00: 5f6d 6f74 696f 6e5f 616e 676c 652c 2063  _motion_angle, c
+00013e10: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
+00013e20: 696f 6e2c 2063 7572 7265 6e74 5f64 6973  ion, current_dis
+00013e30: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
+00013e40: 2063 7572 7265 6e74 5f72 6164 6961 6c5f   current_radial_
+00013e50: 616e 676c 652c 2063 7572 7265 6e74 5f63  angle, current_c
+00013e60: 656c 6c5f 6178 6973 5f6d 6173 6b0d 0a20  ell_axis_mask.. 
+00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e80: 2020 7365 6c66 2e75 6e69 7175 655f 6666    self.unique_ff
+00013e90: 745f 7072 6f70 6572 7469 6573 5b74 7261  t_properties[tra
+00013ea0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
+00013eb0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00013ec0: 3a75 6e69 7175 655f 6666 745f 7072 6f70  :unique_fft_prop
+00013ed0: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
+00013ee0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00013ef0: 645d 7d29 0d0a 2020 2020 2020 2020 2020  d]})..          
+00013f00: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00013f10: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
+00013f20: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00013f30: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
+00013f40: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
+00013f50: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
+00013f60: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
+00013f70: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00013f80: 5d7d 290d 0a0d 0a20 2020 2020 2020 2020  ]})....         
+00013f90: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00013fa0: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
+00013fb0: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
+00013fc0: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
+00013fd0: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
+00013fe0: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
+00013ff0: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
+00014000: 656e 745f 756e 6971 7565 5f69 645d 7d29  ent_unique_id]})
+00014010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014020: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00014030: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
+00014040: 6965 735b 7472 6163 6b5f 6964 5d2e 7570  ies[track_id].up
+00014050: 6461 7465 287b 6375 7272 656e 745f 756e  date({current_un
+00014060: 6971 7565 5f69 643a 756e 6971 7565 5f64  ique_id:unique_d
+00014070: 796e 616d 6963 5f70 726f 7065 7274 6965  ynamic_propertie
+00014080: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+00014090: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
+000140a0: 0a0d 0a20 2020 2064 6566 205f 7365 636f  ...    def _seco
+000140b0: 6e64 5f63 6861 6e6e 656c 5f73 706f 7473  nd_channel_spots
+000140c0: 2873 656c 662c 2066 7261 6d65 2c20 7a2c  (self, frame, z,
+000140d0: 2079 2c20 782c 2063 656c 6c5f 6964 2c20   y, x, cell_id, 
+000140e0: 7472 6163 6b5f 6964 293a 0d0a 2020 2020  track_id):..    
+000140f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00014100: 2020 2020 2074 7265 652c 2063 656e 7472       tree, centr
+00014110: 6f69 6473 2c20 6c61 6265 6c73 2c20 766f  oids, labels, vo
+00014120: 6c75 6d65 2c20 696e 7465 6e73 6974 795f  lume, intensity_
+00014130: 6d65 616e 2c20 696e 7465 6e73 6974 795f  mean, intensity_
+00014140: 746f 7461 6c2c 2062 6f75 6e64 696e 675f  total, bounding_
+00014150: 626f 7865 7320 3d20 7365 6c66 2e5f 7469  boxes = self._ti
+00014160: 6d65 645f 6368 616e 6e65 6c5f 7365 675f  med_channel_seg_
+00014170: 696d 6167 655b 7374 7228 696e 7428 666c  image[str(int(fl
+00014180: 6f61 7428 6672 616d 6529 2929 5d0d 0a20  oat(frame)))].. 
+00014190: 2020 2020 2020 2020 2020 2070 6978 656c             pixel
+000141a0: 7465 7374 6c6f 6361 7469 6f6e 203d 2028  testlocation = (
+000141b0: 7a2c 792c 7829 0d0a 2020 2020 2020 2020  z,y,x)..        
+000141c0: 2020 2020 6469 7374 2c20 696e 6465 7820      dist, index 
+000141d0: 3d20 7472 6565 2e71 7565 7279 2870 6978  = tree.query(pix
+000141e0: 656c 7465 7374 6c6f 6361 7469 6f6e 290d  eltestlocation).
+000141f0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00014200: 2062 626f 7820 3d20 626f 756e 6469 6e67   bbox = bounding
+00014210: 5f62 6f78 6573 5b69 6e64 6578 5d0d 0a20  _boxes[index].. 
+00014220: 2020 2020 2020 2020 2020 2073 697a 657a             sizez
+00014230: 203d 2061 6273 2862 626f 785b 305d 202d   = abs(bbox[0] -
+00014240: 2062 626f 785b 335d 290d 0a20 2020 2020   bbox[3])..     
+00014250: 2020 2020 2020 2073 697a 6579 203d 2061         sizey = a
+00014260: 6273 2862 626f 785b 315d 202d 2062 626f  bs(bbox[1] - bbo
+00014270: 785b 345d 290d 0a20 2020 2020 2020 2020  x[4])..         
+00014280: 2020 2073 697a 6578 203d 2061 6273 2862     sizex = abs(b
+00014290: 626f 785b 325d 202d 2062 626f 785b 355d  box[2] - bbox[5]
+000142a0: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+000142b0: 7665 746f 5f76 6f6c 756d 6520 3d20 7369  veto_volume = si
+000142c0: 7a65 7820 2a20 7369 7a65 7920 2a20 7369  zex * sizey * si
+000142d0: 7a65 7a0d 0a20 2020 2020 2020 2020 2020  zez..           
+000142e0: 2076 6574 6f5f 7261 6469 7573 203d 206d   veto_radius = m
+000142f0: 6174 682e 706f 7728 3320 2a20 7665 746f  ath.pow(3 * veto
+00014300: 5f76 6f6c 756d 6520 2f20 2834 202a 206d  _volume / (4 * m
+00014310: 6174 682e 7069 292c 2031 2e30 202f 2033  ath.pi), 1.0 / 3
+00014320: 2e30 290d 0a0d 0a20 2020 2020 2020 2020  .0)....         
+00014330: 2020 206c 6f63 6174 696f 6e20 3d20 2863     location = (c
+00014340: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
+00014350: 305d 202a 2073 656c 662e 7a63 616c 6962  0] * self.zcalib
+00014360: 7261 7469 6f6e 2c20 6365 6e74 726f 6964  ration, centroid
+00014370: 735b 696e 6465 785d 5b31 5d2a 7365 6c66  s[index][1]*self
+00014380: 2e79 6361 6c69 6272 6174 696f 6e2c 2063  .ycalibration, c
+00014390: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
+000143a0: 325d 2a73 656c 662e 7863 616c 6962 7261  2]*self.xcalibra
+000143b0: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
+000143c0: 2020 2051 5541 4c49 5459 203d 206d 6174     QUALITY = mat
+000143d0: 682e 706f 7728 766f 6c75 6d65 5b69 6e64  h.pow(volume[ind
+000143e0: 6578 5d2c 2031 2e30 2f33 2e30 290d 0a20  ex], 1.0/3.0).. 
+000143f0: 2020 2020 2020 2020 2020 2052 4144 4955             RADIU
+00014400: 5320 3d20 6d61 7468 2e70 6f77 2876 6f6c  S = math.pow(vol
+00014410: 756d 655b 696e 6465 785d 202a 2073 656c  ume[index] * sel
+00014420: 662e 7863 616c 6962 7261 7469 6f6e 202a  f.xcalibration *
+00014430: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
+00014440: 6f6e 202a 2073 656c 662e 7a63 616c 6962  on * self.zcalib
+00014450: 7261 7469 6f6e 2c20 312e 302f 332e 3029  ration, 1.0/3.0)
+00014460: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00014470: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+00014480: 6173 6b2c 206d 6173 6b63 656e 7472 6f69  ask, maskcentroi
+00014490: 6420 3d20 7365 6c66 2e5f 6765 745f 626f  d = self._get_bo
+000144a0: 756e 6461 7279 5f64 6973 7428 6672 616d  undary_dist(fram
+000144b0: 652c 206c 6f63 6174 696f 6e29 0d0a 2020  e, location)..  
+000144c0: 2020 2020 2020 2020 2020 6966 2064 6973            if dis
+000144d0: 7420 3c3d 2032 202a 2076 6574 6f5f 7261  t <= 2 * veto_ra
+000144e0: 6469 7573 3a0d 0a20 2020 2020 2020 2020  dius:..         
+000144f0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+00014500: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+00014510: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+00014520: 6964 5d20 3d20 7b0d 0a20 2020 2020 2020  id] = {..       
+00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014540: 2073 656c 662e 6365 6c6c 6964 5f6b 6579   self.cellid_key
+00014550: 3a20 696e 7428 6365 6c6c 5f69 6429 2c20  : int(cell_id), 
+00014560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014570: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00014580: 7261 6d65 6964 5f6b 6579 203a 2069 6e74  rameid_key : int
+00014590: 2866 7261 6d65 292c 0d0a 2020 2020 2020  (frame),..      
+000145a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145b0: 2020 7365 6c66 2e7a 706f 7369 645f 6b65    self.zposid_ke
+000145c0: 7920 3a20 666c 6f61 7428 6365 6e74 726f  y : float(centro
+000145d0: 6964 735b 696e 6465 785d 5b30 5d2a 2073  ids[index][0]* s
+000145e0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+000145f0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00014600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014610: 2e79 706f 7369 645f 6b65 7920 3a20 666c  .yposid_key : fl
+00014620: 6f61 7428 6365 6e74 726f 6964 735b 696e  oat(centroids[in
+00014630: 6465 785d 5b31 5d2a 2073 656c 662e 7963  dex][1]* self.yc
+00014640: 616c 6962 7261 7469 6f6e 292c 0d0a 2020  alibration),..  
+00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014660: 2020 2020 2020 7365 6c66 2e78 706f 7369        self.xposi
+00014670: 645f 6b65 7920 3a20 666c 6f61 7428 6365  d_key : float(ce
+00014680: 6e74 726f 6964 735b 696e 6465 785d 5b32  ntroids[index][2
+00014690: 5d2a 2073 656c 662e 7863 616c 6962 7261  ]* self.xcalibra
+000146a0: 7469 6f6e 292c 0d0a 2020 2020 2020 2020  tion),..        
+000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146c0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+000146d0: 3a20 696e 7428 7472 6163 6b5f 6964 292c  : int(track_id),
+000146e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000146f0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00014700: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+00014710: 6579 203a 2028 666c 6f61 7428 696e 7465  ey : (float(inte
+00014720: 6e73 6974 795f 746f 7461 6c5b 696e 6465  nsity_total[inde
+00014730: 785d 2929 2c0d 0a20 2020 2020 2020 2020  x])),..         
+00014740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014750: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+00014760: 7479 5f6b 6579 203a 2028 666c 6f61 7428  ty_key : (float(
+00014770: 696e 7465 6e73 6974 795f 6d65 616e 5b69  intensity_mean[i
+00014780: 6e64 6578 5d29 292c 0d0a 2020 2020 2020  ndex])),..      
+00014790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147a0: 2020 7365 6c66 2e72 6164 6975 735f 6b65    self.radius_ke
+000147b0: 7920 3a20 2866 6c6f 6174 2852 4144 4955  y : (float(RADIU
+000147c0: 5329 292c 0d0a 2020 2020 2020 2020 2020  S)),..          
+000147d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000147e0: 6c66 2e71 7561 6c69 7479 5f6b 6579 203a  lf.quality_key :
+000147f0: 2028 666c 6f61 7428 5155 414c 4954 5929   (float(QUALITY)
+00014800: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00014810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014820: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
+00014830: 6173 6b5f 6b65 793a 2066 6c6f 6174 2864  ask_key: float(d
+00014840: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00014850: 6b29 2c0d 0a20 2020 2020 2020 2020 2020  k),..           
+00014860: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014870: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
+00014880: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
+00014890: 6365 6e74 726f 6964 5b30 5d29 2c0d 0a20  centroid[0]),.. 
+000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148b0: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
+000148c0: 6365 6e74 726f 6964 5f79 5f6b 6579 3a20  centroid_y_key: 
+000148d0: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
+000148e0: 6964 5b31 5d29 2c0d 0a20 2020 2020 2020  id[1]),..       
+000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014900: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
+00014910: 6964 5f78 5f6b 6579 3a20 666c 6f61 7428  id_x_key: float(
+00014920: 6d61 736b 6365 6e74 726f 6964 5b32 5d29  maskcentroid[2])
+00014930: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00014940: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+00014950: 2020 2020 656c 6966 2063 656c 6c5f 6964      elif cell_id
+00014960: 2069 6e20 7365 6c66 2e65 6467 655f 736f   in self.edge_so
+00014970: 7572 6365 5f6c 6f6f 6b75 702e 6b65 7973  urce_lookup.keys
+00014980: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00014990: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000149a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000149b0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+000149c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000149d0: 6573 5b63 656c 6c5f 6964 5d20 3d20 7365  es[cell_id] = se
+000149e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000149f0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+00014a00: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
+00014a10: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+00014a20: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+00014a30: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+00014a40: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+00014a50: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+00014a60: 795f 6b65 793a 202d 317d 290d 0a20 2020  y_key: -1})..   
+00014a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a80: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+00014a90: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014aa0: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
+00014ab0: 6461 7465 287b 7365 6c66 2e6d 6561 6e5f  date({self.mean_
+00014ac0: 696e 7465 6e73 6974 795f 6b65 793a 202d  intensity_key: -
+00014ad0: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
+00014ae0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00014af0: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+00014b00: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+00014b10: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
+00014b20: 6c66 2e72 6164 6975 735f 6b65 793a 202d  lf.radius_key: -
+00014b30: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
+00014b40: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00014b50: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+00014b60: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+00014b70: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
+00014b80: 6c66 2e71 7561 6c69 7479 5f6b 6579 3a20  lf.quality_key: 
+00014b90: 2d31 7d29 0d0a 0d0a 0d0a 0d0a 2020 2020  -1})........    
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bb0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00014bc0: 2020 2064 6566 205f 6469 6374 5f75 7064     def _dict_upd
+00014bd0: 6174 6528 7365 6c66 2c20 756e 6971 7565  ate(self, unique
+00014be0: 5f74 7261 636b 6c65 745f 6964 733a 204c  _tracklet_ids: L
+00014bf0: 6973 742c 2020 6365 6c6c 5f69 643a 2069  ist,  cell_id: i
+00014c00: 6e74 2c20 7472 6163 6b5f 6964 3a20 696e  nt, track_id: in
+00014c10: 742c 2073 6f75 7263 655f 6964 3a20 696e  t, source_id: in
+00014c20: 742c 2074 6172 6765 745f 6964 3a20 696e  t, target_id: in
+00014c30: 7429 3a0d 0a0d 0a20 0d0a 2020 2020 2020  t):.... ..      
+00014c40: 2020 6765 6e65 7261 7469 6f6e 5f69 6420    generation_id 
+00014c50: 3d20 7365 6c66 2e67 656e 6572 6174 696f  = self.generatio
+00014c60: 6e5f 6469 6374 5b63 656c 6c5f 6964 5d0d  n_dict[cell_id].
+00014c70: 0a20 2020 2020 2020 2074 7261 636b 6c65  .        trackle
+00014c80: 745f 6964 203d 2073 656c 662e 7472 6163  t_id = self.trac
+00014c90: 6b6c 6574 5f64 6963 745b 6365 6c6c 5f69  klet_dict[cell_i
+00014ca0: 645d 0d0a 0d0a 2020 2020 2020 2020 756e  d]....        un
+00014cb0: 6971 7565 5f69 6420 3d20 7374 7228 7472  ique_id = str(tr
+00014cc0: 6163 6b5f 6964 2920 2b20 2073 7472 2867  ack_id) +  str(g
+00014cd0: 656e 6572 6174 696f 6e5f 6964 2920 2b20  eneration_id) + 
+00014ce0: 7374 7228 7472 6163 6b6c 6574 5f69 6429  str(tracklet_id)
+00014cf0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00014d00: 2020 2020 7665 635f 6d61 736b 203d 205b      vec_mask = [
+00014d10: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014d20: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014d30: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014d40: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00014d50: 645f 785f 6b65 795d 292c 2066 6c6f 6174  d_x_key]), float
+00014d60: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014d70: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014d80: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00014d90: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
+00014da0: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
+00014db0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014dc0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00014dd0: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
+00014de0: 656e 7472 6f69 645f 7a5f 6b65 795d 2920  entroid_z_key]) 
+00014df0: 5d0d 0a0d 0a20 2020 2020 2020 2076 6563  ]....        vec
+00014e00: 5f63 656c 6c20 3d20 5b66 6c6f 6174 2873  _cell = [float(s
+00014e10: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014e20: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014e30: 656c 6c5f 6964 295d 5b73 656c 662e 7870  ell_id)][self.xp
+00014e40: 6f73 6964 5f6b 6579 5d29 202c 200d 0a20  osid_key]) , .. 
+00014e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e60: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00014e70: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014e80: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014e90: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00014ea0: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
+00014eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ec0: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+00014ed0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014ee0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014ef0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00014f00: 2e7a 706f 7369 645f 6b65 795d 295d 0d0a  .zposid_key])]..
+00014f10: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
+00014f20: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
+00014f30: 2876 6563 5f6d 6173 6b2c 2076 6563 5f63  (vec_mask, vec_c
+00014f40: 656c 6c29 0d0a 0d0a 2020 2020 2020 2020  ell)....        
+00014f50: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014f60: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014f70: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00014f80: 287b 7365 6c66 2e72 6164 6961 6c5f 616e  ({self.radial_an
+00014f90: 676c 655f 6b65 7920 3a20 616e 676c 657d  gle_key : angle}
+00014fa0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+00014fb0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00014fc0: 2075 6e69 7175 655f 7472 6163 6b6c 6574   unique_tracklet
+00014fd0: 5f69 6473 2e61 7070 656e 6428 7374 7228  _ids.append(str(
+00014fe0: 756e 6971 7565 5f69 6429 290d 0a20 2020  unique_id))..   
+00014ff0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015000: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015010: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015020: 7064 6174 6528 7b73 656c 662e 756e 6971  pdate({self.uniq
+00015030: 7565 6964 5f6b 6579 203a 2073 7472 2875  ueid_key : str(u
+00015040: 6e69 7175 655f 6964 297d 290d 0a20 2020  nique_id)})..   
+00015050: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015060: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015070: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015080: 7064 6174 6528 7b73 656c 662e 7472 6163  pdate({self.trac
+00015090: 6b6c 6574 6964 5f6b 6579 203a 2073 7472  kletid_key : str
+000150a0: 2874 7261 636b 6c65 745f 6964 297d 2920  (tracklet_id)}) 
+000150b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000150c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000150d0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000150e0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+000150f0: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
+00015100: 7920 3a20 7374 7228 6765 6e65 7261 7469  y : str(generati
+00015110: 6f6e 5f69 6429 7d29 200d 0a20 2020 2020  on_id)}) ..     
+00015120: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00015130: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015140: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00015150: 6174 6528 7b73 656c 662e 7472 6163 6b69  ate({self.tracki
+00015160: 645f 6b65 7920 3a20 7374 7228 7472 6163  d_key : str(trac
+00015170: 6b5f 6964 297d 290d 0a20 2020 2020 2020  k_id)})..       
+00015180: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00015190: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000151a0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+000151b0: 6528 7b73 656c 662e 6d6f 7469 6f6e 5f61  e({self.motion_a
+000151c0: 6e67 6c65 5f6b 6579 203a 2030 2e30 7d29  ngle_key : 0.0})
+000151d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000151e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000151f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015200: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015210: 2e73 7065 6564 5f6b 6579 203a 2030 2e30  .speed_key : 0.0
+00015220: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
+00015230: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015240: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015250: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015260: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+00015270: 6b65 7920 3a20 302e 307d 290d 0a20 2020  key : 0.0})..   
+00015280: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015290: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000152a0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+000152b0: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
+000152c0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+000152d0: 7273 746b 6579 203a 202d 317d 290d 0a20  rstkey : -1}).. 
+000152e0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000152f0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015300: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015310: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
+00015320: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00015330: 7365 636f 6e64 6b65 7920 3a20 2d31 7d29  secondkey : -1})
+00015340: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00015350: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015360: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015370: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015380: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
+00015390: 7920 3a20 2d31 7d29 0d0a 2020 2020 2020  y : -1})..      
+000153a0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+000153b0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000153c0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+000153d0: 7465 287b 7365 6c66 2e63 656c 6c61 7869  te({self.cellaxi
+000153e0: 735f 6d61 736b 5f6b 6579 203a 202d 317d  s_mask_key : -1}
+000153f0: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+00015400: 736f 7572 6365 5f69 6420 6973 206e 6f74  source_id is not
+00015410: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00015420: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015430: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015440: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015450: 6461 7465 287b 7365 6c66 2e62 6566 6f72  date({self.befor
+00015460: 6569 645f 6b65 7920 3a20 696e 7428 736f  eid_key : int(so
+00015470: 7572 6365 5f69 6429 7d29 0d0a 2020 2020  urce_id)})..    
+00015480: 2020 2020 2020 2020 7665 635f 3120 3d20          vec_1 = 
+00015490: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
+000154a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000154b0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+000154c0: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+000154d0: 5d29 202d 2066 6c6f 6174 2873 656c 662e  ]) - float(self.
+000154e0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000154f0: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
+00015500: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
+00015510: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
+00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015530: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
+00015540: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015550: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015560: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
+00015570: 7369 645f 6b65 795d 2920 2d20 666c 6f61  sid_key]) - floa
+00015580: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015590: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000155a0: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
+000155b0: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
+000155c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000155d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000155e0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000155f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015600: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00015610: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00015620: 202d 2020 666c 6f61 7428 7365 6c66 2e75   -  float(self.u
+00015630: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015640: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
+00015650: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
+00015660: 645f 6b65 795d 295d 0d0a 2020 2020 2020  d_key])]..      
+00015670: 2020 2020 2020 7370 6565 6420 3d20 6e70        speed = np
+00015680: 2e73 7172 7428 6e70 2e64 6f74 2876 6563  .sqrt(np.dot(vec
+00015690: 5f31 2c20 7665 635f 3129 292f 7365 6c66  _1, vec_1))/self
+000156a0: 2e74 6361 6c69 6272 6174 696f 6e0d 0a20  .tcalibration.. 
+000156b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000156c0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000156d0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+000156e0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+000156f0: 662e 7370 6565 645f 6b65 7920 3a20 7370  f.speed_key : sp
+00015700: 6565 647d 290d 0a0d 0a20 2020 2020 2020  eed})....       
+00015710: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
+00015720: 6520 3d20 616e 6775 6c61 725f 6368 616e  e = angular_chan
+00015730: 6765 2876 6563 5f6d 6173 6b2c 2076 6563  ge(vec_mask, vec
+00015740: 5f31 290d 0a0d 0a20 2020 2020 2020 2020  _1)....         
+00015750: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00015760: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015770: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00015780: 6174 6528 7b73 656c 662e 6d6f 7469 6f6e  ate({self.motion
+00015790: 5f61 6e67 6c65 5f6b 6579 203a 206d 6f74  _angle_key : mot
+000157a0: 696f 6e5f 616e 676c 657d 2920 0d0a 0d0a  ion_angle}) ....
+000157b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000157c0: 6f75 7263 655f 6964 2069 6e20 7365 6c66  ource_id in self
+000157d0: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
+000157e0: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
+000157f0: 2020 2020 2020 2020 2020 7072 655f 736f            pre_so
+00015800: 7572 6365 5f69 6420 3d20 7365 6c66 2e65  urce_id = self.e
+00015810: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
+00015820: 705b 736f 7572 6365 5f69 645d 0d0a 2020  p[source_id]..  
+00015830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015840: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00015850: 2020 2020 2020 2020 7665 635f 3220 3d20          vec_2 = 
+00015860: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
+00015870: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015880: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015890: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+000158a0: 5d29 202d 2032 202a 2066 6c6f 6174 2873  ]) - 2 * float(s
+000158b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000158c0: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
+000158d0: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+000158e0: 7870 6f73 6964 5f6b 6579 5d29 202b 2066  xposid_key]) + f
+000158f0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00015900: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015910: 5b69 6e74 2870 7265 5f73 6f75 7263 655f  [int(pre_source_
+00015920: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
+00015930: 5f6b 6579 5d29 2c20 0d0a 2020 2020 2020  _key]), ..      
+00015940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015950: 2020 2020 2020 666c 6f61 7428 7365 6c66        float(self
+00015960: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015970: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015980: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
+00015990: 645f 6b65 795d 2920 2d20 3220 2a20 666c  d_key]) - 2 * fl
+000159a0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000159b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000159c0: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
+000159d0: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+000159e0: 2920 2b20 666c 6f61 7428 7365 6c66 2e75  ) + float(self.u
+000159f0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015a00: 7274 6965 735b 696e 7428 7072 655f 736f  rties[int(pre_so
+00015a10: 7572 6365 5f69 6429 5d5b 7365 6c66 2e79  urce_id)][self.y
+00015a20: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
+00015a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a40: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00015a50: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00015a60: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00015a70: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00015a80: 7a70 6f73 6964 5f6b 6579 5d29 202d 2020  zposid_key]) -  
+00015a90: 3220 2a20 666c 6f61 7428 7365 6c66 2e75  2 * float(self.u
+00015aa0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015ab0: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
+00015ac0: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
+00015ad0: 645f 6b65 795d 2920 2b20 666c 6f61 7428  d_key]) + float(
+00015ae0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015af0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015b00: 7072 655f 736f 7572 6365 5f69 6429 5d5b  pre_source_id)][
+00015b10: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00015b20: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
+00015b30: 2020 2020 2020 2020 6163 6320 3d20 6e70          acc = np
+00015b40: 2e73 7172 7428 6e70 2e64 6f74 2876 6563  .sqrt(np.dot(vec
+00015b50: 5f32 2c20 7665 635f 3229 292f 7365 6c66  _2, vec_2))/self
+00015b60: 2e74 6361 6c69 6272 6174 696f 6e0d 0a20  .tcalibration.. 
+00015b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00015b90: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00015ba0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015bb0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015bc0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015bd0: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
+00015be0: 203a 2061 6363 7d29 0d0a 2020 2020 2020   : acc})..      
+00015bf0: 2020 656c 6966 2073 6f75 7263 655f 6964    elif source_id
+00015c00: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00015c10: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00015c20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015c30: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015c40: 2e75 7064 6174 6528 7b73 656c 662e 6265  .update({self.be
+00015c50: 666f 7265 6964 5f6b 6579 203a 204e 6f6e  foreid_key : Non
+00015c60: 657d 2920 0d0a 2020 2020 2020 2020 2020  e}) ..          
+00015c70: 2020 0d0a 0d0a 2020 2020 2020 2020 6966    ....        if
+00015c80: 2074 6172 6765 745f 6964 2069 7320 6e6f   target_id is no
+00015c90: 7420 4e6f 6e65 3a20 2020 2020 2020 0d0a  t None:       ..
+00015ca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015cb0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015cc0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015cd0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015ce0: 6c66 2e61 6674 6572 6964 5f6b 6579 203a  lf.afterid_key :
+00015cf0: 2069 6e74 2874 6172 6765 745f 6964 297d   int(target_id)}
+00015d00: 2920 0d0a 2020 2020 2020 2020 656c 6966  ) ..        elif
+00015d10: 2074 6172 6765 745f 6964 2069 7320 4e6f   target_id is No
+00015d20: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00015d30: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00015d40: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00015d50: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00015d60: 6528 7b73 656c 662e 6166 7465 7269 645f  e({self.afterid_
+00015d70: 6b65 7920 3a20 4e6f 6e65 7d29 0d0a 2020  key : None})..  
+00015d80: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00015d90: 2020 2020 7365 6c66 2e5f 7365 636f 6e64      self._second
+00015da0: 5f63 6861 6e6e 656c 5f75 7064 6174 6528  _channel_update(
+00015db0: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
+00015dc0: 6429 2020 2020 0d0a 0d0a 0d0a 2020 2020  d)    ......    
+00015dd0: 6465 6620 5f74 656d 706f 7261 6c5f 706c  def _temporal_pl
+00015de0: 6f74 735f 7472 6163 6b6d 6174 6528 7365  ots_trackmate(se
+00015df0: 6c66 293a 0d0a 2020 2020 0d0a 2020 2020  lf):..    ..    
+00015e00: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
+00015e10: 2020 2020 2020 2020 7365 6c66 2e41 7474          self.Att
+00015e20: 7220 3d20 7b7d 0d0a 2020 2020 2020 2020  r = {}..        
+00015e30: 2020 2020 2020 2020 7374 6172 7474 696d          starttim
+00015e40: 6520 3d20 696e 7428 6d69 6e28 7365 6c66  e = int(min(self
+00015e50: 2e41 6c6c 5661 6c75 6573 5b73 656c 662e  .AllValues[self.
+00015e60: 6672 616d 6569 645f 6b65 795d 2929 0d0a  frameid_key]))..
+00015e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e80: 656e 6474 696d 6520 3d20 696e 7428 6d61  endtime = int(ma
+00015e90: 7828 7365 6c66 2e41 6c6c 5661 6c75 6573  x(self.AllValues
+00015ea0: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
+00015eb0: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
+00015ec0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00015ed0: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
+00015ee0: 6d65 203d 205b 5d0d 0a20 2020 2020 2020  me = []..       
+00015ef0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015f00: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00015f10: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
+00015f20: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015f30: 6f74 6963 5f76 6172 5f64 6973 705f 7a20  otic_var_disp_z 
+00015f40: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015f50: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015f60: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
 00015f70: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
 00015f80: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015f90: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
-00015fa0: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00015fb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015fc0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00015fd0: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
-00015fe0: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
-00015ff0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016000: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
-00016010: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00016020: 6b20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  k = []....      
-00016030: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016040: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00016050: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
-00016060: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016070: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00016080: 725f 6469 7370 5f7a 203d 205b 5d0d 0a0d  r_disp_z = []...
-00016090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000160a0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-000160b0: 635f 6d65 616e 5f64 6973 705f 7920 3d20  c_mean_disp_y = 
-000160c0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000160d0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-000160e0: 6f74 6963 5f76 6172 5f64 6973 705f 7920  otic_var_disp_y 
-000160f0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00016100: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00016110: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00016120: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
-00016130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016140: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00016150: 6469 7370 5f78 203d 205b 5d0d 0a0d 0a20  disp_x = [].... 
-00016160: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016170: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00016180: 6d65 616e 5f72 6164 6975 7320 3d20 5b5d  mean_radius = []
+00015f90: 7469 635f 7661 725f 6469 7370 5f79 203d  tic_var_disp_y =
+00015fa0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015fb0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015fc0: 7469 635f 6d65 616e 5f64 6973 705f 7820  tic_mean_disp_x 
+00015fd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015fe0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015ff0: 6963 5f76 6172 5f64 6973 705f 7820 3d20  ic_var_disp_x = 
+00016000: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00016010: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00016020: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
+00016030: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016040: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00016050: 635f 7661 725f 7261 6469 7573 203d 205b  c_var_radius = [
+00016060: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00016070: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00016080: 635f 6d65 616e 5f73 7065 6564 203d 205b  c_mean_speed = [
+00016090: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000160a0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+000160b0: 7661 725f 7370 6565 6420 3d20 5b5d 0d0a  var_speed = []..
+000160c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000160d0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+000160e0: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
+000160f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016100: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f61  lf.mitotic_var_a
+00016110: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
+00016120: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016130: 6d69 746f 7469 635f 6d65 616e 5f64 6972  mitotic_mean_dir
+00016140: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+00016150: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016160: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00016170: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
+00016180: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
 00016190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000161a0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000161b0: 6963 5f76 6172 5f72 6164 6975 7320 3d20  ic_var_radius = 
-000161c0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-000161d0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000161e0: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
-000161f0: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
-00016200: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00016210: 5f6d 6974 6f74 6963 5f76 6172 5f73 7065  _mitotic_var_spe
-00016220: 6564 203d 205b 5d0d 0a0d 0a20 2020 2020  ed = []....     
-00016230: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016240: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00016250: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00016260: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016270: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00016280: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
-00016290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000162a0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-000162b0: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
-000162c0: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
-000162d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000162e0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-000162f0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00016300: 6765 203d 205b 5d0d 0a0d 0a20 2020 2020  ge = []....     
-00016310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016320: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00016330: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00016340: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
-00016350: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016360: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00016370: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00016380: 6b20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  k = []....      
-00016390: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000163a0: 6c6c 5f6d 6561 6e5f 6469 7370 5f7a 203d  ll_mean_disp_z =
-000163b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000163c0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-000163d0: 725f 6469 7370 5f7a 203d 205b 5d0d 0a0d  r_disp_z = []...
-000163e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000163f0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00016400: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
-00016410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016420: 2e61 6c6c 5f76 6172 5f64 6973 705f 7920  .all_var_disp_y 
-00016430: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00016440: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00016450: 5f6d 6561 6e5f 6469 7370 5f78 203d 205b  _mean_disp_x = [
-00016460: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016470: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00016480: 6469 7370 5f78 203d 205b 5d0d 0a0d 0a20  disp_x = [].... 
-00016490: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000164a0: 656c 662e 616c 6c5f 6d65 616e 5f72 6164  elf.all_mean_rad
-000164b0: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
-000164c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000164d0: 6c6c 5f76 6172 5f72 6164 6975 7320 3d20  ll_var_radius = 
-000164e0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-000164f0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00016500: 6561 6e5f 7370 6565 6420 3d20 5b5d 0d0a  ean_speed = []..
-00016510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016520: 7365 6c66 2e61 6c6c 5f76 6172 5f73 7065  self.all_var_spe
-00016530: 6564 203d 205b 5d0d 0a0d 0a20 2020 2020  ed = []....     
-00016540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016550: 616c 6c5f 6d65 616e 5f61 6363 203d 205b  all_mean_acc = [
-00016560: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016570: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00016580: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
-00016590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000165a0: 2e61 6c6c 5f6d 6561 6e5f 6469 7265 6374  .all_mean_direct
-000165b0: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
-000165c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000165d0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-000165e0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-000165f0: 6765 203d 205b 5d0d 0a0d 0a20 2020 2020  ge = []....     
-00016600: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016610: 616c 6c5f 6d65 616e 5f64 6973 7461 6e63  all_mean_distanc
-00016620: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
-00016630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016640: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00016650: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00016660: 6b20 3d20 5b5d 0d0a 0d0a 0d0a 2020 2020  k = []......    
-00016670: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00016680: 7370 6f74 735f 7472 6163 6b73 203d 207b  spots_tracks = {
-00016690: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-000166a0: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
-000166b0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000166c0: 5f70 726f 7065 7274 6965 732e 6974 656d  _properties.item
-000166d0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-000166e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000166f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016700: 2020 2020 616c 6c5f 7370 6f74 7320 3d20      all_spots = 
-00016710: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016720: 5f70 726f 7065 7274 6965 735b 6b5d 0d0a  _properties[k]..
-00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016740: 2020 2020 2020 6966 2073 656c 662e 7472        if self.tr
-00016750: 6163 6b69 645f 6b65 7920 696e 2061 6c6c  ackid_key in all
-00016760: 5f73 706f 7473 3a0d 0a20 2020 2020 2020  _spots:..       
-00016770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016780: 2020 2061 6c6c 5f73 706f 7473 5f74 7261     all_spots_tra
-00016790: 636b 735b 6b5d 203d 2061 6c6c 5f73 706f  cks[k] = all_spo
-000167a0: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
-000167b0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-000167c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000167d0: 2020 2020 2020 2020 2020 6675 7475 7265            future
-000167e0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-000167f0: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
-00016800: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-00016810: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
-00016820: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
-00016830: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
-00016840: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
-00016850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016860: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00016870: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00016880: 2069 6e20 7471 646d 2872 616e 6765 2873   in tqdm(range(s
-00016890: 7461 7274 7469 6d65 2c20 656e 6474 696d  tarttime, endtim
-000168a0: 6529 2c20 746f 7461 6c3d 656e 6474 696d  e), total=endtim
-000168b0: 6520 2d20 7374 6172 7474 696d 6529 3a0d  e - starttime):.
-000168c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000168d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168f0: 2066 7574 7572 6573 2e61 7070 656e 6428   futures.append(
-00016900: 6578 6563 7574 6f72 2e73 7562 6d69 7428  executor.submit(
-00016910: 7365 6c66 2e5f 636f 6d70 7574 655f 7465  self._compute_te
-00016920: 6d70 6f72 616c 2c20 692c 2061 6c6c 5f73  mporal, i, all_s
-00016930: 706f 7473 5f74 7261 636b 7329 290d 0a20  pots_tracks)).. 
-00016940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016950: 2020 2020 2020 5b72 2e72 6573 756c 7428        [r.result(
-00016960: 2920 666f 7220 7220 696e 2063 6f6e 6375  ) for r in concu
-00016970: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
-00016980: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
-00016990: 6573 295d 0d0a 0d0a 0d0a 2020 2020 6465  es)]......    de
-000169a0: 6620 5f63 6f6d 7075 7465 5f74 656d 706f  f _compute_tempo
-000169b0: 7261 6c28 7365 6c66 2c20 692c 2061 6c6c  ral(self, i, all
-000169c0: 5f73 706f 7473 5f74 7261 636b 7329 3a20  _spots_tracks): 
-000169d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000169e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000169f0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00016a00: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00016a10: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016a20: 746f 7469 635f 6469 7370 5f79 203d 205b  totic_disp_y = [
-00016a30: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016a40: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00016a50: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
-00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a70: 6d69 746f 7469 635f 7261 6469 7573 203d  mitotic_radius =
-00016a80: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016a90: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016aa0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
-00016ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ac0: 206d 6974 6f74 6963 5f61 6363 203d 205b   mitotic_acc = [
-00016ad0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016ae0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00016af0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00016b00: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-00016b10: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00016b20: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
-00016b30: 6c5f 6d61 736b 203d 205b 5d0d 0a0d 0a20  l_mask = [].... 
-00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b50: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00016b60: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-00016b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b80: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00016b90: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00016ba0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00016bb0: 5f6d 6974 6f74 6963 5f64 6973 705f 7820  _mitotic_disp_x 
-00016bc0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016bd0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00016be0: 746f 7469 635f 7261 6469 7573 203d 205b  totic_radius = [
-00016bf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016c00: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00016c10: 6963 5f73 7065 6564 203d 205b 5d0d 0a20  ic_speed = [].. 
-00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c30: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f61     non_mitotic_a
-00016c40: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-00016c50: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00016c60: 5f6d 6974 6f74 6963 5f64 6972 6563 7469  _mitotic_directi
-00016c70: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00016c80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016c90: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00016ca0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00016cb0: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
-00016cc0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00016cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ce0: 2020 2020 2061 6c6c 5f64 6973 705f 7a20       all_disp_z 
-00016cf0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016d00: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-00016d10: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00016d20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00016d30: 6c6c 5f64 6973 705f 7820 3d20 5b5d 0d0a  ll_disp_x = []..
-00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d50: 2020 2020 616c 6c5f 7261 6469 7573 203d      all_radius =
-00016d60: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016d70: 2020 2020 2020 2020 2061 6c6c 5f73 7065           all_spe
-00016d80: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
-00016d90: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00016da0: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00016db0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00016dc0: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
-00016dd0: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
-00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016df0: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
-00016e00: 6c5f 6d61 736b 203d 205b 5d0d 0a0d 0a0d  l_mask = [].....
-00016e10: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00016e20: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-00016e30: 7629 2069 6e20 616c 6c5f 7370 6f74 735f  v) in all_spots_
-00016e40: 7472 6163 6b73 2e69 7465 6d73 2829 3a0d  tracks.items():.
-00016e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e60: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00016e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e80: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00016e90: 6e74 5f74 696d 6520 3d20 616c 6c5f 7370  nt_time = all_sp
-00016ea0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00016eb0: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d0d  lf.frameid_key].
-00016ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ed0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016ee0: 6f74 6963 203d 2061 6c6c 5f73 706f 7473  otic = all_spots
-00016ef0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00016f00: 6469 7669 6469 6e67 5f6b 6579 5d0d 0a20  dividing_key].. 
-00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00016f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f40: 2020 2020 2020 2020 6966 2069 203d 3d20          if i == 
-00016f50: 696e 7428 6375 7272 656e 745f 7469 6d65  int(current_time
-00016f60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00016f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f80: 2020 2020 2020 6966 206d 6974 6f74 6963        if mitotic
-00016f90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fb0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016fc0: 6963 5f64 6973 705f 7a2e 6170 7065 6e64  ic_disp_z.append
-00016fd0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00016fe0: 735b 6b5d 5b73 656c 662e 7a70 6f73 6964  s[k][self.zposid
-00016ff0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017020: 6d69 746f 7469 635f 6469 7370 5f79 2e61  mitotic_disp_y.a
-00017030: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017040: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e79  tracks[k][self.y
-00017050: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017080: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00017090: 705f 782e 6170 7065 6e64 2861 6c6c 5f73  p_x.append(all_s
-000170a0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-000170b0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
-000170c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170e0: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
-000170f0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017100: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
-00017110: 5d20 3e20 303a 0d0a 2020 2020 2020 2020  ] > 0:..        
-00017120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017140: 2020 206d 6974 6f74 6963 5f72 6164 6975     mitotic_radiu
-00017150: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
-00017160: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017170: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
+000161a0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+000161b0: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
+000161c0: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
+000161d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000161e0: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
+000161f0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00016200: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016210: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00016220: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+00016230: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
+00016240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016250: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00016260: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
+00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016280: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00016290: 5f6d 6561 6e5f 6469 7370 5f79 203d 205b  _mean_disp_y = [
+000162a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000162b0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+000162c0: 7469 635f 7661 725f 6469 7370 5f79 203d  tic_var_disp_y =
+000162d0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+000162e0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+000162f0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00016300: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00016310: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016320: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+00016330: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
+00016340: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016350: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00016360: 6561 6e5f 7261 6469 7573 203d 205b 5d0d  ean_radius = [].
+00016370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016380: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00016390: 635f 7661 725f 7261 6469 7573 203d 205b  c_var_radius = [
+000163a0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000163b0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+000163c0: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
+000163d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000163e0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+000163f0: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
+00016400: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
+00016410: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016420: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00016430: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
+00016440: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016450: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f61  on_mitotic_var_a
+00016460: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
+00016470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016480: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00016490: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000164a0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+000164b0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000164c0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+000164d0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+000164e0: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
+000164f0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016500: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00016510: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00016520: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
+00016530: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00016540: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00016550: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00016560: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016570: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00016580: 6c5f 6d65 616e 5f64 6973 705f 7a20 3d20  l_mean_disp_z = 
+00016590: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000165a0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+000165b0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
+000165c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165d0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
+000165e0: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
+000165f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016600: 616c 6c5f 7661 725f 6469 7370 5f79 203d  all_var_disp_y =
+00016610: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00016620: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00016630: 6d65 616e 5f64 6973 705f 7820 3d20 5b5d  mean_disp_x = []
+00016640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016650: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
+00016660: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
+00016670: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016680: 6c66 2e61 6c6c 5f6d 6561 6e5f 7261 6469  lf.all_mean_radi
+00016690: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+000166a0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000166b0: 6c5f 7661 725f 7261 6469 7573 203d 205b  l_var_radius = [
+000166c0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000166d0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+000166e0: 616e 5f73 7065 6564 203d 205b 5d0d 0a20  an_speed = [].. 
+000166f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016700: 656c 662e 616c 6c5f 7661 725f 7370 6565  elf.all_var_spee
+00016710: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
+00016720: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00016730: 6c6c 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ll_mean_acc = []
+00016740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016750: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f61    self.all_var_a
+00016760: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
+00016770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016780: 616c 6c5f 6d65 616e 5f64 6972 6563 7469  all_mean_directi
+00016790: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+000167a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000167b0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
+000167c0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+000167d0: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
+000167e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000167f0: 6c6c 5f6d 6561 6e5f 6469 7374 616e 6365  ll_mean_distance
+00016800: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00016810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016820: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00016830: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00016840: 203d 205b 5d0d 0a0d 0a0d 0a20 2020 2020   = []......     
+00016850: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
+00016860: 706f 7473 5f74 7261 636b 7320 3d20 7b7d  pots_tracks = {}
+00016870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016880: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+00016890: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000168a0: 7072 6f70 6572 7469 6573 2e69 7465 6d73  properties.items
+000168b0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+000168c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168e0: 2020 2061 6c6c 5f73 706f 7473 203d 2073     all_spots = s
+000168f0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00016900: 7072 6f70 6572 7469 6573 5b6b 5d0d 0a20  properties[k].. 
+00016910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016920: 2020 2020 2069 6620 7365 6c66 2e74 7261       if self.tra
+00016930: 636b 6964 5f6b 6579 2069 6e20 616c 6c5f  ckid_key in all_
+00016940: 7370 6f74 733a 0d0a 2020 2020 2020 2020  spots:..        
+00016950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016960: 2020 616c 6c5f 7370 6f74 735f 7472 6163    all_spots_trac
+00016970: 6b73 5b6b 5d20 3d20 616c 6c5f 7370 6f74  ks[k] = all_spot
+00016980: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00016990: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+000169a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000169b0: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+000169c0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000169d0: 2020 2020 2020 2077 6974 6820 636f 6e63         with conc
+000169e0: 7572 7265 6e74 2e66 7574 7572 6573 2e54  urrent.futures.T
+000169f0: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+00016a00: 7228 6d61 785f 776f 726b 6572 7320 3d20  r(max_workers = 
+00016a10: 6f73 2e63 7075 5f63 6f75 6e74 2829 2920  os.cpu_count()) 
+00016a20: 6173 2065 7865 6375 746f 723a 0d0a 2020  as executor:..  
+00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00016a50: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00016a60: 696e 2074 7164 6d28 7261 6e67 6528 7374  in tqdm(range(st
+00016a70: 6172 7474 696d 652c 2065 6e64 7469 6d65  arttime, endtime
+00016a80: 292c 2074 6f74 616c 3d65 6e64 7469 6d65  ), total=endtime
+00016a90: 202d 2073 7461 7274 7469 6d65 293a 0d0a   - starttime):..
+00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ab0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00016ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ad0: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
+00016ae0: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
+00016af0: 656c 662e 5f63 6f6d 7075 7465 5f74 656d  elf._compute_tem
+00016b00: 706f 7261 6c2c 2069 2c20 616c 6c5f 7370  poral, i, all_sp
+00016b10: 6f74 735f 7472 6163 6b73 2929 0d0a 200d  ots_tracks)).. .
+00016b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016b30: 2020 2020 205b 722e 7265 7375 6c74 2829       [r.result()
+00016b40: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
+00016b50: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
+00016b60: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
+00016b70: 7329 5d0d 0a0d 0a0d 0a20 2020 2064 6566  s)]......    def
+00016b80: 205f 636f 6d70 7574 655f 7465 6d70 6f72   _compute_tempor
+00016b90: 616c 2873 656c 662c 2069 2c20 616c 6c5f  al(self, i, all_
+00016ba0: 7370 6f74 735f 7472 6163 6b73 293a 2020  spots_tracks):  
+00016bb0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00016bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bd0: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00016be0: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+00016bf0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016c00: 6f74 6963 5f64 6973 705f 7920 3d20 5b5d  otic_disp_y = []
+00016c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016c20: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016c30: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
+00016c40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016c50: 6974 6f74 6963 5f72 6164 6975 7320 3d20  itotic_radius = 
+00016c60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016c70: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016c80: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00016c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ca0: 6d69 746f 7469 635f 6163 6320 3d20 5b5d  mitotic_acc = []
+00016cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016cc0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016cd0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00016ce0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016cf0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016d00: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+00016d10: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 2020  _mask = []....  
+00016d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d30: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00016d40: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+00016d50: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016d60: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00016d70: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00016d80: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016d90: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
+00016da0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016db0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016dc0: 6f74 6963 5f72 6164 6975 7320 3d20 5b5d  otic_radius = []
+00016dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016de0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00016df0: 635f 7370 6565 6420 3d20 5b5d 0d0a 2020  c_speed = []..  
+00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e10: 2020 6e6f 6e5f 6d69 746f 7469 635f 6163    non_mitotic_ac
+00016e20: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
+00016e30: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016e40: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+00016e50: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
+00016e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016e70: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00016e80: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00016e90: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
+00016ea0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00016eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ec0: 2020 2020 616c 6c5f 6469 7370 5f7a 203d      all_disp_z =
+00016ed0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016ee0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+00016ef0: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
+00016f00: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00016f10: 6c5f 6469 7370 5f78 203d 205b 5d0d 0a20  l_disp_x = [].. 
+00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f30: 2020 2061 6c6c 5f72 6164 6975 7320 3d20     all_radius = 
+00016f40: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016f50: 2020 2020 2020 2020 616c 6c5f 7370 6565          all_spee
+00016f60: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
+00016f70: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00016f80: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
+00016f90: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00016fa0: 6c5f 6469 7265 6374 696f 6e61 6c5f 6368  l_directional_ch
+00016fb0: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
+00016fc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00016fd0: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+00016fe0: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 0d0a  _mask = []......
+00016ff0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00017000: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+00017010: 2920 696e 2061 6c6c 5f73 706f 7473 5f74  ) in all_spots_t
+00017020: 7261 636b 732e 6974 656d 7328 293a 0d0a  racks.items():..
+00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017040: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00017050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017060: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00017070: 745f 7469 6d65 203d 2061 6c6c 5f73 706f  t_time = all_spo
+00017080: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017090: 662e 6672 616d 6569 645f 6b65 795d 0d0a  f.frameid_key]..
+000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170b0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+000170c0: 7469 6320 3d20 616c 6c5f 7370 6f74 735f  tic = all_spots_
+000170d0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e64  tracks[k][self.d
+000170e0: 6976 6964 696e 675f 6b65 795d 0d0a 2020  ividing_key]..  
+000170f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017100: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017120: 2020 2020 2020 2069 6620 6920 3d3d 2069         if i == i
+00017130: 6e74 2863 7572 7265 6e74 5f74 696d 6529  nt(current_time)
+00017140: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017160: 2020 2020 2069 6620 6d69 746f 7469 633a       if mitotic:
+00017170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00017180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171a0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171d0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-000171e0: 635f 7261 6469 7573 2e61 7070 656e 6428  c_radius.append(
-000171f0: 4e6f 6e65 2920 2020 2020 2020 0d0a 2020  None)       ..  
-00017200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017220: 2020 2020 2020 6d69 746f 7469 635f 7370        mitotic_sp
-00017230: 6565 642e 6170 7065 6e64 2861 6c6c 5f73  eed.append(all_s
-00017240: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017250: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
-00017260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017280: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017290: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
-000172a0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-000172b0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-000172c0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
-000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172f0: 206d 6974 6f74 6963 5f64 6972 6563 7469   mitotic_directi
-00017300: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00017310: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017320: 636b 735b 6b5d 5b73 656c 662e 6d6f 7469  cks[k][self.moti
-00017330: 6f6e 5f61 6e67 6c65 5f6b 6579 5d29 0d0a  on_angle_key])..
-00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017360: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00017370: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017380: 736b 2e61 7070 656e 6428 616c 6c5f 7370  sk.append(all_sp
-00017390: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-000173a0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-000173b0: 5f6d 6173 6b5f 6b65 795d 290d 0a0d 0a0d  _mask_key]).....
-000173c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173e0: 2020 2069 6620 6e6f 7420 6d69 746f 7469     if not mitoti
-000173f0: 633a 0d0a 2020 2020 2020 2020 2020 2020  c:..            
-00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017410: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00017420: 6d69 746f 7469 635f 6469 7370 5f7a 2e61  mitotic_disp_z.a
-00017430: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017440: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e7a  tracks[k][self.z
-00017450: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017480: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00017490: 5f64 6973 705f 792e 6170 7065 6e64 2861  _disp_y.append(a
-000174a0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000174b0: 6b5d 5b73 656c 662e 7970 6f73 6964 5f6b  k][self.yposid_k
-000174c0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-000174f0: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
-00017500: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017510: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017520: 2e78 706f 7369 645f 6b65 795d 290d 0a20  .xposid_key]).. 
+00017190: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000171a0: 635f 6469 7370 5f7a 2e61 7070 656e 6428  c_disp_z.append(
+000171b0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000171c0: 5b6b 5d5b 7365 6c66 2e7a 706f 7369 645f  [k][self.zposid_
+000171d0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171f0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017200: 6974 6f74 6963 5f64 6973 705f 792e 6170  itotic_disp_y.ap
+00017210: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017220: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
+00017230: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017260: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00017270: 5f78 2e61 7070 656e 6428 616c 6c5f 7370  _x.append(all_sp
+00017280: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017290: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
+000172a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172c0: 2020 2020 2020 2020 2069 6620 616c 6c5f           if all_
+000172d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000172e0: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+000172f0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017320: 2020 6d69 746f 7469 635f 7261 6469 7573    mitotic_radius
+00017330: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00017340: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00017350: 2e72 6164 6975 735f 6b65 795d 290d 0a20  .radius_key]).. 
+00017360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017380: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00017390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173b0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+000173c0: 5f72 6164 6975 732e 6170 7065 6e64 284e  _radius.append(N
+000173d0: 6f6e 6529 2020 2020 2020 200d 0a20 2020  one)       ..   
+000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017400: 2020 2020 206d 6974 6f74 6963 5f73 7065       mitotic_spe
+00017410: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
+00017420: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017430: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
+00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017460: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00017470: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
+00017480: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017490: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+000174a0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174d0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+000174e0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+000174f0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017500: 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74 696f  ks[k][self.motio
+00017510: 6e5f 616e 676c 655f 6b65 795d 290d 0a20  n_angle_key]).. 
+00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017550: 2020 2020 2020 2069 6620 616c 6c5f 7370         if all_sp
-00017560: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017570: 6c66 2e72 6164 6975 735f 6b65 795d 203e  lf.radius_key] >
-00017580: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00017590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017540: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00017550: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00017560: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
+00017570: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017580: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+00017590: 6d61 736b 5f6b 6579 5d29 0d0a 0d0a 0d0a  mask_key])......
 000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175b0: 206e 6f6e 5f6d 6974 6f74 6963 5f72 6164   non_mitotic_rad
-000175c0: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
-000175d0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-000175e0: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
-000175f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017610: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00017620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017640: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017650: 5f6d 6974 6f74 6963 5f72 6164 6975 732e  _mitotic_radius.
-00017660: 6170 7065 6e64 284e 6f6e 6529 2020 2020  append(None)    
-00017670: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176a0: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-000176b0: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
-000176c0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-000176d0: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
-000176e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017700: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00017710: 6963 5f61 6363 2e61 7070 656e 6428 616c  ic_acc.append(al
-00017720: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017730: 5d5b 7365 6c66 2e61 6363 656c 6572 6174  ][self.accelerat
-00017740: 696f 6e5f 6b65 795d 290d 0a20 2020 2020  ion_key])..     
-00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017770: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00017780: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00017790: 652e 6170 7065 6e64 2861 6c6c 5f73 706f  e.append(all_spo
-000177a0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-000177b0: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
-000177c0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-000177d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177e0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-000177f0: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-00017800: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-00017810: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017820: 6163 6b73 5b6b 5d5b 7365 6c66 2e64 6973  acks[k][self.dis
-00017830: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-00017840: 6b65 795d 290d 0a0d 0a20 2020 2020 2020  key])....       
-00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017860: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017870: 6973 705f 7a2e 6170 7065 6e64 2861 6c6c  isp_z.append(all
-00017880: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017890: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
-000178a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000178b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178c0: 2020 2020 2020 616c 6c5f 6469 7370 5f79        all_disp_y
-000178d0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-000178e0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-000178f0: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
-00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017920: 2061 6c6c 5f64 6973 705f 782e 6170 7065   all_disp_x.appe
-00017930: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017940: 636b 735b 6b5d 5b73 656c 662e 7870 6f73  cks[k][self.xpos
-00017950: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017970: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00017980: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017990: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
-000179a0: 6579 5d20 3e20 303a 0d0a 2020 2020 2020  ey] > 0:..      
+000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175c0: 2020 6966 206e 6f74 206d 6974 6f74 6963    if not mitotic
+000175d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175f0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00017600: 6974 6f74 6963 5f64 6973 705f 7a2e 6170  itotic_disp_z.ap
+00017610: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017620: 7261 636b 735b 6b5d 5b73 656c 662e 7a70  racks[k][self.zp
+00017630: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017660: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017670: 6469 7370 5f79 2e61 7070 656e 6428 616c  disp_y.append(al
+00017680: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017690: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+000176a0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176c0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+000176d0: 5f6d 6974 6f74 6963 5f64 6973 705f 782e  _mitotic_disp_x.
+000176e0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+000176f0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017700: 7870 6f73 6964 5f6b 6579 5d29 0d0a 2020  xposid_key])..  
+00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017730: 2020 2020 2020 6966 2061 6c6c 5f73 706f        if all_spo
+00017740: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017750: 662e 7261 6469 7573 5f6b 6579 5d20 3e20  f.radius_key] > 
+00017760: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00017770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017790: 6e6f 6e5f 6d69 746f 7469 635f 7261 6469  non_mitotic_radi
+000177a0: 7573 2e61 7070 656e 6428 616c 6c5f 7370  us.append(all_sp
+000177b0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000177c0: 6c66 2e72 6164 6975 735f 6b65 795d 290d  lf.radius_key]).
+000177d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177f0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017820: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017830: 6d69 746f 7469 635f 7261 6469 7573 2e61  mitotic_radius.a
+00017840: 7070 656e 6428 4e6f 6e65 2920 2020 2020  ppend(None)     
+00017850: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017870: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00017880: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
+00017890: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+000178a0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000178b0: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
+000178c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178e0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+000178f0: 635f 6163 632e 6170 7065 6e64 2861 6c6c  c_acc.append(all
+00017900: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017910: 5b73 656c 662e 6163 6365 6c65 7261 7469  [self.accelerati
+00017920: 6f6e 5f6b 6579 5d29 0d0a 2020 2020 2020  on_key])..      
+00017930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017950: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00017960: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00017970: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00017980: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00017990: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
+000179a0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
 000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179d0: 616c 6c5f 7261 6469 7573 2e61 7070 656e  all_radius.appen
-000179e0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000179f0: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
-00017a00: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
-00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00017a30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a50: 2020 2020 2020 2020 616c 6c5f 7261 6469          all_radi
-00017a60: 7573 2e61 7070 656e 6428 4e6f 6e65 2920  us.append(None) 
-00017a70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a90: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
-00017aa0: 6565 642e 6170 7065 6e64 2861 6c6c 5f73  eed.append(all_s
-00017ab0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017ac0: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
-00017ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000179c0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+000179d0: 5f6d 6974 6f74 6963 5f64 6973 7461 6e63  _mitotic_distanc
+000179e0: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+000179f0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017a00: 636b 735b 6b5d 5b73 656c 662e 6469 7374  cks[k][self.dist
+00017a10: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+00017a20: 6579 5d29 0d0a 0d0a 2020 2020 2020 2020  ey])....        
+00017a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a40: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00017a50: 7370 5f7a 2e61 7070 656e 6428 616c 6c5f  sp_z.append(all_
+00017a60: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017a70: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00017a80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017aa0: 2020 2020 2061 6c6c 5f64 6973 705f 792e       all_disp_y.
+00017ab0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017ac0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017ad0: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
 00017ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017af0: 2020 2061 6c6c 5f61 6363 2e61 7070 656e     all_acc.appen
-00017b00: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00017b10: 6b73 5b6b 5d5b 7365 6c66 2e61 6363 656c  ks[k][self.accel
-00017b20: 6572 6174 696f 6e5f 6b65 795d 290d 0a20  eration_key]).. 
-00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b00: 616c 6c5f 6469 7370 5f78 2e61 7070 656e  all_disp_x.appen
+00017b10: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017b20: 6b73 5b6b 5d5b 7365 6c66 2e78 706f 7369  ks[k][self.xposi
+00017b30: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
 00017b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b50: 2061 6c6c 5f64 6972 6563 7469 6f6e 616c   all_directional
-00017b60: 5f63 6861 6e67 652e 6170 7065 6e64 2861  _change.append(a
-00017b70: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017b80: 6b5d 5b73 656c 662e 6d6f 7469 6f6e 5f61  k][self.motion_a
-00017b90: 6e67 6c65 5f6b 6579 5d29 2020 200d 0a20  ngle_key])   .. 
-00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bc0: 2061 6c6c 5f64 6973 7461 6e63 655f 6365   all_distance_ce
-00017bd0: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 2861  ll_mask.append(a
-00017be0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017bf0: 6b5d 5b73 656c 662e 6469 7374 616e 6365  k][self.distance
-00017c00: 5f63 656c 6c5f 6d61 736b 5f6b 6579 5d29  _cell_mask_key])
-00017c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017b50: 2020 2020 2020 2020 2020 2069 6620 616c             if al
+00017b60: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017b70: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
+00017b80: 795d 203e 2030 3a0d 0a20 2020 2020 2020  y] > 0:..       
+00017b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ba0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017bb0: 6c6c 5f72 6164 6975 732e 6170 7065 6e64  ll_radius.append
+00017bc0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017bd0: 735b 6b5d 5b73 656c 662e 7261 6469 7573  s[k][self.radius
+00017be0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00017c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017c50: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00017c60: 6469 7370 5f7a 203d 206e 702e 6162 7328  disp_z = np.abs(
-00017c70: 6e70 2e64 6966 6628 6d69 746f 7469 635f  np.diff(mitotic_
-00017c80: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00017c90: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00017ca0: 746f 7469 635f 6469 7370 5f79 203d 206e  totic_disp_y = n
-00017cb0: 702e 6162 7328 6e70 2e64 6966 6628 6d69  p.abs(np.diff(mi
-00017cc0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
-00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ce0: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
-00017cf0: 5f78 203d 206e 702e 6162 7328 6e70 2e64  _x = np.abs(np.d
-00017d00: 6966 6628 6d69 746f 7469 635f 6469 7370  iff(mitotic_disp
-00017d10: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00017d20: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00017d30: 6d69 746f 7469 635f 6469 7370 5f7a 203d  mitotic_disp_z =
-00017d40: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-00017d50: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00017d60: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
-00017d70: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00017d80: 746f 7469 635f 6469 7370 5f79 203d 206e  totic_disp_y = n
-00017d90: 702e 6162 7328 6e70 2e64 6966 6628 6e6f  p.abs(np.diff(no
-00017da0: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-00017db0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00017dc0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00017dd0: 7469 635f 6469 7370 5f78 203d 206e 702e  tic_disp_x = np.
-00017de0: 6162 7328 6e70 2e64 6966 6628 6e6f 6e5f  abs(np.diff(non_
-00017df0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
-00017e00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017e10: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
-00017e20: 5f7a 203d 206e 702e 6162 7328 6e70 2e64  _z = np.abs(np.d
-00017e30: 6966 6628 616c 6c5f 6469 7370 5f7a 2929  iff(all_disp_z))
-00017e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017e50: 2020 2020 2020 616c 6c5f 6469 7370 5f79        all_disp_y
-00017e60: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-00017e70: 6628 616c 6c5f 6469 7370 5f79 2929 0d0a  f(all_disp_y))..
-00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e90: 2020 2020 616c 6c5f 6469 7370 5f78 203d      all_disp_x =
-00017ea0: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-00017eb0: 616c 6c5f 6469 7370 5f78 2929 0d0a 0d0a  all_disp_x))....
-00017ec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ee0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f00: 7365 6c66 2e74 696d 652e 6170 7065 6e64  self.time.append
-00017f10: 2869 202a 2073 656c 662e 7463 616c 6962  (i * self.tcalib
-00017f20: 7261 7469 6f6e 290d 0a0d 0a0d 0a20 2020  ration)......   
-00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f40: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00017f50: 616e 5f64 6973 705f 7a2e 6170 7065 6e64  an_disp_z.append
-00017f60: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-00017f70: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
-00017f80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017f90: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00017fa0: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00017fb0: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
-00017fc0: 705f 7a29 290d 0a0d 0a20 2020 2020 2020  p_z))....       
-00017fd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017fe0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00017ff0: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-00018000: 6d65 616e 286d 6974 6f74 6963 5f64 6973  mean(mitotic_dis
-00018010: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00018020: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018030: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-00018040: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
-00018050: 286d 6974 6f74 6963 5f64 6973 705f 7929  (mitotic_disp_y)
-00018060: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018070: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00018080: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00018090: 782e 6170 7065 6e64 286e 702e 6d65 616e  x.append(np.mean
-000180a0: 286d 6974 6f74 6963 5f64 6973 705f 7829  (mitotic_disp_x)
-000180b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000180c0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-000180d0: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
-000180e0: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-000180f0: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
-00018100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018110: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018120: 635f 6d65 616e 5f72 6164 6975 732e 6170  c_mean_radius.ap
-00018130: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00018140: 6f74 6963 5f72 6164 6975 7329 290d 0a20  otic_radius)).. 
-00018150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018160: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018170: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
-00018180: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018190: 5f72 6164 6975 7329 290d 0a20 2020 2020  _radius))..     
-000181a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000181b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000181c0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000181d0: 635f 6d65 616e 5f73 7065 6564 2e61 7070  c_mean_speed.app
-000181e0: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-000181f0: 7469 635f 7370 6565 6429 290d 0a20 2020  tic_speed))..   
-00018200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018210: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00018220: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
-00018230: 702e 7374 6428 6d69 746f 7469 635f 7370  p.std(mitotic_sp
-00018240: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-00018250: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018260: 662e 6d69 746f 7469 635f 6d65 616e 5f61  f.mitotic_mean_a
-00018270: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
-00018280: 6e28 6d69 746f 7469 635f 6163 6329 290d  n(mitotic_acc)).
-00018290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000182a0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000182b0: 635f 7661 725f 6163 632e 6170 7065 6e64  c_var_acc.append
-000182c0: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-000182d0: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
-000182e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000182f0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00018300: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00018310: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
-00018320: 286d 6974 6f74 6963 5f64 6972 6563 7469  (mitotic_directi
-00018330: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
-00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018350: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018360: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
-00018370: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00018380: 2e73 7464 286d 6974 6f74 6963 5f64 6972  .std(mitotic_dir
-00018390: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-000183a0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000183b0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000183c0: 746f 7469 635f 6d65 616e 5f64 6973 7461  totic_mean_dista
-000183d0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-000183e0: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-000183f0: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
-00018400: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-00018410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018420: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00018430: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018440: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
-00018450: 286d 6974 6f74 6963 5f64 6973 7461 6e63  (mitotic_distanc
-00018460: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a0d  e_cell_mask))...
-00018470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018480: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00018490: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-000184a0: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
-000184b0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-000184c0: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-000184d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000184e0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-000184f0: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00018500: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-00018510: 5f64 6973 705f 7a29 290d 0a0d 0a20 2020  _disp_z))....   
+00017c30: 2020 2020 2020 2061 6c6c 5f72 6164 6975         all_radiu
+00017c40: 732e 6170 7065 6e64 284e 6f6e 6529 2020  s.append(None)  
+00017c50: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c70: 2020 2020 2020 2020 2061 6c6c 5f73 7065           all_spe
+00017c80: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
+00017c90: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017ca0: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
+00017cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cd0: 2020 616c 6c5f 6163 632e 6170 7065 6e64    all_acc.append
+00017ce0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017cf0: 735b 6b5d 5b73 656c 662e 6163 6365 6c65  s[k][self.accele
+00017d00: 7261 7469 6f6e 5f6b 6579 5d29 0d0a 2020  ration_key])..  
+00017d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d30: 616c 6c5f 6469 7265 6374 696f 6e61 6c5f  all_directional_
+00017d40: 6368 616e 6765 2e61 7070 656e 6428 616c  change.append(al
+00017d50: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017d60: 5d5b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ][self.motion_an
+00017d70: 676c 655f 6b65 795d 2920 2020 0d0a 2020  gle_key])   ..  
+00017d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017da0: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
+00017db0: 6c5f 6d61 736b 2e61 7070 656e 6428 616c  l_mask.append(al
+00017dc0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017dd0: 5d5b 7365 6c66 2e64 6973 7461 6e63 655f  ][self.distance_
+00017de0: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
+00017df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e10: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00017e20: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017e30: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00017e40: 6973 705f 7a20 3d20 6e70 2e61 6273 286e  isp_z = np.abs(n
+00017e50: 702e 6469 6666 286d 6974 6f74 6963 5f64  p.diff(mitotic_d
+00017e60: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+00017e70: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00017e80: 6f74 6963 5f64 6973 705f 7920 3d20 6e70  otic_disp_y = np
+00017e90: 2e61 6273 286e 702e 6469 6666 286d 6974  .abs(np.diff(mit
+00017ea0: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
+00017eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ec0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+00017ed0: 7820 3d20 6e70 2e61 6273 286e 702e 6469  x = np.abs(np.di
+00017ee0: 6666 286d 6974 6f74 6963 5f64 6973 705f  ff(mitotic_disp_
+00017ef0: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
+00017f00: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00017f10: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
+00017f20: 6e70 2e61 6273 286e 702e 6469 6666 286e  np.abs(np.diff(n
+00017f30: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00017f40: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+00017f50: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00017f60: 6f74 6963 5f64 6973 705f 7920 3d20 6e70  otic_disp_y = np
+00017f70: 2e61 6273 286e 702e 6469 6666 286e 6f6e  .abs(np.diff(non
+00017f80: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
+00017f90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017fa0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00017fb0: 6963 5f64 6973 705f 7820 3d20 6e70 2e61  ic_disp_x = np.a
+00017fc0: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
+00017fd0: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00017fe0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017ff0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+00018000: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
+00018010: 6666 2861 6c6c 5f64 6973 705f 7a29 290d  ff(all_disp_z)).
+00018020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018030: 2020 2020 2061 6c6c 5f64 6973 705f 7920       all_disp_y 
+00018040: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+00018050: 2861 6c6c 5f64 6973 705f 7929 290d 0a20  (all_disp_y)).. 
+00018060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018070: 2020 2061 6c6c 5f64 6973 705f 7820 3d20     all_disp_x = 
+00018080: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
+00018090: 6c6c 5f64 6973 705f 7829 290d 0a0d 0a0d  ll_disp_x)).....
+000180a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000180d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000180e0: 656c 662e 7469 6d65 2e61 7070 656e 6428  elf.time.append(
+000180f0: 6920 2a20 7365 6c66 2e74 6361 6c69 6272  i * self.tcalibr
+00018100: 6174 696f 6e29 0d0a 0d0a 0d0a 2020 2020  ation)......    
+00018110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018120: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+00018130: 6e5f 6469 7370 5f7a 2e61 7070 656e 6428  n_disp_z.append(
+00018140: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
+00018150: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
+00018160: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018170: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+00018180: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+00018190: 7374 6428 6d69 746f 7469 635f 6469 7370  std(mitotic_disp
+000181a0: 5f7a 2929 0d0a 0d0a 2020 2020 2020 2020  _z))....        
+000181b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000181c0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+000181d0: 7370 5f79 2e61 7070 656e 6428 6e70 2e6d  sp_y.append(np.m
+000181e0: 6561 6e28 6d69 746f 7469 635f 6469 7370  ean(mitotic_disp
+000181f0: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
+00018200: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018210: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00018220: 792e 6170 7065 6e64 286e 702e 7374 6428  y.append(np.std(
+00018230: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
+00018240: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018250: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018260: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
+00018270: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018280: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+00018290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000182a0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000182b0: 6963 5f76 6172 5f64 6973 705f 782e 6170  ic_var_disp_x.ap
+000182c0: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
+000182d0: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
+000182e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182f0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018300: 5f6d 6561 6e5f 7261 6469 7573 2e61 7070  _mean_radius.app
+00018310: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
+00018320: 7469 635f 7261 6469 7573 2929 0d0a 2020  tic_radius))..  
+00018330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018340: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00018350: 6172 5f72 6164 6975 732e 6170 7065 6e64  ar_radius.append
+00018360: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
+00018370: 7261 6469 7573 2929 0d0a 2020 2020 2020  radius))..      
+00018380: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00018390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183a0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+000183b0: 5f6d 6561 6e5f 7370 6565 642e 6170 7065  _mean_speed.appe
+000183c0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+000183d0: 6963 5f73 7065 6564 2929 0d0a 2020 2020  ic_speed))..    
+000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183f0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00018400: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
+00018410: 2e73 7464 286d 6974 6f74 6963 5f73 7065  .std(mitotic_spe
+00018420: 6564 2929 0d0a 0d0a 2020 2020 2020 2020  ed))....        
+00018430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018440: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6163  .mitotic_mean_ac
+00018450: 632e 6170 7065 6e64 286e 702e 6d65 616e  c.append(np.mean
+00018460: 286d 6974 6f74 6963 5f61 6363 2929 0d0a  (mitotic_acc))..
+00018470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018480: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018490: 5f76 6172 5f61 6363 2e61 7070 656e 6428  _var_acc.append(
+000184a0: 6e70 2e73 7464 286d 6974 6f74 6963 5f61  np.std(mitotic_a
+000184b0: 6363 2929 0d0a 0d0a 2020 2020 2020 2020  cc))....        
+000184c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000184d0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+000184e0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+000184f0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018500: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+00018510: 6e61 6c5f 6368 616e 6765 2929 0d0a 2020  nal_change))..  
 00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018530: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00018540: 635f 6d65 616e 5f64 6973 705f 792e 6170  c_mean_disp_y.ap
-00018550: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00018560: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
-00018570: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018580: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00018590: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-000185a0: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
-000185b0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-000185c0: 705f 7929 290d 0a0d 0a20 2020 2020 2020  p_y))....       
-000185d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000185e0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-000185f0: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
-00018600: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00018610: 6f74 6963 5f64 6973 705f 7829 290d 0a20  otic_disp_x)).. 
-00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018630: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00018640: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
-00018650: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
-00018660: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
-00018670: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018680: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018690: 6e5f 6d69 746f 7469 635f 6d65 616e 5f72  n_mitotic_mean_r
-000186a0: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-000186b0: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-000186c0: 5f72 6164 6975 7329 290d 0a20 2020 2020  _radius))..     
-000186d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000186e0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-000186f0: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
-00018700: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-00018710: 6f74 6963 5f72 6164 6975 7329 290d 0a0d  otic_radius))...
-00018720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018730: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00018740: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-00018750: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018760: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00018770: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00018780: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018790: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
-000187a0: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
-000187b0: 6428 6e6f 6e5f 6d69 746f 7469 635f 7370  d(non_mitotic_sp
-000187c0: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-000187d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000187e0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-000187f0: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
-00018800: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018810: 635f 6163 6329 290d 0a20 2020 2020 2020  c_acc))..       
-00018820: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018830: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00018840: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
-00018850: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-00018860: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
-00018870: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018880: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00018890: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-000188a0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-000188b0: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-000188c0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000188d0: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
-000188e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000188f0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00018900: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018910: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
-00018920: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6972  (non_mitotic_dir
-00018930: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-00018940: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-00018950: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018960: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00018970: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018980: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
-00018990: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-000189a0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000189b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000189c0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000189d0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-000189e0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-000189f0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-00018a00: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-00018a10: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-00018a20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018a30: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018a40: 5f6d 6561 6e5f 6469 7370 5f7a 2e61 7070  _mean_disp_z.app
-00018a50: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-00018a60: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00018a70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018a80: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-00018a90: 7a2e 6170 7065 6e64 286e 702e 7374 6428  z.append(np.std(
-00018aa0: 616c 6c5f 6469 7370 5f7a 2929 0d0a 0d0a  all_disp_z))....
-00018ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ac0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00018ad0: 6e5f 6469 7370 5f79 2e61 7070 656e 6428  n_disp_y.append(
-00018ae0: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7370  np.mean(all_disp
-00018af0: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
-00018b00: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00018b10: 6c6c 5f76 6172 5f64 6973 705f 792e 6170  ll_var_disp_y.ap
-00018b20: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00018b30: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
-00018b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b50: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00018b60: 7370 5f78 2e61 7070 656e 6428 6e70 2e6d  sp_x.append(np.m
-00018b70: 6561 6e28 616c 6c5f 6469 7370 5f78 2929  ean(all_disp_x))
-00018b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018b90: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00018ba0: 6172 5f64 6973 705f 782e 6170 7065 6e64  ar_disp_x.append
-00018bb0: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
-00018bc0: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00018bd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018be0: 2e61 6c6c 5f6d 6561 6e5f 7261 6469 7573  .all_mean_radius
-00018bf0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018c00: 616c 6c5f 7261 6469 7573 2929 0d0a 2020  all_radius))..  
-00018c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c20: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f72    self.all_var_r
-00018c30: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00018c40: 7374 6428 616c 6c5f 7261 6469 7573 2929  std(all_radius))
-00018c50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018c60: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018c70: 5f6d 6561 6e5f 7370 6565 642e 6170 7065  _mean_speed.appe
-00018c80: 6e64 286e 702e 6d65 616e 2861 6c6c 5f73  nd(np.mean(all_s
-00018c90: 7065 6564 2929 0d0a 2020 2020 2020 2020  peed))..        
-00018ca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018cb0: 2e61 6c6c 5f76 6172 5f73 7065 6564 2e61  .all_var_speed.a
-00018cc0: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00018cd0: 5f73 7065 6564 2929 0d0a 0d0a 2020 2020  _speed))....    
-00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cf0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6163  self.all_mean_ac
-00018d00: 632e 6170 7065 6e64 286e 702e 6d65 616e  c.append(np.mean
-00018d10: 2861 6c6c 5f61 6363 2929 0d0a 2020 2020  (all_acc))..    
-00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d30: 7365 6c66 2e61 6c6c 5f76 6172 5f61 6363  self.all_var_acc
-00018d40: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
-00018d50: 6c6c 5f61 6363 2929 0d0a 0d0a 0d0a 0d0a  ll_acc))........
-00018d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d70: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00018d80: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
-00018d90: 616e 6765 2e61 7070 656e 6428 6e70 2e6d  ange.append(np.m
-00018da0: 6561 6e28 616c 6c5f 6469 7265 6374 696f  ean(all_directio
-00018db0: 6e61 6c5f 6368 616e 6765 2929 0d0a 2020  nal_change))..  
-00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dd0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00018de0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00018df0: 652e 6170 7065 6e64 286e 702e 7374 6428  e.append(np.std(
-00018e00: 616c 6c5f 6469 7265 6374 696f 6e61 6c5f  all_directional_
-00018e10: 6368 616e 6765 2929 0d0a 0d0a 2020 2020  change))....    
-00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e30: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00018e40: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018e50: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018e60: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
-00018e70: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
-00018e80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018e90: 6c66 2e61 6c6c 5f76 6172 5f64 6973 7461  lf.all_var_dista
-00018ea0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00018eb0: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00018ec0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018ed0: 736b 2929 0d0a 2020 2020 2020 2020 2020  sk))..          
-00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ef0: 2020 0d0a 2020 2020 2020 2020 0d0a 6465    ..        ..de
-00018f00: 6620 626f 756e 6461 7279 5f70 6f69 6e74  f boundary_point
-00018f10: 7328 6d61 736b 2c20 7863 616c 6962 7261  s(mask, xcalibra
-00018f20: 7469 6f6e 2c20 7963 616c 6962 7261 7469  tion, ycalibrati
-00018f30: 6f6e 2c20 7a63 616c 6962 7261 7469 6f6e  on, zcalibration
-00018f40: 293a 0d0a 0d0a 2020 2020 6e64 696d 203d  ):....    ndim =
-00018f50: 206c 656e 286d 6173 6b2e 7368 6170 6529   len(mask.shape)
-00018f60: 0d0a 2020 2020 7469 6d65 645f 6d61 736b  ..    timed_mask
-00018f70: 203d 207b 7d0d 0a20 2020 206d 6173 6b20   = {}..    mask 
-00018f80: 3d20 6d61 736b 203e 2030 0d0a 2020 2020  = mask > 0..    
-00018f90: 6d61 736b 203d 206d 6173 6b2e 6173 7479  mask = mask.asty
-00018fa0: 7065 2827 7569 6e74 3827 290d 0a20 2020  pe('uint8')..   
-00018fb0: 2023 2059 5820 7368 6170 6564 206f 626a   # YX shaped obj
-00018fc0: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
-00018fd0: 203d 3d20 323a 0d0a 2020 2020 2020 2020   == 2:..        
-00018fe0: 0d0a 2020 2020 2020 2020 626f 756e 6461  ..        bounda
-00018ff0: 7279 203d 2066 696e 645f 626f 756e 6461  ry = find_bounda
-00019000: 7269 6573 286d 6173 6b29 0d0a 2020 2020  ries(mask)..    
-00019010: 2020 2020 7265 6769 6f6e 6365 6e74 726f      regioncentro
-00019020: 6964 203d 2028 302c 2920 2b20 636f 6d70  id = (0,) + comp
-00019030: 7574 655f 6365 6e74 726f 6964 2862 6f75  ute_centroid(bou
-00019040: 6e64 6172 7929 200d 0a20 2020 2020 2020  ndary) ..       
-00019050: 2069 6e64 6963 6573 203d 206e 702e 7768   indices = np.wh
-00019060: 6572 6528 626f 756e 6461 7279 203e 2030  ere(boundary > 0
-00019070: 290d 0a20 2020 2020 2020 2072 6561 6c5f  )..        real_
-00019080: 696e 6469 6365 7320 3d20 6e70 2e74 7261  indices = np.tra
-00019090: 6e73 706f 7365 286e 702e 6173 6172 7261  nspose(np.asarra
-000190a0: 7928 696e 6469 6365 732c 2064 7479 7065  y(indices, dtype
-000190b0: 3d6e 702e 666c 6f61 7433 3229 292e 636f  =np.float32)).co
-000190c0: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
-000190d0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
-000190e0: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
-000190f0: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
-00019100: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019110: 735b 6a5d 5b30 5d20 3d20 7265 616c 5f69  s[j][0] = real_i
-00019120: 6e64 6963 6573 5b6a 5d5b 305d 202a 2079  ndices[j][0] * y
-00019130: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00019140: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-00019150: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
-00019160: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-00019170: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
-00019180: 0a0d 0a20 2020 2020 2020 2074 7265 6520  ...        tree 
-00019190: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
-000191a0: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
-000191b0: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
-000191c0: 6f62 6a65 6374 2063 6f6e 7461 696e 7320  object contains 
-000191d0: 6c69 7374 206f 6620 616c 6c20 7468 6520  list of all the 
-000191e0: 706f 696e 7473 2066 6f72 2061 6c6c 2074  points for all t
-000191f0: 6865 206c 6162 656c 7320 696e 2074 6865  he labels in the
-00019200: 204d 6173 6b20 696d 6167 6520 7769 7468   Mask image with
-00019210: 2074 6865 206c 6162 656c 2069 6420 616e   the label id an
-00019220: 6420 766f 6c75 6d65 206f 6620 6561 6368  d volume of each
-00019230: 206c 6162 656c 0d0a 2020 2020 2020 2020   label..        
-00019240: 7469 6d65 645f 6d61 736b 5b73 7472 2830  timed_mask[str(0
-00019250: 295d 203d 205b 7472 6565 2c20 696e 6469  )] = [tree, indi
-00019260: 6365 732c 2072 6567 696f 6e63 656e 7472  ces, regioncentr
-00019270: 6f69 645d 0d0a 0d0a 2020 2020 2320 5459  oid]....    # TY
-00019280: 5820 7368 6170 6564 206f 626a 6563 740d  X shaped object.
-00019290: 0a20 2020 2069 6620 6e64 696d 203d 3d20  .    if ndim == 
-000192a0: 333a 0d0a 0d0a 0d0a 2020 2020 2020 2020  3:......        
-000192b0: 666f 7220 6920 696e 2074 7164 6d28 7261  for i in tqdm(ra
-000192c0: 6e67 6528 302c 206d 6173 6b2e 7368 6170  nge(0, mask.shap
-000192d0: 655b 305d 2929 3a0d 0a20 2020 2020 2020  e[0])):..       
-000192e0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000192f0: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
-00019300: 6172 7920 3d20 6669 6e64 5f62 6f75 6e64  ary = find_bound
-00019310: 6172 6965 7328 6d61 736b 5b69 2c3a 5d29  aries(mask[i,:])
-00019320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019330: 2020 7265 6769 6f6e 6365 6e74 726f 6964    regioncentroid
-00019340: 203d 2028 302c 2920 2b20 636f 6d70 7574   = (0,) + comput
-00019350: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
-00019360: 6172 7929 200d 0a20 2020 2020 2020 2020  ary) ..         
-00019370: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-00019380: 206e 702e 7768 6572 6528 626f 756e 6461   np.where(bounda
-00019390: 7279 203e 2030 290d 0a20 2020 2020 2020  ry > 0)..       
-000193a0: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-000193b0: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
-000193c0: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
-000193d0: 696e 6469 6365 732c 2064 7479 7065 3d6e  indices, dtype=n
-000193e0: 702e 666c 6f61 7433 3229 292e 636f 7079  p.float32)).copy
-000193f0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-00019400: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-00019410: 616e 6765 2830 2c20 6c65 6e28 7265 616c  ange(0, len(real
-00019420: 5f69 6e64 6963 6573 2929 3a0d 0a0d 0a20  _indices)):.... 
-00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019440: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
-00019450: 6a5d 5b30 5d20 3d20 7265 616c 5f69 6e64  j][0] = real_ind
-00019460: 6963 6573 5b6a 5d5b 305d 202a 2079 6361  ices[j][0] * yca
-00019470: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00019480: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00019490: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-000194a0: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
-000194b0: 5b6a 5d5b 315d 202a 2078 6361 6c69 6272  [j][1] * xcalibr
-000194c0: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
-000194d0: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
-000194e0: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
-000194f0: 7265 616c 5f69 6e64 6963 6573 290d 0a0d  real_indices)...
+00018530: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00018540: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+00018550: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+00018560: 7374 6428 6d69 746f 7469 635f 6469 7265  std(mitotic_dire
+00018570: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
+00018580: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018590: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+000185a0: 6f74 6963 5f6d 6561 6e5f 6469 7374 616e  otic_mean_distan
+000185b0: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+000185c0: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
+000185d0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+000185e0: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
+000185f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018600: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+00018610: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018620: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
+00018630: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00018640: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
+00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018660: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018670: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
+00018680: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018690: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+000186a0: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
+000186b0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000186c0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+000186d0: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+000186e0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+000186f0: 6469 7370 5f7a 2929 0d0a 0d0a 2020 2020  disp_z))....    
+00018700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018710: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00018720: 5f6d 6561 6e5f 6469 7370 5f79 2e61 7070  _mean_disp_y.app
+00018730: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+00018740: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
+00018750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018760: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018770: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00018780: 792e 6170 7065 6e64 286e 702e 7374 6428  y.append(np.std(
+00018790: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+000187a0: 5f79 2929 0d0a 0d0a 2020 2020 2020 2020  _y))....        
+000187b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000187c0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+000187d0: 6e5f 6469 7370 5f78 2e61 7070 656e 6428  n_disp_x.append(
+000187e0: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+000187f0: 7469 635f 6469 7370 5f78 2929 0d0a 2020  tic_disp_x))..  
+00018800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018810: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018820: 6963 5f76 6172 5f64 6973 705f 782e 6170  ic_var_disp_x.ap
+00018830: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
+00018840: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+00018850: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018860: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018870: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 7261  _mitotic_mean_ra
+00018880: 6469 7573 2e61 7070 656e 6428 6e70 2e6d  dius.append(np.m
+00018890: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+000188a0: 7261 6469 7573 2929 0d0a 2020 2020 2020  radius))..      
+000188b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000188c0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+000188d0: 6172 5f72 6164 6975 732e 6170 7065 6e64  ar_radius.append
+000188e0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
+000188f0: 7469 635f 7261 6469 7573 2929 0d0a 0d0a  tic_radius))....
+00018900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018910: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018920: 6f74 6963 5f6d 6561 6e5f 7370 6565 642e  otic_mean_speed.
+00018930: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00018940: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
+00018950: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018960: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018970: 5f6d 6974 6f74 6963 5f76 6172 5f73 7065  _mitotic_var_spe
+00018980: 6564 2e61 7070 656e 6428 6e70 2e73 7464  ed.append(np.std
+00018990: 286e 6f6e 5f6d 6974 6f74 6963 5f73 7065  (non_mitotic_spe
+000189a0: 6564 2929 0d0a 0d0a 2020 2020 2020 2020  ed))....        
+000189b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000189c0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+000189d0: 6e5f 6163 632e 6170 7065 6e64 286e 702e  n_acc.append(np.
+000189e0: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
+000189f0: 5f61 6363 2929 0d0a 2020 2020 2020 2020  _acc))..        
+00018a00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018a10: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00018a20: 5f61 6363 2e61 7070 656e 6428 6e70 2e73  _acc.append(np.s
+00018a30: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f61  td(non_mitotic_a
+00018a40: 6363 2929 0d0a 0d0a 2020 2020 2020 2020  cc))....        
+00018a50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018a60: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00018a70: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
+00018a80: 616e 6765 2e61 7070 656e 6428 6e70 2e6d  ange.append(np.m
+00018a90: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+00018aa0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00018ab0: 6765 2929 0d0a 2020 2020 2020 2020 2020  ge))..          
+00018ac0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018ad0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+00018ae0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00018af0: 652e 6170 7065 6e64 286e 702e 7374 6428  e.append(np.std(
+00018b00: 6e6f 6e5f 6d69 746f 7469 635f 6469 7265  non_mitotic_dire
+00018b10: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
+00018b20: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00018b30: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018b40: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+00018b50: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018b60: 6b2e 6170 7065 6e64 286e 702e 6d65 616e  k.append(np.mean
+00018b70: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+00018b80: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+00018b90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018ba0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018bb0: 6d69 746f 7469 635f 7661 725f 6469 7374  mitotic_var_dist
+00018bc0: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00018bd0: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
+00018be0: 5f6d 6974 6f74 6963 5f64 6973 7461 6e63  _mitotic_distanc
+00018bf0: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a0d  e_cell_mask))...
+00018c00: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018c10: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018c20: 6d65 616e 5f64 6973 705f 7a2e 6170 7065  mean_disp_z.appe
+00018c30: 6e64 286e 702e 6d65 616e 2861 6c6c 5f64  nd(np.mean(all_d
+00018c40: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+00018c50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018c60: 662e 616c 6c5f 7661 725f 6469 7370 5f7a  f.all_var_disp_z
+00018c70: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
+00018c80: 6c6c 5f64 6973 705f 7a29 290d 0a0d 0a20  ll_disp_z)).... 
+00018c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ca0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00018cb0: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
+00018cc0: 702e 6d65 616e 2861 6c6c 5f64 6973 705f  p.mean(all_disp_
+00018cd0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+00018ce0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018cf0: 6c5f 7661 725f 6469 7370 5f79 2e61 7070  l_var_disp_y.app
+00018d00: 656e 6428 6e70 2e73 7464 2861 6c6c 5f64  end(np.std(all_d
+00018d10: 6973 705f 7929 290d 0a0d 0a20 2020 2020  isp_y))....     
+00018d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018d30: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00018d40: 705f 782e 6170 7065 6e64 286e 702e 6d65  p_x.append(np.me
+00018d50: 616e 2861 6c6c 5f64 6973 705f 7829 290d  an(all_disp_x)).
+00018d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018d70: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00018d80: 725f 6469 7370 5f78 2e61 7070 656e 6428  r_disp_x.append(
+00018d90: 6e70 2e73 7464 2861 6c6c 5f64 6973 705f  np.std(all_disp_
+00018da0: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
+00018db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018dc0: 616c 6c5f 6d65 616e 5f72 6164 6975 732e  all_mean_radius.
+00018dd0: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+00018de0: 6c6c 5f72 6164 6975 7329 290d 0a20 2020  ll_radius))..   
+00018df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e00: 2073 656c 662e 616c 6c5f 7661 725f 7261   self.all_var_ra
+00018e10: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
+00018e20: 7464 2861 6c6c 5f72 6164 6975 7329 290d  td(all_radius)).
+00018e30: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018e40: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018e50: 6d65 616e 5f73 7065 6564 2e61 7070 656e  mean_speed.appen
+00018e60: 6428 6e70 2e6d 6561 6e28 616c 6c5f 7370  d(np.mean(all_sp
+00018e70: 6565 6429 290d 0a20 2020 2020 2020 2020  eed))..         
+00018e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018e90: 616c 6c5f 7661 725f 7370 6565 642e 6170  all_var_speed.ap
+00018ea0: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
+00018eb0: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
+00018ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018ed0: 656c 662e 616c 6c5f 6d65 616e 5f61 6363  elf.all_mean_acc
+00018ee0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018ef0: 616c 6c5f 6163 6329 290d 0a20 2020 2020  all_acc))..     
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018f10: 656c 662e 616c 6c5f 7661 725f 6163 632e  elf.all_var_acc.
+00018f20: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018f30: 6c5f 6163 6329 290d 0a0d 0a0d 0a0d 0a20  l_acc))........ 
+00018f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f50: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00018f60: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018f70: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
+00018f80: 616e 2861 6c6c 5f64 6972 6563 7469 6f6e  an(all_direction
+00018f90: 616c 5f63 6861 6e67 6529 290d 0a20 2020  al_change))..   
+00018fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fb0: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00018fc0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00018fd0: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
+00018fe0: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
+00018ff0: 6861 6e67 6529 290d 0a0d 0a20 2020 2020  hange))....     
+00019000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019010: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00019020: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00019030: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+00019040: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+00019050: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+00019060: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019070: 662e 616c 6c5f 7661 725f 6469 7374 616e  f.all_var_distan
+00019080: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+00019090: 656e 6428 6e70 2e73 7464 2861 6c6c 5f64  end(np.std(all_d
+000190a0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000190b0: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
+000190c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190d0: 200d 0a20 2020 2020 2020 200d 0a64 6566   ..        ..def
+000190e0: 2062 6f75 6e64 6172 795f 706f 696e 7473   boundary_points
+000190f0: 286d 6173 6b2c 2078 6361 6c69 6272 6174  (mask, xcalibrat
+00019100: 696f 6e2c 2079 6361 6c69 6272 6174 696f  ion, ycalibratio
+00019110: 6e2c 207a 6361 6c69 6272 6174 696f 6e29  n, zcalibration)
+00019120: 3a0d 0a0d 0a20 2020 206e 6469 6d20 3d20  :....    ndim = 
+00019130: 6c65 6e28 6d61 736b 2e73 6861 7065 290d  len(mask.shape).
+00019140: 0a20 2020 2074 696d 6564 5f6d 6173 6b20  .    timed_mask 
+00019150: 3d20 7b7d 0d0a 2020 2020 6d61 736b 203d  = {}..    mask =
+00019160: 206d 6173 6b20 3e20 300d 0a20 2020 206d   mask > 0..    m
+00019170: 6173 6b20 3d20 6d61 736b 2e61 7374 7970  ask = mask.astyp
+00019180: 6528 2775 696e 7438 2729 0d0a 2020 2020  e('uint8')..    
+00019190: 2320 5958 2073 6861 7065 6420 6f62 6a65  # YX shaped obje
+000191a0: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
+000191b0: 3d3d 2032 3a0d 0a20 2020 2020 2020 200d  == 2:..        .
+000191c0: 0a20 2020 2020 2020 2062 6f75 6e64 6172  .        boundar
+000191d0: 7920 3d20 6669 6e64 5f62 6f75 6e64 6172  y = find_boundar
+000191e0: 6965 7328 6d61 736b 290d 0a20 2020 2020  ies(mask)..     
+000191f0: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
+00019200: 6420 3d20 2830 2c29 202b 2063 6f6d 7075  d = (0,) + compu
+00019210: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
+00019220: 6461 7279 2920 0d0a 2020 2020 2020 2020  dary) ..        
+00019230: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
+00019240: 7265 2862 6f75 6e64 6172 7920 3e20 3029  re(boundary > 0)
+00019250: 0d0a 2020 2020 2020 2020 7265 616c 5f69  ..        real_i
+00019260: 6e64 6963 6573 203d 206e 702e 7472 616e  ndices = np.tran
+00019270: 7370 6f73 6528 6e70 2e61 7361 7272 6179  spose(np.asarray
+00019280: 2869 6e64 6963 6573 2c20 6474 7970 653d  (indices, dtype=
+00019290: 6e70 2e66 6c6f 6174 3332 2929 2e63 6f70  np.float32)).cop
+000192a0: 7928 290d 0a0d 0a20 2020 2020 2020 2066  y()....        f
+000192b0: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+000192c0: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
+000192d0: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
+000192e0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+000192f0: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
+00019300: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
+00019310: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00019320: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+00019330: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
+00019340: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+00019350: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
+00019360: 0d0a 2020 2020 2020 2020 7472 6565 203d  ..        tree =
+00019370: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+00019380: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
+00019390: 2020 2020 2020 2020 2320 5468 6973 206f          # This o
+000193a0: 626a 6563 7420 636f 6e74 6169 6e73 206c  bject contains l
+000193b0: 6973 7420 6f66 2061 6c6c 2074 6865 2070  ist of all the p
+000193c0: 6f69 6e74 7320 666f 7220 616c 6c20 7468  oints for all th
+000193d0: 6520 6c61 6265 6c73 2069 6e20 7468 6520  e labels in the 
+000193e0: 4d61 736b 2069 6d61 6765 2077 6974 6820  Mask image with 
+000193f0: 7468 6520 6c61 6265 6c20 6964 2061 6e64  the label id and
+00019400: 2076 6f6c 756d 6520 6f66 2065 6163 6820   volume of each 
+00019410: 6c61 6265 6c0d 0a20 2020 2020 2020 2074  label..        t
+00019420: 696d 6564 5f6d 6173 6b5b 7374 7228 3029  imed_mask[str(0)
+00019430: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
+00019440: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
+00019450: 6964 5d0d 0a0d 0a20 2020 2023 2054 5958  id]....    # TYX
+00019460: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
+00019470: 2020 2020 6966 206e 6469 6d20 3d3d 2033      if ndim == 3
+00019480: 3a0d 0a0d 0a0d 0a20 2020 2020 2020 2066  :......        f
+00019490: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
+000194a0: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
+000194b0: 5b30 5d29 293a 0d0a 2020 2020 2020 2020  [0])):..        
+000194c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000194d0: 2020 2020 2020 2020 2020 626f 756e 6461            bounda
+000194e0: 7279 203d 2066 696e 645f 626f 756e 6461  ry = find_bounda
+000194f0: 7269 6573 286d 6173 6b5b 692c 3a5d 290d  ries(mask[i,:]).
 00019500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019510: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
-00019520: 6929 5d20 3d20 5b74 7265 652c 2069 6e64  i)] = [tree, ind
-00019530: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
-00019540: 726f 6964 5d0d 0a20 2020 2020 2020 2020  roid]..         
-00019550: 2020 200d 0a20 2020 2023 2054 5a59 5820     ..    # TZYX 
-00019560: 7368 6170 6564 206f 626a 6563 740d 0a20  shaped object.. 
-00019570: 2020 2069 6620 6e64 696d 203d 3d20 343a     if ndim == 4:
-00019580: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00019590: 274d 6173 6b73 206d 6164 6520 696e 746f  'Masks made into
-000195a0: 2061 2034 4420 6379 6c69 6e64 6572 2c20   a 4D cylinder, 
-000195b0: 7570 2729 0d0a 2020 2020 2020 2020 626f  up')..        bo
-000195c0: 756e 6461 7279 203d 206e 702e 7a65 726f  undary = np.zero
-000195d0: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-000195e0: 5b6d 6173 6b2e 7368 6170 655b 305d 2c20  [mask.shape[0], 
-000195f0: 6d61 736b 2e73 6861 7065 5b31 5d2c 206d  mask.shape[1], m
-00019600: 6173 6b2e 7368 6170 655b 325d 2c20 6d61  ask.shape[2], ma
-00019610: 736b 2e73 6861 7065 5b33 5d5d 0d0a 2020  sk.shape[3]]..  
-00019620: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00019630: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00019640: 302c 206d 6173 6b2e 7368 6170 655b 305d  0, mask.shape[0]
-00019650: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00019660: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
-00019670: 756e 6461 7279 5b69 2c3a 5d20 3d20 6669  undary[i,:] = fi
-00019680: 6e64 5f62 6f75 6e64 6172 6965 7328 6d61  nd_boundaries(ma
-00019690: 736b 5b69 2c3a 5d29 0d0a 2020 2020 2020  sk[i,:])..      
-000196a0: 2020 2020 2020 7265 6769 6f6e 6365 6e74        regioncent
-000196b0: 726f 6964 203d 2063 6f6d 7075 7465 5f63  roid = compute_c
-000196c0: 656e 7472 6f69 6428 626f 756e 6461 7279  entroid(boundary
-000196d0: 5b69 2c3a 5d29 200d 0a20 2020 2020 2020  [i,:]) ..       
-000196e0: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-000196f0: 702e 7768 6572 6528 626f 756e 6461 7279  p.where(boundary
-00019700: 5b69 2c3a 5d20 3e20 3029 0d0a 2020 2020  [i,:] > 0)..    
-00019710: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-00019720: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
-00019730: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
-00019740: 6e64 6963 6573 2c20 6474 7970 653d 6e70  ndices, dtype=np
-00019750: 2e66 6c6f 6174 3332 2929 2e63 6f70 7928  .float32)).copy(
-00019760: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00019770: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-00019780: 302c 206c 656e 2872 6561 6c5f 696e 6469  0, len(real_indi
-00019790: 6365 7329 293a 0d0a 0d0a 2020 2020 2020  ces)):....      
-000197a0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000197b0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-000197c0: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-000197d0: 6a5d 5b30 5d20 2a20 7a63 616c 6962 7261  j][0] * zcalibra
-000197e0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-000197f0: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-00019800: 6e64 6963 6573 5b6a 5d5b 315d 203d 2072  ndices[j][1] = r
-00019810: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-00019820: 5d20 2a20 7963 616c 6962 7261 7469 6f6e  ] * ycalibration
-00019830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019840: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-00019850: 6573 5b6a 5d5b 325d 203d 2072 6561 6c5f  es[j][2] = real_
-00019860: 696e 6469 6365 735b 6a5d 5b32 5d20 2a20  indices[j][2] * 
-00019870: 7863 616c 6962 7261 7469 6f6e 0d0a 0d0a  xcalibration....
-00019880: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-00019890: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
-000198a0: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
-000198b0: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-000198c0: 6d65 645f 6d61 736b 5b73 7472 2869 295d  med_mask[str(i)]
-000198d0: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
-000198e0: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
-000198f0: 645d 0d0a 2020 2020 7072 696e 7428 2743  d]..    print('C
-00019900: 6f6d 7075 7465 6420 7468 6520 626f 756e  omputed the boun
-00019910: 6461 7279 2070 6f69 6e74 7327 290d 0a0d  dary points')...
-00019920: 0a20 2020 2072 6574 7572 6e20 7469 6d65  .    return time
-00019930: 645f 6d61 736b 2c20 626f 756e 6461 7279  d_mask, boundary
-00019940: 2020 2020 2020 2020 0d0a 0d0a 6465 6620          ....def 
-00019950: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
-00019960: 2862 696e 6172 795f 696d 6167 6529 3a0d  (binary_image):.
-00019970: 0a20 2020 2023 2045 6e73 7572 6520 6269  .    # Ensure bi
-00019980: 6e61 7279 2069 6d61 6765 2069 7320 6120  nary image is a 
-00019990: 4e75 6d50 7920 6172 7261 790d 0a20 2020  NumPy array..   
-000199a0: 2062 696e 6172 795f 696d 6167 6520 3d20   binary_image = 
-000199b0: 6e70 2e61 7272 6179 2862 696e 6172 795f  np.array(binary_
-000199c0: 696d 6167 6529 0d0a 0d0a 2020 2020 7768  image)....    wh
-000199d0: 6974 655f 7069 7865 6c73 203d 206e 702e  ite_pixels = np.
-000199e0: 7768 6572 6528 6269 6e61 7279 5f69 6d61  where(binary_ima
-000199f0: 6765 203d 3d20 3129 0d0a 2020 2020 6e75  ge == 1)..    nu
-00019a00: 6d5f 7069 7865 6c73 203d 206c 656e 2877  m_pixels = len(w
-00019a10: 6869 7465 5f70 6978 656c 735b 305d 290d  hite_pixels[0]).
-00019a20: 0a0d 0a20 2020 2023 2043 6f6d 7075 7465  ...    # Compute
-00019a30: 2074 6865 2063 656e 7472 6f69 6420 6f66   the centroid of
-00019a40: 2074 6865 2077 6869 7465 2070 6978 656c   the white pixel
-00019a50: 7320 696e 2074 6865 2062 6f75 6e64 6172  s in the boundar
-00019a60: 7920 696d 6167 650d 0a20 2020 2063 656e  y image..    cen
-00019a70: 7472 6f69 6420 3d20 6e70 2e7a 6572 6f73  troid = np.zeros
-00019a80: 2862 696e 6172 795f 696d 6167 652e 6e64  (binary_image.nd
-00019a90: 696d 290d 0a20 2020 2066 6f72 2064 696d  im)..    for dim
-00019aa0: 2069 6e20 7261 6e67 6528 6269 6e61 7279   in range(binary
-00019ab0: 5f69 6d61 6765 2e6e 6469 6d29 3a0d 0a20  _image.ndim):.. 
-00019ac0: 2020 2020 2020 2063 656e 7472 6f69 645b         centroid[
-00019ad0: 6469 6d5d 203d 2077 6869 7465 5f70 6978  dim] = white_pix
-00019ae0: 656c 735b 6469 6d5d 2e73 756d 2829 202f  els[dim].sum() /
-00019af0: 206e 756d 5f70 6978 656c 730d 0a0d 0a20   num_pixels.... 
-00019b00: 2020 2072 6574 7572 6e20 6365 6e74 726f     return centro
-00019b10: 6964 0d0a 0d0a 0d0a 0d0a 200d 0a0d 0a64  id........ ....d
-00019b20: 6566 2067 6574 5f63 7376 5f64 6174 6128  ef get_csv_data(
-00019b30: 6373 7629 3a0d 0a0d 0a20 2020 2020 2020  csv):....       
-00019b40: 2064 6174 6173 6574 203d 2070 642e 7265   dataset = pd.re
-00019b50: 6164 5f63 7376 280d 0a20 2020 2020 2020  ad_csv(..       
-00019b60: 2020 2020 2063 7376 2c20 6465 6c69 6d69       csv, delimi
-00019b70: 7465 723d 222c 222c 2065 6e63 6f64 696e  ter=",", encodin
-00019b80: 673d 2275 6e69 636f 6465 5f65 7363 6170  g="unicode_escap
-00019b90: 6522 2c20 6c6f 775f 6d65 6d6f 7279 3d46  e", low_memory=F
-00019ba0: 616c 7365 0d0a 2020 2020 2020 2020 295b  alse..        )[
-00019bb0: 333a 5d0d 0a20 2020 2020 2020 2064 6174  3:]..        dat
-00019bc0: 6173 6574 5f69 6e64 6578 203d 2064 6174  aset_index = dat
-00019bd0: 6173 6574 2e69 6e64 6578 0d0a 2020 2020  aset.index..    
-00019be0: 2020 2020 7265 7475 726e 2064 6174 6173      return datas
-00019bf0: 6574 2c20 6461 7461 7365 745f 696e 6465  et, dataset_inde
-00019c00: 780d 0a20 2020 200d 0a64 6566 2067 6574  x..    ..def get
-00019c10: 5f73 706f 745f 6461 7461 7365 7428 7370  _spot_dataset(sp
-00019c20: 6f74 5f64 6174 6173 6574 2c20 7472 6163  ot_dataset, trac
-00019c30: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00019c40: 6b65 7973 2c20 7863 616c 6962 7261 7469  keys, xcalibrati
-00019c50: 6f6e 2c20 7963 616c 6962 7261 7469 6f6e  on, ycalibration
-00019c60: 2c20 7a63 616c 6962 7261 7469 6f6e 2c20  , zcalibration, 
-00019c70: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
-00019c80: 2c20 6465 7465 6374 696f 6e63 6861 6e6e  , detectionchann
-00019c90: 656c 293a 0d0a 2020 2020 2020 2020 416c  el):..        Al
-00019ca0: 6c56 616c 7565 7320 3d20 7b7d 0d0a 2020  lValues = {}..  
-00019cb0: 2020 2020 2020 706f 7369 7820 3d20 7472        posix = tr
-00019cc0: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00019cd0: 745f 6b65 7973 5b22 706f 7369 7822 5d0d  t_keys["posix"].
-00019ce0: 0a20 2020 2020 2020 2070 6f73 6979 203d  .        posiy =
-00019cf0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-00019d00: 7370 6f74 5f6b 6579 735b 2270 6f73 6979  spot_keys["posiy
-00019d10: 225d 0d0a 2020 2020 2020 2020 706f 7369  "]..        posi
-00019d20: 7a20 3d20 7472 6163 6b5f 616e 616c 7973  z = track_analys
-00019d30: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
-00019d40: 7369 7a22 5d0d 0a20 2020 2020 2020 2066  siz"]..        f
-00019d50: 7261 6d65 203d 2074 7261 636b 5f61 6e61  rame = track_ana
-00019d60: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-00019d70: 2266 7261 6d65 225d 0d0a 2020 2020 2020  "frame"]..      
-00019d80: 2020 0d0a 2020 2020 2020 2020 4c6f 6361    ..        Loca
-00019d90: 7469 6f6e 5820 3d20 280d 0a20 2020 2020  tionX = (..     
-00019da0: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
-00019db0: 7365 745b 706f 7369 785d 2e61 7374 7970  set[posix].astyp
-00019dc0: 6528 2266 6c6f 6174 2229 202f 2078 6361  e("float") / xca
-00019dd0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00019de0: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
-00019df0: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
-00019e00: 7469 6f6e 5920 3d20 280d 0a20 2020 2020  tionY = (..     
-00019e10: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
-00019e20: 7365 745b 706f 7369 795d 2e61 7374 7970  set[posiy].astyp
-00019e30: 6528 2266 6c6f 6174 2229 202f 2079 6361  e("float") / yca
-00019e40: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00019e50: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
-00019e60: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
-00019e70: 7469 6f6e 5a20 3d20 280d 0a20 2020 2020  tionZ = (..     
-00019e80: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
-00019e90: 7365 745b 706f 7369 7a5d 2e61 7374 7970  set[posiz].astyp
-00019ea0: 6528 2266 6c6f 6174 2229 202f 207a 6361  e("float") / zca
-00019eb0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00019ec0: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
-00019ed0: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
-00019ee0: 7469 6f6e 5420 3d20 2873 706f 745f 6461  tionT = (spot_da
-00019ef0: 7461 7365 745b 6672 616d 655d 2e61 7374  taset[frame].ast
-00019f00: 7970 6528 2266 6c6f 6174 2229 292e 6173  ype("float")).as
-00019f10: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
-00019f20: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-00019f30: 2069 676e 6f72 655f 7661 6c75 6573 203d   ignore_values =
-00019f40: 205b 7472 6163 6b5f 616e 616c 7973 6973   [track_analysis
-00019f50: 5f73 706f 745f 6b65 7973 5b22 6d65 616e  _spot_keys["mean
-00019f60: 5f69 6e74 656e 7369 7479 225d 2c74 7261  _intensity"],tra
-00019f70: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00019f80: 5f6b 6579 735b 2274 6f74 616c 5f69 6e74  _keys["total_int
-00019f90: 656e 7369 7479 225d 5d0d 0a20 2020 2020  ensity"]]..     
-00019fa0: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
-00019fb0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-00019fc0: 706f 745f 6b65 7973 2e69 7465 6d73 2829  pot_keys.items()
-00019fd0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00019fe0: 2020 2020 2069 6620 6465 7465 6374 696f       if detectio
-00019ff0: 6e63 6861 6e6e 656c 203d 3d20 313a 0d0a  nchannel == 1:..
-0001a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a010: 2020 2020 2069 6620 6b20 3d3d 2022 6d65       if k == "me
-0001a020: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
-0001a030: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-0001a040: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0001a050: 616c 7565 203d 2074 7261 636b 5f61 6e61  alue = track_ana
-0001a060: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-0001a070: 226d 6561 6e5f 696e 7465 6e73 6974 7922  "mean_intensity"
-0001a080: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001a090: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-0001a0a0: 6c56 616c 7565 735b 7661 6c75 655d 203d  lValues[value] =
-0001a0b0: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
-0001a0c0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a0d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a0e0: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
-0001a0f0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0001a100: 6368 3222 3a0d 0a20 2020 2020 2020 2020  ch2":..         
-0001a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a120: 2020 7661 6c75 6520 3d20 7472 6163 6b5f    value = track_
-0001a130: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001a140: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
-0001a150: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
-0001a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a170: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
-0001a180: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
-0001a190: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
-0001a1a0: 6174 2229 2020 2020 2020 200d 0a0d 0a20  at")       .... 
-0001a1b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001a1c0: 6620 7620 6e6f 7420 696e 2069 676e 6f72  f v not in ignor
-0001a1d0: 655f 7661 6c75 6573 3a0d 0a20 2020 2020  e_values:..     
+00019510: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
+00019520: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
+00019530: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
+00019540: 7279 2920 0d0a 2020 2020 2020 2020 2020  ry) ..          
+00019550: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+00019560: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
+00019570: 7920 3e20 3029 0d0a 2020 2020 2020 2020  y > 0)..        
+00019580: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+00019590: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
+000195a0: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
+000195b0: 6e64 6963 6573 2c20 6474 7970 653d 6e70  ndices, dtype=np
+000195c0: 2e66 6c6f 6174 3332 2929 2e63 6f70 7928  .float32)).copy(
+000195d0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+000195e0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+000195f0: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
+00019600: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
+00019610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019620: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+00019630: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
+00019640: 6365 735b 6a5d 5b30 5d20 2a20 7963 616c  ces[j][0] * ycal
+00019650: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00019660: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00019670: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+00019680: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+00019690: 6a5d 5b31 5d20 2a20 7863 616c 6962 7261  j][1] * xcalibra
+000196a0: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+000196b0: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
+000196c0: 7061 7469 616c 2e63 4b44 5472 6565 2872  patial.cKDTree(r
+000196d0: 6561 6c5f 696e 6469 6365 7329 0d0a 0d0a  eal_indices)....
+000196e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196f0: 7469 6d65 645f 6d61 736b 5b73 7472 2869  timed_mask[str(i
+00019700: 295d 203d 205b 7472 6565 2c20 696e 6469  )] = [tree, indi
+00019710: 6365 732c 2072 6567 696f 6e63 656e 7472  ces, regioncentr
+00019720: 6f69 645d 0d0a 2020 2020 2020 2020 2020  oid]..          
+00019730: 2020 0d0a 2020 2020 2320 545a 5958 2073    ..    # TZYX s
+00019740: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
+00019750: 2020 6966 206e 6469 6d20 3d3d 2034 3a0d    if ndim == 4:.
+00019760: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+00019770: 4d61 736b 7320 6d61 6465 2069 6e74 6f20  Masks made into 
+00019780: 6120 3444 2063 796c 696e 6465 722c 2075  a 4D cylinder, u
+00019790: 7027 290d 0a20 2020 2020 2020 2062 6f75  p')..        bou
+000197a0: 6e64 6172 7920 3d20 6e70 2e7a 6572 6f73  ndary = np.zeros
+000197b0: 280d 0a20 2020 2020 2020 2020 2020 205b  (..            [
+000197c0: 6d61 736b 2e73 6861 7065 5b30 5d2c 206d  mask.shape[0], m
+000197d0: 6173 6b2e 7368 6170 655b 315d 2c20 6d61  ask.shape[1], ma
+000197e0: 736b 2e73 6861 7065 5b32 5d2c 206d 6173  sk.shape[2], mas
+000197f0: 6b2e 7368 6170 655b 335d 5d0d 0a20 2020  k.shape[3]]..   
+00019800: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00019810: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+00019820: 2c20 6d61 736b 2e73 6861 7065 5b30 5d29  , mask.shape[0])
+00019830: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
+00019840: 0a20 2020 2020 2020 2020 2020 2062 6f75  .            bou
+00019850: 6e64 6172 795b 692c 3a5d 203d 2066 696e  ndary[i,:] = fin
+00019860: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
+00019870: 6b5b 692c 3a5d 290d 0a20 2020 2020 2020  k[i,:])..       
+00019880: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
+00019890: 6f69 6420 3d20 636f 6d70 7574 655f 6365  oid = compute_ce
+000198a0: 6e74 726f 6964 2862 6f75 6e64 6172 795b  ntroid(boundary[
+000198b0: 692c 3a5d 2920 0d0a 2020 2020 2020 2020  i,:]) ..        
+000198c0: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
+000198d0: 2e77 6865 7265 2862 6f75 6e64 6172 795b  .where(boundary[
+000198e0: 692c 3a5d 203e 2030 290d 0a20 2020 2020  i,:] > 0)..     
+000198f0: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+00019900: 6365 7320 3d20 6e70 2e74 7261 6e73 706f  ces = np.transpo
+00019910: 7365 286e 702e 6173 6172 7261 7928 696e  se(np.asarray(in
+00019920: 6469 6365 732c 2064 7479 7065 3d6e 702e  dices, dtype=np.
+00019930: 666c 6f61 7433 3229 292e 636f 7079 2829  float32)).copy()
+00019940: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019950: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+00019960: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
+00019970: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
+00019980: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00019990: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+000199a0: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+000199b0: 5d5b 305d 202a 207a 6361 6c69 6272 6174  ][0] * zcalibrat
+000199c0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+000199d0: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+000199e0: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
+000199f0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+00019a00: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
+00019a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019a20: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+00019a30: 735b 6a5d 5b32 5d20 3d20 7265 616c 5f69  s[j][2] = real_i
+00019a40: 6e64 6963 6573 5b6a 5d5b 325d 202a 2078  ndices[j][2] * x
+00019a50: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
+00019a60: 2020 2020 2020 2020 2020 2074 7265 6520             tree 
+00019a70: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
+00019a80: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
+00019a90: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00019aa0: 6564 5f6d 6173 6b5b 7374 7228 6929 5d20  ed_mask[str(i)] 
+00019ab0: 3d20 5b74 7265 652c 2069 6e64 6963 6573  = [tree, indices
+00019ac0: 2c20 7265 6769 6f6e 6365 6e74 726f 6964  , regioncentroid
+00019ad0: 5d0d 0a20 2020 2070 7269 6e74 2827 436f  ]..    print('Co
+00019ae0: 6d70 7574 6564 2074 6865 2062 6f75 6e64  mputed the bound
+00019af0: 6172 7920 706f 696e 7473 2729 0d0a 0d0a  ary points')....
+00019b00: 2020 2020 7265 7475 726e 2074 696d 6564      return timed
+00019b10: 5f6d 6173 6b2c 2062 6f75 6e64 6172 7920  _mask, boundary 
+00019b20: 2020 2020 2020 200d 0a0d 0a64 6566 2063         ....def c
+00019b30: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
+00019b40: 6269 6e61 7279 5f69 6d61 6765 293a 0d0a  binary_image):..
+00019b50: 2020 2020 2320 456e 7375 7265 2062 696e      # Ensure bin
+00019b60: 6172 7920 696d 6167 6520 6973 2061 204e  ary image is a N
+00019b70: 756d 5079 2061 7272 6179 0d0a 2020 2020  umPy array..    
+00019b80: 6269 6e61 7279 5f69 6d61 6765 203d 206e  binary_image = n
+00019b90: 702e 6172 7261 7928 6269 6e61 7279 5f69  p.array(binary_i
+00019ba0: 6d61 6765 290d 0a0d 0a20 2020 2077 6869  mage)....    whi
+00019bb0: 7465 5f70 6978 656c 7320 3d20 6e70 2e77  te_pixels = np.w
+00019bc0: 6865 7265 2862 696e 6172 795f 696d 6167  here(binary_imag
+00019bd0: 6520 3d3d 2031 290d 0a20 2020 206e 756d  e == 1)..    num
+00019be0: 5f70 6978 656c 7320 3d20 6c65 6e28 7768  _pixels = len(wh
+00019bf0: 6974 655f 7069 7865 6c73 5b30 5d29 0d0a  ite_pixels[0])..
+00019c00: 0d0a 2020 2020 2320 436f 6d70 7574 6520  ..    # Compute 
+00019c10: 7468 6520 6365 6e74 726f 6964 206f 6620  the centroid of 
+00019c20: 7468 6520 7768 6974 6520 7069 7865 6c73  the white pixels
+00019c30: 2069 6e20 7468 6520 626f 756e 6461 7279   in the boundary
+00019c40: 2069 6d61 6765 0d0a 2020 2020 6365 6e74   image..    cent
+00019c50: 726f 6964 203d 206e 702e 7a65 726f 7328  roid = np.zeros(
+00019c60: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
+00019c70: 6d29 0d0a 2020 2020 666f 7220 6469 6d20  m)..    for dim 
+00019c80: 696e 2072 616e 6765 2862 696e 6172 795f  in range(binary_
+00019c90: 696d 6167 652e 6e64 696d 293a 0d0a 2020  image.ndim):..  
+00019ca0: 2020 2020 2020 6365 6e74 726f 6964 5b64        centroid[d
+00019cb0: 696d 5d20 3d20 7768 6974 655f 7069 7865  im] = white_pixe
+00019cc0: 6c73 5b64 696d 5d2e 7375 6d28 2920 2f20  ls[dim].sum() / 
+00019cd0: 6e75 6d5f 7069 7865 6c73 0d0a 0d0a 2020  num_pixels....  
+00019ce0: 2020 7265 7475 726e 2063 656e 7472 6f69    return centroi
+00019cf0: 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465  d........ ....de
+00019d00: 6620 6765 745f 6373 765f 6461 7461 2863  f get_csv_data(c
+00019d10: 7376 293a 0d0a 0d0a 2020 2020 2020 2020  sv):....        
+00019d20: 6461 7461 7365 7420 3d20 7064 2e72 6561  dataset = pd.rea
+00019d30: 645f 6373 7628 0d0a 2020 2020 2020 2020  d_csv(..        
+00019d40: 2020 2020 6373 762c 2064 656c 696d 6974      csv, delimit
+00019d50: 6572 3d22 2c22 2c20 656e 636f 6469 6e67  er=",", encoding
+00019d60: 3d22 756e 6963 6f64 655f 6573 6361 7065  ="unicode_escape
+00019d70: 222c 206c 6f77 5f6d 656d 6f72 793d 4661  ", low_memory=Fa
+00019d80: 6c73 650d 0a20 2020 2020 2020 2029 5b33  lse..        )[3
+00019d90: 3a5d 0d0a 2020 2020 2020 2020 6461 7461  :]..        data
+00019da0: 7365 745f 696e 6465 7820 3d20 6461 7461  set_index = data
+00019db0: 7365 742e 696e 6465 780d 0a20 2020 2020  set.index..     
+00019dc0: 2020 2072 6574 7572 6e20 6461 7461 7365     return datase
+00019dd0: 742c 2064 6174 6173 6574 5f69 6e64 6578  t, dataset_index
+00019de0: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+00019df0: 7370 6f74 5f64 6174 6173 6574 2873 706f  spot_dataset(spo
+00019e00: 745f 6461 7461 7365 742c 2074 7261 636b  t_dataset, track
+00019e10: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00019e20: 6579 732c 2078 6361 6c69 6272 6174 696f  eys, xcalibratio
+00019e30: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
+00019e40: 207a 6361 6c69 6272 6174 696f 6e2c 2041   zcalibration, A
+00019e50: 7474 7269 6275 7465 426f 786e 616d 652c  ttributeBoxname,
+00019e60: 2064 6574 6563 7469 6f6e 6368 616e 6e65   detectionchanne
+00019e70: 6c29 3a0d 0a20 2020 2020 2020 2041 6c6c  l):..        All
+00019e80: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
+00019e90: 2020 2020 2070 6f73 6978 203d 2074 7261       posix = tra
+00019ea0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00019eb0: 5f6b 6579 735b 2270 6f73 6978 225d 0d0a  _keys["posix"]..
+00019ec0: 2020 2020 2020 2020 706f 7369 7920 3d20          posiy = 
+00019ed0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00019ee0: 706f 745f 6b65 7973 5b22 706f 7369 7922  pot_keys["posiy"
+00019ef0: 5d0d 0a20 2020 2020 2020 2070 6f73 697a  ]..        posiz
+00019f00: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+00019f10: 735f 7370 6f74 5f6b 6579 735b 2270 6f73  s_spot_keys["pos
+00019f20: 697a 225d 0d0a 2020 2020 2020 2020 6672  iz"]..        fr
+00019f30: 616d 6520 3d20 7472 6163 6b5f 616e 616c  ame = track_anal
+00019f40: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00019f50: 6672 616d 6522 5d0d 0a20 2020 2020 2020  frame"]..       
+00019f60: 200d 0a20 2020 2020 2020 204c 6f63 6174   ..        Locat
+00019f70: 696f 6e58 203d 2028 0d0a 2020 2020 2020  ionX = (..      
+00019f80: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+00019f90: 6574 5b70 6f73 6978 5d2e 6173 7479 7065  et[posix].astype
+00019fa0: 2822 666c 6f61 7422 2920 2f20 7863 616c  ("float") / xcal
+00019fb0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00019fc0: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+00019fd0: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+00019fe0: 696f 6e59 203d 2028 0d0a 2020 2020 2020  ionY = (..      
+00019ff0: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+0001a000: 6574 5b70 6f73 6979 5d2e 6173 7479 7065  et[posiy].astype
+0001a010: 2822 666c 6f61 7422 2920 2f20 7963 616c  ("float") / ycal
+0001a020: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001a030: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+0001a040: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+0001a050: 696f 6e5a 203d 2028 0d0a 2020 2020 2020  ionZ = (..      
+0001a060: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+0001a070: 6574 5b70 6f73 697a 5d2e 6173 7479 7065  et[posiz].astype
+0001a080: 2822 666c 6f61 7422 2920 2f20 7a63 616c  ("float") / zcal
+0001a090: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001a0a0: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+0001a0b0: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+0001a0c0: 696f 6e54 203d 2028 7370 6f74 5f64 6174  ionT = (spot_dat
+0001a0d0: 6173 6574 5b66 7261 6d65 5d2e 6173 7479  aset[frame].asty
+0001a0e0: 7065 2822 666c 6f61 7422 2929 2e61 7374  pe("float")).ast
+0001a0f0: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+0001a100: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0001a110: 6967 6e6f 7265 5f76 616c 7565 7320 3d20  ignore_values = 
+0001a120: 5b74 7261 636b 5f61 6e61 6c79 7369 735f  [track_analysis_
+0001a130: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
+0001a140: 696e 7465 6e73 6974 7922 5d2c 7472 6163  intensity"],trac
+0001a150: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+0001a160: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
+0001a170: 6e73 6974 7922 5d5d 0d0a 2020 2020 2020  nsity"]]..      
+0001a180: 2020 666f 7220 286b 2c76 2920 696e 2074    for (k,v) in t
+0001a190: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001a1a0: 6f74 5f6b 6579 732e 6974 656d 7328 293a  ot_keys.items():
+0001a1b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001a1c0: 2020 2020 6966 2064 6574 6563 7469 6f6e      if detection
+0001a1d0: 6368 616e 6e65 6c20 3d3d 2031 3a0d 0a20  channel == 1:.. 
 0001a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0001a200: 2020 2020 2020 2020 2020 2041 6c6c 5661             AllVa
-0001a210: 6c75 6573 5b76 5d20 3d20 7370 6f74 5f64  lues[v] = spot_d
-0001a220: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
-0001a230: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
-0001a240: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001a250: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
-0001a260: 7565 735b 706f 7369 785d 203d 2072 6f75  ues[posix] = rou
-0001a270: 6e64 284c 6f63 6174 696f 6e58 2c33 290d  nd(LocationX,3).
-0001a280: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
-0001a290: 6573 5b70 6f73 6979 5d20 3d20 726f 756e  es[posiy] = roun
-0001a2a0: 6428 4c6f 6361 7469 6f6e 592c 3329 0d0a  d(LocationY,3)..
-0001a2b0: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
-0001a2c0: 735b 706f 7369 7a5d 203d 2072 6f75 6e64  s[posiz] = round
-0001a2d0: 284c 6f63 6174 696f 6e5a 2c33 290d 0a20  (LocationZ,3).. 
-0001a2e0: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-0001a2f0: 5b66 7261 6d65 5d20 3d20 726f 756e 6428  [frame] = round(
-0001a300: 4c6f 6361 7469 6f6e 542c 3329 0d0a 2020  LocationT,3)..  
-0001a310: 2020 2020 2020 4174 7472 6962 7574 6569        Attributei
-0001a320: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0001a330: 2041 7474 7269 6275 7465 6964 732e 6170   Attributeids.ap
-0001a340: 7065 6e64 2841 7474 7269 6275 7465 426f  pend(AttributeBo
-0001a350: 786e 616d 6529 0d0a 2020 2020 2020 2020  xname)..        
-0001a360: 666f 7220 6174 7472 6962 7574 656e 616d  for attributenam
-0001a370: 6520 696e 2041 6c6c 5661 6c75 6573 2e6b  e in AllValues.k
-0001a380: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-0001a390: 2020 2020 2020 4174 7472 6962 7574 6569        Attributei
-0001a3a0: 6473 2e61 7070 656e 6428 6174 7472 6962  ds.append(attrib
-0001a3b0: 7574 656e 616d 6529 2020 2020 0d0a 2020  utename)    ..  
-0001a3c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001a3d0: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-0001a3e0: 7475 726e 2041 7474 7269 6275 7465 6964  turn Attributeid
-0001a3f0: 732c 2041 6c6c 5661 6c75 6573 2020 2020  s, AllValues    
-0001a400: 200d 0a20 2020 200d 0a64 6566 2067 6574   ..    ..def get
-0001a410: 5f74 7261 636b 5f64 6174 6173 6574 2874  _track_dataset(t
-0001a420: 7261 636b 5f64 6174 6173 6574 2c20 7472  rack_dataset, tr
-0001a430: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001a440: 745f 6b65 7973 2c20 7472 6163 6b5f 616e  t_keys, track_an
-0001a450: 616c 7973 6973 5f74 7261 636b 5f6b 6579  alysis_track_key
-0001a460: 732c 2054 7261 636b 4174 7472 6962 7574  s, TrackAttribut
-0001a470: 6542 6f78 6e61 6d65 293a 0d0a 0d0a 2020  eBoxname):....  
-0001a480: 2020 2020 2020 416c 6c54 7261 636b 5661        AllTrackVa
-0001a490: 6c75 6573 203d 207b 7d0d 0a20 2020 2020  lues = {}..     
-0001a4a0: 2020 2074 7261 636b 5f69 6420 3d20 7472     track_id = tr
-0001a4b0: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001a4c0: 745f 6b65 7973 5b22 7472 6163 6b5f 6964  t_keys["track_id
-0001a4d0: 225d 0d0a 2020 2020 2020 2020 5469 6420  "]..        Tid 
-0001a4e0: 3d20 7472 6163 6b5f 6461 7461 7365 745b  = track_dataset[
-0001a4f0: 7472 6163 6b5f 6964 5d2e 6173 7479 7065  track_id].astype
-0001a500: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
-0001a510: 2020 0d0a 2020 2020 2020 2020 416c 6c54    ..        AllT
-0001a520: 7261 636b 5661 6c75 6573 5b74 7261 636b  rackValues[track
-0001a530: 5f69 645d 203d 2054 6964 0d0a 2020 2020  _id] = Tid..    
-0001a540: 2020 0d0a 2020 2020 2020 2020 666f 7220    ..        for 
-0001a550: 286b 2c20 7629 2069 6e20 7472 6163 6b5f  (k, v) in track_
-0001a560: 616e 616c 7973 6973 5f74 7261 636b 5f6b  analysis_track_k
-0001a570: 6579 732e 6974 656d 7328 293a 0d0a 0d0a  eys.items():....
-0001a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a590: 7820 3d20 7472 6163 6b5f 6461 7461 7365  x = track_datase
-0001a5a0: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
-0001a5b0: 6174 2229 0d0a 2020 2020 2020 2020 2020  at")..          
-0001a5c0: 2020 2020 2020 6d69 6e76 616c 203d 206d        minval = m
-0001a5d0: 696e 2878 290d 0a20 2020 2020 2020 2020  in(x)..         
-0001a5e0: 2020 2020 2020 206d 6178 7661 6c20 3d20         maxval = 
-0001a5f0: 6d61 7828 7829 0d0a 0d0a 2020 2020 2020  max(x)....      
-0001a600: 2020 2020 2020 2020 2020 6966 206d 696e            if min
-0001a610: 7661 6c20 3e20 3020 616e 6420 6d61 7876  val > 0 and maxv
-0001a620: 616c 203c 3d20 313a 0d0a 0d0a 2020 2020  al <= 1:....    
-0001a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a640: 7820 3d20 7820 2b20 310d 0a0d 0a20 2020  x = x + 1....   
-0001a650: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-0001a660: 5472 6163 6b56 616c 7565 735b 6b5d 203d  TrackValues[k] =
-0001a670: 2072 6f75 6e64 2878 2c20 3329 0d0a 0d0a   round(x, 3)....
-0001a680: 2020 2020 2020 2020 5472 6163 6b41 7474          TrackAtt
-0001a690: 7269 6275 7465 6964 7320 3d20 5b5d 0d0a  ributeids = []..
-0001a6a0: 2020 2020 2020 2020 5472 6163 6b41 7474          TrackAtt
-0001a6b0: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
-0001a6c0: 2854 7261 636b 4174 7472 6962 7574 6542  (TrackAttributeB
-0001a6d0: 6f78 6e61 6d65 290d 0a20 2020 2020 2020  oxname)..       
-0001a6e0: 2066 6f72 2061 7474 7269 6275 7465 6e61   for attributena
-0001a6f0: 6d65 2069 6e20 7472 6163 6b5f 616e 616c  me in track_anal
-0001a700: 7973 6973 5f74 7261 636b 5f6b 6579 732e  ysis_track_keys.
-0001a710: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
-0001a720: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
-0001a730: 7574 6569 6473 2e61 7070 656e 6428 6174  uteids.append(at
-0001a740: 7472 6962 7574 656e 616d 6529 2020 2020  tributename)    
-0001a750: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-0001a760: 7265 7475 726e 2054 7261 636b 4174 7472  return TrackAttr
-0001a770: 6962 7574 6569 6473 2c20 416c 6c54 7261  ibuteids, AllTra
-0001a780: 636b 5661 6c75 6573 0d0a 2020 2020 0d0a  ckValues..    ..
-0001a790: 6465 6620 6765 745f 6564 6765 735f 6461  def get_edges_da
-0001a7a0: 7461 7365 7428 6564 6765 735f 6461 7461  taset(edges_data
-0001a7b0: 7365 742c 2065 6467 6573 5f64 6174 6173  set, edges_datas
-0001a7c0: 6574 5f69 6e64 6578 2c20 7472 6163 6b5f  et_index, track_
-0001a7d0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001a7e0: 7973 2c20 7472 6163 6b5f 616e 616c 7973  ys, track_analys
-0001a7f0: 6973 5f65 6467 6573 5f6b 6579 7329 3a0d  is_edges_keys):.
-0001a800: 0a0d 0a20 2020 2020 2020 2041 6c6c 4564  ...        AllEd
-0001a810: 6765 7356 616c 7565 7320 3d20 7b7d 0d0a  gesValues = {}..
-0001a820: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
-0001a830: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
-0001a840: 735f 7370 6f74 5f6b 6579 735b 2274 7261  s_spot_keys["tra
-0001a850: 636b 5f69 6422 5d0d 0a20 2020 2020 2020  ck_id"]..       
-0001a860: 2054 6964 203d 2065 6467 6573 5f64 6174   Tid = edges_dat
-0001a870: 6173 6574 5b74 7261 636b 5f69 645d 2e61  aset[track_id].a
-0001a880: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001a890: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-0001a8a0: 3d20 6e70 2e77 6865 7265 2854 6964 203d  = np.where(Tid =
-0001a8b0: 3d20 3029 0d0a 2020 2020 2020 2020 6d61  = 0)..        ma
-0001a8c0: 7874 7261 636b 5f69 6420 3d20 6d61 7828  xtrack_id = max(
-0001a8d0: 5469 6429 0d0a 2020 2020 2020 2020 636f  Tid)..        co
-0001a8e0: 6e64 6974 696f 6e5f 696e 6469 6365 7320  ndition_indices 
-0001a8f0: 3d20 6564 6765 735f 6461 7461 7365 745f  = edges_dataset_
-0001a900: 696e 6465 785b 696e 6469 6365 735d 0d0a  index[indices]..
-0001a910: 2020 2020 2020 2020 5469 645b 636f 6e64          Tid[cond
-0001a920: 6974 696f 6e5f 696e 6469 6365 735d 203d  ition_indices] =
-0001a930: 206d 6178 7472 6163 6b5f 6964 202b 2031   maxtrack_id + 1
-0001a940: 0d0a 2020 2020 2020 2020 416c 6c45 6467  ..        AllEdg
-0001a950: 6573 5661 6c75 6573 5b74 7261 636b 5f69  esValues[track_i
-0001a960: 645d 203d 2054 6964 0d0a 0d0a 2020 2020  d] = Tid....    
-0001a970: 2020 2020 666f 7220 6b20 696e 2074 7261      for k in tra
-0001a980: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
-0001a990: 735f 6b65 7973 2e76 616c 7565 7328 293a  s_keys.values():
-0001a9a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a9b0: 6966 206b 2021 3d20 7472 6163 6b5f 6964  if k != track_id
-0001a9c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a9d0: 2020 2078 203d 2065 6467 6573 5f64 6174     x = edges_dat
-0001a9e0: 6173 6574 5b6b 5d2e 6173 7479 7065 2822  aset[k].astype("
-0001a9f0: 666c 6f61 7422 290d 0a0d 0a20 2020 2020  float")....     
-0001aa00: 2020 2020 2020 2020 2020 2041 6c6c 4564             AllEd
-0001aa10: 6765 7356 616c 7565 735b 6b5d 203d 2078  gesValues[k] = x
-0001aa20: 2020 200d 0a20 2020 2020 2020 2020 0d0a     ..         ..
-0001aa30: 2020 2020 2020 2020 7265 7475 726e 2041          return A
-0001aa40: 6c6c 4564 6765 7356 616c 7565 7320 2020  llEdgesValues   
-0001aa50: 0d0a 2020 2020 0d0a 2020 2020 2020 200d  ..    ..       .
-0001aa60: 0a20 2020 200d 0a64 6566 2073 6361 6c65  .    ..def scale
-0001aa70: 5f76 616c 7565 2878 2c20 7363 616c 6520  _value(x, scale 
-0001aa80: 3d20 3235 3520 2a20 3235 3529 3a0d 0a0d  = 255 * 255):...
-0001aa90: 0a0d 0a20 2020 2020 7265 7475 726e 2078  ...     return x
-0001aaa0: 202a 2073 6361 6c65 2020 200d 0a20 2020   * scale   ..   
-0001aab0: 200d 0a0d 0a0d 0a64 6566 2070 726f 625f   ......def prob_
-0001aac0: 7369 676d 6f69 6428 7829 3a0d 0a20 2020  sigmoid(x):..   
-0001aad0: 2072 6574 7572 6e20 3120 2d20 6d61 7468   return 1 - math
-0001aae0: 2e65 7870 282d 7829 0d0a 0d0a 0d0a 6465  .exp(-x)......de
-0001aaf0: 6620 616e 6775 6c61 725f 6368 616e 6765  f angular_change
-0001ab00: 2876 6563 5f30 2c20 7665 635f 3129 3a0d  (vec_0, vec_1):.
-0001ab10: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0001ab20: 2020 2076 6563 5f30 203d 2076 6563 5f30     vec_0 = vec_0
-0001ab30: 202f 206e 702e 6c69 6e61 6c67 2e6e 6f72   / np.linalg.nor
-0001ab40: 6d28 7665 635f 3029 0d0a 2020 2020 2020  m(vec_0)..      
-0001ab50: 2020 7665 635f 3120 3d20 7665 635f 3120    vec_1 = vec_1 
-0001ab60: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
-0001ab70: 2876 6563 5f31 290d 0a20 2020 2020 2020  (vec_1)..       
-0001ab80: 2061 6e67 6c65 203d 206e 702e 6172 6363   angle = np.arcc
-0001ab90: 6f73 286e 702e 636c 6970 286e 702e 646f  os(np.clip(np.do
-0001aba0: 7428 7665 635f 302c 2076 6563 5f31 292c  t(vec_0, vec_1),
-0001abb0: 202d 312e 302c 2031 2e30 2929 0d0a 2020   -1.0, 1.0))..  
-0001abc0: 2020 2020 2020 616e 676c 6520 3d20 616e        angle = an
-0001abd0: 676c 6520 2a20 3138 3020 2f20 6e70 2e70  gle * 180 / np.p
-0001abe0: 690d 0a20 2020 2020 2020 2072 6574 7572  i..        retur
-0001abf0: 6e20 616e 676c 650d 0a20 2020 2020 0d0a  n angle..     ..
-0001ac00: 0d0a 6465 6620 6576 616c 5f62 6f6f 6c28  ..def eval_bool(
-0001ac10: 7661 6c75 6529 3a0d 0a20 2020 2020 2020  value):..       
-0001ac20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0001ac30: 2020 2020 2069 6620 7661 6c75 6520 203d       if value  =
-0001ac40: 3d20 2754 7275 6527 3a20 0d0a 2020 2020  = 'True': ..    
-0001ac50: 2020 2020 2020 2020 2020 2020 6469 765f              div_
-0001ac60: 6b65 7920 3d20 5472 7565 0d0a 2020 2020  key = True..    
-0001ac70: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001ac80: 2020 2020 2020 2020 2020 2064 6976 5f6b             div_k
-0001ac90: 6579 203d 2046 616c 7365 200d 0a0d 0a20  ey = False .... 
-0001aca0: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-0001acb0: 765f 6b65 7920 2020 2020 2020 2020 2020  v_key           
-0001acc0: 2020 2020 200d 0a0d 0a64 6566 2063 6865       ....def che
-0001acd0: 636b 5f61 6e64 5f75 7064 6174 655f 6d61  ck_and_update_ma
-0001ace0: 736b 286d 6173 6b2c 696d 6167 6529 3a0d  sk(mask,image):.
-0001acf0: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
-0001ad00: 2020 6966 206c 656e 286d 6173 6b2e 7368    if len(mask.sh
-0001ad10: 6170 6529 203c 206c 656e 2869 6d61 6765  ape) < len(image
-0001ad20: 2e73 6861 7065 293a 0d0a 2020 2020 2020  .shape):..      
-0001ad30: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
-0001ad40: 6b20 3d20 6e70 2e7a 6572 6f73 280d 0a20  k = np.zeros(.. 
-0001ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad60: 2020 2020 2020 2020 2020 205b 0d0a 2020             [..  
-0001ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad80: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001ad90: 6167 652e 7368 6170 655b 305d 2c0d 0a20  age.shape[0],.. 
-0001ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001adc0: 6d61 6765 2e73 6861 7065 5b31 5d2c 0d0a  mage.shape[1],..
-0001add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adf0: 696d 6167 652e 7368 6170 655b 325d 2c0d  image.shape[2],.
-0001ae00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae20: 2069 6d61 6765 2e73 6861 7065 5b33 5d2c   image.shape[3],
-0001ae30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ae40: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-0001ae50: 2064 7479 7065 3d22 7569 6e74 3822 0d0a   dtype="uint8"..
-0001ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae70: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001ae80: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0001ae90: 7261 6e67 6528 302c 2075 7064 6174 655f  range(0, update_
-0001aea0: 6d61 736b 2e73 6861 7065 5b30 5d29 3a0d  mask.shape[0]):.
-0001aeb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001aec0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-0001aed0: 302c 2075 7064 6174 655f 6d61 736b 2e73  0, update_mask.s
-0001aee0: 6861 7065 5b31 5d29 3a0d 0a0d 0a20 2020  hape[1]):....   
-0001aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af00: 2075 7064 6174 655f 6d61 736b 5b69 2c20   update_mask[i, 
-0001af10: 6a2c 203a 2c20 3a5d 203d 206d 6173 6b5b  j, :, :] = mask[
-0001af20: 692c 203a 2c20 3a5d 0d0a 2020 2020 2020  i, :, :]..      
-0001af30: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0001af40: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-0001af50: 6d61 736b 203d 206d 6173 6b0d 0a0d 0a20  mask = mask.... 
-0001af60: 2020 2020 2020 2072 6574 7572 6e20 7570         return up
-0001af70: 6461 7465 5f6d 6173 6b20 2020 2020 2020  date_mask       
-0001af80: 200d 0a20 2020 2020 2020 0d0a             ..       ..
+0001a1f0: 2020 2020 6966 206b 203d 3d20 226d 6561      if k == "mea
+0001a200: 6e5f 696e 7465 6e73 6974 795f 6368 3222  n_intensity_ch2"
+0001a210: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001a220: 2020 2020 2020 2020 2020 2020 2020 7661                va
+0001a230: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
+0001a240: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001a250: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
+0001a260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a270: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
+0001a280: 5661 6c75 6573 5b76 616c 7565 5d20 3d20  Values[value] = 
+0001a290: 7370 6f74 5f64 6174 6173 6574 5b76 5d2e  spot_dataset[v].
+0001a2a0: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001a2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a2c0: 2020 2020 2020 6966 206b 203d 3d20 2274        if k == "t
+0001a2d0: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
+0001a2e0: 6832 223a 0d0a 2020 2020 2020 2020 2020  h2":..          
+0001a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a300: 2076 616c 7565 203d 2074 7261 636b 5f61   value = track_a
+0001a310: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001a320: 735b 2274 6f74 616c 5f69 6e74 656e 7369  s["total_intensi
+0001a330: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
+0001a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a350: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
+0001a360: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
+0001a370: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001a380: 7422 2920 2020 2020 2020 0d0a 0d0a 2020  t")       ....  
+0001a390: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001a3a0: 2076 206e 6f74 2069 6e20 6967 6e6f 7265   v not in ignore
+0001a3b0: 5f76 616c 7565 733a 0d0a 2020 2020 2020  _values:..      
+0001a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0001a3e0: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
+0001a3f0: 7565 735b 765d 203d 2073 706f 745f 6461  ues[v] = spot_da
+0001a400: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+0001a410: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+0001a420: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+0001a430: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
+0001a440: 6573 5b70 6f73 6978 5d20 3d20 726f 756e  es[posix] = roun
+0001a450: 6428 4c6f 6361 7469 6f6e 582c 3329 0d0a  d(LocationX,3)..
+0001a460: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+0001a470: 735b 706f 7369 795d 203d 2072 6f75 6e64  s[posiy] = round
+0001a480: 284c 6f63 6174 696f 6e59 2c33 290d 0a20  (LocationY,3).. 
+0001a490: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+0001a4a0: 5b70 6f73 697a 5d20 3d20 726f 756e 6428  [posiz] = round(
+0001a4b0: 4c6f 6361 7469 6f6e 5a2c 3329 0d0a 2020  LocationZ,3)..  
+0001a4c0: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001a4d0: 6672 616d 655d 203d 2072 6f75 6e64 284c  frame] = round(L
+0001a4e0: 6f63 6174 696f 6e54 2c33 290d 0a20 2020  ocationT,3)..   
+0001a4f0: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001a500: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0001a510: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+0001a520: 656e 6428 4174 7472 6962 7574 6542 6f78  end(AttributeBox
+0001a530: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
+0001a540: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
+0001a550: 2069 6e20 416c 6c56 616c 7565 732e 6b65   in AllValues.ke
+0001a560: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+0001a570: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001a580: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
+0001a590: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
+0001a5a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001a5b0: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+0001a5c0: 7572 6e20 4174 7472 6962 7574 6569 6473  urn Attributeids
+0001a5d0: 2c20 416c 6c56 616c 7565 7320 2020 2020  , AllValues     
+0001a5e0: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+0001a5f0: 7472 6163 6b5f 6461 7461 7365 7428 7472  track_dataset(tr
+0001a600: 6163 6b5f 6461 7461 7365 742c 2074 7261  ack_dataset, tra
+0001a610: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a620: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
+0001a630: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
+0001a640: 2c20 5472 6163 6b41 7474 7269 6275 7465  , TrackAttribute
+0001a650: 426f 786e 616d 6529 3a0d 0a0d 0a20 2020  Boxname):....   
+0001a660: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
+0001a670: 7565 7320 3d20 7b7d 0d0a 2020 2020 2020  ues = {}..      
+0001a680: 2020 7472 6163 6b5f 6964 203d 2074 7261    track_id = tra
+0001a690: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a6a0: 5f6b 6579 735b 2274 7261 636b 5f69 6422  _keys["track_id"
+0001a6b0: 5d0d 0a20 2020 2020 2020 2054 6964 203d  ]..        Tid =
+0001a6c0: 2074 7261 636b 5f64 6174 6173 6574 5b74   track_dataset[t
+0001a6d0: 7261 636b 5f69 645d 2e61 7374 7970 6528  rack_id].astype(
+0001a6e0: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+0001a6f0: 200d 0a20 2020 2020 2020 2041 6c6c 5472   ..        AllTr
+0001a700: 6163 6b56 616c 7565 735b 7472 6163 6b5f  ackValues[track_
+0001a710: 6964 5d20 3d20 5469 640d 0a20 2020 2020  id] = Tid..     
+0001a720: 200d 0a20 2020 2020 2020 2066 6f72 2028   ..        for (
+0001a730: 6b2c 2076 2920 696e 2074 7261 636b 5f61  k, v) in track_a
+0001a740: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+0001a750: 7973 2e69 7465 6d73 2829 3a0d 0a0d 0a20  ys.items():.... 
+0001a760: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001a770: 203d 2074 7261 636b 5f64 6174 6173 6574   = track_dataset
+0001a780: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001a790: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+0001a7a0: 2020 2020 206d 696e 7661 6c20 3d20 6d69       minval = mi
+0001a7b0: 6e28 7829 0d0a 2020 2020 2020 2020 2020  n(x)..          
+0001a7c0: 2020 2020 2020 6d61 7876 616c 203d 206d        maxval = m
+0001a7d0: 6178 2878 290d 0a0d 0a20 2020 2020 2020  ax(x)....       
+0001a7e0: 2020 2020 2020 2020 2069 6620 6d69 6e76           if minv
+0001a7f0: 616c 203e 2030 2061 6e64 206d 6178 7661  al > 0 and maxva
+0001a800: 6c20 3c3d 2031 3a0d 0a0d 0a20 2020 2020  l <= 1:....     
+0001a810: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001a820: 203d 2078 202b 2031 0d0a 0d0a 2020 2020   = x + 1....    
+0001a830: 2020 2020 2020 2020 2020 2020 416c 6c54              AllT
+0001a840: 7261 636b 5661 6c75 6573 5b6b 5d20 3d20  rackValues[k] = 
+0001a850: 726f 756e 6428 782c 2033 290d 0a0d 0a20  round(x, 3).... 
+0001a860: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
+0001a870: 6962 7574 6569 6473 203d 205b 5d0d 0a20  ibuteids = [].. 
+0001a880: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
+0001a890: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
+0001a8a0: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
+0001a8b0: 786e 616d 6529 0d0a 2020 2020 2020 2020  xname)..        
+0001a8c0: 666f 7220 6174 7472 6962 7574 656e 616d  for attributenam
+0001a8d0: 6520 696e 2074 7261 636b 5f61 6e61 6c79  e in track_analy
+0001a8e0: 7369 735f 7472 6163 6b5f 6b65 7973 2e6b  sis_track_keys.k
+0001a8f0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+0001a900: 2020 2020 5472 6163 6b41 7474 7269 6275      TrackAttribu
+0001a910: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
+0001a920: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
+0001a930: 0a20 2020 200d 0a20 2020 2020 2020 2072  .    ..        r
+0001a940: 6574 7572 6e20 5472 6163 6b41 7474 7269  eturn TrackAttri
+0001a950: 6275 7465 6964 732c 2041 6c6c 5472 6163  buteids, AllTrac
+0001a960: 6b56 616c 7565 730d 0a20 2020 200d 0a64  kValues..    ..d
+0001a970: 6566 2067 6574 5f65 6467 6573 5f64 6174  ef get_edges_dat
+0001a980: 6173 6574 2865 6467 6573 5f64 6174 6173  aset(edges_datas
+0001a990: 6574 2c20 6564 6765 735f 6461 7461 7365  et, edges_datase
+0001a9a0: 745f 696e 6465 782c 2074 7261 636b 5f61  t_index, track_a
+0001a9b0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001a9c0: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
+0001a9d0: 735f 6564 6765 735f 6b65 7973 293a 0d0a  s_edges_keys):..
+0001a9e0: 0d0a 2020 2020 2020 2020 416c 6c45 6467  ..        AllEdg
+0001a9f0: 6573 5661 6c75 6573 203d 207b 7d0d 0a20  esValues = {}.. 
+0001aa00: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+0001aa10: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+0001aa20: 5f73 706f 745f 6b65 7973 5b22 7472 6163  _spot_keys["trac
+0001aa30: 6b5f 6964 225d 0d0a 2020 2020 2020 2020  k_id"]..        
+0001aa40: 5469 6420 3d20 6564 6765 735f 6461 7461  Tid = edges_data
+0001aa50: 7365 745b 7472 6163 6b5f 6964 5d2e 6173  set[track_id].as
+0001aa60: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+0001aa70: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+0001aa80: 206e 702e 7768 6572 6528 5469 6420 3d3d   np.where(Tid ==
+0001aa90: 2030 290d 0a20 2020 2020 2020 206d 6178   0)..        max
+0001aaa0: 7472 6163 6b5f 6964 203d 206d 6178 2854  track_id = max(T
+0001aab0: 6964 290d 0a20 2020 2020 2020 2063 6f6e  id)..        con
+0001aac0: 6469 7469 6f6e 5f69 6e64 6963 6573 203d  dition_indices =
+0001aad0: 2065 6467 6573 5f64 6174 6173 6574 5f69   edges_dataset_i
+0001aae0: 6e64 6578 5b69 6e64 6963 6573 5d0d 0a20  ndex[indices].. 
+0001aaf0: 2020 2020 2020 2054 6964 5b63 6f6e 6469         Tid[condi
+0001ab00: 7469 6f6e 5f69 6e64 6963 6573 5d20 3d20  tion_indices] = 
+0001ab10: 6d61 7874 7261 636b 5f69 6420 2b20 310d  maxtrack_id + 1.
+0001ab20: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
+0001ab30: 7356 616c 7565 735b 7472 6163 6b5f 6964  sValues[track_id
+0001ab40: 5d20 3d20 5469 640d 0a0d 0a20 2020 2020  ] = Tid....     
+0001ab50: 2020 2066 6f72 206b 2069 6e20 7472 6163     for k in trac
+0001ab60: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+0001ab70: 5f6b 6579 732e 7661 6c75 6573 2829 3a0d  _keys.values():.
+0001ab80: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0001ab90: 6620 6b20 213d 2074 7261 636b 5f69 643a  f k != track_id:
+0001aba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001abb0: 2020 7820 3d20 6564 6765 735f 6461 7461    x = edges_data
+0001abc0: 7365 745b 6b5d 2e61 7374 7970 6528 2266  set[k].astype("f
+0001abd0: 6c6f 6174 2229 0d0a 0d0a 2020 2020 2020  loat")....      
+0001abe0: 2020 2020 2020 2020 2020 416c 6c45 6467            AllEdg
+0001abf0: 6573 5661 6c75 6573 5b6b 5d20 3d20 7820  esValues[k] = x 
+0001ac00: 2020 0d0a 2020 2020 2020 2020 200d 0a20    ..         .. 
+0001ac10: 2020 2020 2020 2072 6574 7572 6e20 416c         return Al
+0001ac20: 6c45 6467 6573 5661 6c75 6573 2020 200d  lEdgesValues   .
+0001ac30: 0a20 2020 200d 0a20 2020 2020 2020 0d0a  .    ..       ..
+0001ac40: 2020 2020 0d0a 6465 6620 7363 616c 655f      ..def scale_
+0001ac50: 7661 6c75 6528 782c 2073 6361 6c65 203d  value(x, scale =
+0001ac60: 2032 3535 202a 2032 3535 293a 0d0a 0d0a   255 * 255):....
+0001ac70: 0d0a 2020 2020 2072 6574 7572 6e20 7820  ..     return x 
+0001ac80: 2a20 7363 616c 6520 2020 0d0a 2020 2020  * scale   ..    
+0001ac90: 0d0a 0d0a 0d0a 6465 6620 7072 6f62 5f73  ......def prob_s
+0001aca0: 6967 6d6f 6964 2878 293a 0d0a 2020 2020  igmoid(x):..    
+0001acb0: 7265 7475 726e 2031 202d 206d 6174 682e  return 1 - math.
+0001acc0: 6578 7028 2d78 290d 0a0d 0a0d 0a64 6566  exp(-x)......def
+0001acd0: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+0001ace0: 7665 635f 302c 2076 6563 5f31 293a 0d0a  vec_0, vec_1):..
+0001acf0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001ad00: 2020 7665 635f 3020 3d20 7665 635f 3020    vec_0 = vec_0 
+0001ad10: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
+0001ad20: 2876 6563 5f30 290d 0a20 2020 2020 2020  (vec_0)..       
+0001ad30: 2076 6563 5f31 203d 2076 6563 5f31 202f   vec_1 = vec_1 /
+0001ad40: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
+0001ad50: 7665 635f 3129 0d0a 2020 2020 2020 2020  vec_1)..        
+0001ad60: 616e 676c 6520 3d20 6e70 2e61 7263 636f  angle = np.arcco
+0001ad70: 7328 6e70 2e63 6c69 7028 6e70 2e64 6f74  s(np.clip(np.dot
+0001ad80: 2876 6563 5f30 2c20 7665 635f 3129 2c20  (vec_0, vec_1), 
+0001ad90: 2d31 2e30 2c20 312e 3029 290d 0a20 2020  -1.0, 1.0))..   
+0001ada0: 2020 2020 2061 6e67 6c65 203d 2061 6e67       angle = ang
+0001adb0: 6c65 202a 2031 3830 202f 206e 702e 7069  le * 180 / np.pi
+0001adc0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001add0: 2061 6e67 6c65 0d0a 2020 2020 200d 0a0d   angle..     ...
+0001ade0: 0a64 6566 2065 7661 6c5f 626f 6f6c 2876  .def eval_bool(v
+0001adf0: 616c 7565 293a 0d0a 2020 2020 2020 2020  alue):..        
+0001ae00: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001ae10: 2020 2020 6966 2076 616c 7565 2020 3d3d      if value  ==
+0001ae20: 2027 5472 7565 273a 200d 0a20 2020 2020   'True': ..     
+0001ae30: 2020 2020 2020 2020 2020 2064 6976 5f6b             div_k
+0001ae40: 6579 203d 2054 7275 650d 0a20 2020 2020  ey = True..     
+0001ae50: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0001ae60: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
+0001ae70: 7920 3d20 4661 6c73 6520 0d0a 0d0a 2020  y = False ....  
+0001ae80: 2020 2020 2020 7265 7475 726e 2064 6976        return div
+0001ae90: 5f6b 6579 2020 2020 2020 2020 2020 2020  _key            
+0001aea0: 2020 2020 0d0a 0d0a 6465 6620 6368 6563      ....def chec
+0001aeb0: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
+0001aec0: 6b28 6d61 736b 2c69 6d61 6765 293a 0d0a  k(mask,image):..
+0001aed0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001aee0: 2069 6620 6c65 6e28 6d61 736b 2e73 6861   if len(mask.sha
+0001aef0: 7065 2920 3c20 6c65 6e28 696d 6167 652e  pe) < len(image.
+0001af00: 7368 6170 6529 3a0d 0a20 2020 2020 2020  shape):..       
+0001af10: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
+0001af20: 203d 206e 702e 7a65 726f 7328 0d0a 2020   = np.zeros(..  
+0001af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af40: 2020 2020 2020 2020 2020 5b0d 0a20 2020            [..   
+0001af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af60: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001af70: 6765 2e73 6861 7065 5b30 5d2c 0d0a 2020  ge.shape[0],..  
+0001af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af90: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0001afa0: 6167 652e 7368 6170 655b 315d 2c0d 0a20  age.shape[1],.. 
+0001afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001afd0: 6d61 6765 2e73 6861 7065 5b32 5d2c 0d0a  mage.shape[2],..
+0001afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b000: 696d 6167 652e 7368 6170 655b 335d 2c0d  image.shape[3],.
+0001b010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b020: 2020 2020 2020 2020 2020 2020 205d 2c20               ], 
+0001b030: 6474 7970 653d 2275 696e 7438 220d 0a20  dtype="uint8".. 
+0001b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b050: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001b060: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0001b070: 616e 6765 2830 2c20 7570 6461 7465 5f6d  ange(0, update_m
+0001b080: 6173 6b2e 7368 6170 655b 305d 293a 0d0a  ask.shape[0]):..
+0001b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0a0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+0001b0b0: 2c20 7570 6461 7465 5f6d 6173 6b2e 7368  , update_mask.sh
+0001b0c0: 6170 655b 315d 293a 0d0a 0d0a 2020 2020  ape[1]):....    
+0001b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0e0: 7570 6461 7465 5f6d 6173 6b5b 692c 206a  update_mask[i, j
+0001b0f0: 2c20 3a2c 203a 5d20 3d20 6d61 736b 5b69  , :, :] = mask[i
+0001b100: 2c20 3a2c 203a 5d0d 0a20 2020 2020 2020  , :, :]..       
+0001b110: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0001b120: 2020 2020 2020 2020 7570 6461 7465 5f6d          update_m
+0001b130: 6173 6b20 3d20 6d61 736b 0d0a 0d0a 2020  ask = mask....  
+0001b140: 2020 2020 2020 7265 7475 726e 2075 7064        return upd
+0001b150: 6174 655f 6d61 736b 2020 2020 2020 2020  ate_mask        
+0001b160: 0d0a 2020 2020 2020 200d 0a              ..       ..
```

### Comparing `napatrackmater-3.8.3/napatrackmater/Trackvector.py` & `napatrackmater-3.8.4/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater/__init__.py` & `napatrackmater-3.8.4/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater/clustering.py` & `napatrackmater-3.8.4/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.8.4/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater/fate_mapping.py` & `napatrackmater-3.8.4/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater/pretrained.py` & `napatrackmater-3.8.4/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.8.4/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.3
+Version: 3.8.4
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.8.3/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.8.4/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.3/setup.py` & `napatrackmater-3.8.4/setup.py`

 * *Files identical despite different names*

