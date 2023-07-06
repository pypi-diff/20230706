# Comparing `tmp/napatrackmater-3.8.1.tar.gz` & `tmp/napatrackmater-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.8.1.tar", last modified: Mon Jul  3 18:01:07 2023, max compression
+gzip compressed data, was "napatrackmater-3.8.2.tar", last modified: Thu Jul  6 07:51:15 2023, max compression
```

## Comparing `napatrackmater-3.8.1.tar` & `napatrackmater-3.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 18:01:07.906640 napatrackmater-3.8.1/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.1/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-03 18:01:07.901640 napatrackmater-3.8.1/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.1/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 18:01:07.709174 napatrackmater-3.8.1/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.1/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.1/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   108116 2023-07-03 17:00:55.000000 napatrackmater-3.8.1/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.1/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.1/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-06-15 20:51:11.000000 napatrackmater-3.8.1/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.1/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.1/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.1/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-03 18:00:32.000000 napatrackmater-3.8.1/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 18:01:07.871442 napatrackmater-3.8.1/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-03 18:01:07.000000 napatrackmater-3.8.1/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-03 18:01:07.000000 napatrackmater-3.8.1/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-03 18:01:07.000000 napatrackmater-3.8.1/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-03 18:01:07.000000 napatrackmater-3.8.1/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-03 18:01:07.000000 napatrackmater-3.8.1/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-03 18:01:07.000000 napatrackmater-3.8.1/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-03 18:01:07.907640 napatrackmater-3.8.1/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.1/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 07:51:15.360526 napatrackmater-3.8.2/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.2/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-06 07:51:15.357297 napatrackmater-3.8.2/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.2/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 07:51:15.165947 napatrackmater-3.8.2/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.2/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.2/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110477 2023-07-06 07:43:11.000000 napatrackmater-3.8.2/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.2/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.2/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    14327 2023-07-03 20:00:06.000000 napatrackmater-3.8.2/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.2/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.2/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.2/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-06 07:50:45.000000 napatrackmater-3.8.2/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-06 07:51:15.325229 napatrackmater-3.8.2/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-06 07:51:14.000000 napatrackmater-3.8.2/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-06 07:51:14.000000 napatrackmater-3.8.2/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-06 07:51:14.000000 napatrackmater-3.8.2/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-06 07:51:14.000000 napatrackmater-3.8.2/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-06 07:51:14.000000 napatrackmater-3.8.2/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-06 07:51:14.000000 napatrackmater-3.8.2/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-06 07:51:15.362526 napatrackmater-3.8.2/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.2/setup.py
```

### Comparing `napatrackmater-3.8.1/LICENSE` & `napatrackmater-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/PKG-INFO` & `napatrackmater-3.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.1
+Version: 3.8.2
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.8.1/README.md` & `napatrackmater-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.8.2/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.8.2/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/napatrackmater/Trackmate.py` & `napatrackmater-3.8.2/napatrackmater/Trackmate.py`

 * *Files 2% similar despite different names*

```diff
@@ -960,5799 +960,5946 @@
 00003bf0: 736f 7572 6365 5f69 6473 2e61 7070 656e  source_ids.appen
 00003c00: 6428 736f 7572 6365 5f69 6429 0d0a 2020  d(source_id)..  
 00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003c20: 2020 2020 2020 2020 2020 616c 6c5f 7461            all_ta
 00003c30: 7267 6574 5f69 6473 2e61 7070 656e 6428  rget_ids.append(
 00003c40: 7461 7267 6574 5f69 6429 0d0a 2020 2020  target_id)..    
 00003c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c60: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c80: 2020 2020 2020 6966 2073 6f75 7263 655f        if source_
-00003c90: 6964 2069 6e20 7365 6c66 2e65 6467 655f  id in self.edge_
-00003ca0: 7461 7267 6574 5f6c 6f6f 6b75 702e 6b65  target_lookup.ke
-00003cb0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cd0: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
-00003ce0: 7461 7267 6574 5f6c 6f6f 6b75 705b 736f  target_lookup[so
-00003cf0: 7572 6365 5f69 645d 2e61 7070 656e 6428  urce_id].append(
-00003d00: 7461 7267 6574 5f69 6429 0d0a 2020 2020  target_id)..    
-00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d20: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
-00003d30: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d50: 2020 2020 7365 6c66 2e65 6467 655f 7461      self.edge_ta
-00003d60: 7267 6574 5f6c 6f6f 6b75 705b 736f 7572  rget_lookup[sour
-00003d70: 6365 5f69 645d 203d 205b 7461 7267 6574  ce_id] = [target
-00003d80: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2020 7365 6c66 2e65 6467 655f 736f 7572    self.edge_sour
-00003db0: 6365 5f6c 6f6f 6b75 705b 7461 7267 6574  ce_lookup[target
-00003dc0: 5f69 645d 203d 2073 6f75 7263 655f 6964  _id] = source_id
-00003dd0: 200d 0a0d 0a20 2020 2020 2020 2072 6574   ....        ret
-00003de0: 7572 6e20 616c 6c5f 736f 7572 6365 5f69  urn all_source_i
-00003df0: 6473 2c20 616c 6c5f 7461 7267 6574 5f69  ds, all_target_i
-00003e00: 6473 200d 0a0d 0a0d 0a20 2020 2064 6566  ds ......    def
-00003e10: 205f 6372 6561 7465 5f67 656e 6572 6174   _create_generat
-00003e20: 696f 6e73 2873 656c 662c 2061 6c6c 5f73  ions(self, all_s
-00003e30: 6f75 7263 655f 6964 732c 2061 6c6c 5f74  ource_ids, all_t
-00003e40: 6172 6765 745f 6964 7329 3a0d 0a20 2020  arget_ids):..   
-00003e50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00003e60: 726f 6f74 5f6c 6561 6620 3d20 5b5d 0d0a  root_leaf = []..
-00003e70: 2020 2020 2020 2020 726f 6f74 5f72 6f6f          root_roo
-00003e80: 7420 3d20 5b5d 0d0a 2020 2020 2020 2020  t = []..        
-00003e90: 726f 6f74 5f73 706c 6974 7320 3d20 5b5d  root_splits = []
-00003ea0: 0d0a 2020 2020 2020 2020 7370 6c69 745f  ..        split_
-00003eb0: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
-00003ec0: 2020 2023 4765 7420 7468 6520 726f 6f74     #Get the root
-00003ed0: 2069 640d 0a20 2020 2020 2020 2066 6f72   id..        for
-00003ee0: 2073 6f75 7263 655f 6964 2069 6e20 616c   source_id in al
-00003ef0: 6c5f 736f 7572 6365 5f69 6473 3a0d 0a20  l_source_ids:.. 
-00003f00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00003f10: 736f 7572 6365 5f69 6420 6e6f 7420 696e  source_id not in
-00003f20: 2061 6c6c 5f74 6172 6765 745f 6964 733a   all_target_ids:
-00003f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003f40: 2020 2020 2072 6f6f 745f 726f 6f74 2e61       root_root.a
-00003f50: 7070 656e 6428 736f 7572 6365 5f69 6429  ppend(source_id)
-00003f60: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00003f70: 2020 2020 2020 0d0a 2020 2020 2020 200d        ..       .
-00003f80: 0a20 2020 2020 2020 2023 4765 7420 7468  .        #Get th
-00003f90: 6520 6c65 6166 7320 616e 6420 7370 6c69  e leafs and spli
-00003fa0: 7473 2020 2020 200d 0a20 2020 2020 2020  ts     ..       
-00003fb0: 2066 6f72 2074 6172 6765 745f 6964 2069   for target_id i
-00003fc0: 6e20 616c 6c5f 7461 7267 6574 5f69 6473  n all_target_ids
-00003fd0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003fe0: 0d0a 2020 2020 2020 2020 2020 2020 2069  ..             i
-00003ff0: 6620 7461 7267 6574 5f69 6420 6e6f 7420  f target_id not 
-00004000: 696e 2061 6c6c 5f73 6f75 7263 655f 6964  in all_source_id
-00004010: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00004020: 2020 2020 2020 726f 6f74 5f6c 6561 662e        root_leaf.
-00004030: 6170 7065 6e64 2874 6172 6765 745f 6964  append(target_id
-00004040: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004050: 7370 6c69 745f 636f 756e 7420 3d20 616c  split_count = al
-00004060: 6c5f 736f 7572 6365 5f69 6473 2e63 6f75  l_source_ids.cou
-00004070: 6e74 2874 6172 6765 745f 6964 290d 0a20  nt(target_id).. 
-00004080: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00004090: 706c 6974 5f63 6f75 6e74 203e 2031 3a0d  plit_count > 1:.
-000040a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000040b0: 2020 2020 2020 2072 6f6f 745f 7370 6c69         root_spli
-000040c0: 7473 2e61 7070 656e 6428 7461 7267 6574  ts.append(target
-000040d0: 5f69 6429 0d0a 0d0a 0d0a 2020 2020 2020  _id)......      
-000040e0: 2020 7265 7475 726e 2072 6f6f 745f 726f    return root_ro
-000040f0: 6f74 2c20 726f 6f74 5f73 706c 6974 732c  ot, root_splits,
-00004100: 2072 6f6f 745f 6c65 6166 0d0a 0d0a 2020   root_leaf....  
-00004110: 2020 6465 6620 5f73 6f72 745f 6469 7669    def _sort_divi
-00004120: 6469 6e67 5f63 656c 6c73 2873 656c 662c  ding_cells(self,
-00004130: 2072 6f6f 745f 7370 6c69 7473 293a 0d0a   root_splits):..
-00004140: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-00004150: 6964 5f74 696d 6573 203d 205b 5d0d 0a20  id_times = [].. 
-00004160: 2020 2020 2020 2020 2020 6365 6c6c 5f69            cell_i
-00004170: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-00004180: 2020 2020 666f 7220 726f 6f74 5f73 706c      for root_spl
-00004190: 6974 2069 6e20 726f 6f74 5f73 706c 6974  it in root_split
-000041a0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000041b0: 2020 2020 2020 7370 6c69 745f 6365 6c6c        split_cell
-000041c0: 5f69 645f 7469 6d65 203d 2073 656c 662e  _id_time = self.
-000041d0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000041e0: 6572 7469 6573 5b72 6f6f 745f 7370 6c69  erties[root_spli
-000041f0: 745d 5b73 656c 662e 6672 616d 6569 645f  t][self.frameid_
-00004200: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
-00004210: 2020 2020 2020 2020 6365 6c6c 5f69 645f          cell_id_
-00004220: 7469 6d65 732e 6170 7065 6e64 2873 706c  times.append(spl
-00004230: 6974 5f63 656c 6c5f 6964 5f74 696d 6529  it_cell_id_time)
-00004240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004250: 2020 2020 6365 6c6c 5f69 6473 2e61 7070      cell_ids.app
-00004260: 656e 6428 726f 6f74 5f73 706c 6974 290d  end(root_split).
-00004270: 0a20 2020 2020 2020 2020 2020 736f 7274  .           sort
-00004280: 6564 5f69 6e64 6963 6573 203d 2073 6f72  ed_indices = sor
-00004290: 7465 6428 7261 6e67 6528 6c65 6e28 6365  ted(range(len(ce
-000042a0: 6c6c 5f69 645f 7469 6d65 7329 292c 206b  ll_id_times)), k
-000042b0: 6579 3d6c 616d 6264 6120 6b3a 2063 656c  ey=lambda k: cel
-000042c0: 6c5f 6964 5f74 696d 6573 5b6b 5d29 0d0a  l_id_times[k])..
-000042d0: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-000042e0: 645f 6365 6c6c 5f69 6473 203d 205b 6365  d_cell_ids = [ce
-000042f0: 6c6c 5f69 6473 5b69 5d20 666f 7220 6920  ll_ids[i] for i 
-00004300: 696e 2073 6f72 7465 645f 696e 6469 6365  in sorted_indice
-00004310: 735d 0d0a 0d0a 2020 2020 2020 2020 2020  s]....          
-00004320: 2072 6574 7572 6e20 736f 7274 6564 5f63   return sorted_c
-00004330: 656c 6c5f 6964 7320 2020 2020 2020 0d0a  ell_ids       ..
-00004340: 0d0a 2020 2020 6465 6620 5f69 7465 7261  ..    def _itera
-00004350: 7465 5f73 706c 6974 5f64 6f77 6e28 7365  te_split_down(se
-00004360: 6c66 2c20 726f 6f74 5f72 6f6f 742c 2072  lf, root_root, r
-00004370: 6f6f 745f 6c65 6166 2c20 726f 6f74 5f73  oot_leaf, root_s
-00004380: 706c 6974 7329 3a0d 0a20 2020 2020 2020  plits):..       
-00004390: 2020 0d0a 2020 2020 2020 2020 736f 7274    ..        sort
-000043a0: 6564 5f72 6f6f 745f 7370 6c69 7473 203d  ed_root_splits =
-000043b0: 2073 656c 662e 5f73 6f72 745f 6469 7669   self._sort_divi
-000043c0: 6469 6e67 5f63 656c 6c73 2872 6f6f 745f  ding_cells(root_
-000043d0: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
-000043e0: 2067 656e 5f63 6f75 6e74 203d 2030 0d0a   gen_count = 0..
-000043f0: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-00004400: 5f63 6f75 6e74 203d 2030 0d0a 2020 2020  _count = 0..    
-00004410: 2020 2020 666f 7220 726f 6f74 5f61 6c6c      for root_all
-00004420: 2069 6e20 726f 6f74 5f72 6f6f 743a 0d0a   in root_root:..
-00004430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004440: 7365 6c66 2e67 656e 6572 6174 696f 6e5f  self.generation_
-00004450: 6469 6374 5b72 6f6f 745f 616c 6c5d 203d  dict[root_all] =
-00004460: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
-00004470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004480: 2e74 7261 636b 6c65 745f 6469 6374 5b72  .tracklet_dict[r
-00004490: 6f6f 745f 616c 6c5d 203d 2074 7261 636b  oot_all] = track
-000044a0: 6c65 745f 636f 756e 740d 0a20 2020 2020  let_count..     
-000044b0: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
-000044c0: 6f74 5f61 6c6c 2069 6e20 7365 6c66 2e65  ot_all in self.e
-000044d0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-000044e0: 7020 616e 6420 726f 6f74 5f61 6c6c 206e  p and root_all n
-000044f0: 6f74 2069 6e20 736f 7274 6564 5f72 6f6f  ot in sorted_roo
-00004500: 745f 7370 6c69 7473 3a0d 0a20 2020 2020  t_splits:..     
+00003c60: 2020 2020 2020 2020 6966 2073 6f75 7263          if sourc
+00003c70: 655f 6964 2069 6e20 7365 6c66 2e65 6467  e_id in self.edg
+00003c80: 655f 7461 7267 6574 5f6c 6f6f 6b75 702e  e_target_lookup.
+00003c90: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
+00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cb0: 2020 2020 2020 2020 7365 6c66 2e65 6467          self.edg
+00003cc0: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
+00003cd0: 736f 7572 6365 5f69 645d 2e61 7070 656e  source_id].appen
+00003ce0: 6428 7461 7267 6574 5f69 6429 0d0a 2020  d(target_id)..  
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d00: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
+00003d10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00003d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d30: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
+00003d40: 7461 7267 6574 5f6c 6f6f 6b75 705b 736f  target_lookup[so
+00003d50: 7572 6365 5f69 645d 203d 205b 7461 7267  urce_id] = [targ
+00003d60: 6574 5f69 645d 0d0a 2020 2020 2020 2020  et_id]..        
+00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d80: 2020 2020 7365 6c66 2e65 6467 655f 736f      self.edge_so
+00003d90: 7572 6365 5f6c 6f6f 6b75 705b 7461 7267  urce_lookup[targ
+00003da0: 6574 5f69 645d 203d 2073 6f75 7263 655f  et_id] = source_
+00003db0: 6964 200d 0a0d 0a20 2020 2020 2020 2072  id ....        r
+00003dc0: 6574 7572 6e20 616c 6c5f 736f 7572 6365  eturn all_source
+00003dd0: 5f69 6473 2c20 616c 6c5f 7461 7267 6574  _ids, all_target
+00003de0: 5f69 6473 200d 0a0d 0a0d 0a20 2020 2064  _ids ......    d
+00003df0: 6566 205f 6372 6561 7465 5f67 656e 6572  ef _create_gener
+00003e00: 6174 696f 6e73 2873 656c 662c 2061 6c6c  ations(self, all
+00003e10: 5f73 6f75 7263 655f 6964 732c 2061 6c6c  _source_ids, all
+00003e20: 5f74 6172 6765 745f 6964 7329 3a0d 0a20  _target_ids):.. 
+00003e30: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003e40: 2020 726f 6f74 5f6c 6561 6620 3d20 5b5d    root_leaf = []
+00003e50: 0d0a 2020 2020 2020 2020 726f 6f74 5f72  ..        root_r
+00003e60: 6f6f 7420 3d20 5b5d 0d0a 2020 2020 2020  oot = []..      
+00003e70: 2020 726f 6f74 5f73 706c 6974 7320 3d20    root_splits = 
+00003e80: 5b5d 0d0a 2020 2020 2020 2020 7370 6c69  []..        spli
+00003e90: 745f 636f 756e 7420 3d20 300d 0a20 2020  t_count = 0..   
+00003ea0: 2020 2020 2023 4765 7420 7468 6520 726f       #Get the ro
+00003eb0: 6f74 2069 640d 0a20 2020 2020 2020 2066  ot id..        f
+00003ec0: 6f72 2073 6f75 7263 655f 6964 2069 6e20  or source_id in 
+00003ed0: 616c 6c5f 736f 7572 6365 5f69 6473 3a0d  all_source_ids:.
+00003ee0: 0a20 2020 2020 2020 2020 2020 2020 2069  .              i
+00003ef0: 6620 736f 7572 6365 5f69 6420 6e6f 7420  f source_id not 
+00003f00: 696e 2061 6c6c 5f74 6172 6765 745f 6964  in all_target_id
+00003f10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00003f20: 2020 2020 2020 2072 6f6f 745f 726f 6f74         root_root
+00003f30: 2e61 7070 656e 6428 736f 7572 6365 5f69  .append(source_i
+00003f40: 6429 200d 0a20 2020 2020 2020 2020 2020  d) ..           
+00003f50: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003f60: 200d 0a20 2020 2020 2020 2023 4765 7420   ..        #Get 
+00003f70: 7468 6520 6c65 6166 7320 616e 6420 7370  the leafs and sp
+00003f80: 6c69 7473 2020 2020 200d 0a20 2020 2020  lits     ..     
+00003f90: 2020 2066 6f72 2074 6172 6765 745f 6964     for target_id
+00003fa0: 2069 6e20 616c 6c5f 7461 7267 6574 5f69   in all_target_i
+00003fb0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00003fc0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00003fd0: 2069 6620 7461 7267 6574 5f69 6420 6e6f   if target_id no
+00003fe0: 7420 696e 2061 6c6c 5f73 6f75 7263 655f  t in all_source_
+00003ff0: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+00004000: 2020 2020 2020 2020 726f 6f74 5f6c 6561          root_lea
+00004010: 662e 6170 7065 6e64 2874 6172 6765 745f  f.append(target_
+00004020: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
+00004030: 2020 7370 6c69 745f 636f 756e 7420 3d20    split_count = 
+00004040: 616c 6c5f 736f 7572 6365 5f69 6473 2e63  all_source_ids.c
+00004050: 6f75 6e74 2874 6172 6765 745f 6964 290d  ount(target_id).
+00004060: 0a20 2020 2020 2020 2020 2020 2020 6966  .             if
+00004070: 2073 706c 6974 5f63 6f75 6e74 203e 2031   split_count > 1
+00004080: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004090: 2020 2020 2020 2020 2072 6f6f 745f 7370           root_sp
+000040a0: 6c69 7473 2e61 7070 656e 6428 7461 7267  lits.append(targ
+000040b0: 6574 5f69 6429 0d0a 0d0a 0d0a 2020 2020  et_id)......    
+000040c0: 2020 2020 7265 7475 726e 2072 6f6f 745f      return root_
+000040d0: 726f 6f74 2c20 726f 6f74 5f73 706c 6974  root, root_split
+000040e0: 732c 2072 6f6f 745f 6c65 6166 0d0a 0d0a  s, root_leaf....
+000040f0: 2020 2020 6465 6620 5f73 6f72 745f 6469      def _sort_di
+00004100: 7669 6469 6e67 5f63 656c 6c73 2873 656c  viding_cells(sel
+00004110: 662c 2072 6f6f 745f 7370 6c69 7473 293a  f, root_splits):
+00004120: 0d0a 2020 2020 2020 2020 2020 2063 656c  ..           cel
+00004130: 6c5f 6964 5f74 696d 6573 203d 205b 5d0d  l_id_times = [].
+00004140: 0a20 2020 2020 2020 2020 2020 6365 6c6c  .           cell
+00004150: 5f69 6473 203d 205b 5d0d 0a20 2020 2020  _ids = []..     
+00004160: 2020 2020 2020 666f 7220 726f 6f74 5f73        for root_s
+00004170: 706c 6974 2069 6e20 726f 6f74 5f73 706c  plit in root_spl
+00004180: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
+00004190: 2020 2020 2020 2020 7370 6c69 745f 6365          split_ce
+000041a0: 6c6c 5f69 645f 7469 6d65 203d 2073 656c  ll_id_time = sel
+000041b0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000041c0: 6f70 6572 7469 6573 5b72 6f6f 745f 7370  operties[root_sp
+000041d0: 6c69 745d 5b73 656c 662e 6672 616d 6569  lit][self.framei
+000041e0: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
+000041f0: 2020 2020 2020 2020 2020 6365 6c6c 5f69            cell_i
+00004200: 645f 7469 6d65 732e 6170 7065 6e64 2873  d_times.append(s
+00004210: 706c 6974 5f63 656c 6c5f 6964 5f74 696d  plit_cell_id_tim
+00004220: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00004230: 2020 2020 2020 6365 6c6c 5f69 6473 2e61        cell_ids.a
+00004240: 7070 656e 6428 726f 6f74 5f73 706c 6974  ppend(root_split
+00004250: 290d 0a20 2020 2020 2020 2020 2020 736f  )..           so
+00004260: 7274 6564 5f69 6e64 6963 6573 203d 2073  rted_indices = s
+00004270: 6f72 7465 6428 7261 6e67 6528 6c65 6e28  orted(range(len(
+00004280: 6365 6c6c 5f69 645f 7469 6d65 7329 292c  cell_id_times)),
+00004290: 206b 6579 3d6c 616d 6264 6120 6b3a 2063   key=lambda k: c
+000042a0: 656c 6c5f 6964 5f74 696d 6573 5b6b 5d29  ell_id_times[k])
+000042b0: 0d0a 2020 2020 2020 2020 2020 2073 6f72  ..           sor
+000042c0: 7465 645f 6365 6c6c 5f69 6473 203d 205b  ted_cell_ids = [
+000042d0: 6365 6c6c 5f69 6473 5b69 5d20 666f 7220  cell_ids[i] for 
+000042e0: 6920 696e 2073 6f72 7465 645f 696e 6469  i in sorted_indi
+000042f0: 6365 735d 0d0a 0d0a 2020 2020 2020 2020  ces]....        
+00004300: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+00004310: 5f63 656c 6c5f 6964 7320 2020 2020 2020  _cell_ids       
+00004320: 0d0a 0d0a 2020 2020 6465 6620 5f69 7465  ....    def _ite
+00004330: 7261 7465 5f6e 6f6e 5f64 6976 6964 696e  rate_non_dividin
+00004340: 6728 7365 6c66 2c20 726f 6f74 5f72 6f6f  g(self, root_roo
+00004350: 742c 2072 6f6f 745f 6c65 6166 293a 0d0a  t, root_leaf):..
+00004360: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00004370: 2020 2020 2020 2020 2020 2067 656e 5f63             gen_c
+00004380: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+00004390: 2020 2020 2020 7472 6163 6b6c 6574 5f63        tracklet_c
+000043a0: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+000043b0: 2020 2020 2020 666f 7220 726f 6f74 5f61        for root_a
+000043c0: 6c6c 2069 6e20 726f 6f74 5f72 6f6f 743a  ll in root_root:
+000043d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000043e0: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
+000043f0: 6174 696f 6e5f 6469 6374 5b72 6f6f 745f  ation_dict[root_
+00004400: 616c 6c5d 203d 2067 656e 5f63 6f75 6e74  all] = gen_count
+00004410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004420: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+00004430: 6c65 745f 6469 6374 5b72 6f6f 745f 616c  let_dict[root_al
+00004440: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
+00004450: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+00004460: 2020 2020 2020 2020 2069 6620 726f 6f74           if root
+00004470: 5f61 6c6c 2069 6e20 7365 6c66 2e65 6467  _all in self.edg
+00004480: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
+00004490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000044a0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+000044b0: 745f 6365 6c6c 203d 2073 656c 662e 6564  t_cell = self.ed
+000044c0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+000044d0: 5b72 6f6f 745f 616c 6c5d 5b30 5d0d 0a20  [root_all][0].. 
+000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044f0: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
+00004500: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
 00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004520: 7461 7267 6574 5f63 656c 6c73 203d 2073  target_cells = s
-00004530: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-00004540: 6c6f 6f6b 7570 5b72 6f6f 745f 616c 6c5d  lookup[root_all]
-00004550: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-00004560: 2020 2020 2020 2020 2020 7768 696c 6520            while 
-00004570: 7461 7267 6574 5f63 656c 6c73 206e 6f74  target_cells not
-00004580: 2069 6e20 736f 7274 6564 5f72 6f6f 745f   in sorted_root_
-00004590: 7370 6c69 7473 3a0d 0a20 2020 2020 2020  splits:..       
-000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045b0: 2020 2020 2073 656c 662e 6765 6e65 7261       self.genera
-000045c0: 7469 6f6e 5f64 6963 745b 7461 7267 6574  tion_dict[target
-000045d0: 5f63 656c 6c73 5d20 3d20 6765 6e5f 636f  _cells] = gen_co
-000045e0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004600: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
-00004610: 6963 745b 7461 7267 6574 5f63 656c 6c73  ict[target_cells
-00004620: 5d20 3d20 7472 6163 6b6c 6574 5f63 6f75  ] = tracklet_cou
-00004630: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00004640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004650: 6966 2074 6172 6765 745f 6365 6c6c 7320  if target_cells 
-00004660: 696e 2073 656c 662e 6564 6765 5f74 6172  in self.edge_tar
-00004670: 6765 745f 6c6f 6f6b 7570 3a0d 0a20 2020  get_lookup:..   
-00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004690: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-000046a0: 6765 745f 6365 6c6c 7320 3d20 7365 6c66  get_cells = self
-000046b0: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-000046c0: 6b75 705b 7461 7267 6574 5f63 656c 6c73  kup[target_cells
-000046d0: 5d5b 305d 0d0a 2020 2020 2020 2020 2020  ][0]..          
-000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2020 2020 6966 2074 6172 6765 745f        if target_
-00004700: 6365 6c6c 7320 696e 2072 6f6f 745f 6c65  cells in root_le
-00004710: 6166 3a0d 0a20 2020 2020 2020 2020 2020  af:..           
-00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-00004740: 6e65 7261 7469 6f6e 5f64 6963 745b 7461  neration_dict[ta
-00004750: 7267 6574 5f63 656c 6c73 5d20 3d20 6765  rget_cells] = ge
-00004760: 6e5f 636f 756e 740d 0a20 2020 2020 2020  n_count..       
-00004770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004780: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00004790: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
-000047a0: 7461 7267 6574 5f63 656c 6c73 5d20 3d20  target_cells] = 
-000047b0: 7472 6163 6b6c 6574 5f63 6f75 6e74 0d0a  tracklet_count..
-000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047e0: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 2062 7265 616b 2020 2020 0d0a 2020 2020   break    ..    
-00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 200d 0a20 2020 2020 2020 2066 6f72 2072   ..        for r
-00004860: 6f6f 745f 7370 6c69 7420 696e 2073 6f72  oot_split in sor
-00004870: 7465 645f 726f 6f74 5f73 706c 6974 733a  ted_root_splits:
-00004880: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00004890: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
-000048a0: 6374 5b72 6f6f 745f 7370 6c69 745d 203d  ct[root_split] =
-000048b0: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
-000048c0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-000048d0: 636b 6c65 745f 6469 6374 5b72 6f6f 745f  cklet_dict[root_
-000048e0: 7370 6c69 745d 203d 2074 7261 636b 6c65  split] = trackle
-000048f0: 745f 636f 756e 740d 0a20 2020 2020 2020  t_count..       
-00004900: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
-00004910: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
-00004920: 7267 6574 5f6c 6f6f 6b75 705b 726f 6f74  rget_lookup[root
-00004930: 5f73 706c 6974 5d0d 0a20 2020 2020 2020  _split]..       
-00004940: 2020 2020 2067 656e 5f63 6f75 6e74 202b       gen_count +
-00004950: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
-00004960: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00004970: 6c65 6e28 7461 7267 6574 5f63 656c 6c73  len(target_cells
-00004980: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00004990: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-000049a0: 5f63 6f75 6e74 202b 3d20 310d 0a20 2020  _count += 1..   
-000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049c0: 7461 7267 6574 5f63 656c 6c5f 6964 203d  target_cell_id =
-000049d0: 2074 6172 6765 745f 6365 6c6c 735b 695d   target_cells[i]
-000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00004a00: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-00004a10: 6e65 7261 7469 6f6e 5f64 6963 745b 7461  neration_dict[ta
-00004a20: 7267 6574 5f63 656c 6c5f 6964 5d20 3d20  rget_cell_id] = 
-00004a30: 6765 6e5f 636f 756e 740d 0a20 2020 2020  gen_count..     
-00004a40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004a50: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
-00004a60: 5b74 6172 6765 745f 6365 6c6c 5f69 645d  [target_cell_id]
-00004a70: 203d 2074 7261 636b 6c65 745f 636f 756e   = tracklet_coun
-00004a80: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-00004a90: 2020 2020 2020 7768 696c 6520 7461 7267        while targ
-00004aa0: 6574 5f63 656c 6c5f 6964 206e 6f74 2069  et_cell_id not i
-00004ab0: 6e20 736f 7274 6564 5f72 6f6f 745f 7370  n sorted_root_sp
-00004ac0: 6c69 7473 3a0d 0a20 2020 2020 2020 2020  lits:..         
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ae0: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
-00004af0: 6c5f 6964 2069 6e20 7365 6c66 2e65 6467  l_id in self.edg
-00004b00: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
-00004b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b30: 2020 7461 7267 6574 5f63 656c 6c5f 6964    target_cell_id
-00004b40: 203d 2073 656c 662e 6564 6765 5f74 6172   = self.edge_tar
-00004b50: 6765 745f 6c6f 6f6b 7570 5b74 6172 6765  get_lookup[targe
-00004b60: 745f 6365 6c6c 5f69 645d 5b30 5d0d 0a20  t_cell_id][0].. 
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004b90: 656c 662e 6765 6e65 7261 7469 6f6e 5f64  elf.generation_d
-00004ba0: 6963 745b 7461 7267 6574 5f63 656c 6c5f  ict[target_cell_
-00004bb0: 6964 5d20 3d20 6765 6e5f 636f 756e 740d  id] = gen_count.
-00004bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004be0: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
-00004bf0: 6963 745b 7461 7267 6574 5f63 656c 6c5f  ict[target_cell_
-00004c00: 6964 5d20 3d20 7472 6163 6b6c 6574 5f63  id] = tracklet_c
-00004c10: 6f75 6e74 0d0a 0d0a 2020 2020 2020 2020  ount....        
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
-00004c40: 745f 6365 6c6c 5f69 6420 696e 2072 6f6f  t_cell_id in roo
-00004c50: 745f 6c65 6166 3a0d 0a20 2020 2020 2020  t_leaf:..       
-00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00004c80: 662e 6765 6e65 7261 7469 6f6e 5f64 6963  f.generation_dic
-00004c90: 745b 7461 7267 6574 5f63 656c 6c5f 6964  t[target_cell_id
-00004ca0: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
-00004ce0: 5f64 6963 745b 7461 7267 6574 5f63 656c  _dict[target_cel
-00004cf0: 6c5f 6964 5d20 3d20 7472 6163 6b6c 6574  l_id] = tracklet
-00004d00: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
-00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d20: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00004d30: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
-00004d40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00004d50: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d70: 2020 2020 2020 2020 2062 7265 616b 2020           break  
-00004d80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00004d90: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00004da0: 5f63 656c 6c5f 6964 2069 6e20 736f 7274  _cell_id in sort
-00004db0: 6564 5f72 6f6f 745f 7370 6c69 7473 3a0d  ed_root_splits:.
-00004dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004dd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00004de0: 662e 6765 6e65 7261 7469 6f6e 5f64 6963  f.generation_dic
-00004df0: 745b 7461 7267 6574 5f63 656c 6c5f 6964  t[target_cell_id
-00004e00: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
-00004e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004e30: 7472 6163 6b6c 6574 5f64 6963 745b 7461  tracklet_dict[ta
-00004e40: 7267 6574 5f63 656c 6c5f 6964 5d20 3d20  rget_cell_id] = 
-00004e50: 7472 6163 6b6c 6574 5f63 6f75 6e74 2020  tracklet_count  
-00004e60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e80: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ea0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00004eb0: 6465 6620 5f67 6574 5f62 6f75 6e64 6172  def _get_boundar
-00004ec0: 795f 6469 7374 2873 656c 662c 2066 7261  y_dist(self, fra
-00004ed0: 6d65 2c20 7465 7374 6c6f 6361 7469 6f6e  me, testlocation
-00004ee0: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
-00004ef0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00004f00: 6173 6b20 6973 206e 6f74 204e 6f6e 653a  ask is not None:
-00004f10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00004f20: 2020 2020 7472 6565 2c20 696e 6469 6365      tree, indice
-00004f30: 732c 206d 6173 6b63 656e 7472 6f69 6420  s, maskcentroid 
-00004f40: 3d20 7365 6c66 2e74 696d 6564 5f6d 6173  = self.timed_mas
-00004f50: 6b5b 7374 7228 696e 7428 666c 6f61 7428  k[str(int(float(
-00004f60: 6672 616d 6529 2929 5d0d 0a20 2020 2020  frame)))]..     
+00004520: 2020 2020 2069 6620 7461 7267 6574 5f63       if target_c
+00004530: 656c 6c20 696e 2073 656c 662e 6564 6765  ell in self.edge
+00004540: 5f74 6172 6765 745f 6c6f 6f6b 7570 3a0d  _target_lookup:.
+00004550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2073 656c 662e 6765 6e65 7261       self.genera
+00004580: 7469 6f6e 5f64 6963 745b 7461 7267 6574  tion_dict[target
+00004590: 5f63 656c 6c5d 203d 2067 656e 5f63 6f75  _cell] = gen_cou
+000045a0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045c0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+000045d0: 636b 6c65 745f 6469 6374 5b74 6172 6765  cklet_dict[targe
+000045e0: 745f 6365 6c6c 5d20 3d20 7472 6163 6b6c  t_cell] = trackl
+000045f0: 6574 5f63 6f75 6e74 0d0a 2020 2020 2020  et_count..      
+00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004610: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00004620: 7267 6574 5f63 656c 6c20 3d20 7365 6c66  rget_cell = self
+00004630: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00004640: 6b75 705b 7461 7267 6574 5f63 656c 6c5d  kup[target_cell]
+00004650: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004670: 2020 2020 2065 6c69 6620 7461 7267 6574       elif target
+00004680: 5f63 656c 6c20 696e 2072 6f6f 745f 6c65  _cell in root_le
+00004690: 6166 3a0d 0a20 2020 2020 2020 2020 2020  af:..           
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+000046c0: 6e65 7261 7469 6f6e 5f64 6963 745b 7461  neration_dict[ta
+000046d0: 7267 6574 5f63 656c 6c5d 203d 2067 656e  rget_cell] = gen
+000046e0: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
+000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004710: 2e74 7261 636b 6c65 745f 6469 6374 5b74  .tracklet_dict[t
+00004720: 6172 6765 745f 6365 6c6c 5d20 3d20 7472  arget_cell] = tr
+00004730: 6163 6b6c 6574 5f63 6f75 6e74 0d0a 2020  acklet_count..  
+00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004760: 2020 6272 6561 6b0d 0a0d 0a20 2020 2064    break....    d
+00004770: 6566 205f 6974 6572 6174 655f 6469 7669  ef _iterate_divi
+00004780: 6469 6e67 5f72 6563 7572 7369 7665 2873  ding_recursive(s
+00004790: 656c 662c 2072 6f6f 745f 6c65 6166 2c20  elf, root_leaf, 
+000047a0: 7461 7267 6574 5f63 656c 6c73 2c20 736f  target_cells, so
+000047b0: 7274 6564 5f72 6f6f 745f 7370 6c69 7473  rted_root_splits
+000047c0: 2c20 6765 6e5f 636f 756e 742c 2074 7261  , gen_count, tra
+000047d0: 636b 6c65 745f 636f 756e 7429 3a0d 0a20  cklet_count):.. 
+000047e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000047f0: 2020 2020 2020 2020 206e 6578 745f 6974           next_it
+00004800: 6572 5f63 656c 6c73 203d 205b 5d0d 0a20  er_cells = [].. 
+00004810: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00004820: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
+00004830: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
+00004840: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00004850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004860: 2074 6172 6765 745f 6365 6c6c 203d 2074   target_cell = t
+00004870: 6172 6765 745f 6365 6c6c 735b 695d 0d0a  arget_cells[i]..
+00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000048a0: 2020 6966 2074 6172 6765 745f 6365 6c6c    if target_cell
+000048b0: 203d 3d20 726f 6f74 5f6c 6561 663a 0d0a   == root_leaf:..
+000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048d0: 2020 2020 7365 6c66 2e67 656e 6572 6174      self.generat
+000048e0: 696f 6e5f 6469 6374 5b74 6172 6765 745f  ion_dict[target_
+000048f0: 6365 6c6c 5d20 3d20 6765 6e5f 636f 756e  cell] = gen_coun
+00004900: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+00004910: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+00004920: 6b6c 6574 5f64 6963 745b 7461 7267 6574  klet_dict[target
+00004930: 5f63 656c 6c5d 203d 2074 7261 636b 6c65  _cell] = trackle
+00004940: 745f 636f 756e 740d 0a20 2020 2020 2020  t_count..       
+00004950: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00004960: 7572 6e0d 0a20 2020 2020 2020 2020 2020  urn..           
+00004970: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
+00004980: 756e 7420 3d20 7472 6163 6b6c 6574 5f63  unt = tracklet_c
+00004990: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+000049a0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+000049b0: 656e 6572 6174 696f 6e5f 6469 6374 5b74  eneration_dict[t
+000049c0: 6172 6765 745f 6365 6c6c 5d20 3d20 6765  arget_cell] = ge
+000049d0: 6e5f 636f 756e 740d 0a20 2020 2020 2020  n_count..       
+000049e0: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+000049f0: 6163 6b6c 6574 5f64 6963 745b 7461 7267  acklet_dict[targ
+00004a00: 6574 5f63 656c 6c5d 203d 2074 7261 636b  et_cell] = track
+00004a10: 6c65 745f 636f 756e 740d 0a20 2020 2020  let_count..     
+00004a20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00004a30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004a40: 7461 7267 6574 5f63 656c 6c20 696e 2073  target_cell in s
+00004a50: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
+00004a60: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
+00004a70: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00004a80: 745f 7461 7267 6574 5f63 656c 6c73 203d  t_target_cells =
+00004a90: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
+00004aa0: 745f 6c6f 6f6b 7570 5b74 6172 6765 745f  t_lookup[target_
+00004ab0: 6365 6c6c 5d0d 0a20 2020 2020 2020 2020  cell]..         
+00004ac0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00004ad0: 7461 7267 6574 5f63 656c 6c20 3d20 6e65  target_cell = ne
+00004ae0: 7874 5f74 6172 6765 745f 6365 6c6c 735b  xt_target_cells[
+00004af0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00004b00: 2020 2020 2020 2020 7768 696c 6520 6e65          while ne
+00004b10: 7874 5f74 6172 6765 745f 6365 6c6c 206e  xt_target_cell n
+00004b20: 6f74 2069 6e20 736f 7274 6564 5f72 6f6f  ot in sorted_roo
+00004b30: 745f 7370 6c69 7473 2061 6e64 206e 6578  t_splits and nex
+00004b40: 745f 7461 7267 6574 5f63 656c 6c20 6e6f  t_target_cell no
+00004b50: 7420 696e 2072 6f6f 745f 6c65 6166 3a0d  t in root_leaf:.
+00004b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b70: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+00004b80: 6e65 7261 7469 6f6e 5f64 6963 745b 6e65  neration_dict[ne
+00004b90: 7874 5f74 6172 6765 745f 6365 6c6c 5d20  xt_target_cell] 
+00004ba0: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
+00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bc0: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
+00004bd0: 6574 5f64 6963 745b 6e65 7874 5f74 6172  et_dict[next_tar
+00004be0: 6765 745f 6365 6c6c 5d20 3d20 7472 6163  get_cell] = trac
+00004bf0: 6b6c 6574 5f63 6f75 6e74 0d0a 2020 2020  klet_count..    
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c10: 2020 2020 6966 206e 6578 745f 7461 7267      if next_targ
+00004c20: 6574 5f63 656c 6c20 696e 2073 656c 662e  et_cell in self.
+00004c30: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00004c40: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
+00004c70: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
+00004c80: 6172 6765 745f 6c6f 6f6b 7570 5b6e 6578  arget_lookup[nex
+00004c90: 745f 7461 7267 6574 5f63 656c 6c5d 0d0a  t_target_cell]..
+00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cb0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00004cc0: 5f74 6172 6765 745f 6365 6c6c 203d 206e  _target_cell = n
+00004cd0: 6578 745f 7461 7267 6574 5f63 656c 6c73  ext_target_cells
+00004ce0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00004cf0: 2020 2020 2020 2020 206e 6578 745f 6974           next_it
+00004d00: 6572 5f63 656c 6c73 2e61 7070 656e 6428  er_cells.append(
+00004d10: 5b6e 6578 745f 7461 7267 6574 5f63 656c  [next_target_cel
+00004d20: 6c2c 2074 7261 636b 6c65 745f 636f 756e  l, tracklet_coun
+00004d30: 745d 290d 0a0d 0a20 2020 2020 2020 2020  t])....         
+00004d40: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00004d50: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00004d60: 656e 286e 6578 745f 6974 6572 5f63 656c  en(next_iter_cel
+00004d70: 6c73 2929 3a0d 0a20 2020 2020 2020 2020  ls)):..         
+00004d80: 2020 2020 2020 206e 6578 745f 7461 7267         next_targ
+00004d90: 6574 5f63 656c 6c2c 2074 7261 636b 6c65  et_cell, trackle
+00004da0: 745f 636f 756e 745f 6365 6c6c 203d 206e  t_count_cell = n
+00004db0: 6578 745f 6974 6572 5f63 656c 6c73 5b69  ext_iter_cells[i
+00004dc0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00004dd0: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00004de0: 6f6e 5f64 6963 745b 6e65 7874 5f74 6172  on_dict[next_tar
+00004df0: 6765 745f 6365 6c6c 5d20 3d20 6765 6e5f  get_cell] = gen_
+00004e00: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+00004e10: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+00004e20: 6b6c 6574 5f64 6963 745b 6e65 7874 5f74  klet_dict[next_t
+00004e30: 6172 6765 745f 6365 6c6c 5d20 3d20 7472  arget_cell] = tr
+00004e40: 6163 6b6c 6574 5f63 6f75 6e74 5f63 656c  acklet_count_cel
+00004e50: 6c20 200d 0a20 2020 2020 2020 2020 2020  l  ..           
+00004e60: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00004e70: 2020 2069 6620 6c65 6e28 6e65 7874 5f69     if len(next_i
+00004e80: 7465 725f 6365 6c6c 7329 203e 2030 3a0d  ter_cells) > 0:.
+00004e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ea0: 206e 6578 745f 6765 6e5f 636f 756e 7420   next_gen_count 
+00004eb0: 3d20 6765 6e5f 636f 756e 7420 2b20 310d  = gen_count + 1.
+00004ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ed0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00004ee0: 6c65 6e28 6e65 7874 5f69 7465 725f 6365  len(next_iter_ce
+00004ef0: 6c6c 7329 293a 0d0a 2020 2020 2020 2020  lls)):..        
+00004f00: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00004f10: 6c65 745f 636f 756e 7420 2b3d 2031 0d0a  let_count += 1..
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f30: 2020 206e 6578 745f 7461 7267 6574 5f63     next_target_c
+00004f40: 656c 6c2c 2074 7261 636b 6c65 745f 636f  ell, tracklet_co
+00004f50: 756e 745f 6365 6c6c 203d 206e 6578 745f  unt_cell = next_
+00004f60: 6974 6572 5f63 656c 6c73 5b69 5d0d 0a20  iter_cells[i].. 
 00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00004f90: 2020 2020 2023 2047 6574 2074 6865 206c       # Get the l
-00004fa0: 6f63 6174 696f 6e20 616e 6420 6469 7374  ocation and dist
-00004fb0: 616e 6365 2074 6f20 7468 6520 6e65 6172  ance to the near
-00004fc0: 6573 7420 626f 756e 6461 7279 2070 6f69  est boundary poi
-00004fd0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00004fe0: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
-00004ff0: 6c5f 6d61 736b 2c20 6c6f 6361 7469 6f6e  l_mask, location
-00005000: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
-00005010: 7279 2874 6573 746c 6f63 6174 696f 6e29  ry(testlocation)
-00005020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005030: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
-00005040: 6d61 736b 203d 206d 6178 2830 2c20 6469  mask = max(0, di
-00005050: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00005060: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005070: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005080: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00005090: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-000050a0: 6365 6c6c 5f6d 6173 6b20 3d20 300d 0a20  cell_mask = 0.. 
-000050b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000050c0: 6173 6b63 656e 7472 6f69 6420 3d20 2831  askcentroid = (1
-000050d0: 2c31 2c31 290d 0a0d 0a20 2020 2020 2020  ,1,1)....       
-000050e0: 2072 6574 7572 6e20 6469 7374 616e 6365   return distance
-000050f0: 5f63 656c 6c5f 6d61 736b 2c20 6d61 736b  _cell_mask, mask
-00005100: 6365 6e74 726f 6964 2020 2020 2020 2020  centroid        
-00005110: 0d0a 2020 2020 2020 2020 200d 0a0d 0a20  ..         .... 
-00005120: 2020 2064 6566 205f 7472 6163 6b5f 636f     def _track_co
-00005130: 6d70 7574 6572 2873 656c 662c 2074 7261  mputer(self, tra
-00005140: 636b 2c20 7472 6163 6b5f 6964 293a 0d0a  ck, track_id):..
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005180: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000051b0: 5f63 656c 6c5f 6964 7320 3d20 5b5d 0d0a  _cell_ids = []..
-000051c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051d0: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-000051e0: 7565 5f74 7261 636b 6c65 745f 6964 7320  ue_tracklet_ids 
-000051f0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005210: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005230: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
-00005240: 616c 6c5f 7461 7267 6574 5f69 6473 203d  all_target_ids =
-00005250: 2020 7365 6c66 2e5f 6765 6e65 7261 7465    self._generate
-00005260: 5f67 656e 6572 6174 696f 6e73 2874 7261  _generations(tra
-00005270: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
-00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005290: 2072 6f6f 745f 726f 6f74 2c20 726f 6f74   root_root, root
-000052a0: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
-000052b0: 6166 203d 2073 656c 662e 5f63 7265 6174  af = self._creat
-000052c0: 655f 6765 6e65 7261 7469 6f6e 7328 616c  e_generations(al
-000052d0: 6c5f 736f 7572 6365 5f69 6473 2c20 616c  l_source_ids, al
-000052e0: 6c5f 7461 7267 6574 5f69 6473 2920 0d0a  l_target_ids) ..
+00004f80: 2020 6966 206e 6578 745f 7461 7267 6574    if next_target
+00004f90: 5f63 656c 6c20 696e 2073 656c 662e 6564  _cell in self.ed
+00004fa0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00004fb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004fc0: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00004fd0: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
+00004fe0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00004ff0: 5b6e 6578 745f 7461 7267 6574 5f63 656c  [next_target_cel
+00005000: 6c5d 0d0a 2020 2020 2020 2020 2020 2020  l]..            
+00005010: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005020: 5f69 7465 7261 7465 5f64 6976 6964 696e  _iterate_dividin
+00005030: 675f 7265 6375 7273 6976 6528 726f 6f74  g_recursive(root
+00005040: 5f6c 6561 662c 2074 6172 6765 745f 6365  _leaf, target_ce
+00005050: 6c6c 732c 2073 6f72 7465 645f 726f 6f74  lls, sorted_root
+00005060: 5f73 706c 6974 732c 206e 6578 745f 6765  _splits, next_ge
+00005070: 6e5f 636f 756e 742c 2074 7261 636b 6c65  n_count, trackle
+00005080: 745f 636f 756e 7429 2020 2020 2020 0d0a  t_count)      ..
+00005090: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000050a0: 2020 6465 6620 5f69 7465 7261 7465 5f64    def _iterate_d
+000050b0: 6976 6964 696e 6728 7365 6c66 2c20 726f  ividing(self, ro
+000050c0: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
+000050d0: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
+000050e0: 3a0d 0a20 2020 2020 2020 2020 2020 2067  :..            g
+000050f0: 656e 5f63 6f75 6e74 203d 2030 0d0a 2020  en_count = 0..  
+00005100: 2020 2020 2020 2020 2020 7472 6163 6b6c            trackl
+00005110: 6574 5f63 6f75 6e74 203d 2030 0d0a 2020  et_count = 0..  
+00005120: 2020 2020 2020 2020 2020 666f 7220 726f            for ro
+00005130: 6f74 5f61 6c6c 2069 6e20 726f 6f74 5f72  ot_all in root_r
+00005140: 6f6f 743a 0d0a 2020 2020 2020 2020 2020  oot:..          
+00005150: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00005160: 656e 6572 6174 696f 6e5f 6469 6374 5b72  eneration_dict[r
+00005170: 6f6f 745f 616c 6c5d 203d 2067 656e 5f63  oot_all] = gen_c
+00005180: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+00005190: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+000051a0: 7261 636b 6c65 745f 6469 6374 5b72 6f6f  racklet_dict[roo
+000051b0: 745f 616c 6c5d 203d 2074 7261 636b 6c65  t_all] = trackle
+000051c0: 745f 636f 756e 740d 0a20 2020 2020 2020  t_count..       
+000051d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000051e0: 726f 6f74 5f61 6c6c 2069 6e20 7365 6c66  root_all in self
+000051f0: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00005200: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
+00005210: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00005220: 6172 6765 745f 6365 6c6c 203d 2073 656c  arget_cell = sel
+00005230: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
+00005240: 6f6b 7570 5b72 6f6f 745f 616c 6c5d 5b30  okup[root_all][0
+00005250: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00005260: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+00005270: 6520 7461 7267 6574 5f63 656c 6c20 6e6f  e target_cell no
+00005280: 7420 696e 2072 6f6f 745f 7370 6c69 7473  t in root_splits
+00005290: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052b0: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
+000052c0: 6c20 696e 2073 656c 662e 6564 6765 5f74  l in self.edge_t
+000052d0: 6172 6765 745f 6c6f 6f6b 7570 3a0d 0a20  arget_lookup:.. 
+000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005300: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005310: 2e5f 6974 6572 6174 655f 7370 6c69 745f  ._iterate_split_
-00005320: 646f 776e 2872 6f6f 745f 726f 6f74 2c20  down(root_root, 
-00005330: 726f 6f74 5f6c 6561 662c 2072 6f6f 745f  root_leaf, root_
-00005340: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
-00005350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005360: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 206e 756d 6265 725f 6469 7669 6469     number_dividi
-00005390: 6e67 203d 206c 656e 2872 6f6f 745f 7370  ng = len(root_sp
-000053a0: 6c69 7473 290d 0a20 2020 2020 2020 2020  lits)..         
-000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053c0: 2020 2023 2044 6574 6572 6d69 6e65 2069     # Determine i
-000053d0: 6620 6120 7472 6163 6b20 6861 7320 6469  f a track has di
-000053e0: 7669 7369 6f6e 7320 6f72 206e 6f6e 650d  visions or none.
-000053f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005400: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005410: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
-00005420: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005440: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00005450: 7565 5f74 7261 636b 5f6d 6974 6f73 6973  ue_track_mitosis
-00005460: 5f6c 6162 656c 5b74 7261 636b 5f69 645d  _label[track_id]
-00005470: 203d 205b 312c 206e 756d 6265 725f 6469   = [1, number_di
-00005480: 7669 6469 6e67 5d0d 0a20 2020 2020 2020  viding]..       
-00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054a0: 2020 2020 2020 2020 2064 6976 6964 696e           dividin
-000054b0: 675f 7472 616a 6563 746f 7279 203d 2054  g_trajectory = T
-000054c0: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
-000054f0: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
-00005500: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005530: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
-00005540: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
-00005550: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
-00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00005580: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
-00005590: 2069 6e20 7365 6c66 2e44 6976 6964 696e   in self.Dividin
-000055a0: 6754 7261 636b 4964 733a 2020 2020 200d  gTrackIds:     .
-000055b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055d0: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
-000055e0: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
-000055f0: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
-00005600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005620: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00005650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005660: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005670: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
-00005680: 5f6d 6974 6f73 6973 5f6c 6162 656c 5b74  _mitosis_label[t
-00005690: 7261 636b 5f69 645d 203d 205b 302c 2030  rack_id] = [0, 0
-000056a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 2020 2064 6976 6964 696e 675f 7472 616a     dividing_traj
-000056d0: 6563 746f 7279 203d 2046 616c 7365 0d0a  ectory = False..
-000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
-00005710: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
-00005720: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005750: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-00005760: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
-00005770: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
-00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005790: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
-000057a0: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
-000057b0: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
-000057c0: 6473 3a20 2020 200d 0a20 2020 2020 2020  ds:    ..       
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000057f0: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
-00005800: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
-00005810: 6b5f 6964 2929 0d0a 0d0a 2020 2020 2020  k_id))....      
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 2020 2020 2020 666f 7220 6c65 6166 2069        for leaf i
-00005840: 6e20 726f 6f74 5f6c 6561 663a 0d0a 2020  n root_leaf:..  
-00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2073 6f75 7263 655f 6c65 6166 203d 2073   source_leaf = s
-00005880: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
-00005890: 6c6f 6f6b 7570 5b6c 6561 665d 0d0a 2020  lookup[leaf]..  
-000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058c0: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
-000058d0: 732e 6170 7065 6e64 286c 6561 6629 200d  s.append(leaf) .
-000058e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005900: 2020 2020 7365 6c66 2e5f 6469 6374 5f75      self._dict_u
-00005910: 7064 6174 6528 756e 6971 7565 5f74 7261  pdate(unique_tra
-00005920: 636b 6c65 745f 6964 732c 206c 6561 662c  cklet_ids, leaf,
-00005930: 2074 7261 636b 5f69 642c 2073 6f75 7263   track_id, sourc
-00005940: 655f 6c65 6166 2c20 4e6f 6e65 290d 0a20  e_leaf, None).. 
-00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005970: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00005980: 6f74 5f70 726f 7065 7274 6965 735b 6c65  ot_properties[le
-00005990: 6166 5d2e 7570 6461 7465 287b 7365 6c66  af].update({self
-000059a0: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
-000059b0: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
-000059c0: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059e0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000059f0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00005a00: 7274 6965 735b 6c65 6166 5d2e 7570 6461  rties[leaf].upda
-00005a10: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
-00005a20: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
-00005a30: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
-00005a40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a60: 666f 7220 736f 7572 6365 5f69 6420 696e  for source_id in
-00005a70: 2061 6c6c 5f73 6f75 7263 655f 6964 733a   all_source_ids:
-00005a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005aa0: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00005ab0: 5f69 6473 203d 2073 656c 662e 6564 6765  _ids = self.edge
-00005ac0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
-00005ad0: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
-00005ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005300: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00005310: 6f6e 5f64 6963 745b 7461 7267 6574 5f63  on_dict[target_c
+00005320: 656c 6c5d 203d 2067 656e 5f63 6f75 6e74  ell] = gen_count
+00005330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005350: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+00005360: 6c65 745f 6469 6374 5b74 6172 6765 745f  let_dict[target_
+00005370: 6365 6c6c 5d20 3d20 7472 6163 6b6c 6574  cell] = tracklet
+00005380: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
+00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053a0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+000053b0: 6574 5f63 656c 6c20 3d20 7365 6c66 2e65  et_cell = self.e
+000053c0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
+000053d0: 705b 7461 7267 6574 5f63 656c 6c5d 5b30  p[target_cell][0
+000053e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005400: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+00005410: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+00005420: 645f 726f 6f74 5f73 706c 6974 7320 3d20  d_root_splits = 
+00005430: 7365 6c66 2e5f 736f 7274 5f64 6976 6964  self._sort_divid
+00005440: 696e 675f 6365 6c6c 7328 726f 6f74 5f73  ing_cells(root_s
+00005450: 706c 6974 7329 0d0a 2020 2020 2020 2020  plits)..        
+00005460: 2020 2020 6765 6e5f 636f 756e 7420 3d20      gen_count = 
+00005470: 300d 0a20 2020 2020 2020 2020 2020 2074  0..            t
+00005480: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
+00005490: 300d 0a20 2020 2020 2020 2020 2020 206e  0..            n
+000054a0: 6578 745f 6765 6e5f 636f 756e 7420 3d20  ext_gen_count = 
+000054b0: 300d 0a20 2020 2020 2020 2020 2020 2066  0..            f
+000054c0: 6972 7374 5f73 706c 6974 203d 2073 6f72  irst_split = sor
+000054d0: 7465 645f 726f 6f74 5f73 706c 6974 735b  ted_root_splits[
+000054e0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+000054f0: 7365 6c66 2e67 656e 6572 6174 696f 6e5f  self.generation_
+00005500: 6469 6374 5b66 6972 7374 5f73 706c 6974  dict[first_split
+00005510: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
+00005520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005530: 7472 6163 6b6c 6574 5f64 6963 745b 6669  tracklet_dict[fi
+00005540: 7273 745f 7370 6c69 745d 203d 2074 7261  rst_split] = tra
+00005550: 636b 6c65 745f 636f 756e 740d 0a20 2020  cklet_count..   
+00005560: 2020 2020 2020 2020 2069 6620 6669 7273           if firs
+00005570: 745f 7370 6c69 7420 696e 2073 656c 662e  t_split in self.
+00005580: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00005590: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+000055a0: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
+000055b0: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
+000055c0: 7267 6574 5f6c 6f6f 6b75 705b 6669 7273  rget_lookup[firs
+000055d0: 745f 7370 6c69 745d 0d0a 2020 2020 2020  t_split]..      
+000055e0: 2020 2020 2020 2020 2020 6e65 7874 5f67            next_g
+000055f0: 656e 5f63 6f75 6e74 202b 3d20 310d 0a20  en_count += 1.. 
+00005600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005610: 656c 662e 5f69 7465 7261 7465 5f64 6976  elf._iterate_div
+00005620: 6964 696e 675f 7265 6375 7273 6976 6528  iding_recursive(
+00005630: 726f 6f74 5f6c 6561 662c 2074 6172 6765  root_leaf, targe
+00005640: 745f 6365 6c6c 732c 2073 6f72 7465 645f  t_cells, sorted_
+00005650: 726f 6f74 5f73 706c 6974 732c 206e 6578  root_splits, nex
+00005660: 745f 6765 6e5f 636f 756e 742c 2074 7261  t_gen_count, tra
+00005670: 636b 6c65 745f 636f 756e 7429 0d0a 2020  cklet_count)..  
+00005680: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056b0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+000056c0: 2020 6465 6620 5f69 7465 7261 7465 5f73    def _iterate_s
+000056d0: 706c 6974 5f64 6f77 6e28 7365 6c66 2c20  plit_down(self, 
+000056e0: 726f 6f74 5f72 6f6f 742c 2072 6f6f 745f  root_root, root_
+000056f0: 6c65 6166 2c20 726f 6f74 5f73 706c 6974  leaf, root_split
+00005700: 7329 3a0d 0a20 2020 2020 2020 2020 0d0a  s):..         ..
+00005710: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
+00005720: 6f6f 745f 7370 6c69 7473 2920 3d3d 2030  oot_splits) == 0
+00005730: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005740: 2020 7365 6c66 2e5f 6974 6572 6174 655f    self._iterate_
+00005750: 6e6f 6e5f 6469 7669 6469 6e67 2872 6f6f  non_dividing(roo
+00005760: 745f 726f 6f74 2c20 726f 6f74 5f6c 6561  t_root, root_lea
+00005770: 6629 0d0a 2020 2020 2020 2020 6966 206c  f)..        if l
+00005780: 656e 2872 6f6f 745f 7370 6c69 7473 2920  en(root_splits) 
+00005790: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
+000057a0: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
+000057b0: 7465 5f64 6976 6964 696e 6728 726f 6f74  te_dividing(root
+000057c0: 5f72 6f6f 742c 2072 6f6f 745f 6c65 6166  _root, root_leaf
+000057d0: 2c20 726f 6f74 5f73 706c 6974 7329 2020  , root_splits)  
+000057e0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
+00005810: 6765 745f 626f 756e 6461 7279 5f64 6973  get_boundary_dis
+00005820: 7428 7365 6c66 2c20 6672 616d 652c 2074  t(self, frame, t
+00005830: 6573 746c 6f63 6174 696f 6e29 3a0d 0a20  estlocation):.. 
+00005840: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00005850: 2020 6966 2073 656c 662e 6d61 736b 2069    if self.mask i
+00005860: 7320 6e6f 7420 4e6f 6e65 3a0d 0a0d 0a20  s not None:.... 
+00005870: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00005880: 7265 652c 2069 6e64 6963 6573 2c20 6d61  ree, indices, ma
+00005890: 736b 6365 6e74 726f 6964 203d 2073 656c  skcentroid = sel
+000058a0: 662e 7469 6d65 645f 6d61 736b 5b73 7472  f.timed_mask[str
+000058b0: 2869 6e74 2866 6c6f 6174 2866 7261 6d65  (int(float(frame
+000058c0: 2929 295d 0d0a 2020 2020 2020 2020 2020  )))]..          
+000058d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058f0: 2320 4765 7420 7468 6520 6c6f 6361 7469  # Get the locati
+00005900: 6f6e 2061 6e64 2064 6973 7461 6e63 6520  on and distance 
+00005910: 746f 2074 6865 206e 6561 7265 7374 2062  to the nearest b
+00005920: 6f75 6e64 6172 7920 706f 696e 740d 0a20  oundary point.. 
+00005930: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005940: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00005950: 6b2c 206c 6f63 6174 696f 6e69 6e64 6578  k, locationindex
+00005960: 203d 2074 7265 652e 7175 6572 7928 7465   = tree.query(te
+00005970: 7374 6c6f 6361 7469 6f6e 290d 0a20 2020  stlocation)..   
+00005980: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00005990: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+000059a0: 3d20 6d61 7828 302c 2064 6973 7461 6e63  = max(0, distanc
+000059b0: 655f 6365 6c6c 5f6d 6173 6b29 0d0a 2020  e_cell_mask)..  
+000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059d0: 200d 0a20 2020 2020 2020 2065 6c73 653a   ..        else:
+000059e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000059f0: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
+00005a00: 6d61 736b 203d 2030 0d0a 2020 2020 2020  mask = 0..      
+00005a10: 2020 2020 2020 2020 2020 6d61 736b 6365            maskce
+00005a20: 6e74 726f 6964 203d 2028 312c 312c 3129  ntroid = (1,1,1)
+00005a30: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00005a40: 726e 2064 6973 7461 6e63 655f 6365 6c6c  rn distance_cell
+00005a50: 5f6d 6173 6b2c 206d 6173 6b63 656e 7472  _mask, maskcentr
+00005a60: 6f69 6420 2020 2020 2020 200d 0a20 2020  oid        ..   
+00005a70: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
+00005a80: 6620 5f74 7261 636b 5f63 6f6d 7075 7465  f _track_compute
+00005a90: 7228 7365 6c66 2c20 7472 6163 6b2c 2074  r(self, track, t
+00005aa0: 7261 636b 5f69 6429 3a0d 0a20 2020 2020  rack_id):..     
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ac0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ae0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00005b10: 6964 732e 6170 7065 6e64 2873 6f75 7263  ids.append(sourc
-00005b20: 655f 6964 290d 0a20 2020 2020 2020 2020  e_id)..         
-00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005b50: 526f 6f74 0d0a 2020 2020 2020 2020 2020  Root..          
-00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005b80: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00005b90: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
-00005ba0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-00005bb0: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
-00005bc0: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
-00005bd0: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
-00005be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00005c10: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
-00005c20: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
-00005c30: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
-00005c40: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
-00005c50: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
-00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
-00005c90: 6420 6e6f 7420 696e 2061 6c6c 5f74 6172  d not in all_tar
-00005ca0: 6765 745f 6964 733a 0d0a 2020 2020 2020  get_ids:..      
+00005b00: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
+00005b10: 5f69 6473 203d 205b 5d0d 0a20 2020 2020  _ids = []..     
+00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b30: 2020 2020 2020 2075 6e69 7175 655f 7472         unique_tr
+00005b40: 6163 6b6c 6574 5f69 6473 203d 205b 5d0d  acklet_ids = [].
+00005b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00005b70: 5f73 6f75 7263 655f 6964 732c 2061 6c6c  _source_ids, all
+00005b80: 5f74 6172 6765 745f 6964 7320 3d20 2073  _target_ids =  s
+00005b90: 656c 662e 5f67 656e 6572 6174 655f 6765  elf._generate_ge
+00005ba0: 6e65 7261 7469 6f6e 7328 7472 6163 6b29  nerations(track)
+00005bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00005bd0: 6f74 5f72 6f6f 742c 2072 6f6f 745f 7370  ot_root, root_sp
+00005be0: 6c69 7473 2c20 726f 6f74 5f6c 6561 6620  lits, root_leaf 
+00005bf0: 3d20 7365 6c66 2e5f 6372 6561 7465 5f67  = self._create_g
+00005c00: 656e 6572 6174 696f 6e73 2861 6c6c 5f73  enerations(all_s
+00005c10: 6f75 7263 655f 6964 732c 2061 6c6c 5f74  ource_ids, all_t
+00005c20: 6172 6765 745f 6964 7329 200d 0a20 2020  arget_ids) ..   
+00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c40: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c60: 2020 2020 2020 2073 656c 662e 5f69 7465         self._ite
+00005c70: 7261 7465 5f73 706c 6974 5f64 6f77 6e28  rate_split_down(
+00005c80: 726f 6f74 5f72 6f6f 742c 2072 6f6f 745f  root_root, root_
+00005c90: 6c65 6166 2c20 726f 6f74 5f73 706c 6974  leaf, root_split
+00005ca0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
 00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 6e75 6d62 6572 5f64 6976 6964 696e 6720  number_dividing 
+00005cd0: 3d20 6c65 6e28 726f 6f74 5f73 706c 6974  = len(root_split
+00005ce0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
 00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00005d10: 7461 7267 6574 5f69 6420 696e 2074 6172  target_id in tar
-00005d20: 6765 745f 6964 733a 0d0a 2020 2020 2020  get_ids:..      
+00005d00: 2320 4465 7465 726d 696e 6520 6966 2061  # Determine if a
+00005d10: 2074 7261 636b 2068 6173 2064 6976 6973   track has divis
+00005d20: 696f 6e73 206f 7220 6e6f 6e65 0d0a 2020  ions or none..  
 00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005d60: 662e 5f64 6963 745f 7570 6461 7465 2875  f._dict_update(u
-00005d70: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
-00005d80: 6473 2c20 736f 7572 6365 5f69 642c 2074  ds, source_id, t
-00005d90: 7261 636b 5f69 642c 204e 6f6e 652c 2074  rack_id, None, t
-00005da0: 6172 6765 745f 6964 290d 0a20 2020 2020  arget_id)..     
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005de0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00005df0: 726f 7065 7274 6965 735b 7461 7267 6574  roperties[target
-00005e00: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-00005e10: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
-00005e20: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
-00005e30: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
-00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d40: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00005d50: 2872 6f6f 745f 7370 6c69 7473 2920 3e20  (root_splits) > 
+00005d60: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d80: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00005d90: 7472 6163 6b5f 6d69 746f 7369 735f 6c61  track_mitosis_la
+00005da0: 6265 6c5b 7472 6163 6b5f 6964 5d20 3d20  bel[track_id] = 
+00005db0: 5b31 2c20 6e75 6d62 6572 5f64 6976 6964  [1, number_divid
+00005dc0: 696e 675d 0d0a 2020 2020 2020 2020 2020  ing]..          
+00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005de0: 2020 2020 2020 6469 7669 6469 6e67 5f74        dividing_t
+00005df0: 7261 6a65 6374 6f72 7920 3d20 5472 7565  rajectory = True
+00005e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
+00005e30: 6429 206e 6f74 2069 6e20 7365 6c66 2e41  d) not in self.A
+00005e40: 6c6c 5472 6163 6b49 6473 3a0d 0a20 2020  llTrackIds:..   
 00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005e70: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00005e80: 6572 7469 6573 5b74 6172 6765 745f 6964  erties[target_id
-00005e90: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
-00005ea0: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
-00005eb0: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
-00005ec0: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
-00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ef0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e70: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
+00005e80: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
+00005e90: 636b 5f69 6429 290d 0a20 2020 2020 2020  ck_id))..       
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005eb0: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
+00005ec0: 7472 6163 6b5f 6964 2920 6e6f 7420 696e  track_id) not in
+00005ed0: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
+00005ee0: 6163 6b49 6473 3a20 2020 2020 0d0a 2020  ackIds:     ..  
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 2020 2020 2023 4e6f 726d 616c 2020 2020       #Normal    
-00005f30: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00005f10: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
+00005f20: 7261 636b 4964 732e 6170 7065 6e64 2869  rackIds.append(i
+00005f30: 6e74 2874 7261 636b 5f69 6429 290d 0a20  nt(track_id)).. 
 00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 2020 736f 7572 6365 5f73 6f75 7263      source_sourc
-00005f70: 655f 6964 203d 2073 656c 662e 6564 6765  e_id = self.edge
-00005f80: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b73  _source_lookup[s
-00005f90: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2020 2020 2020 2020 2066 6f72 2074 6172           for tar
-00005fd0: 6765 745f 6964 2069 6e20 7461 7267 6574  get_id in target
-00005fe0: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
+00005f60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f80: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005fb0: 2e75 6e69 7175 655f 7472 6163 6b5f 6d69  .unique_track_mi
+00005fc0: 746f 7369 735f 6c61 6265 6c5b 7472 6163  tosis_label[trac
+00005fd0: 6b5f 6964 5d20 3d20 5b30 2c20 305d 0d0a  k_id] = [0, 0]..
+00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006020: 5f64 6963 745f 7570 6461 7465 2875 6e69  _dict_update(uni
-00006030: 7175 655f 7472 6163 6b6c 6574 5f69 6473  que_tracklet_ids
-00006040: 2c20 736f 7572 6365 5f69 642c 2074 7261  , source_id, tra
-00006050: 636b 5f69 642c 2073 6f75 7263 655f 736f  ck_id, source_so
-00006060: 7572 6365 5f69 642c 2074 6172 6765 745f  urce_id, target_
-00006070: 6964 2920 0d0a 2020 2020 2020 2020 2020  id) ..          
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000060b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000060c0: 7274 6965 735b 7461 7267 6574 5f69 645d  rties[target_id]
-000060d0: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
-000060e0: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
-000060f0: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-00006100: 7d29 200d 0a20 2020 2020 2020 2020 2020  }) ..           
+00006000: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
+00006010: 6f72 7920 3d20 4661 6c73 650d 0a20 2020  ory = False..   
+00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006030: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006040: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
+00006050: 7420 696e 2073 656c 662e 416c 6c54 7261  t in self.AllTra
+00006060: 636b 4964 733a 0d0a 2020 2020 2020 2020  ckIds:..        
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006090: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
+000060a0: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
+000060b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060d0: 2020 2020 6966 2069 6e74 2874 7261 636b      if int(track
+000060e0: 5f69 6429 206e 6f74 2069 6e20 7365 6c66  _id) not in self
+000060f0: 2e4e 6f72 6d61 6c54 7261 636b 4964 733a  .NormalTrackIds:
+00006100: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006130: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00006140: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00006150: 7469 6573 5b74 6172 6765 745f 6964 5d2e  ties[target_id].
-00006160: 7570 6461 7465 287b 7365 6c66 2e6e 756d  update({self.num
-00006170: 6265 725f 6469 7669 6469 6e67 5f6b 6579  ber_dividing_key
-00006180: 203a 206e 756d 6265 725f 6469 7669 6469   : number_dividi
-00006190: 6e67 7d29 0d0a 2020 2020 2020 2020 2020  ng})..          
-000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061b0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000061c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006200: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006220: 2020 2020 2020 2020 2066 6f72 2063 7572           for cur
-00006230: 7265 6e74 5f72 6f6f 7420 696e 2072 6f6f  rent_root in roo
-00006240: 745f 726f 6f74 3a0d 0a20 2020 2020 2020  t_root:..       
-00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006270: 2e72 6f6f 745f 7370 6f74 735b 696e 7428  .root_spots[int(
-00006280: 6375 7272 656e 745f 726f 6f74 295d 203d  current_root)] =
-00006290: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000062a0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000062b0: 2863 7572 7265 6e74 5f72 6f6f 7429 5d0d  (current_root)].
-000062c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000062d0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006300: 616c 6c5f 6375 7272 656e 745f 6365 6c6c  all_current_cell
-00006310: 5f69 6473 5b69 6e74 2874 7261 636b 5f69  _ids[int(track_i
-00006320: 6429 5d20 3d20 6375 7272 656e 745f 6365  d)] = current_ce
-00006330: 6c6c 5f69 6473 0d0a 2020 2020 2020 2020  ll_ids..        
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00006360: 6765 286c 656e 2863 7572 7265 6e74 5f63  ge(len(current_c
-00006370: 656c 6c5f 6964 7329 293a 0d0a 2020 2020  ell_ids)):..    
-00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063c0: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
-000063d0: 7428 6375 7272 656e 745f 6365 6c6c 5f69  t(current_cell_i
-000063e0: 6473 5b69 5d29 2020 2020 0d0a 2020 2020  ds[i])    ..    
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 616c 6c5f 6469 6374 5f76 616c 7565 7320  all_dict_values 
-00006420: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
-00006430: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
-00006440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006120: 2020 2020 2020 2020 2020 7365 6c66 2e4e            self.N
+00006130: 6f72 6d61 6c54 7261 636b 4964 732e 6170  ormalTrackIds.ap
+00006140: 7065 6e64 2869 6e74 2874 7261 636b 5f69  pend(int(track_i
+00006150: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
+00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006170: 2020 2066 6f72 206c 6561 6620 696e 2072     for leaf in r
+00006180: 6f6f 745f 6c65 6166 3a0d 0a20 2020 2020  oot_leaf:..     
+00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061a0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+000061b0: 7572 6365 5f6c 6561 6620 3d20 7365 6c66  urce_leaf = self
+000061c0: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
+000061d0: 6b75 705b 6c65 6166 5d0d 0a20 2020 2020  kup[leaf]..     
+000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061f0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00006200: 7272 656e 745f 6365 6c6c 5f69 6473 2e61  rrent_cell_ids.a
+00006210: 7070 656e 6428 6c65 6166 2920 0d0a 2020  ppend(leaf) ..  
+00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006240: 2073 656c 662e 5f64 6963 745f 7570 6461   self._dict_upda
+00006250: 7465 2875 6e69 7175 655f 7472 6163 6b6c  te(unique_trackl
+00006260: 6574 5f69 6473 2c20 6c65 6166 2c20 7472  et_ids, leaf, tr
+00006270: 6163 6b5f 6964 2c20 736f 7572 6365 5f6c  ack_id, source_l
+00006280: 6561 662c 204e 6f6e 6529 0d0a 2020 2020  eaf, None)..    
+00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000062b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000062c0: 7072 6f70 6572 7469 6573 5b6c 6561 665d  properties[leaf]
+000062d0: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
+000062e0: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
+000062f0: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
+00006300: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00006330: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00006340: 6573 5b6c 6561 665d 2e75 7064 6174 6528  es[leaf].update(
+00006350: 7b73 656c 662e 6e75 6d62 6572 5f64 6976  {self.number_div
+00006360: 6964 696e 675f 6b65 7920 3a20 6e75 6d62  iding_key : numb
+00006370: 6572 5f64 6976 6964 696e 677d 290d 0a0d  er_dividing})...
+00006380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006390: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000063a0: 2073 6f75 7263 655f 6964 2069 6e20 616c   source_id in al
+000063b0: 6c5f 736f 7572 6365 5f69 6473 3a0d 0a20  l_source_ids:.. 
+000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063e0: 2020 2020 2020 2074 6172 6765 745f 6964         target_id
+000063f0: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
+00006400: 7267 6574 5f6c 6f6f 6b75 705b 736f 7572  rget_lookup[sour
+00006410: 6365 5f69 645d 0d0a 2020 2020 2020 2020  ce_id]..        
+00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006440: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
+00006450: 2e61 7070 656e 6428 736f 7572 6365 5f69  .append(source_i
+00006460: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
 00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006480: 2020 2020 2020 2020 2020 2074 203d 2069             t = i
-00006490: 6e74 2866 6c6f 6174 2861 6c6c 5f64 6963  nt(float(all_dic
-000064a0: 745f 7661 6c75 6573 5b73 656c 662e 6672  t_values[self.fr
-000064b0: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
-000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064e0: 2020 7a20 3d20 666c 6f61 7428 616c 6c5f    z = float(all_
-000064f0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00006500: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
-00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006480: 2020 2020 2020 2020 2020 2020 2352 6f6f              #Roo
+00006490: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000064c0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000064d0: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
+000064e0: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
+000064f0: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
+00006500: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
+00006510: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
 00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006530: 2020 2079 203d 2066 6c6f 6174 2861 6c6c     y = float(all
-00006540: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-00006550: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
-00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006580: 2020 2020 7820 3d20 666c 6f61 7428 616c      x = float(al
-00006590: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-000065a0: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
-000065b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006530: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006540: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00006550: 6f70 6572 7469 6573 5b73 6f75 7263 655f  operties[source_
+00006560: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00006570: 2e6e 756d 6265 725f 6469 7669 6469 6e67  .number_dividing
+00006580: 5f6b 6579 203a 206e 756d 6265 725f 6469  _key : number_di
+00006590: 7669 6469 6e67 7d29 0d0a 2020 2020 2020  viding})..      
+000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065c0: 2020 6966 2073 6f75 7263 655f 6964 206e    if source_id n
+000065d0: 6f74 2069 6e20 616c 6c5f 7461 7267 6574  ot in all_target
+000065e0: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
 000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 7370 6f74 5f63 656e 7472 6f69 6420    spot_centroid 
-00006610: 3d20 2872 6f75 6e64 287a 292f 7365 6c66  = (round(z)/self
-00006620: 2e7a 6361 6c69 6272 6174 696f 6e2c 2072  .zcalibration, r
-00006630: 6f75 6e64 2879 292f 7365 6c66 2e79 6361  ound(y)/self.yca
-00006640: 6c69 6272 6174 696f 6e2c 2072 6f75 6e64  libration, round
-00006650: 2878 292f 7365 6c66 2e78 6361 6c69 6272  (x)/self.xcalibr
-00006660: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00006600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006610: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006640: 2020 2020 2020 2020 2066 6f72 2074 6172           for tar
+00006650: 6765 745f 6964 2069 6e20 7461 7267 6574  get_id in target
+00006660: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
 00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00006690: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
-000066a0: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
-000066b0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-000066c0: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
-000066d0: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-000066e0: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
-000066f0: 6272 6174 696f 6e29 0d0a 0d0a 2020 2020  bration)....    
+00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006690: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000066a0: 6469 6374 5f75 7064 6174 6528 756e 6971  dict_update(uniq
+000066b0: 7565 5f74 7261 636b 6c65 745f 6964 732c  ue_tracklet_ids,
+000066c0: 2073 6f75 7263 655f 6964 2c20 7472 6163   source_id, trac
+000066d0: 6b5f 6964 2c20 4e6f 6e65 2c20 7461 7267  k_id, None, targ
+000066e0: 6574 5f69 6429 0d0a 2020 2020 2020 2020  et_id)..        
+000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006720: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00006730: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
-00006740: 7370 6f74 5f63 656e 7472 6f69 645d 203d  spot_centroid] =
-00006750: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
-00006760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006770: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00006780: 7175 655f 7472 6163 6b5f 6365 6e74 726f  que_track_centro
-00006790: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
-000067a0: 6e74 726f 6964 5d20 3d20 7472 6163 6b5f  ntroid] = track_
-000067b0: 6964 0d0a 0d0a 2020 2020 2020 2020 2020  id....          
-000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067d0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
-000067e0: 2874 2920 696e 2073 656c 662e 5f74 696d  (t) in self._tim
-000067f0: 6564 5f63 656e 7472 6f69 643a 0d0a 2020  ed_centroid:..  
-00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006720: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00006730: 6572 7469 6573 5b74 6172 6765 745f 6964  erties[target_id
+00006740: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
+00006750: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
+00006760: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
+00006770: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
+00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067a0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000067b0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+000067c0: 6965 735b 7461 7267 6574 5f69 645d 2e75  ies[target_id].u
+000067d0: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
+000067e0: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
+000067f0: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
+00006800: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
 00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006820: 2020 2020 2020 2020 2074 7265 652c 2073           tree, s
-00006830: 706f 745f 6365 6e74 726f 6964 7320 3d20  pot_centroids = 
-00006840: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
-00006850: 726f 6964 5b73 7472 2874 295d 0d0a 2020  roid[str(t)]..  
-00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
-00006890: 6e74 726f 6964 732e 6170 7065 6e64 2873  ntroids.append(s
-000068a0: 706f 745f 6365 6e74 726f 6964 290d 0a20  pot_centroid).. 
-000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
-000068e0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-000068f0: 2873 706f 745f 6365 6e74 726f 6964 7329  (spot_centroids)
-00006900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006920: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006930: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
-00006940: 645b 7374 7228 7429 5d20 3d20 7472 6565  d[str(t)] = tree
-00006950: 2c20 7370 6f74 5f63 656e 7472 6f69 6473  , spot_centroids
-00006960: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006980: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069b0: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
-000069c0: 6e74 726f 6964 7320 3d20 5b5d 0d0a 2020  ntroids = []..  
+00006820: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00006830: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006860: 2020 234e 6f72 6d61 6c20 2020 2020 2020    #Normal       
+00006870: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068a0: 2073 6f75 7263 655f 736f 7572 6365 5f69   source_source_i
+000068b0: 6420 3d20 7365 6c66 2e65 6467 655f 736f  d = self.edge_so
+000068c0: 7572 6365 5f6c 6f6f 6b75 705b 736f 7572  urce_lookup[sour
+000068d0: 6365 5f69 645d 0d0a 2020 2020 2020 2020  ce_id]..        
+000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006900: 2020 2020 2020 666f 7220 7461 7267 6574        for target
+00006910: 5f69 6420 696e 2074 6172 6765 745f 6964  _id in target_id
+00006920: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006950: 2020 2020 2020 2020 7365 6c66 2e5f 6469          self._di
+00006960: 6374 5f75 7064 6174 6528 756e 6971 7565  ct_update(unique
+00006970: 5f74 7261 636b 6c65 745f 6964 732c 2073  _tracklet_ids, s
+00006980: 6f75 7263 655f 6964 2c20 7472 6163 6b5f  ource_id, track_
+00006990: 6964 2c20 736f 7572 6365 5f73 6f75 7263  id, source_sourc
+000069a0: 655f 6964 2c20 7461 7267 6574 5f69 6429  e_id, target_id)
+000069b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
-00006a00: 6e74 726f 6964 732e 6170 7065 6e64 2873  ntroids.append(s
-00006a10: 706f 745f 6365 6e74 726f 6964 290d 0a20  pot_centroid).. 
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a40: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
-00006a50: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-00006a60: 2873 706f 745f 6365 6e74 726f 6964 7329  (spot_centroids)
-00006a70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006aa0: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
-00006ab0: 645b 7374 7228 7429 5d20 3d20 7472 6565  d[str(t)] = tree
-00006ac0: 2c20 7370 6f74 5f63 656e 7472 6f69 6473  , spot_centroids
-00006ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00006af0: 0d0a 2020 2020 6465 6620 5f6d 6173 7465  ..    def _maste
-00006b00: 725f 7472 6163 6b5f 636f 6d70 7574 6572  r_track_computer
-00006b10: 2873 656c 662c 2074 7261 636b 2c20 7472  (self, track, tr
-00006b20: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
+000069e0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000069f0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00006a00: 6573 5b74 6172 6765 745f 6964 5d2e 7570  es[target_id].up
+00006a10: 6461 7465 287b 7365 6c66 2e64 6976 6964  date({self.divid
+00006a20: 696e 675f 6b65 7920 3a20 6469 7669 6469  ing_key : dividi
+00006a30: 6e67 5f74 7261 6a65 6374 6f72 797d 2920  ng_trajectory}) 
+00006a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00006a80: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00006a90: 735b 7461 7267 6574 5f69 645d 2e75 7064  s[target_id].upd
+00006aa0: 6174 6528 7b73 656c 662e 6e75 6d62 6572  ate({self.number
+00006ab0: 5f64 6976 6964 696e 675f 6b65 7920 3a20  _dividing_key : 
+00006ac0: 6e75 6d62 6572 5f64 6976 6964 696e 677d  number_dividing}
+00006ad0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006af0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b40: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00006b40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b80: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00006b90: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bb0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00006bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bd0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 2061 6c6c 5f73 6f75 7263 655f 6964 732c   all_source_ids,
-00006c00: 2061 6c6c 5f74 6172 6765 745f 6964 7320   all_target_ids 
-00006c10: 3d20 2073 656c 662e 5f67 656e 6572 6174  =  self._generat
-00006c20: 655f 6765 6e65 7261 7469 6f6e 7328 7472  e_generations(tr
-00006c30: 6163 6b29 0d0a 2020 2020 2020 2020 2020  ack)..          
-00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c50: 2020 726f 6f74 5f72 6f6f 742c 2072 6f6f    root_root, roo
-00006c60: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
-00006c70: 6561 6620 3d20 7365 6c66 2e5f 6372 6561  eaf = self._crea
-00006c80: 7465 5f67 656e 6572 6174 696f 6e73 2861  te_generations(a
-00006c90: 6c6c 5f73 6f75 7263 655f 6964 732c 2061  ll_source_ids, a
-00006ca0: 6c6c 5f74 6172 6765 745f 6964 7329 200d  ll_target_ids) .
-00006cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006cc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006cd0: 662e 5f69 7465 7261 7465 5f73 706c 6974  f._iterate_split
-00006ce0: 5f64 6f77 6e28 726f 6f74 5f72 6f6f 742c  _down(root_root,
-00006cf0: 2072 6f6f 745f 6c65 6166 2c20 726f 6f74   root_leaf, root
-00006d00: 5f73 706c 6974 7329 0d0a 2020 2020 2020  _splits)..      
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00006b60: 2020 2020 2020 666f 7220 6375 7272 656e        for curren
+00006b70: 745f 726f 6f74 2069 6e20 726f 6f74 5f72  t_root in root_r
+00006b80: 6f6f 743a 0d0a 2020 2020 2020 2020 2020  oot:..          
+00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ba0: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
+00006bb0: 6f74 5f73 706f 7473 5b69 6e74 2863 7572  ot_spots[int(cur
+00006bc0: 7265 6e74 5f72 6f6f 7429 5d20 3d20 7365  rent_root)] = se
+00006bd0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00006be0: 726f 7065 7274 6965 735b 696e 7428 6375  roperties[int(cu
+00006bf0: 7272 656e 745f 726f 6f74 295d 0d0a 2020  rrent_root)]..  
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c30: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00006c40: 5f63 7572 7265 6e74 5f63 656c 6c5f 6964  _current_cell_id
+00006c50: 735b 696e 7428 7472 6163 6b5f 6964 295d  s[int(track_id)]
+00006c60: 203d 2063 7572 7265 6e74 5f63 656c 6c5f   = current_cell_
+00006c70: 6964 730d 0a20 2020 2020 2020 2020 2020  ids..           
+00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c90: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00006ca0: 6c65 6e28 6375 7272 656e 745f 6365 6c6c  len(current_cell
+00006cb0: 5f69 6473 2929 3a0d 0a20 2020 2020 2020  _ids)):..       
+00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ce0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d00: 2020 2020 2020 206b 203d 2069 6e74 2863         k = int(c
+00006d10: 7572 7265 6e74 5f63 656c 6c5f 6964 735b  urrent_cell_ids[
+00006d20: 695d 2920 2020 200d 0a20 2020 2020 2020  i])    ..       
 00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2320 4465 7465 726d 696e 6520      # Determine 
-00006d50: 6966 2061 2074 7261 636b 2068 6173 2064  if a track has d
-00006d60: 6976 6973 696f 6e73 206f 7220 6e6f 6e65  ivisions or none
-00006d70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006d80: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00006d90: 6d62 6572 5f64 6976 6964 696e 6720 3d20  mber_dividing = 
-00006da0: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
-00006db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006dd0: 206c 656e 2872 6f6f 745f 7370 6c69 7473   len(root_splits
-00006de0: 2920 3e20 303a 0d0a 2020 2020 2020 2020  ) > 0:..        
-00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e00: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00006e10: 7175 655f 7472 6163 6b5f 6d69 746f 7369  que_track_mitosi
-00006e20: 735f 6c61 6265 6c5b 7472 6163 6b5f 6964  s_label[track_id
-00006e30: 5d20 3d20 5b31 2c20 6e75 6d62 6572 5f64  ] = [1, number_d
-00006e40: 6976 6964 696e 675d 0d0a 2020 2020 2020  ividing]..      
+00006d40: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00006d50: 5f64 6963 745f 7661 6c75 6573 203d 2073  _dict_values = s
+00006d60: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00006d70: 7072 6f70 6572 7469 6573 5b6b 5d0d 0a20  properties[k].. 
+00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006da0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006dc0: 2020 2020 2020 2020 7420 3d20 696e 7428          t = int(
+00006dd0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+00006de0: 616c 7565 735b 7365 6c66 2e66 7261 6d65  alues[self.frame
+00006df0: 6964 5f6b 6579 5d29 290d 0a20 2020 2020  id_key]))..     
+00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e10: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+00006e20: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+00006e30: 745f 7661 6c75 6573 5b73 656c 662e 7a70  t_values[self.zp
+00006e40: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
 00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 2020 2020 2020 2020 6469 7669 6469            dividi
-00006e70: 6e67 5f74 7261 6a65 6374 6f72 7920 3d20  ng_trajectory = 
-00006e80: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
-00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ea0: 2020 2020 2020 6966 2069 6e74 2874 7261        if int(tra
-00006eb0: 636b 5f69 6429 206e 6f74 2069 6e20 7365  ck_id) not in se
-00006ec0: 6c66 2e41 6c6c 5472 6163 6b49 6473 3a0d  lf.AllTrackIds:.
-00006ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ef0: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
-00006f00: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
-00006f10: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
+00006e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e70: 7920 3d20 666c 6f61 7428 616c 6c5f 6469  y = float(all_di
+00006e80: 6374 5f76 616c 7565 735b 7365 6c66 2e79  ct_values[self.y
+00006e90: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ec0: 2078 203d 2066 6c6f 6174 2861 6c6c 5f64   x = float(all_d
+00006ed0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00006ee0: 7870 6f73 6964 5f6b 6579 5d29 0d0a 2020  xposid_key])..  
+00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f10: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
 00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00006f40: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
-00006f50: 7420 696e 2073 656c 662e 4469 7669 6469  t in self.Dividi
-00006f60: 6e67 5472 6163 6b49 6473 3a20 2020 2020  ngTrackIds:     
-00006f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f90: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
-00006fa0: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
-00006fb0: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
-00006fc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fe0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007000: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-00007040: 6b5f 6d69 746f 7369 735f 6c61 6265 6c5b  k_mitosis_label[
-00007050: 7472 6163 6b5f 6964 5d20 3d20 5b30 2c20  track_id] = [0, 
-00007060: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007080: 2020 2020 6469 7669 6469 6e67 5f74 7261      dividing_tra
-00007090: 6a65 6374 6f72 7920 3d20 4661 6c73 650d  jectory = False.
-000070a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
-000070d0: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
-000070e0: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
-000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006f40: 706f 745f 6365 6e74 726f 6964 203d 2028  pot_centroid = (
+00006f50: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
+00006f60: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
+00006f70: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
+00006f80: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
+00006f90: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
+00006fa0: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
+00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fc0: 2020 2020 2020 2020 2066 7261 6d65 5f73           frame_s
+00006fd0: 706f 745f 6365 6e74 726f 6964 203d 2028  pot_centroid = (
+00006fe0: 742c 726f 756e 6428 7a29 2f73 656c 662e  t,round(z)/self.
+00006ff0: 7a63 616c 6962 7261 7469 6f6e 2c20 726f  zcalibration, ro
+00007000: 756e 6428 7929 2f73 656c 662e 7963 616c  und(y)/self.ycal
+00007010: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
+00007020: 7829 2f73 656c 662e 7863 616c 6962 7261  x)/self.xcalibra
+00007030: 7469 6f6e 290d 0a0d 0a20 2020 2020 2020  tion)....       
+00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007050: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007060: 662e 756e 6971 7565 5f73 706f 745f 6365  f.unique_spot_ce
+00007070: 6e74 726f 6964 5b66 7261 6d65 5f73 706f  ntroid[frame_spo
+00007080: 745f 6365 6e74 726f 6964 5d20 3d20 6b0d  t_centroid] = k.
+00007090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070b0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000070c0: 5f74 7261 636b 5f63 656e 7472 6f69 645b  _track_centroid[
+000070d0: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
+000070e0: 6f69 645d 203d 2074 7261 636b 5f69 640d  oid] = track_id.
+000070f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-00007120: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
-00007130: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
+00007110: 2020 2020 2020 2069 6620 7374 7228 7429         if str(t)
+00007120: 2069 6e20 7365 6c66 2e5f 7469 6d65 645f   in self._timed_
+00007130: 6365 6e74 726f 6964 3a0d 0a20 2020 2020  centroid:..     
 00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
-00007160: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
-00007170: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-00007180: 4964 733a 2020 2020 0d0a 2020 2020 2020  Ids:    ..      
-00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000071b0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-000071c0: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
-000071d0: 636b 5f69 6429 290d 0a0d 0a20 2020 2020  ck_id))....     
-000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071f0: 2020 2020 2020 2066 6f72 206c 6561 6620         for leaf 
-00007200: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
-00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007230: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
-00007240: 6861 6e6e 656c 5f75 7064 6174 6528 6c65  hannel_update(le
-00007250: 6166 2c20 7472 6163 6b5f 6964 290d 0a20  af, track_id).. 
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007280: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
-00007290: 6473 2e61 7070 656e 6428 6c65 6166 2920  ds.append(leaf) 
-000072a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007160: 2020 2020 2020 7472 6565 2c20 7370 6f74        tree, spot
+00007170: 5f63 656e 7472 6f69 6473 203d 2073 656c  _centroids = sel
+00007180: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
+00007190: 645b 7374 7228 7429 5d0d 0a20 2020 2020  d[str(t)]..     
+000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071c0: 2020 2020 2020 7370 6f74 5f63 656e 7472        spot_centr
+000071d0: 6f69 6473 2e61 7070 656e 6428 7370 6f74  oids.append(spot
+000071e0: 5f63 656e 7472 6f69 6429 0d0a 2020 2020  _centroid)..    
+000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007210: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
+00007220: 6174 6961 6c2e 634b 4454 7265 6528 7370  atial.cKDTree(sp
+00007230: 6f74 5f63 656e 7472 6f69 6473 290d 0a20  ot_centroids).. 
+00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00007270: 7469 6d65 645f 6365 6e74 726f 6964 5b73  timed_centroid[s
+00007280: 7472 2874 295d 203d 2074 7265 652c 2073  tr(t)] = tree, s
+00007290: 706f 745f 6365 6e74 726f 6964 7320 0d0a  pot_centroids ..
+000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072c0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000072d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000072e0: 5b6c 6561 665d 2e75 7064 6174 6528 7b73  [leaf].update({s
-000072f0: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
-00007300: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
-00007310: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
+000072c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072f0: 2020 2020 2020 7370 6f74 5f63 656e 7472        spot_centr
+00007300: 6f69 6473 203d 205b 5d0d 0a20 2020 2020  oids = []..     
+00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007330: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007340: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00007350: 6f70 6572 7469 6573 5b6c 6561 665d 2e75  operties[leaf].u
-00007360: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
-00007370: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
-00007380: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
-00007390: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
-000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 2066 6f72 2073 6f75 7263 655f 6964 2069   for source_id i
-000073c0: 6e20 616c 6c5f 736f 7572 6365 5f69 6473  n all_source_ids
-000073d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000073e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073f0: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
-00007400: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
-00007410: 6528 736f 7572 6365 5f69 642c 2074 7261  e(source_id, tra
-00007420: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
-00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007440: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007450: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00007460: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
-00007470: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
-00007480: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
-00007490: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-000074a0: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
+00007330: 2020 2020 2020 7370 6f74 5f63 656e 7472        spot_centr
+00007340: 6f69 6473 2e61 7070 656e 6428 7370 6f74  oids.append(spot
+00007350: 5f63 656e 7472 6f69 6429 0d0a 2020 2020  _centroid)..    
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007380: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
+00007390: 6174 6961 6c2e 634b 4454 7265 6528 7370  atial.cKDTree(sp
+000073a0: 6f74 5f63 656e 7472 6f69 6473 290d 0a20  ot_centroids).. 
+000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000073e0: 7469 6d65 645f 6365 6e74 726f 6964 5b73  timed_centroid[s
+000073f0: 7472 2874 295d 203d 2074 7265 652c 2073  tr(t)] = tree, s
+00007400: 706f 745f 6365 6e74 726f 6964 730d 0a20  pot_centroids.. 
+00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007420: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00007430: 2020 2064 6566 205f 6d61 7374 6572 5f74     def _master_t
+00007440: 7261 636b 5f63 6f6d 7075 7465 7228 7365  rack_computer(se
+00007450: 6c66 2c20 7472 6163 6b2c 2074 7261 636b  lf, track, track
+00007460: 5f69 6429 3a0d 0a20 2020 2020 2020 2020  _id):..         
+00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007480: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00007490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074c0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000074d0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000074e0: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
-000074f0: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
-00007500: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
-00007510: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
-00007520: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
-00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007540: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00007550: 6365 6c6c 5f69 6473 2e61 7070 656e 6428  cell_ids.append(
-00007560: 736f 7572 6365 5f69 6429 0d0a 2020 2020  source_id)..    
-00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000075c0: 6375 7272 656e 745f 726f 6f74 2069 6e20  current_root in 
-000075d0: 726f 6f74 5f72 6f6f 743a 0d0a 2020 2020  root_root:..    
-000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007600: 656c 662e 5f73 6563 6f6e 645f 6368 616e  elf._second_chan
-00007610: 6e65 6c5f 7570 6461 7465 2863 7572 7265  nel_update(curre
-00007620: 6e74 5f72 6f6f 742c 2074 7261 636b 5f69  nt_root, track_i
-00007630: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007650: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
-00007660: 5f73 706f 7473 5b69 6e74 2863 7572 7265  _spots[int(curre
-00007670: 6e74 5f72 6f6f 7429 5d20 3d20 7365 6c66  nt_root)] = self
-00007680: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00007690: 7065 7274 6965 735b 696e 7428 6375 7272  perties[int(curr
-000076a0: 656e 745f 726f 6f74 295d 0d0a 2020 2020  ent_root)]..    
+000074c0: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
+000074d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007520: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00007530: 6c5f 736f 7572 6365 5f69 6473 2c20 616c  l_source_ids, al
+00007540: 6c5f 7461 7267 6574 5f69 6473 203d 2020  l_target_ids =  
+00007550: 7365 6c66 2e5f 6765 6e65 7261 7465 5f67  self._generate_g
+00007560: 656e 6572 6174 696f 6e73 2874 7261 636b  enerations(track
+00007570: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007580: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007590: 6f6f 745f 726f 6f74 2c20 726f 6f74 5f73  oot_root, root_s
+000075a0: 706c 6974 732c 2072 6f6f 745f 6c65 6166  plits, root_leaf
+000075b0: 203d 2073 656c 662e 5f63 7265 6174 655f   = self._create_
+000075c0: 6765 6e65 7261 7469 6f6e 7328 616c 6c5f  generations(all_
+000075d0: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
+000075e0: 7461 7267 6574 5f69 6473 2920 0d0a 2020  target_ids) ..  
+000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007600: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00007610: 6974 6572 6174 655f 7370 6c69 745f 646f  iterate_split_do
+00007620: 776e 2872 6f6f 745f 726f 6f74 2c20 726f  wn(root_root, ro
+00007630: 6f74 5f6c 6561 662c 2072 6f6f 745f 7370  ot_leaf, root_sp
+00007640: 6c69 7473 290d 0a20 2020 2020 2020 2020  lits)..         
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007680: 2023 2044 6574 6572 6d69 6e65 2069 6620   # Determine if 
+00007690: 6120 7472 6163 6b20 6861 7320 6469 7669  a track has divi
+000076a0: 7369 6f6e 7320 6f72 206e 6f6e 650d 0a20  sions or none.. 
 000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000076d0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000076e0: 7072 6f70 6572 7469 6573 5b73 6f75 7263  properties[sourc
-000076f0: 655f 6964 5d2e 7570 6461 7465 287b 7365  e_id].update({se
-00007700: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
-00007710: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
-00007720: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
+000076c0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+000076d0: 725f 6469 7669 6469 6e67 203d 206c 656e  r_dividing = len
+000076e0: 2872 6f6f 745f 7370 6c69 7473 290d 0a20  (root_splits).. 
+000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007700: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00007710: 6e28 726f 6f74 5f73 706c 6974 7329 203e  n(root_splits) >
+00007720: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
 00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007750: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00007760: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
-00007770: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
-00007780: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
-00007790: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
-000077a0: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00007740: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00007750: 5f74 7261 636b 5f6d 6974 6f73 6973 5f6c  _track_mitosis_l
+00007760: 6162 656c 5b74 7261 636b 5f69 645d 203d  abel[track_id] =
+00007770: 205b 312c 206e 756d 6265 725f 6469 7669   [1, number_divi
+00007780: 6469 6e67 5d0d 0a20 2020 2020 2020 2020  ding]..         
+00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077a0: 2020 2020 2020 2064 6976 6964 696e 675f         dividing_
+000077b0: 7472 616a 6563 746f 7279 203d 2054 7275  trajectory = Tru
+000077c0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
 000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077e0: 2020 2073 656c 662e 616c 6c5f 6375 7272     self.all_curr
-000077f0: 656e 745f 6365 6c6c 5f69 6473 5b69 6e74  ent_cell_ids[int
-00007800: 2874 7261 636b 5f69 6429 5d20 3d20 6375  (track_id)] = cu
-00007810: 7272 656e 745f 6365 6c6c 5f69 6473 0d0a  rrent_cell_ids..
+000077e0: 2020 2069 6620 696e 7428 7472 6163 6b5f     if int(track_
+000077f0: 6964 2920 6e6f 7420 696e 2073 656c 662e  id) not in self.
+00007800: 416c 6c54 7261 636b 4964 733a 0d0a 2020  AllTrackIds:..  
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00007860: 6e20 7261 6e67 6528 6c65 6e28 6375 7272  n range(len(curr
-00007870: 656e 745f 6365 6c6c 5f69 6473 2929 3a0d  ent_cell_ids)):.
-00007880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00007830: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+00007840: 6473 2e61 7070 656e 6428 696e 7428 7472  ds.append(int(tr
+00007850: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
+00007860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007870: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
+00007880: 2874 7261 636b 5f69 6429 206e 6f74 2069  (track_id) not i
+00007890: 6e20 7365 6c66 2e44 6976 6964 696e 6754  n self.DividingT
+000078a0: 7261 636b 4964 733a 2020 2020 200d 0a20  rackIds:     .. 
 000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078c0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-000078d0: 203d 2069 6e74 2863 7572 7265 6e74 5f63   = int(current_c
-000078e0: 656c 6c5f 6964 735b 695d 2920 2020 0d0a  ell_ids[i])   ..
-000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078d0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
+000078e0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+000078f0: 696e 7428 7472 6163 6b5f 6964 2929 0d0a  int(track_id))..
 00007900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007930: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-00007940: 6374 5f76 616c 7565 7320 3d20 7365 6c66  ct_values = self
-00007950: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00007960: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
-00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079b0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079d0: 2020 2020 2020 2020 2020 7420 3d20 696e            t = in
-000079e0: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
-000079f0: 5f76 616c 7565 735b 7365 6c66 2e66 7261  _values[self.fra
-00007a00: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
-00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a30: 207a 203d 2066 6c6f 6174 2861 6c6c 5f64   z = float(all_d
-00007a40: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00007a50: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a80: 2020 7920 3d20 666c 6f61 7428 616c 6c5f    y = float(all_
-00007a90: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00007aa0: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 2020 2078 203d 2066 6c6f 6174 2861 6c6c     x = float(all
-00007ae0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-00007af0: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
-00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b20: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b40: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00007b50: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
-00007b60: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
-00007b70: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-00007b80: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
-00007b90: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-00007ba0: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
-00007bb0: 6272 6174 696f 6e29 200d 0a0d 0a20 2020  bration) ....   
-00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00007bf0: 745f 6365 6e74 726f 6964 5b66 7261 6d65  t_centroid[frame
-00007c00: 5f73 706f 745f 6365 6e74 726f 6964 5d20  _spot_centroid] 
-00007c10: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c30: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00007c40: 6971 7565 5f74 7261 636b 5f63 656e 7472  ique_track_centr
-00007c50: 6f69 645b 6672 616d 655f 7370 6f74 5f63  oid[frame_spot_c
-00007c60: 656e 7472 6f69 645d 203d 2074 7261 636b  entroid] = track
-00007c70: 5f69 640d 0a20 2020 2020 2020 2020 2020  _id..           
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00007ca0: 6620 5f73 6563 6f6e 645f 6368 616e 6e65  f _second_channe
-00007cb0: 6c5f 7570 6461 7465 2873 656c 662c 2063  l_update(self, c
-00007cc0: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
-00007cd0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00007ce0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00007cf0: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-00007d00: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-00007d10: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00007d20: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00007d30: 2020 2020 2020 2020 6672 616d 6520 3d20          frame = 
-00007d40: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00007d50: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00007d60: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e66  cell_id)][self.f
-00007d70: 7261 6d65 6964 5f6b 6579 5d0d 0a20 2020  rameid_key]..   
-00007d80: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-00007d90: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00007da0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00007db0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00007dc0: 7a70 6f73 6964 5f6b 6579 5d2f 7365 6c66  zposid_key]/self
-00007dd0: 2e7a 6361 6c69 6272 6174 696f 6e0d 0a20  .zcalibration.. 
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00007df0: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
-00007e00: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00007e10: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00007e20: 662e 7970 6f73 6964 5f6b 6579 5d2f 7365  f.yposid_key]/se
-00007e30: 6c66 2e79 6361 6c69 6272 6174 696f 6e0d  lf.ycalibration.
-00007e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e50: 2078 203d 2073 656c 662e 756e 6971 7565   x = self.unique
-00007e60: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00007e70: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00007e80: 656c 662e 7870 6f73 6964 5f6b 6579 5d2f  elf.xposid_key]/
-00007e90: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00007ea0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00007eb0: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
-00007ec0: 6368 616e 6e65 6c5f 7370 6f74 7328 6672  channel_spots(fr
-00007ed0: 616d 652c 207a 2c20 792c 2078 2c20 6365  ame, z, y, x, ce
-00007ee0: 6c6c 5f69 642c 2074 7261 636b 5f69 6429  ll_id, track_id)
-00007ef0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00007f00: 6465 6620 5f66 696e 616c 5f74 7261 636b  def _final_track
-00007f10: 7328 7365 6c66 2c20 7472 6163 6b5f 6964  s(self, track_id
-00007f20: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
-00007f50: 6473 203d 2073 656c 662e 616c 6c5f 6375  ds = self.all_cu
-00007f60: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
-00007f70: 6e74 2874 7261 636b 5f69 6429 5d0d 0a20  nt(track_id)].. 
+00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007920: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007940: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007970: 662e 756e 6971 7565 5f74 7261 636b 5f6d  f.unique_track_m
+00007980: 6974 6f73 6973 5f6c 6162 656c 5b74 7261  itosis_label[tra
+00007990: 636b 5f69 645d 203d 205b 302c 2030 5d0d  ck_id] = [0, 0].
+000079a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079c0: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
+000079d0: 746f 7279 203d 2046 616c 7365 0d0a 2020  tory = False..  
+000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007a00: 2069 6e74 2874 7261 636b 5f69 6429 206e   int(track_id) n
+00007a10: 6f74 2069 6e20 7365 6c66 2e41 6c6c 5472  ot in self.AllTr
+00007a20: 6163 6b49 6473 3a0d 0a20 2020 2020 2020  ackIds:..       
+00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007a50: 662e 416c 6c54 7261 636b 4964 732e 6170  f.AllTrackIds.ap
+00007a60: 7065 6e64 2869 6e74 2874 7261 636b 5f69  pend(int(track_i
+00007a70: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
+00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a90: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
+00007aa0: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
+00007ab0: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
+00007ac0: 3a20 2020 200d 0a20 2020 2020 2020 2020  :    ..         
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007af0: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
+00007b00: 7070 656e 6428 696e 7428 7472 6163 6b5f  ppend(int(track_
+00007b10: 6964 2929 0d0a 0d0a 2020 2020 2020 2020  id))....        
+00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b30: 2020 2020 666f 7220 6c65 6166 2069 6e20      for leaf in 
+00007b40: 726f 6f74 5f6c 6561 663a 0d0a 2020 2020  root_leaf:..    
+00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007b70: 656c 662e 5f73 6563 6f6e 645f 6368 616e  elf._second_chan
+00007b80: 6e65 6c5f 7570 6461 7465 286c 6561 662c  nel_update(leaf,
+00007b90: 2074 7261 636b 5f69 6429 0d0a 2020 2020   track_id)..    
+00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00007bc0: 7572 7265 6e74 5f63 656c 6c5f 6964 732e  urrent_cell_ids.
+00007bd0: 6170 7065 6e64 286c 6561 6629 200d 0a20  append(leaf) .. 
+00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c00: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00007c10: 6f74 5f70 726f 7065 7274 6965 735b 6c65  ot_properties[le
+00007c20: 6166 5d2e 7570 6461 7465 287b 7365 6c66  af].update({self
+00007c30: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
+00007c40: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
+00007c50: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
+00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c70: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007c80: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00007c90: 7274 6965 735b 6c65 6166 5d2e 7570 6461  rties[leaf].upda
+00007ca0: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
+00007cb0: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
+00007cc0: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
+00007cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007ce0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00007cf0: 7220 736f 7572 6365 5f69 6420 696e 2061  r source_id in a
+00007d00: 6c6c 5f73 6f75 7263 655f 6964 733a 0d0a  ll_source_ids:..
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d30: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
+00007d40: 6368 616e 6e65 6c5f 7570 6461 7465 2873  channel_update(s
+00007d50: 6f75 7263 655f 6964 2c20 7472 6163 6b5f  ource_id, track_
+00007d60: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
+00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d80: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00007d90: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00007da0: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
+00007db0: 7064 6174 6528 7b73 656c 662e 6469 7669  pdate({self.divi
+00007dc0: 6469 6e67 5f6b 6579 203a 2064 6976 6964  ding_key : divid
+00007dd0: 696e 675f 7472 616a 6563 746f 7279 7d29  ing_trajectory})
+00007de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e00: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00007e10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00007e20: 5b73 6f75 7263 655f 6964 5d2e 7570 6461  [source_id].upda
+00007e30: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
+00007e40: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
+00007e50: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
+00007e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e80: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
+00007e90: 6c5f 6964 732e 6170 7065 6e64 2873 6f75  l_ids.append(sou
+00007ea0: 7263 655f 6964 290d 0a20 2020 2020 2020  rce_id)..       
+00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ed0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ef0: 2020 2020 2020 2020 2066 6f72 2063 7572           for cur
+00007f00: 7265 6e74 5f72 6f6f 7420 696e 2072 6f6f  rent_root in roo
+00007f10: 745f 726f 6f74 3a0d 0a20 2020 2020 2020  t_root:..       
+00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007f40: 2e5f 7365 636f 6e64 5f63 6861 6e6e 656c  ._second_channel
+00007f50: 5f75 7064 6174 6528 6375 7272 656e 745f  _update(current_
+00007f60: 726f 6f74 2c20 7472 6163 6b5f 6964 290d  root, track_id).
+00007f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f90: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00007fa0: 6e74 5f74 7261 636b 6c65 7473 203d 207b  nt_tracklets = {
-00007fb0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00007fc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00007fd0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00007fe0: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-00007ff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008000: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008020: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008030: 6920 696e 2072 616e 6765 286c 656e 2863  i in range(len(c
-00008040: 7572 7265 6e74 5f63 656c 6c5f 6964 7329  urrent_cell_ids)
-00008050: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008070: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080a0: 2020 6b20 3d20 696e 7428 6375 7272 656e    k = int(curren
-000080b0: 745f 6365 6c6c 5f69 6473 5b69 5d29 2020  t_cell_ids[i])  
-000080c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080e0: 2020 2020 2020 2020 616c 6c5f 6469 6374          all_dict
-000080f0: 5f76 616c 7565 7320 3d20 7365 6c66 2e75  _values = self.u
-00008100: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00008110: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
-00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008130: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00008140: 6971 7565 5f69 6420 3d20 7374 7228 616c  ique_id = str(al
-00008150: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00008160: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
-00008170: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007f90: 2020 2020 7365 6c66 2e72 6f6f 745f 7370      self.root_sp
+00007fa0: 6f74 735b 696e 7428 6375 7272 656e 745f  ots[int(current_
+00007fb0: 726f 6f74 295d 203d 2073 656c 662e 756e  root)] = self.un
+00007fc0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00007fd0: 7469 6573 5b69 6e74 2863 7572 7265 6e74  ties[int(current
+00007fe0: 5f72 6f6f 7429 5d0d 0a20 2020 2020 2020  _root)]..       
+00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008010: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00008020: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
+00008030: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00008040: 6469 7669 6469 6e67 5f6b 6579 203a 2064  dividing_key : d
+00008050: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
+00008060: 7279 7d29 0d0a 2020 2020 2020 2020 2020  ry})..          
+00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008080: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00008090: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000080a0: 7469 6573 5b73 6f75 7263 655f 6964 5d2e  ties[source_id].
+000080b0: 7570 6461 7465 287b 7365 6c66 2e6e 756d  update({self.num
+000080c0: 6265 725f 6469 7669 6469 6e67 5f6b 6579  ber_dividing_key
+000080d0: 203a 206e 756d 6265 725f 6469 7669 6469   : number_dividi
+000080e0: 6e67 7d29 0d0a 2020 2020 2020 2020 2020  ng})..          
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008100: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008120: 7365 6c66 2e61 6c6c 5f63 7572 7265 6e74  self.all_current
+00008130: 5f63 656c 6c5f 6964 735b 696e 7428 7472  _cell_ids[int(tr
+00008140: 6163 6b5f 6964 295d 203d 2063 7572 7265  ack_id)] = curre
+00008150: 6e74 5f63 656c 6c5f 6964 730d 0a20 2020  nt_cell_ids..   
+00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008190: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-000081a0: 7261 636b 5f69 6420 3d20 7374 7228 616c  rack_id = str(al
-000081b0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-000081c0: 6c66 2e74 7261 636b 6964 5f6b 6579 5d29  lf.trackid_key])
-000081d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081f0: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
-00008200: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00008210: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
-00008220: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
+00008190: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+000081a0: 616e 6765 286c 656e 2863 7572 7265 6e74  ange(len(current
+000081b0: 5f63 656c 6c5f 6964 7329 293a 0d0a 2020  _cell_ids)):..  
+000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008200: 2020 2020 2020 2020 2020 2020 6b20 3d20              k = 
+00008210: 696e 7428 6375 7272 656e 745f 6365 6c6c  int(current_cell
+00008220: 5f69 6473 5b69 5d29 2020 200d 0a20 2020  _ids[i])   ..   
 00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-00008250: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00008260: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
-00008270: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008290: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-000082a0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-000082b0: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
-000082c0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008250: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 2020 2020 2061 6c6c 5f64 6963 745f         all_dict_
+00008280: 7661 6c75 6573 203d 2073 656c 662e 756e  values = self.un
+00008290: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000082a0: 7469 6573 5b6b 5d0d 0a20 2020 2020 2020  ties[k]..       
+000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082c0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082e0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-000082f0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00008300: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
-00008310: 6f73 6964 5f6b 6579 5d29 0d0a 0d0a 2020  osid_key])....  
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008340: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
-00008350: 6574 732c 2063 7572 7265 6e74 5f74 7261  ets, current_tra
-00008360: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-00008370: 7320 3d20 7365 6c66 2e5f 7472 6163 6b6c  s = self._trackl
-00008380: 6574 5f61 6e64 5f70 726f 7065 7274 6965  et_and_propertie
-00008390: 7328 616c 6c5f 6469 6374 5f76 616c 7565  s(all_dict_value
-000083a0: 732c 2074 2c20 7a2c 2079 2c20 782c 206b  s, t, z, y, x, k
-000083b0: 2c20 6375 7272 656e 745f 7472 6163 6b5f  , current_track_
-000083c0: 6964 2c20 756e 6971 7565 5f69 642c 2063  id, unique_id, c
-000083d0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-000083e0: 2c20 6375 7272 656e 745f 7472 6163 6b6c  , current_trackl
-000083f0: 6574 735f 7072 6f70 6572 7469 6573 290d  ets_properties).
-00008400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008420: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-00008430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008440: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-00008450: 636b 6c65 7473 203d 206e 702e 6173 6172  cklets = np.asar
-00008460: 7261 7928 6375 7272 656e 745f 7472 6163  ray(current_trac
-00008470: 6b6c 6574 735b 7374 7228 7472 6163 6b5f  klets[str(track_
-00008480: 6964 295d 2c20 6474 7970 653d 6e70 2e66  id)], dtype=np.f
-00008490: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084b0: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-000084c0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-000084d0: 7320 3d20 6e70 2e61 7361 7272 6179 2863  s = np.asarray(c
-000084e0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-000084f0: 5f70 726f 7065 7274 6965 735b 7374 7228  _properties[str(
-00008500: 7472 6163 6b5f 6964 295d 2c20 6474 7970  track_id)], dtyp
-00008510: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00008560: 6971 7565 5f74 7261 636b 735b 7472 6163  ique_tracks[trac
-00008570: 6b5f 6964 5d20 3d20 6375 7272 656e 745f  k_id] = current_
-00008580: 7472 6163 6b6c 6574 7320 2020 2020 0d0a  tracklets     ..
-00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000085b0: 2e75 6e69 7175 655f 7472 6163 6b5f 7072  .unique_track_pr
-000085c0: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-000085d0: 645d 203d 2063 7572 7265 6e74 5f74 7261  d] = current_tra
-000085e0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-000085f0: 7320 2020 200d 0a0d 0a20 2020 2064 6566  s    ....    def
-00008600: 205f 7472 6163 6b6c 6574 5f61 6e64 5f70   _tracklet_and_p
-00008610: 726f 7065 7274 6965 7328 7365 6c66 2c20  roperties(self, 
-00008620: 616c 6c5f 6469 6374 5f76 616c 7565 732c  all_dict_values,
-00008630: 2074 2c20 7a2c 2079 2c20 782c 206b 2c20   t, z, y, x, k, 
-00008640: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
-00008650: 2c20 756e 6971 7565 5f69 642c 2063 7572  , unique_id, cur
-00008660: 7265 6e74 5f74 7261 636b 6c65 7473 2c20  rent_tracklets, 
-00008670: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00008680: 735f 7072 6f70 6572 7469 6573 293a 0d0a  s_properties):..
-00008690: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086c0: 2067 656e 5f69 6420 3d20 696e 7428 666c   gen_id = int(fl
-000086d0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-000086e0: 7565 735b 7365 6c66 2e67 656e 6572 6174  ues[self.generat
-000086f0: 696f 6e69 645f 6b65 795d 2929 0d0a 2020  ionid_key]))..  
-00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008720: 2020 7370 6565 6420 3d20 666c 6f61 7428    speed = float(
-00008730: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00008740: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
-00008750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2020 2020 2020 6163 6365 6c65 7261 7469        accelerati
-00008780: 6f6e 203d 2066 6c6f 6174 2861 6c6c 5f64  on = float(all_d
-00008790: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-000087a0: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-000087b0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087d0: 2020 2020 2020 2020 6d6f 7469 6f6e 5f61          motion_a
-000087e0: 6e67 6c65 203d 2066 6c6f 6174 2861 6c6c  ngle = float(all
-000087f0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-00008800: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
-00008810: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 2020 2020 2020 2020 2020 7261 6469 616c            radial
-00008840: 5f61 6e67 6c65 203d 2066 6c6f 6174 2861  _angle = float(a
-00008850: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00008860: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
-00008870: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00008880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008890: 2020 2020 2020 2020 2020 2020 7261 6469              radi
-000088a0: 7573 203d 2066 6c6f 6174 2861 6c6c 5f64  us = float(all_d
-000088b0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-000088c0: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088f0: 2020 766f 6c75 6d65 5f70 6978 656c 7320    volume_pixels 
-00008900: 3d20 696e 7428 666c 6f61 7428 616c 6c5f  = int(float(all_
-00008910: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00008920: 2e71 7561 6c69 7479 5f6b 6579 5d29 290d  .quality_key])).
-00008930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008950: 2020 2020 2074 6f74 616c 5f69 6e74 656e       total_inten
-00008960: 7369 7479 203d 2020 666c 6f61 7428 616c  sity =  float(al
-00008970: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00008980: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-00008990: 7479 5f6b 6579 5d29 0d0a 2020 2020 2020  ty_key])..      
+000082e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008310: 2020 2020 2020 2074 203d 2069 6e74 2866         t = int(f
+00008320: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
+00008330: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
+00008340: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
+00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008360: 2020 2020 2020 2020 2020 2020 2020 7a20                z 
+00008370: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+00008380: 5f76 616c 7565 735b 7365 6c66 2e7a 706f  _values[self.zpo
+00008390: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083b0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+000083c0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+000083d0: 745f 7661 6c75 6573 5b73 656c 662e 7970  t_values[self.yp
+000083e0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008410: 7820 3d20 666c 6f61 7428 616c 6c5f 6469  x = float(all_di
+00008420: 6374 5f76 616c 7565 735b 7365 6c66 2e78  ct_values[self.x
+00008430: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008460: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008480: 2020 2020 2020 2020 2066 7261 6d65 5f73           frame_s
+00008490: 706f 745f 6365 6e74 726f 6964 203d 2028  pot_centroid = (
+000084a0: 742c 726f 756e 6428 7a29 2f73 656c 662e  t,round(z)/self.
+000084b0: 7a63 616c 6962 7261 7469 6f6e 2c20 726f  zcalibration, ro
+000084c0: 756e 6428 7929 2f73 656c 662e 7963 616c  und(y)/self.ycal
+000084d0: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
+000084e0: 7829 2f73 656c 662e 7863 616c 6962 7261  x)/self.xcalibra
+000084f0: 7469 6f6e 2920 0d0a 0d0a 2020 2020 2020  tion) ....      
+00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008510: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008520: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
+00008530: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
+00008540: 6f74 5f63 656e 7472 6f69 645d 203d 206b  ot_centroid] = k
+00008550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00008580: 655f 7472 6163 6b5f 6365 6e74 726f 6964  e_track_centroid
+00008590: 5b66 7261 6d65 5f73 706f 745f 6365 6e74  [frame_spot_cent
+000085a0: 726f 6964 5d20 3d20 7472 6163 6b5f 6964  roid] = track_id
+000085b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085d0: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
+000085e0: 7365 636f 6e64 5f63 6861 6e6e 656c 5f75  second_channel_u
+000085f0: 7064 6174 6528 7365 6c66 2c20 6365 6c6c  pdate(self, cell
+00008600: 5f69 642c 2074 7261 636b 5f69 6429 3a0d  _id, track_id):.
+00008610: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00008620: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00008630: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+00008640: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+00008650: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00008660: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00008670: 2020 2020 2066 7261 6d65 203d 2073 656c       frame = sel
+00008680: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00008690: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+000086a0: 6c5f 6964 295d 5b73 656c 662e 6672 616d  l_id)][self.fram
+000086b0: 6569 645f 6b65 795d 0d0a 2020 2020 2020  eid_key]..      
+000086c0: 2020 2020 2020 2020 2020 7a20 3d20 7365            z = se
+000086d0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000086e0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000086f0: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
+00008700: 7369 645f 6b65 795d 2f73 656c 662e 7a63  sid_key]/self.zc
+00008710: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00008720: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+00008730: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00008740: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00008750: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
+00008760: 706f 7369 645f 6b65 795d 2f73 656c 662e  posid_key]/self.
+00008770: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+00008780: 2020 2020 2020 2020 2020 2020 2020 7820                x 
+00008790: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+000087a0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000087b0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+000087c0: 2e78 706f 7369 645f 6b65 795d 2f73 656c  .xposid_key]/sel
+000087d0: 662e 7863 616c 6962 7261 7469 6f6e 0d0a  f.xcalibration..
+000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087f0: 7365 6c66 2e5f 7365 636f 6e64 5f63 6861  self._second_cha
+00008800: 6e6e 656c 5f73 706f 7473 2866 7261 6d65  nnel_spots(frame
+00008810: 2c20 7a2c 2079 2c20 782c 2063 656c 6c5f  , z, y, x, cell_
+00008820: 6964 2c20 7472 6163 6b5f 6964 290d 0a20  id, track_id).. 
+00008830: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00008840: 205f 6669 6e61 6c5f 7472 6163 6b73 2873   _final_tracks(s
+00008850: 656c 662c 2074 7261 636b 5f69 6429 3a0d  elf, track_id):.
+00008860: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00008870: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008880: 7572 7265 6e74 5f63 656c 6c5f 6964 7320  urrent_cell_ids 
+00008890: 3d20 7365 6c66 2e61 6c6c 5f63 7572 7265  = self.all_curre
+000088a0: 6e74 5f63 656c 6c5f 6964 735b 696e 7428  nt_cell_ids[int(
+000088b0: 7472 6163 6b5f 6964 295d 0d0a 2020 2020  track_id)]..    
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088d0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000088e0: 7472 6163 6b6c 6574 7320 3d20 7b7d 0d0a  tracklets = {}..
+000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008900: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00008910: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
+00008920: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
+00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008940: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008960: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00008970: 6e20 7261 6e67 6528 6c65 6e28 6375 7272  n range(len(curr
+00008980: 656e 745f 6365 6c6c 5f69 6473 2929 3a0d  ent_cell_ids)):.
+00008990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000089b0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
-000089f0: 5f6d 6173 6b20 3d20 666c 6f61 7428 616c  _mask = float(al
-00008a00: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00008a10: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-00008a20: 5f6d 6173 6b5f 6b65 795d 290d 0a0d 0a20  _mask_key]).... 
-00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a50: 2020 2069 6620 7365 6c66 2e73 7572 6661     if self.surfa
-00008a60: 6365 5f61 7265 615f 6b65 7920 696e 2061  ce_area_key in a
-00008a70: 6c6c 5f64 6963 745f 7661 6c75 6573 2e6b  ll_dict_values.k
-00008a80: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-00008a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ab0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000089d0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+000089e0: 203d 2069 6e74 2863 7572 7265 6e74 5f63   = int(current_c
+000089f0: 656c 6c5f 6964 735b 695d 2920 2020 200d  ell_ids[i])    .
+00008a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a20: 2020 2020 2061 6c6c 5f64 6963 745f 7661       all_dict_va
+00008a30: 6c75 6573 203d 2073 656c 662e 756e 6971  lues = self.uniq
+00008a40: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00008a50: 6573 5b6b 5d0d 0a20 2020 2020 2020 2020  es[k]..         
+00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a70: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00008a80: 655f 6964 203d 2073 7472 2861 6c6c 5f64  e_id = str(all_d
+00008a90: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00008aa0: 756e 6971 7565 6964 5f6b 6579 5d29 0d0a  uniqueid_key])..
+00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ae0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00008af0: 705f 6669 7273 7420 3d20 666c 6f61 7428  p_first = float(
-00008b00: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00008b10: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-00008b20: 795f 636f 6d70 5f66 6972 7374 6b65 795d  y_comp_firstkey]
-00008b30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b50: 2020 2020 2020 2020 2020 2020 2020 6563                ec
-00008b60: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00008b70: 7365 636f 6e64 203d 2066 6c6f 6174 2861  second = float(a
-00008b80: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00008b90: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
-00008ba0: 5f63 6f6d 705f 7365 636f 6e64 6b65 795d  _comp_secondkey]
-00008bb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00008ad0: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00008ae0: 6b5f 6964 203d 2073 7472 2861 6c6c 5f64  k_id = str(all_d
+00008af0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00008b00: 7472 6163 6b69 645f 6b65 795d 290d 0a20  trackid_key]).. 
+00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b30: 2020 2074 203d 2069 6e74 2866 6c6f 6174     t = int(float
+00008b40: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00008b50: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
+00008b60: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
+00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b80: 2020 2020 2020 2020 2020 7a20 3d20 666c            z = fl
+00008b90: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+00008ba0: 7565 735b 7365 6c66 2e7a 706f 7369 645f  ues[self.zposid_
+00008bb0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
 00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bd0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00008be0: 7266 6163 655f 6172 6561 203d 2066 6c6f  rface_area = flo
-00008bf0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00008c00: 6573 5b73 656c 662e 7375 7266 6163 655f  es[self.surface_
-00008c10: 6172 6561 5f6b 6579 5d29 0d0a 2020 2020  area_key])..    
-00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c40: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
-00008c50: 5f6d 6173 6b20 3d20 666c 6f61 7428 616c  _mask = float(al
-00008c60: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-00008c70: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
-00008c80: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cb0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00008cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ce0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00008d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d30: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
-00008d40: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00008d50: 6972 7374 203d 202d 310d 0a20 2020 2020  irst = -1..     
-00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bd0: 2020 2020 2020 2020 2020 2079 203d 2066             y = f
+00008be0: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
+00008bf0: 6c75 6573 5b73 656c 662e 7970 6f73 6964  lues[self.yposid
+00008c00: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00008c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c20: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+00008c30: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+00008c40: 616c 7565 735b 7365 6c66 2e78 706f 7369  alues[self.xposi
+00008c50: 645f 6b65 795d 290d 0a0d 0a20 2020 2020  d_key])....     
+00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008c80: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00008c90: 2c20 6375 7272 656e 745f 7472 6163 6b6c  , current_trackl
+00008ca0: 6574 735f 7072 6f70 6572 7469 6573 203d  ets_properties =
+00008cb0: 2073 656c 662e 5f74 7261 636b 6c65 745f   self._tracklet_
+00008cc0: 616e 645f 7072 6f70 6572 7469 6573 2861  and_properties(a
+00008cd0: 6c6c 5f64 6963 745f 7661 6c75 6573 2c20  ll_dict_values, 
+00008ce0: 742c 207a 2c20 792c 2078 2c20 6b2c 2063  t, z, y, x, k, c
+00008cf0: 7572 7265 6e74 5f74 7261 636b 5f69 642c  urrent_track_id,
+00008d00: 2075 6e69 7175 655f 6964 2c20 6375 7272   unique_id, curr
+00008d10: 656e 745f 7472 6163 6b6c 6574 732c 2063  ent_tracklets, c
+00008d20: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00008d30: 5f70 726f 7065 7274 6965 7329 0d0a 2020  _properties)..  
+00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d60: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
 00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d80: 2020 2020 2020 2065 6363 656e 7472 6963         eccentric
-00008d90: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
-00008da0: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
-00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dd0: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
-00008de0: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
-00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e10: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
-00008e20: 3d20 2d31 2020 2020 200d 0a0d 0a20 2020  = -1     ....   
-00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e50: 2066 7261 6d65 5f73 706f 745f 6365 6e74   frame_spot_cent
-00008e60: 726f 6964 203d 2028 742c 726f 756e 6428  roid = (t,round(
-00008e70: 7a29 2f73 656c 662e 7a63 616c 6962 7261  z)/self.zcalibra
-00008e80: 7469 6f6e 2c20 726f 756e 6428 7929 2f73  tion, round(y)/s
-00008e90: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00008ea0: 2c20 726f 756e 6428 7829 2f73 656c 662e  , round(x)/self.
-00008eb0: 7863 616c 6962 7261 7469 6f6e 2920 0d0a  xcalibration) ..
-00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d80: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+00008d90: 6574 7320 3d20 6e70 2e61 7361 7272 6179  ets = np.asarray
+00008da0: 2863 7572 7265 6e74 5f74 7261 636b 6c65  (current_trackle
+00008db0: 7473 5b73 7472 2874 7261 636b 5f69 6429  ts[str(track_id)
+00008dc0: 5d2c 2064 7479 7065 3d6e 702e 666c 6f61  ], dtype=np.floa
+00008dd0: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008df0: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+00008e00: 6574 735f 7072 6f70 6572 7469 6573 203d  ets_properties =
+00008e10: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00008e20: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
+00008e30: 6f70 6572 7469 6573 5b73 7472 2874 7261  operties[str(tra
+00008e40: 636b 5f69 6429 5d2c 2064 7479 7065 3d6e  ck_id)], dtype=n
+00008e50: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
+00008e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e90: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00008ea0: 655f 7472 6163 6b73 5b74 7261 636b 5f69  e_tracks[track_i
+00008eb0: 645d 203d 2063 7572 7265 6e74 5f74 7261  d] = current_tra
+00008ec0: 636b 6c65 7473 2020 2020 200d 0a20 2020  cklets     ..   
 00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ee0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00008ef0: 7370 6f74 5f63 656e 7472 6f69 645b 6672  spot_centroid[fr
-00008f00: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
-00008f10: 645d 203d 206b 0d0a 0d0a 2020 2020 2020  d] = k....      
-00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f30: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00008f40: 2063 7572 7265 6e74 5f74 7261 636b 5f69   current_track_i
-00008f50: 6420 696e 2063 7572 7265 6e74 5f74 7261  d in current_tra
-00008f60: 636b 6c65 7473 3a0d 0a20 2020 2020 2020  cklets:..       
-00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f90: 2074 7261 636b 6c65 745f 6172 7261 7920   tracklet_array 
-00008fa0: 3d20 6375 7272 656e 745f 7472 6163 6b6c  = current_trackl
-00008fb0: 6574 735b 6375 7272 656e 745f 7472 6163  ets[current_trac
-00008fc0: 6b5f 6964 5d0d 0a20 2020 2020 2020 2020  k_id]..         
-00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fe0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00008ff0: 7572 7265 6e74 5f74 7261 636b 6c65 745f  urrent_tracklet_
-00009000: 6172 7261 7920 3d20 6e70 2e61 7272 6179  array = np.array
-00009010: 285b 696e 7428 666c 6f61 7428 756e 6971  ([int(float(uniq
-00009020: 7565 5f69 6429 292c 2074 2c20 7a2f 7365  ue_id)), t, z/se
-00009030: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-00009040: 2079 2f73 656c 662e 7963 616c 6962 7261   y/self.ycalibra
-00009050: 7469 6f6e 2c20 782f 7365 6c66 2e78 6361  tion, x/self.xca
-00009060: 6c69 6272 6174 696f 6e5d 290d 0a20 2020  libration])..   
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009090: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-000090a0: 636b 6c65 7473 5b63 7572 7265 6e74 5f74  cklets[current_t
-000090b0: 7261 636b 5f69 645d 203d 206e 702e 7673  rack_id] = np.vs
-000090c0: 7461 636b 2828 7472 6163 6b6c 6574 5f61  tack((tracklet_a
-000090d0: 7272 6179 2c20 6375 7272 656e 745f 7472  rray, current_tr
-000090e0: 6163 6b6c 6574 5f61 7272 6179 2929 0d0a  acklet_array))..
-000090f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008ee0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00008ef0: 6971 7565 5f74 7261 636b 5f70 726f 7065  ique_track_prope
+00008f00: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
+00008f10: 3d20 6375 7272 656e 745f 7472 6163 6b6c  = current_trackl
+00008f20: 6574 735f 7072 6f70 6572 7469 6573 2020  ets_properties  
+00008f30: 2020 0d0a 0d0a 2020 2020 6465 6620 5f74    ....    def _t
+00008f40: 7261 636b 6c65 745f 616e 645f 7072 6f70  racklet_and_prop
+00008f50: 6572 7469 6573 2873 656c 662c 2061 6c6c  erties(self, all
+00008f60: 5f64 6963 745f 7661 6c75 6573 2c20 742c  _dict_values, t,
+00008f70: 207a 2c20 792c 2078 2c20 6b2c 2063 7572   z, y, x, k, cur
+00008f80: 7265 6e74 5f74 7261 636b 5f69 642c 2075  rent_track_id, u
+00008f90: 6e69 7175 655f 6964 2c20 6375 7272 656e  nique_id, curren
+00008fa0: 745f 7472 6163 6b6c 6574 732c 2063 7572  t_tracklets, cur
+00008fb0: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
+00008fc0: 726f 7065 7274 6965 7329 3a0d 0a20 2020  roperties):..   
+00008fd0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ff0: 2020 2020 2020 2020 2020 2020 2020 6765                ge
+00009000: 6e5f 6964 203d 2069 6e74 2866 6c6f 6174  n_id = int(float
+00009010: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00009020: 5b73 656c 662e 6765 6e65 7261 7469 6f6e  [self.generation
+00009030: 6964 5f6b 6579 5d29 290d 0a20 2020 2020  id_key]))..     
+00009040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009050: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009060: 7065 6564 203d 2066 6c6f 6174 2861 6c6c  peed = float(all
+00009070: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00009080: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
+00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090b0: 2020 2061 6363 656c 6572 6174 696f 6e20     acceleration 
+000090c0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+000090d0: 5f76 616c 7565 735b 7365 6c66 2e61 6363  _values[self.acc
+000090e0: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
+000090f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 2020 2020 2020 2020 2020 7661 6c75 655f            value_
-00009120: 6172 7261 7920 3d20 6375 7272 656e 745f  array = current_
-00009130: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
-00009140: 7469 6573 5b63 7572 7265 6e74 5f74 7261  ties[current_tra
-00009150: 636b 5f69 645d 0d0a 2020 2020 2020 2020  ck_id]..        
+00009110: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
+00009120: 6520 3d20 666c 6f61 7428 616c 6c5f 6469  e = float(all_di
+00009130: 6374 5f76 616c 7565 735b 7365 6c66 2e6d  ct_values[self.m
+00009140: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
+00009150: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009180: 6375 7272 656e 745f 7661 6c75 655f 6172  current_value_ar
-00009190: 7261 7920 3d20 6e70 2e61 7272 6179 285b  ray = np.array([
-000091a0: 742c 2069 6e74 2866 6c6f 6174 2875 6e69  t, int(float(uni
-000091b0: 7175 655f 6964 2929 2c20 6765 6e5f 6964  que_id)), gen_id
-000091c0: 2c20 7261 6469 7573 2c20 766f 6c75 6d65  , radius, volume
-000091d0: 5f70 6978 656c 732c 2065 6363 656e 7472  _pixels, eccentr
-000091e0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-000091f0: 2c20 6563 6365 6e74 7269 6369 7479 5f63  , eccentricity_c
-00009200: 6f6d 705f 7365 636f 6e64 2c20 7375 7266  omp_second, surf
-00009210: 6163 655f 6172 6561 2c20 746f 7461 6c5f  ace_area, total_
-00009220: 696e 7465 6e73 6974 792c 2073 7065 6564  intensity, speed
-00009230: 2c20 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  , motion_angle, 
-00009240: 6163 6365 6c65 7261 7469 6f6e 2c20 6469  acceleration, di
-00009250: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00009260: 2c20 7261 6469 616c 5f61 6e67 6c65 2c20  , radial_angle, 
-00009270: 6365 6c6c 5f61 7869 735f 6d61 736b 5d29  cell_axis_mask])
-00009280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092d0: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
-000092e0: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
-000092f0: 5b63 7572 7265 6e74 5f74 7261 636b 5f69  [current_track_i
-00009300: 645d 203d 206e 702e 7673 7461 636b 2828  d] = np.vstack((
-00009310: 7661 6c75 655f 6172 7261 792c 2063 7572  value_array, cur
-00009320: 7265 6e74 5f76 616c 7565 5f61 7272 6179  rent_value_array
-00009330: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009350: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00009360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009170: 2020 2020 2020 2072 6164 6961 6c5f 616e         radial_an
+00009180: 676c 6520 3d20 666c 6f61 7428 616c 6c5f  gle = float(all_
+00009190: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+000091a0: 2e72 6164 6961 6c5f 616e 676c 655f 6b65  .radial_angle_ke
+000091b0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091d0: 2020 2020 2020 2020 2072 6164 6975 7320           radius 
+000091e0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+000091f0: 5f76 616c 7565 735b 7365 6c66 2e72 6164  _values[self.rad
+00009200: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
+00009210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009220: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00009230: 6f6c 756d 655f 7069 7865 6c73 203d 2069  olume_pixels = i
+00009240: 6e74 2866 6c6f 6174 2861 6c6c 5f64 6963  nt(float(all_dic
+00009250: 745f 7661 6c75 6573 5b73 656c 662e 7175  t_values[self.qu
+00009260: 616c 6974 795f 6b65 795d 2929 0d0a 2020  ality_key]))..  
+00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009290: 2020 746f 7461 6c5f 696e 7465 6e73 6974    total_intensit
+000092a0: 7920 3d20 2066 6c6f 6174 2861 6c6c 5f64  y =  float(all_d
+000092b0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+000092c0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+000092d0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009320: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00009330: 736b 203d 2066 6c6f 6174 2861 6c6c 5f64  sk = float(all_d
+00009340: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00009350: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00009360: 736b 5f6b 6579 5d29 0d0a 0d0a 2020 2020  sk_key])....    
 00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009380: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00009390: 5f74 7261 636b 6c65 745f 6172 7261 7920  _tracklet_array 
-000093a0: 3d20 6e70 2e61 7272 6179 285b 696e 7428  = np.array([int(
-000093b0: 666c 6f61 7428 756e 6971 7565 5f69 6429  float(unique_id)
-000093c0: 292c 2074 2c20 7a2f 7365 6c66 2e7a 6361  ), t, z/self.zca
-000093d0: 6c69 6272 6174 696f 6e2c 2079 2f73 656c  libration, y/sel
-000093e0: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
-000093f0: 782f 7365 6c66 2e78 6361 6c69 6272 6174  x/self.xcalibrat
-00009400: 696f 6e5d 290d 0a20 2020 2020 2020 2020  ion])..         
-00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009420: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009430: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009440: 5b63 7572 7265 6e74 5f74 7261 636b 5f69  [current_track_i
-00009450: 645d 203d 2063 7572 7265 6e74 5f74 7261  d] = current_tra
-00009460: 636b 6c65 745f 6172 7261 7920 0d0a 0d0a  cklet_array ....
+00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009390: 6966 2073 656c 662e 7375 7266 6163 655f  if self.surface_
+000093a0: 6172 6561 5f6b 6579 2069 6e20 616c 6c5f  area_key in all_
+000093b0: 6469 6374 5f76 616c 7565 732e 6b65 7973  dict_values.keys
+000093c0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009410: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+00009420: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00009430: 6972 7374 203d 2066 6c6f 6174 2861 6c6c  irst = float(all
+00009440: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00009450: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+00009460: 6f6d 705f 6669 7273 746b 6579 5d29 0d0a  omp_firstkey])..
 00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009490: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000094a0: 7661 6c75 655f 6172 7261 7920 3d20 6e70  value_array = np
-000094b0: 2e61 7272 6179 285b 742c 2069 6e74 2866  .array([t, int(f
-000094c0: 6c6f 6174 2875 6e69 7175 655f 6964 2929  loat(unique_id))
-000094d0: 2c20 6765 6e5f 6964 2c20 7261 6469 7573  , gen_id, radius
-000094e0: 2c20 766f 6c75 6d65 5f70 6978 656c 732c  , volume_pixels,
-000094f0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
-00009500: 6f6d 705f 6669 7273 742c 2065 6363 656e  omp_first, eccen
-00009510: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00009520: 6f6e 642c 2073 7572 6661 6365 5f61 7265  ond, surface_are
-00009530: 612c 2020 746f 7461 6c5f 696e 7465 6e73  a,  total_intens
-00009540: 6974 792c 2073 7065 6564 2c20 6d6f 7469  ity, speed, moti
-00009550: 6f6e 5f61 6e67 6c65 2c20 6163 6365 6c65  on_angle, accele
-00009560: 7261 7469 6f6e 2c20 6469 7374 616e 6365  ration, distance
-00009570: 5f63 656c 6c5f 6d61 736b 2c20 7261 6469  _cell_mask, radi
-00009580: 616c 5f61 6e67 6c65 2c20 6365 6c6c 5f61  al_angle, cell_a
-00009590: 7869 735f 6d61 736b 205d 290d 0a20 2020  xis_mask ])..   
-000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095c0: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-000095d0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-000095e0: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
-000095f0: 6964 5d20 3d20 6375 7272 656e 745f 7661  id] = current_va
-00009600: 6c75 655f 6172 7261 790d 0a0d 0a20 2020  lue_array....   
+00009490: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
+000094a0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+000094b0: 6f6e 6420 3d20 666c 6f61 7428 616c 6c5f  ond = float(all_
+000094c0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+000094d0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+000094e0: 6d70 5f73 6563 6f6e 646b 6579 5d29 0d0a  mp_secondkey])..
+000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009510: 2020 2020 2020 2020 2020 2073 7572 6661             surfa
+00009520: 6365 5f61 7265 6120 3d20 666c 6f61 7428  ce_area = float(
+00009530: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00009540: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
+00009550: 615f 6b65 795d 290d 0a20 2020 2020 2020  a_key])..       
+00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009580: 2020 2020 6365 6c6c 5f61 7869 735f 6d61      cell_axis_ma
+00009590: 736b 203d 2066 6c6f 6174 2861 6c6c 5f64  sk = float(all_d
+000095a0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+000095b0: 6365 6c6c 6178 6973 5f6d 6173 6b5f 6b65  cellaxis_mask_ke
+000095c0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 2072 6574 7572 6e20 6375 7272 656e 745f   return current_
-00009640: 7472 6163 6b6c 6574 732c 2063 7572 7265  tracklets, curre
-00009650: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-00009660: 7065 7274 6965 7320 2020 2020 0d0a 0d0a  perties     ....
-00009670: 2020 2020 6465 6620 5f6d 6173 7465 725f      def _master_
-00009680: 7370 6f74 5f63 6f6d 7075 7465 7228 7365  spot_computer(se
-00009690: 6c66 2c20 6672 616d 6529 3a0d 0a20 2020  lf, frame):..   
-000096a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000096b0: 2020 2066 6f72 2053 706f 746f 626a 6563     for Spotobjec
-000096c0: 7420 696e 2066 7261 6d65 2e66 696e 6461  t in frame.finda
-000096d0: 6c6c 2827 5370 6f74 2729 3a0d 0a20 2020  ll('Spot'):..   
-000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00009700: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00009710: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
-00009720: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-00009730: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
-00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009750: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00009760: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00009770: 2073 656c 662e 756e 6971 7565 6964 5f6b   self.uniqueid_k
-00009780: 6579 2069 6e20 5370 6f74 6f62 6a65 6374  ey in Spotobject
-00009790: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097d0: 2020 2020 7261 6469 7573 203d 2066 6c6f      radius = flo
-000097e0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-000097f0: 7428 7365 6c66 2e72 6164 6975 735f 6b65  t(self.radius_ke
-00009800: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+00009620: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009640: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009670: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
+00009680: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00009690: 7420 3d20 2d31 0d0a 2020 2020 2020 2020  t = -1..        
+000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+000096d0: 5f63 6f6d 705f 7365 636f 6e64 203d 202d  _comp_second = -
+000096e0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009700: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009710: 7572 6661 6365 5f61 7265 6120 3d20 2d31  urface_area = -1
+00009720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009740: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00009750: 6c6c 5f61 7869 735f 6d61 736b 203d 202d  ll_axis_mask = -
+00009760: 3120 2020 2020 0d0a 0d0a 2020 2020 2020  1     ....      
+00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009780: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00009790: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+000097a0: 6420 3d20 2874 2c72 6f75 6e64 287a 292f  d = (t,round(z)/
+000097b0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+000097c0: 6e2c 2072 6f75 6e64 2879 292f 7365 6c66  n, round(y)/self
+000097d0: 2e79 6361 6c69 6272 6174 696f 6e2c 2072  .ycalibration, r
+000097e0: 6f75 6e64 2878 292f 7365 6c66 2e78 6361  ound(x)/self.xca
+000097f0: 6c69 6272 6174 696f 6e29 200d 0a20 2020  libration) ..   
+00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 2020 2020 2071 7561 6c69 7479 203d 2066       quality = f
-00009830: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-00009840: 6765 7428 7365 6c66 2e71 7561 6c69 7479  get(self.quality
-00009850: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+00009820: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00009830: 745f 6365 6e74 726f 6964 5b66 7261 6d65  t_centroid[frame
+00009840: 5f73 706f 745f 6365 6e74 726f 6964 5d20  _spot_centroid] 
+00009850: 3d20 6b0d 0a0d 0a20 2020 2020 2020 2020  = k....         
 00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009870: 2020 2020 2020 2020 746f 7461 6c5f 696e          total_in
-00009880: 7465 6e73 6974 7920 3d20 666c 6f61 7428  tensity = float(
-00009890: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-000098a0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-000098b0: 6974 795f 6b65 7929 290d 0a20 2020 2020  ity_key))..     
-000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098d0: 2020 2020 2020 2020 2020 206d 6561 6e5f             mean_
-000098e0: 696e 7465 6e73 6974 7920 3d20 666c 6f61  intensity = floa
-000098f0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-00009900: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
-00009910: 7369 7479 5f6b 6579 2929 0d0a 0d0a 2020  sity_key))....  
-00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009930: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009940: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00009950: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-00009960: 645d 203d 207b 0d0a 2020 2020 2020 2020  d] = {..        
-00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009980: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009990: 2e63 656c 6c69 645f 6b65 793a 2069 6e74  .cellid_key: int
-000099a0: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
-000099b0: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
-000099c0: 645f 6b65 7929 2929 2c20 0d0a 2020 2020  d_key))), ..    
-000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099f0: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00009a00: 203a 2069 6e74 2866 6c6f 6174 2853 706f   : int(float(Spo
-00009a10: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-00009a20: 2e66 7261 6d65 6964 5f6b 6579 2929 292c  .frameid_key))),
-00009a30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009870: 2020 2020 2020 2020 2020 2069 6620 6375             if cu
+00009880: 7272 656e 745f 7472 6163 6b5f 6964 2069  rrent_track_id i
+00009890: 6e20 6375 7272 656e 745f 7472 6163 6b6c  n current_trackl
+000098a0: 6574 733a 0d0a 2020 2020 2020 2020 2020  ets:..          
+000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098c0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000098d0: 6163 6b6c 6574 5f61 7272 6179 203d 2063  acklet_array = c
+000098e0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+000098f0: 5b63 7572 7265 6e74 5f74 7261 636b 5f69  [current_track_i
+00009900: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
+00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00009930: 656e 745f 7472 6163 6b6c 6574 5f61 7272  ent_tracklet_arr
+00009940: 6179 203d 206e 702e 6172 7261 7928 5b69  ay = np.array([i
+00009950: 6e74 2866 6c6f 6174 2875 6e69 7175 655f  nt(float(unique_
+00009960: 6964 2929 2c20 742c 207a 2f73 656c 662e  id)), t, z/self.
+00009970: 7a63 616c 6962 7261 7469 6f6e 2c20 792f  zcalibration, y/
+00009980: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+00009990: 6e2c 2078 2f73 656c 662e 7863 616c 6962  n, x/self.xcalib
+000099a0: 7261 7469 6f6e 5d29 0d0a 2020 2020 2020  ration])..      
+000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099d0: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+000099e0: 6574 735b 6375 7272 656e 745f 7472 6163  ets[current_trac
+000099f0: 6b5f 6964 5d20 3d20 6e70 2e76 7374 6163  k_id] = np.vstac
+00009a00: 6b28 2874 7261 636b 6c65 745f 6172 7261  k((tracklet_arra
+00009a10: 792c 2063 7572 7265 6e74 5f74 7261 636b  y, current_track
+00009a20: 6c65 745f 6172 7261 7929 290d 0a0d 0a20  let_array)).... 
+00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a50: 2020 2020 2020 7365 6c66 2e7a 706f 7369        self.zposi
-00009a60: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
-00009a70: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-00009a80: 662e 7a70 6f73 6964 5f6b 6579 2929 2c0d  f.zposid_key)),.
-00009a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a50: 2020 2020 2020 2076 616c 7565 5f61 7272         value_arr
+00009a60: 6179 203d 2063 7572 7265 6e74 5f74 7261  ay = current_tra
+00009a70: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
+00009a80: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
+00009a90: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
 00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
-00009ac0: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
-00009ad0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-00009ae0: 2e79 706f 7369 645f 6b65 7929 292c 0d0a  .yposid_key)),..
-00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b10: 2020 2020 7365 6c66 2e78 706f 7369 645f      self.xposid_
-00009b20: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-00009b30: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-00009b40: 7870 6f73 6964 5f6b 6579 2929 2c0d 0a20  xposid_key)),.. 
-00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b70: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
-00009b80: 7465 6e73 6974 795f 6b65 7920 3a20 746f  tensity_key : to
-00009b90: 7461 6c5f 696e 7465 6e73 6974 792c 0d0a  tal_intensity,..
-00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bc0: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
-00009bd0: 7465 6e73 6974 795f 6b65 7920 3a20 6d65  tensity_key : me
-00009be0: 616e 5f69 6e74 656e 7369 7479 2c0d 0a20  an_intensity,.. 
+00009ab0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00009ac0: 7265 6e74 5f76 616c 7565 5f61 7272 6179  rent_value_array
+00009ad0: 203d 206e 702e 6172 7261 7928 5b74 2c20   = np.array([t, 
+00009ae0: 696e 7428 666c 6f61 7428 756e 6971 7565  int(float(unique
+00009af0: 5f69 6429 292c 2067 656e 5f69 642c 2072  _id)), gen_id, r
+00009b00: 6164 6975 732c 2076 6f6c 756d 655f 7069  adius, volume_pi
+00009b10: 7865 6c73 2c20 6563 6365 6e74 7269 6369  xels, eccentrici
+00009b20: 7479 5f63 6f6d 705f 6669 7273 742c 2065  ty_comp_first, e
+00009b30: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00009b40: 5f73 6563 6f6e 642c 2073 7572 6661 6365  _second, surface
+00009b50: 5f61 7265 612c 2074 6f74 616c 5f69 6e74  _area, total_int
+00009b60: 656e 7369 7479 2c20 7370 6565 642c 206d  ensity, speed, m
+00009b70: 6f74 696f 6e5f 616e 676c 652c 2061 6363  otion_angle, acc
+00009b80: 656c 6572 6174 696f 6e2c 2064 6973 7461  eleration, dista
+00009b90: 6e63 655f 6365 6c6c 5f6d 6173 6b2c 2072  nce_cell_mask, r
+00009ba0: 6164 6961 6c5f 616e 676c 652c 2063 656c  adial_angle, cel
+00009bb0: 6c5f 6178 6973 5f6d 6173 6b5d 290d 0a20  l_axis_mask]).. 
+00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009be0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 2020 2073 656c 662e 7261 6469 7573 5f6b     self.radius_k
-00009c20: 6579 203a 2072 6164 6975 732c 0d0a 2020  ey : radius,..  
-00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c50: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
-00009c60: 6579 203a 2071 7561 6c69 7479 2c0d 0a20  ey : quality,.. 
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c10: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00009c20: 7473 5f70 726f 7065 7274 6965 735b 6375  ts_properties[cu
+00009c30: 7272 656e 745f 7472 6163 6b5f 6964 5d20  rrent_track_id] 
+00009c40: 3d20 6e70 2e76 7374 6163 6b28 2876 616c  = np.vstack((val
+00009c50: 7565 5f61 7272 6179 2c20 6375 7272 656e  ue_array, curren
+00009c60: 745f 7661 6c75 655f 6172 7261 7929 290d  t_value_array)).
+00009c70: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c90: 2020 2073 656c 662e 6469 7374 616e 6365     self.distance
-00009ca0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 3a20  _cell_mask_key: 
-00009cb0: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
-00009cc0: 742e 6765 7428 7365 6c66 2e64 6973 7461  t.get(self.dista
-00009cd0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-00009ce0: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009d10: 756e 6971 7565 6964 5f6b 6579 203a 2073  uniqueid_key : s
-00009d20: 7472 2853 706f 746f 626a 6563 742e 6765  tr(Spotobject.ge
-00009d30: 7428 7365 6c66 2e75 6e69 7175 6569 645f  t(self.uniqueid_
-00009d40: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+00009c90: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cc0: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
+00009cd0: 6163 6b6c 6574 5f61 7272 6179 203d 206e  acklet_array = n
+00009ce0: 702e 6172 7261 7928 5b69 6e74 2866 6c6f  p.array([int(flo
+00009cf0: 6174 2875 6e69 7175 655f 6964 2929 2c20  at(unique_id)), 
+00009d00: 742c 207a 2f73 656c 662e 7a63 616c 6962  t, z/self.zcalib
+00009d10: 7261 7469 6f6e 2c20 792f 7365 6c66 2e79  ration, y/self.y
+00009d20: 6361 6c69 6272 6174 696f 6e2c 2078 2f73  calibration, x/s
+00009d30: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00009d40: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
 00009d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009d70: 2e74 7261 636b 6c65 7469 645f 6b65 7920  .trackletid_key 
-00009d80: 3a20 7374 7228 5370 6f74 6f62 6a65 6374  : str(Spotobject
-00009d90: 2e67 6574 2873 656c 662e 7472 6163 6b6c  .get(self.trackl
-00009da0: 6574 6964 5f6b 6579 2929 2c0d 0a20 2020  etid_key)),..   
+00009d60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00009d70: 656e 745f 7472 6163 6b6c 6574 735b 6375  ent_tracklets[cu
+00009d80: 7272 656e 745f 7472 6163 6b5f 6964 5d20  rrent_track_id] 
+00009d90: 3d20 6375 7272 656e 745f 7472 6163 6b6c  = current_trackl
+00009da0: 6574 5f61 7272 6179 200d 0a0d 0a20 2020  et_array ....   
 00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
-00009de0: 6964 5f6b 6579 203a 2073 7472 2853 706f  id_key : str(Spo
-00009df0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-00009e00: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
-00009e10: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
-00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e30: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00009e40: 7261 636b 6964 5f6b 6579 203a 2073 7472  rackid_key : str
-00009e50: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-00009e60: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-00009e70: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e90: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
-00009ea0: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 203a  tion_angle_key :
-00009eb0: 2028 666c 6f61 7428 5370 6f74 6f62 6a65   (float(Spotobje
-00009ec0: 6374 2e67 6574 2873 656c 662e 6d6f 7469  ct.get(self.moti
-00009ed0: 6f6e 5f61 6e67 6c65 5f6b 6579 2929 292c  on_angle_key))),
-00009ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009dd0: 2020 2020 2063 7572 7265 6e74 5f76 616c       current_val
+00009de0: 7565 5f61 7272 6179 203d 206e 702e 6172  ue_array = np.ar
+00009df0: 7261 7928 5b74 2c20 696e 7428 666c 6f61  ray([t, int(floa
+00009e00: 7428 756e 6971 7565 5f69 6429 292c 2067  t(unique_id)), g
+00009e10: 656e 5f69 642c 2072 6164 6975 732c 2076  en_id, radius, v
+00009e20: 6f6c 756d 655f 7069 7865 6c73 2c20 2065  olume_pixels,  e
+00009e30: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00009e40: 5f66 6972 7374 2c20 6563 6365 6e74 7269  _first, eccentri
+00009e50: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00009e60: 2c20 7375 7266 6163 655f 6172 6561 2c20  , surface_area, 
+00009e70: 2074 6f74 616c 5f69 6e74 656e 7369 7479   total_intensity
+00009e80: 2c20 7370 6565 642c 206d 6f74 696f 6e5f  , speed, motion_
+00009e90: 616e 676c 652c 2061 6363 656c 6572 6174  angle, accelerat
+00009ea0: 696f 6e2c 2064 6973 7461 6e63 655f 6365  ion, distance_ce
+00009eb0: 6c6c 5f6d 6173 6b2c 2072 6164 6961 6c5f  ll_mask, radial_
+00009ec0: 616e 676c 652c 2063 656c 6c5f 6178 6973  angle, cell_axis
+00009ed0: 5f6d 6173 6b20 5d29 0d0a 2020 2020 2020  _mask ])..      
+00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f00: 2020 2020 2020 7365 6c66 2e73 7065 6564        self.speed
-00009f10: 5f6b 6579 203a 2028 666c 6f61 7428 5370  _key : (float(Sp
-00009f20: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-00009f30: 662e 7370 6565 645f 6b65 7929 2929 2c0d  f.speed_key))),.
-00009f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009f00: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+00009f10: 6574 735f 7072 6f70 6572 7469 6573 5b63  ets_properties[c
+00009f20: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
+00009f30: 203d 2063 7572 7265 6e74 5f76 616c 7565   = current_value
+00009f40: 5f61 7272 6179 0d0a 0d0a 2020 2020 2020  _array....      
 00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f60: 2020 2020 2073 656c 662e 6163 6365 6c65       self.accele
-00009f70: 7261 7469 6f6e 5f6b 6579 203a 2028 666c  ration_key : (fl
-00009f80: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-00009f90: 6574 2873 656c 662e 6163 6365 6c65 7261  et(self.accelera
-00009fa0: 7469 6f6e 5f6b 6579 2929 292c 0d0a 2020  tion_key))),..  
-00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fd0: 2020 7365 6c66 2e72 6164 6961 6c5f 616e    self.radial_an
-00009fe0: 676c 655f 6b65 793a 2066 6c6f 6174 2853  gle_key: float(S
-00009ff0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000a000: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
-0000a010: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+00009f60: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00009f70: 7475 726e 2063 7572 7265 6e74 5f74 7261  turn current_tra
+00009f80: 636b 6c65 7473 2c20 6375 7272 656e 745f  cklets, current_
+00009f90: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
+00009fa0: 7469 6573 2020 2020 200d 0a0d 0a20 2020  ties     ....   
+00009fb0: 2064 6566 205f 6d61 7374 6572 5f73 706f   def _master_spo
+00009fc0: 745f 636f 6d70 7574 6572 2873 656c 662c  t_computer(self,
+00009fd0: 2066 7261 6d65 293a 0d0a 2020 2020 2020   frame):..      
+00009fe0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00009ff0: 666f 7220 5370 6f74 6f62 6a65 6374 2069  for Spotobject i
+0000a000: 6e20 6672 616d 652e 6669 6e64 616c 6c28  n frame.findall(
+0000a010: 2753 706f 7427 293a 0d0a 2020 2020 2020  'Spot'):..      
 0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a030: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a050: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000a060: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-0000a070: 6b65 7920 696e 2053 706f 746f 626a 6563  key in Spotobjec
-0000a080: 742e 6b65 7973 2829 3a0d 0a20 2020 2020  t.keys():..     
-0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a0b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-0000a0c0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-0000a0d0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-0000a0e0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-0000a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a030: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000a040: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+0000a050: 6964 203d 2069 6e74 2853 706f 746f 626a  id = int(Spotobj
+0000a060: 6563 742e 6765 7428 7365 6c66 2e73 706f  ect.get(self.spo
+0000a070: 7469 645f 6b65 7929 290d 0a20 2020 2020  tid_key))..     
+0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a090: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000a0a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000a0b0: 6c66 2e75 6e69 7175 6569 645f 6b65 7920  lf.uniqueid_key 
+0000a0c0: 696e 2053 706f 746f 626a 6563 742e 6b65  in Spotobject.ke
+0000a0d0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+0000a0e0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000a0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a140: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-0000a150: 705f 6669 7273 746b 6579 203a 2066 6c6f  p_firstkey : flo
-0000a160: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000a170: 7428 7365 6c66 2e65 6363 656e 7472 6963  t(self.eccentric
-0000a180: 6974 795f 636f 6d70 5f66 6972 7374 6b65  ity_comp_firstke
-0000a190: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000a110: 2072 6164 6975 7320 3d20 666c 6f61 7428   radius = float(
+0000a120: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000a130: 656c 662e 7261 6469 7573 5f6b 6579 2929  elf.radius_key))
+0000a140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a160: 2020 7175 616c 6974 7920 3d20 666c 6f61    quality = floa
+0000a170: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000a180: 2873 656c 662e 7175 616c 6974 795f 6b65  (self.quality_ke
+0000a190: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
 0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a1f0: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
-0000a200: 636f 6d70 5f73 6563 6f6e 646b 6579 203a  comp_secondkey :
-0000a210: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000a220: 742e 6765 7428 7365 6c66 2e65 6363 656e  t.get(self.eccen
-0000a230: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-0000a240: 6f6e 646b 6579 2929 2c0d 0a20 2020 2020  ondkey)),..     
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1b0: 2020 2020 2074 6f74 616c 5f69 6e74 656e       total_inten
+0000a1c0: 7369 7479 203d 2066 6c6f 6174 2853 706f  sity = float(Spo
+0000a1d0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000a1e0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000a1f0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a210: 2020 2020 2020 2020 6d65 616e 5f69 6e74          mean_int
+0000a220: 656e 7369 7479 203d 2066 6c6f 6174 2853  ensity = float(S
+0000a230: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000a240: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000a250: 795f 6b65 7929 290d 0a0d 0a20 2020 2020  y_key))....     
 0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2a0: 2020 2073 656c 662e 7375 7266 6163 655f     self.surface_
-0000a2b0: 6172 6561 5f6b 6579 203a 2066 6c6f 6174  area_key : float
-0000a2c0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000a2d0: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
-0000a2e0: 615f 6b65 7929 292c 0d0a 2020 2020 2020  a_key)),..      
-0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a270: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a280: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000a290: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
+0000a2a0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
+0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2c0: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
+0000a2d0: 6c6c 6964 5f6b 6579 3a20 696e 7428 666c  llid_key: int(fl
+0000a2e0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000a2f0: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
+0000a300: 6579 2929 292c 200d 0a20 2020 2020 2020  ey))), ..       
 0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a340: 2020 7365 6c66 2e63 656c 6c61 7869 735f    self.cellaxis_
-0000a350: 6d61 736b 5f6b 6579 3a20 666c 6f61 7428  mask_key: float(
-0000a360: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000a370: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
-0000a380: 6b5f 6b65 7929 290d 0a20 2020 2020 2020  k_key))..       
-0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a320: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a330: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
+0000a340: 696e 7428 666c 6f61 7428 5370 6f74 6f62  int(float(Spotob
+0000a350: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
+0000a360: 616d 6569 645f 6b65 7929 2929 2c0d 0a20  ameid_key))),.. 
+0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a390: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
+0000a3a0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000a3b0: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
+0000a3c0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
 0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3e0: 2020 2020 207d 290d 0a20 2020 2020 2020       })..       
-0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a410: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3f0: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
+0000a400: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
+0000a410: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
+0000a420: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
 0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a440: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a460: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 2020 656c 6966 2073 656c 662e 756e 6971    elif self.uniq
-0000a490: 7565 6964 5f6b 6579 206e 6f74 2069 6e20  ueid_key not in 
-0000a4a0: 5370 6f74 6f62 6a65 6374 2e6b 6579 7328  Spotobject.keys(
-0000a4b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a450: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+0000a460: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000a470: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
+0000a480: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4b0: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000a4c0: 7369 7479 5f6b 6579 203a 2074 6f74 616c  sity_key : total
+0000a4d0: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
+0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000a520: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
-0000a530: 6e65 6c20 3d3d 2031 3a0d 0a20 2020 2020  nel == 1:..     
+0000a500: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+0000a510: 7369 7479 5f6b 6579 203a 206d 6561 6e5f  sity_key : mean_
+0000a520: 696e 7465 6e73 6974 792c 0d0a 2020 2020  intensity,..    
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000a570: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000a580: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
-0000a590: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000a5a0: 7369 7479 5f63 6832 5f6b 6579 290d 0a20  sity_ch2_key).. 
+0000a550: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
+0000a560: 3a20 7261 6469 7573 2c0d 0a20 2020 2020  : radius,..     
+0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a590: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
+0000a5a0: 3a20 7175 616c 6974 792c 0d0a 2020 2020  : quality,..    
 0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5e0: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
-0000a5f0: 5920 3d20 5370 6f74 6f62 6a65 6374 2e67  Y = Spotobject.g
-0000a600: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
-0000a610: 656e 7369 7479 5f63 6832 5f6b 6579 290d  ensity_ch2_key).
-0000a620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a5d0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+0000a5e0: 6c6c 5f6d 6173 6b5f 6b65 793a 2028 666c  ll_mask_key: (fl
+0000a5f0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000a600: 6574 2873 656c 662e 6469 7374 616e 6365  et(self.distance
+0000a610: 5f63 656c 6c5f 6d61 736b 5f6b 6579 2929  _cell_mask_key))
+0000a620: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
 0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a640: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000a650: 653a 2020 2020 2020 2020 0d0a 2020 2020  e:        ..    
-0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a690: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
-0000a6a0: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
-0000a6b0: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
-0000a6c0: 6e73 6974 795f 6368 315f 6b65 7929 0d0a  nsity_ch1_key)..
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a640: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+0000a650: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
+0000a660: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000a670: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000a680: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6a0: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000a6b0: 6163 6b6c 6574 6964 5f6b 6579 203a 2073  ackletid_key : s
+0000a6c0: 7472 2853 706f 746f 626a 6563 742e 6765  tr(Spotobject.ge
+0000a6d0: 7428 7365 6c66 2e74 7261 636b 6c65 7469  t(self.trackleti
+0000a6e0: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
 0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
-0000a710: 5459 203d 2053 706f 746f 626a 6563 742e  TY = Spotobject.
-0000a720: 6765 7428 7365 6c66 2e6d 6561 6e5f 696e  get(self.mean_in
-0000a730: 7465 6e73 6974 795f 6368 315f 6b65 7929  tensity_ch1_key)
-0000a740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a760: 2020 2020 2020 2020 2020 2020 2020 5241                RA
-0000a770: 4449 5553 203d 2066 6c6f 6174 2853 706f  DIUS = float(Spo
-0000a780: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000a790: 2e72 6164 6975 735f 6b65 7929 290d 0a20  .radius_key)).. 
-0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7c0: 2020 2020 2020 2020 2020 2051 5541 4c49             QUALI
-0000a7d0: 5459 203d 2066 6c6f 6174 2853 706f 746f  TY = float(Spoto
-0000a7e0: 626a 6563 742e 6765 7428 7365 6c66 2e71  bject.get(self.q
-0000a7f0: 7561 6c69 7479 5f6b 6579 2929 2020 2020  uality_key))    
-0000a800: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a820: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000a830: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000a840: 2066 6c6f 6174 2854 4f54 414c 5f49 4e54   float(TOTAL_INT
-0000a850: 454e 5349 5459 290d 0a20 2020 2020 2020  ENSITY)..       
-0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a880: 2020 2020 204d 4541 4e5f 494e 5445 4e53       MEAN_INTENS
-0000a890: 4954 5920 3d20 666c 6f61 7428 4d45 414e  ITY = float(MEAN
-0000a8a0: 5f49 4e54 454e 5349 5459 290d 0a20 2020  _INTENSITY)..   
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8d0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-0000a8e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000a8f0: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
-0000a900: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a920: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a930: 656c 662e 6365 6c6c 6964 5f6b 6579 3a20  elf.cellid_key: 
-0000a940: 696e 7428 6365 6c6c 5f69 6429 2c20 0d0a  int(cell_id), ..
-0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a710: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
+0000a720: 6b65 7920 3a20 7374 7228 5370 6f74 6f62  key : str(Spotob
+0000a730: 6a65 6374 2e67 6574 2873 656c 662e 6765  ject.get(self.ge
+0000a740: 6e65 7261 7469 6f6e 6964 5f6b 6579 2929  nerationid_key))
+0000a750: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a770: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000a780: 6b69 645f 6b65 7920 3a20 7374 7228 5370  kid_key : str(Sp
+0000a790: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000a7a0: 662e 7472 6163 6b69 645f 6b65 7929 292c  f.trackid_key)),
+0000a7b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7d0: 2020 2020 2020 7365 6c66 2e6d 6f74 696f        self.motio
+0000a7e0: 6e5f 616e 676c 655f 6b65 7920 3a20 2866  n_angle_key : (f
+0000a7f0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000a800: 6765 7428 7365 6c66 2e6d 6f74 696f 6e5f  get(self.motion_
+0000a810: 616e 676c 655f 6b65 7929 2929 2c0d 0a20  angle_key))),.. 
+0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a840: 2020 2073 656c 662e 7370 6565 645f 6b65     self.speed_ke
+0000a850: 7920 3a20 2866 6c6f 6174 2853 706f 746f  y : (float(Spoto
+0000a860: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+0000a870: 7065 6564 5f6b 6579 2929 292c 0d0a 2020  peed_key))),..  
+0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8a0: 2020 7365 6c66 2e61 6363 656c 6572 6174    self.accelerat
+0000a8b0: 696f 6e5f 6b65 7920 3a20 2866 6c6f 6174  ion_key : (float
+0000a8c0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000a8d0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+0000a8e0: 6e5f 6b65 7929 2929 2c0d 0a20 2020 2020  n_key))),..     
+0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a900: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a910: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
+0000a920: 5f6b 6579 3a20 666c 6f61 7428 5370 6f74  _key: float(Spot
+0000a930: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000a940: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
+0000a950: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
 0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a980: 2e66 7261 6d65 6964 5f6b 6579 203a 2069  .frameid_key : i
-0000a990: 6e74 2866 6c6f 6174 2853 706f 746f 626a  nt(float(Spotobj
-0000a9a0: 6563 742e 6765 7428 7365 6c66 2e66 7261  ect.get(self.fra
-0000a9b0: 6d65 6964 5f6b 6579 2929 292c 0d0a 2020  meid_key))),..  
-0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a970: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a990: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000a9a0: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
+0000a9b0: 2069 6e20 5370 6f74 6f62 6a65 6374 2e6b   in Spotobject.k
+0000a9c0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
 0000a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9e0: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
-0000a9f0: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000aa00: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000aa10: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
-0000aa20: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000a9e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a9f0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+0000aa00: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+0000aa10: 5f69 6429 5d2e 7570 6461 7465 287b 0d0a  _id)].update({..
+0000aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa50: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
-0000aa60: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000aa70: 6563 742e 6765 7428 7365 6c66 2e79 706f  ect.get(self.ypo
-0000aa80: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
-0000aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aab0: 2020 2020 2020 2020 7365 6c66 2e78 706f          self.xpo
-0000aac0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-0000aad0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000aae0: 656c 662e 7870 6f73 6964 5f6b 6579 2929  elf.xposid_key))
-0000aaf0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa70: 2020 2020 2020 2020 7365 6c66 2e65 6363          self.ecc
+0000aa80: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+0000aa90: 6972 7374 6b65 7920 3a20 666c 6f61 7428  irstkey : float(
+0000aaa0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000aab0: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+0000aac0: 5f63 6f6d 705f 6669 7273 746b 6579 2929  _comp_firstkey))
+0000aad0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ab20: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000ab30: 6974 795f 6b65 7920 3a20 544f 5441 4c5f  ity_key : TOTAL_
-0000ab40: 494e 5445 4e53 4954 592c 0d0a 2020 2020  INTENSITY,..    
-0000ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab70: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
-0000ab80: 6e5f 696e 7465 6e73 6974 795f 6b65 7920  n_intensity_key 
-0000ab90: 3a20 4d45 414e 5f49 4e54 454e 5349 5459  : MEAN_INTENSITY
-0000aba0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ab30: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+0000ab40: 705f 7365 636f 6e64 6b65 7920 3a20 666c  p_secondkey : fl
+0000ab50: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000ab60: 6574 2873 656c 662e 6563 6365 6e74 7269  et(self.eccentri
+0000ab70: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+0000ab80: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000abd0: 656c 662e 7261 6469 7573 5f6b 6579 203a  elf.radius_key :
-0000abe0: 2052 4144 4955 532c 0d0a 2020 2020 2020   RADIUS,..      
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
-0000ac20: 7479 5f6b 6579 203a 2051 5541 4c49 5459  ty_key : QUALITY
-0000ac30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abe0: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
+0000abf0: 615f 6b65 7920 3a20 666c 6f61 7428 5370  a_key : float(Sp
+0000ac00: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000ac10: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
+0000ac20: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac50: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-0000ac60: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000ac70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000aca0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-0000acb0: 2064 6566 205f 7370 6f74 5f63 6f6d 7075   def _spot_compu
-0000acc0: 7465 7228 7365 6c66 2c20 6672 616d 6529  ter(self, frame)
-0000acd0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2066  :....          f
-0000ace0: 6f72 2053 706f 746f 626a 6563 7420 696e  or Spotobject in
-0000acf0: 2066 7261 6d65 2e66 696e 6461 6c6c 2827   frame.findall('
-0000ad00: 5370 6f74 2729 3a0d 0a20 2020 2020 2020  Spot'):..       
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ac80: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
+0000ac90: 6b5f 6b65 793a 2066 6c6f 6174 2853 706f  k_key: float(Spo
+0000aca0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000acb0: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
+0000acc0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad20: 2023 2043 7265 6174 6520 6f62 6a65 6374   # Create object
-0000ad30: 2077 6974 6820 756e 6971 7565 2063 656c   with unique cel
-0000ad40: 6c20 4944 0d0a 2020 2020 2020 2020 2020  l ID..          
-0000ad50: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-0000ad60: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
-0000ad70: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000ad80: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
+0000ad20: 2020 7d29 0d0a 2020 2020 2020 2020 2020    })..          
+0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad50: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ada0: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
-0000adb0: 545a 5958 206c 6f63 6174 696f 6e20 6f66  TZYX location of
-0000adc0: 2074 6865 2063 656c 6c73 2069 6e20 7468   the cells in th
-0000add0: 6174 2066 7261 6d65 0d0a 2020 2020 2020  at frame..      
-0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adf0: 2020 6966 2073 656c 662e 6465 7465 6374    if self.detect
-0000ae00: 6f72 6368 616e 6e65 6c20 3d3d 2031 3a0d  orchannel == 1:.
-0000ae10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae30: 2069 6620 5370 6f74 6f62 6a65 6374 2e67   if Spotobject.g
-0000ae40: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000ae50: 7465 6e73 6974 795f 6368 325f 6b65 7929  tensity_ch2_key)
-0000ae60: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ada0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000adb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000adc0: 6c69 6620 7365 6c66 2e75 6e69 7175 6569  lif self.uniquei
+0000add0: 645f 6b65 7920 6e6f 7420 696e 2053 706f  d_key not in Spo
+0000ade0: 746f 626a 6563 742e 6b65 7973 2829 3a0d  tobject.keys():.
+0000adf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae50: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000ae60: 2e64 6574 6563 746f 7263 6861 6e6e 656c  .detectorchannel
+0000ae70: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
 0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae90: 2020 2020 2020 2054 4f54 414c 5f49 4e54         TOTAL_INT
-0000aea0: 454e 5349 5459 203d 2066 6c6f 6174 2853  ENSITY = float(S
-0000aeb0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000aec0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000aed0: 7479 5f63 6832 5f6b 6579 2929 0d0a 2020  ty_ch2_key))..  
-0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aea0: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
+0000aeb0: 4c5f 494e 5445 4e53 4954 5920 3d20 5370  L_INTENSITY = Sp
+0000aec0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000aed0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000aee0: 795f 6368 325f 6b65 7929 0d0a 2020 2020  y_ch2_key)..    
 0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af00: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
-0000af10: 5349 5459 203d 2066 6c6f 6174 2853 706f  SITY = float(Spo
-0000af20: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000af30: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-0000af40: 6368 325f 6b65 7929 290d 0a20 2020 2020  ch2_key))..     
-0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000af70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af90: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
-0000afa0: 4e54 454e 5349 5459 203d 202d 310d 0a20  NTENSITY = -1.. 
+0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af20: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000af30: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
+0000af40: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+0000af50: 6974 795f 6368 325f 6b65 7929 0d0a 2020  ity_ch2_key)..  
+0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af80: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
+0000af90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afd0: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
-0000afe0: 5349 5459 203d 202d 3120 2020 2020 2020  SITY = -1       
-0000aff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b000: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-0000b010: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000afc0: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
+0000afd0: 414c 5f49 4e54 454e 5349 5459 203d 2053  AL_INTENSITY = S
+0000afe0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000aff0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000b000: 7479 5f63 6831 5f6b 6579 290d 0a20 2020  ty_ch1_key)..   
+0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b030: 2020 2020 2020 2020 2069 6620 5370 6f74           if Spot
-0000b040: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b050: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000b060: 6368 315f 6b65 7929 2069 7320 6e6f 7420  ch1_key) is not 
-0000b070: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b040: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000b050: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
+0000b060: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
+0000b070: 7369 7479 5f63 6831 5f6b 6579 290d 0a20  sity_ch1_key).. 
 0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b090: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000b0a0: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000b0b0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000b0c0: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
-0000b0d0: 5f69 6e74 656e 7369 7479 5f63 6831 5f6b  _intensity_ch1_k
-0000b0e0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0a0: 2020 2020 2020 2020 2020 2052 4144 4955             RADIU
+0000b0b0: 5320 3d20 666c 6f61 7428 5370 6f74 6f62  S = float(Spotob
+0000b0c0: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
+0000b0d0: 6469 7573 5f6b 6579 2929 0d0a 2020 2020  dius_key))..    
+0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b100: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000b110: 414e 5f49 4e54 454e 5349 5459 203d 2066  AN_INTENSITY = f
-0000b120: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b130: 6765 7428 7365 6c66 2e6d 6561 6e5f 696e  get(self.mean_in
-0000b140: 7465 6e73 6974 795f 6368 315f 6b65 7929  tensity_ch1_key)
-0000b150: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b170: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1a0: 2020 544f 5441 4c5f 494e 5445 4e53 4954    TOTAL_INTENSIT
-0000b1b0: 5920 3d20 2d31 0d0a 2020 2020 2020 2020  Y = -1..        
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1e0: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
-0000b1f0: 202d 3120 2020 2020 2020 2020 0d0a 0d0a   -1         ....
+0000b100: 2020 2020 2020 2020 5155 414c 4954 5920          QUALITY 
+0000b110: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000b120: 6374 2e67 6574 2873 656c 662e 7175 616c  ct.get(self.qual
+0000b130: 6974 795f 6b65 7929 2920 2020 2020 0d0a  ity_key))     ..
+0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b160: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
+0000b170: 4c5f 494e 5445 4e53 4954 5920 3d20 666c  L_INTENSITY = fl
+0000b180: 6f61 7428 544f 5441 4c5f 494e 5445 4e53  oat(TOTAL_INTENS
+0000b190: 4954 5929 0d0a 2020 2020 2020 2020 2020  ITY)..          
+0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1c0: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
+0000b1d0: 203d 2066 6c6f 6174 284d 4541 4e5f 494e   = float(MEAN_IN
+0000b1e0: 5445 4e53 4954 5929 0d0a 2020 2020 2020  TENSITY)..      
+0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b230: 2020 2020 2020 2020 2020 5241 4449 5553            RADIUS
-0000b240: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000b250: 6563 742e 6765 7428 7365 6c66 2e72 6164  ect.get(self.rad
-0000b260: 6975 735f 6b65 7929 290d 0a20 2020 2020  ius_key))..     
-0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b280: 2020 2051 5541 4c49 5459 203d 2066 6c6f     QUALITY = flo
-0000b290: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000b2a0: 7428 7365 6c66 2e71 7561 6c69 7479 5f6b  t(self.quality_k
-0000b2b0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000b2c0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000b2d0: 7374 6c6f 6361 7469 6f6e 203d 2028 666c  stlocation = (fl
-0000b2e0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000b2f0: 6574 2873 656c 662e 7a70 6f73 6964 5f6b  et(self.zposid_k
-0000b300: 6579 2929 2c20 666c 6f61 7428 5370 6f74  ey)), float(Spot
-0000b310: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b320: 7970 6f73 6964 5f6b 6579 2929 2c20 2066  yposid_key)),  f
-0000b330: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b340: 6765 7428 7365 6c66 2e78 706f 7369 645f  get(self.xposid_
-0000b350: 6b65 7929 2929 0d0a 2020 2020 2020 2020  key)))..        
-0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b370: 6672 616d 6520 3d20 5370 6f74 6f62 6a65  frame = Spotobje
-0000b380: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
-0000b390: 6569 645f 6b65 7929 0d0a 2020 2020 2020  eid_key)..      
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
-0000b3c0: 6d61 736b 2c20 6d61 736b 6365 6e74 726f  mask, maskcentro
-0000b3d0: 6964 203d 2073 656c 662e 5f67 6574 5f62  id = self._get_b
-0000b3e0: 6f75 6e64 6172 795f 6469 7374 2866 7261  oundary_dist(fra
-0000b3f0: 6d65 2c20 7465 7374 6c6f 6361 7469 6f6e  me, testlocation
-0000b400: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000b410: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b430: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000b440: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000b450: 5b63 656c 6c5f 6964 5d20 3d20 7b0d 0a20  [cell_id] = {.. 
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b480: 6365 6c6c 6964 5f6b 6579 3a20 696e 7428  cellid_key: int(
-0000b490: 6365 6c6c 5f69 6429 2c20 0d0a 2020 2020  cell_id), ..    
+0000b210: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000b220: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000b230: 735b 6365 6c6c 5f69 645d 203d 207b 0d0a  s[cell_id] = {..
+0000b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b270: 2e63 656c 6c69 645f 6b65 793a 2069 6e74  .cellid_key: int
+0000b280: 2863 656c 6c5f 6964 292c 200d 0a20 2020  (cell_id), ..   
+0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2b0: 2020 2020 2020 2020 2073 656c 662e 6672           self.fr
+0000b2c0: 616d 6569 645f 6b65 7920 3a20 696e 7428  ameid_key : int(
+0000b2d0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000b2e0: 2e67 6574 2873 656c 662e 6672 616d 6569  .get(self.framei
+0000b2f0: 645f 6b65 7929 2929 2c0d 0a20 2020 2020  d_key))),..     
+0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b320: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
+0000b330: 6964 5f6b 6579 203a 2066 6c6f 6174 2853  id_key : float(S
+0000b340: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b350: 6c66 2e7a 706f 7369 645f 6b65 7929 292c  lf.zposid_key)),
+0000b360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b380: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b390: 6c66 2e79 706f 7369 645f 6b65 7920 3a20  lf.yposid_key : 
+0000b3a0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000b3b0: 2e67 6574 2873 656c 662e 7970 6f73 6964  .get(self.yposid
+0000b3c0: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3f0: 2020 2020 2073 656c 662e 7870 6f73 6964       self.xposid
+0000b400: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000b410: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b420: 2e78 706f 7369 645f 6b65 7929 292c 0d0a  .xposid_key)),..
+0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b460: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000b470: 5f6b 6579 203a 2054 4f54 414c 5f49 4e54  _key : TOTAL_INT
+0000b480: 454e 5349 5459 2c0d 0a20 2020 2020 2020  ENSITY,..       
+0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4b0: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
-0000b4c0: 6d65 6964 5f6b 6579 203a 2069 6e74 2866  meid_key : int(f
-0000b4d0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b4e0: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
-0000b4f0: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 2020 2020 2020 7365 6c66 2e7a 706f 7369        self.zposi
-0000b520: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
-0000b530: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b540: 662e 7a70 6f73 6964 5f6b 6579 2929 2c0d  f.zposid_key)),.
-0000b550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b560: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b570: 662e 7970 6f73 6964 5f6b 6579 203a 2066  f.yposid_key : f
-0000b580: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b590: 6765 7428 7365 6c66 2e79 706f 7369 645f  get(self.yposid_
-0000b5a0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
-0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5c0: 2020 2020 7365 6c66 2e78 706f 7369 645f      self.xposid_
-0000b5d0: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-0000b5e0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b5f0: 7870 6f73 6964 5f6b 6579 2929 2c0d 0a20  xposid_key)),.. 
-0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b620: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000b630: 6b65 7920 3a20 544f 5441 4c5f 494e 5445  key : TOTAL_INTE
-0000b640: 4e53 4954 592c 0d0a 2020 2020 2020 2020  NSITY,..        
-0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b660: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
-0000b670: 7465 6e73 6974 795f 6b65 7920 3a20 4d45  tensity_key : ME
-0000b680: 414e 5f49 4e54 454e 5349 5459 2c0d 0a20  AN_INTENSITY,.. 
-0000b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b6b0: 7261 6469 7573 5f6b 6579 203a 2052 4144  radius_key : RAD
-0000b6c0: 4955 532c 0d0a 2020 2020 2020 2020 2020  IUS,..          
+0000b4b0: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
+0000b4c0: 6e74 656e 7369 7479 5f6b 6579 203a 204d  ntensity_key : M
+0000b4d0: 4541 4e5f 494e 5445 4e53 4954 592c 0d0a  EAN_INTENSITY,..
+0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b500: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b510: 2e72 6164 6975 735f 6b65 7920 3a20 5241  .radius_key : RA
+0000b520: 4449 5553 2c0d 0a20 2020 2020 2020 2020  DIUS,..         
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b550: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
+0000b560: 6b65 7920 3a20 5155 414c 4954 590d 0a20  key : QUALITY.. 
+0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b590: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+0000b5a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000b5b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000b5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b5e0: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
+0000b5f0: 6620 5f73 706f 745f 636f 6d70 7574 6572  f _spot_computer
+0000b600: 2873 656c 662c 2066 7261 6d65 293a 0d0a  (self, frame):..
+0000b610: 0d0a 2020 2020 2020 2020 2020 666f 7220  ..          for 
+0000b620: 5370 6f74 6f62 6a65 6374 2069 6e20 6672  Spotobject in fr
+0000b630: 616d 652e 6669 6e64 616c 6c28 2753 706f  ame.findall('Spo
+0000b640: 7427 293a 0d0a 2020 2020 2020 2020 2020  t'):..          
+0000b650: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000b660: 4372 6561 7465 206f 626a 6563 7420 7769  Create object wi
+0000b670: 7468 2075 6e69 7175 6520 6365 6c6c 2049  th unique cell I
+0000b680: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+0000b690: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+0000b6a0: 6964 203d 2069 6e74 2853 706f 746f 626a  id = int(Spotobj
+0000b6b0: 6563 742e 6765 7428 7365 6c66 2e73 706f  ect.get(self.spo
+0000b6c0: 7469 645f 6b65 7929 290d 0a20 2020 2020  tid_key))..     
 0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6e0: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
-0000b6f0: 6579 203a 2051 5541 4c49 5459 2c0d 0a20  ey : QUALITY,.. 
-0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b720: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000b730: 736b 5f6b 6579 3a20 666c 6f61 7428 6469  sk_key: float(di
-0000b740: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000b750: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b770: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-0000b780: 645f 7a5f 6b65 793a 2066 6c6f 6174 286d  d_z_key: float(m
-0000b790: 6173 6b63 656e 7472 6f69 645b 305d 292c  askcentroid[0]),
-0000b7a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b7c0: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-0000b7d0: 795f 6b65 793a 2066 6c6f 6174 286d 6173  y_key: float(mas
-0000b7e0: 6b63 656e 7472 6f69 645b 315d 292c 0d0a  kcentroid[1]),..
-0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b800: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b810: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
-0000b820: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
-0000b830: 656e 7472 6f69 645b 325d 2920 0d0a 2020  entroid[2]) ..  
-0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b850: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-0000b860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b870: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000b880: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000b6e0: 2020 2023 2047 6574 2074 6865 2054 5a59     # Get the TZY
+0000b6f0: 5820 6c6f 6361 7469 6f6e 206f 6620 7468  X location of th
+0000b700: 6520 6365 6c6c 7320 696e 2074 6861 7420  e cells in that 
+0000b710: 6672 616d 650d 0a20 2020 2020 2020 2020  frame..         
+0000b720: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000b730: 6620 7365 6c66 2e64 6574 6563 746f 7263  f self.detectorc
+0000b740: 6861 6e6e 656c 203d 3d20 313a 0d0a 2020  hannel == 1:..  
+0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b760: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000b770: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
+0000b780: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000b790: 7369 7479 5f63 6832 5f6b 6579 2920 6973  sity_ch2_key) is
+0000b7a0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7d0: 2020 2020 544f 5441 4c5f 494e 5445 4e53      TOTAL_INTENS
+0000b7e0: 4954 5920 3d20 666c 6f61 7428 5370 6f74  ITY = float(Spot
+0000b7f0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000b800: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+0000b810: 6368 325f 6b65 7929 290d 0a20 2020 2020  ch2_key))..     
+0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b840: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
+0000b850: 5920 3d20 666c 6f61 7428 5370 6f74 6f62  Y = float(Spotob
+0000b860: 6a65 6374 2e67 6574 2873 656c 662e 6d65  ject.get(self.me
+0000b870: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
+0000b880: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
 0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000b8a0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
 0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8c0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-0000b8d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b8e0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-0000b8f0: 2020 6465 6620 5f67 6574 5f6d 6173 7465    def _get_maste
-0000b900: 725f 786d 6c5f 6461 7461 2873 656c 6629  r_xml_data(self)
-0000b910: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000b920: 6620 7365 6c66 2e63 6861 6e6e 656c 5f73  f self.channel_s
-0000b930: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
-0000b940: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000b950: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b960: 662e 6368 616e 6e65 6c5f 786d 6c5f 636f  f.channel_xml_co
-0000b970: 6e74 656e 7420 3d20 7365 6c66 2e78 6d6c  ntent = self.xml
-0000b980: 5f63 6f6e 7465 6e74 0d0a 2020 2020 2020  _content..      
-0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9a0: 7365 6c66 2e78 6d6c 5f74 7265 6520 3d20  self.xml_tree = 
-0000b9b0: 6574 2e70 6172 7365 2873 656c 662e 786d  et.parse(self.xm
-0000b9c0: 6c5f 7061 7468 290d 0a20 2020 2020 2020  l_path)..       
-0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b9e0: 656c 662e 786d 6c5f 726f 6f74 203d 2073  elf.xml_root = s
-0000b9f0: 656c 662e 786d 6c5f 7472 6565 2e67 6574  elf.xml_tree.get
-0000ba00: 726f 6f74 2829 0d0a 2020 2020 2020 2020  root()..        
-0000ba10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ba20: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f6e  lf.channel_xml_n
-0000ba30: 616d 6520 3d20 2773 6563 6f6e 645f 6368  ame = 'second_ch
-0000ba40: 616e 6e65 6c5f 2720 2b20 6f73 2e70 6174  annel_' + os.pat
-0000ba50: 682e 7370 6c69 7465 7874 286f 732e 7061  h.splitext(os.pa
-0000ba60: 7468 2e62 6173 656e 616d 6528 7365 6c66  th.basename(self
-0000ba70: 2e78 6d6c 5f70 6174 6829 295b 305d 202b  .xml_path))[0] +
-0000ba80: 2027 2e78 6d6c 270d 0a20 2020 2020 2020   '.xml'..       
-0000ba90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000baa0: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000bab0: 7061 7468 203d 206f 732e 7061 7468 2e64  path = os.path.d
-0000bac0: 6972 6e61 6d65 2873 656c 662e 786d 6c5f  irname(self.xml_
-0000bad0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-0000bae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000baf0: 662e 5f63 7265 6174 655f 6368 616e 6e65  f._create_channe
-0000bb00: 6c5f 7472 6565 2829 0d0a 0d0a 2020 2020  l_tree()....    
-0000bb10: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-0000bb20: 7175 655f 6f62 6a65 6374 7320 3d20 7b7d  que_objects = {}
-0000bb30: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000bb40: 6c66 2e75 6e69 7175 655f 7072 6f70 6572  lf.unique_proper
-0000bb50: 7469 6573 203d 207b 7d0d 0a20 2020 2020  ties = {}..     
-0000bb60: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
-0000bb70: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
-0000bb80: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
-0000bb90: 6976 6964 696e 6754 7261 636b 4964 7320  ividingTrackIds 
-0000bba0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000bbb0: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
-0000bbc0: 636b 4964 7320 3d20 5b5d 0d0a 2020 2020  ckIds = []..    
-0000bbd0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-0000bbe0: 5f74 7261 636b 5f70 726f 7065 7274 6965  _track_propertie
-0000bbf0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000bc00: 2020 2020 7365 6c66 2e73 706c 6974 5f70      self.split_p
-0000bc10: 6f69 6e74 735f 7469 6d65 7320 3d20 5b5d  oints_times = []
-0000bc20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000bc30: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000bc40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000bc50: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
-0000bc60: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
-0000bc70: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
-0000bc80: 6469 6e67 5472 6163 6b49 6473 2e61 7070  dingTrackIds.app
-0000bc90: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
-0000bca0: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
-0000bcb0: 616c 5472 6163 6b49 6473 2e61 7070 656e  alTrackIds.appen
-0000bcc0: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
-0000bcd0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000bce0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-0000bcf0: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
-0000bd00: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
-0000bd10: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-0000bd20: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
-0000bd30: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
-0000bd40: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
-0000bd50: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
-0000bd60: 7261 636b 4964 732e 6170 7065 6e64 2873  rackIds.append(s
-0000bd70: 656c 662e 5472 6163 6b69 6442 6f78 290d  elf.TrackidBox).
-0000bd80: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0000bd90: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000bda0: 2020 2020 2020 2020 2073 656c 662e 5370           self.Sp
-0000bdb0: 6f74 6f62 6a65 6374 7320 3d20 7365 6c66  otobjects = self
-0000bdc0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000bdd0: 6428 274d 6f64 656c 2729 2e66 696e 6428  d('Model').find(
-0000bde0: 2741 6c6c 5370 6f74 7327 290d 0a20 2020  'AllSpots')..   
-0000bdf0: 2020 2020 2020 2020 2023 2045 7874 7261           # Extra
-0000be00: 6374 2074 6865 2074 7261 636b 7320 6672  ct the tracks fr
-0000be10: 6f6d 2078 6d6c 0d0a 2020 2020 2020 2020  om xml..        
-0000be20: 2020 2020 7365 6c66 2e74 7261 636b 7320      self.tracks 
-0000be30: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000be40: 6e74 2e66 696e 6428 224d 6f64 656c 2229  nt.find("Model")
-0000be50: 2e66 696e 6428 2241 6c6c 5472 6163 6b73  .find("AllTracks
-0000be60: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000be70: 7365 6c66 2e73 6574 7469 6e67 7320 3d20  self.settings = 
-0000be80: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-0000be90: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
-0000bea0: 292e 6669 6e64 2822 496d 6167 6544 6174  ).find("ImageDat
-0000beb0: 6122 290d 0a20 2020 2020 2020 2020 2020  a")..           
-0000bec0: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-0000bed0: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
-0000bee0: 7365 7474 696e 6773 2e67 6574 2822 7069  settings.get("pi
-0000bef0: 7865 6c77 6964 7468 2229 290d 0a20 2020  xelwidth"))..   
-0000bf00: 2020 2020 2020 2020 2073 656c 662e 7963           self.yc
-0000bf10: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
-0000bf20: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
-0000bf30: 2e67 6574 2822 7069 7865 6c68 6569 6768  .get("pixelheigh
-0000bf40: 7422 2929 0d0a 2020 2020 2020 2020 2020  t"))..          
-0000bf50: 2020 7365 6c66 2e7a 6361 6c69 6272 6174    self.zcalibrat
-0000bf60: 696f 6e20 3d20 666c 6f61 7428 7365 6c66  ion = float(self
-0000bf70: 2e73 6574 7469 6e67 732e 6765 7428 2276  .settings.get("v
-0000bf80: 6f78 656c 6465 7074 6822 2929 0d0a 2020  oxeldepth"))..  
-0000bf90: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000bfa0: 6361 6c69 6272 6174 696f 6e20 3d20 696e  calibration = in
-0000bfb0: 7428 666c 6f61 7428 7365 6c66 2e73 6574  t(float(self.set
-0000bfc0: 7469 6e67 732e 6765 7428 2274 696d 6569  tings.get("timei
-0000bfd0: 6e74 6572 7661 6c22 2929 290d 0a20 2020  nterval")))..   
-0000bfe0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-0000bff0: 7465 6374 6f72 7365 7474 696e 6773 203d  tectorsettings =
-0000c000: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000c010: 742e 6669 6e64 2822 5365 7474 696e 6773  t.find("Settings
-0000c020: 2229 2e66 696e 6428 2244 6574 6563 746f  ").find("Detecto
-0000c030: 7253 6574 7469 6e67 7322 290d 0a20 2020  rSettings")..   
-0000c040: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
-0000c050: 7369 6373 6574 7469 6e67 7320 3d20 7365  sicsettings = se
-0000c060: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000c070: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
-0000c080: 6669 6e64 2822 4261 7369 6353 6574 7469  find("BasicSetti
-0000c090: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
-0000c0a0: 2020 2073 656c 662e 6465 7465 6374 6f72     self.detector
-0000c0b0: 6368 616e 6e65 6c20 3d20 696e 7428 666c  channel = int(fl
-0000c0c0: 6f61 7428 7365 6c66 2e64 6574 6563 746f  oat(self.detecto
-0000c0d0: 7273 6574 7469 6e67 732e 6765 7428 2254  rsettings.get("T
-0000c0e0: 4152 4745 545f 4348 414e 4e45 4c22 2929  ARGET_CHANNEL"))
-0000c0f0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0000c100: 656c 662e 7473 7461 7274 203d 2069 6e74  elf.tstart = int
-0000c110: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
-0000c120: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
-0000c130: 7374 6172 7422 2929 290d 0a20 2020 2020  start")))..     
-0000c140: 2020 2020 2020 2073 656c 662e 7465 6e64         self.tend
-0000c150: 203d 2069 6e74 2866 6c6f 6174 2873 656c   = int(float(sel
-0000c160: 662e 6261 7369 6373 6574 7469 6e67 732e  f.basicsettings.
-0000c170: 6765 7428 2274 656e 6422 2929 2920 2020  get("tend")))   
-0000c180: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-0000c190: 2020 2070 7269 6e74 2827 4974 6572 6174     print('Iterat
-0000c1a0: 696e 6720 6f76 6572 2073 706f 7473 2069  ing over spots i
-0000c1b0: 6e20 6672 616d 6527 290d 0a20 2020 2020  n frame')..     
-0000c1c0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
-0000c1d0: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
-0000c1e0: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
-0000c1f0: 0a0d 0a20 2020 2020 2020 2020 2020 2077  ...            w
-0000c200: 6974 6820 636f 6e63 7572 7265 6e74 2e66  ith concurrent.f
-0000c210: 7574 7572 6573 2e54 6872 6561 6450 6f6f  utures.ThreadPoo
-0000c220: 6c45 7865 6375 746f 7228 6d61 785f 776f  lExecutor(max_wo
-0000c230: 726b 6572 7320 3d20 6f73 2e63 7075 5f63  rkers = os.cpu_c
-0000c240: 6f75 6e74 2829 2920 6173 2065 7865 6375  ount()) as execu
-0000c250: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
-0000c260: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000c270: 2020 2020 2020 2020 666f 7220 6672 616d          for fram
-0000c280: 6520 696e 2073 656c 662e 5370 6f74 6f62  e in self.Spotob
-0000c290: 6a65 6374 732e 6669 6e64 616c 6c28 2753  jects.findall('S
-0000c2a0: 706f 7473 496e 4672 616d 6527 293a 0d0a  potsInFrame'):..
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-0000c2d0: 7265 732e 6170 7065 6e64 2865 7865 6375  res.append(execu
-0000c2e0: 746f 722e 7375 626d 6974 2873 656c 662e  tor.submit(self.
-0000c2f0: 5f6d 6173 7465 725f 7370 6f74 5f63 6f6d  _master_spot_com
-0000c300: 7075 7465 722c 2066 7261 6d65 2929 0d0a  puter, frame))..
-0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c320: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-0000c330: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-0000c340: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c360: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000c390: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
-0000c3a0: 436f 6c6c 6563 7469 6e67 2053 706f 7473  Collecting Spots
-0000c3b0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0000c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3d0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000c3e0: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
-0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c410: 2020 2020 302c 0d0a 2020 2020 2020 2020      0,..        
-0000c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c430: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
-0000c440: 6675 7475 7265 7329 2c0d 0a20 2020 2020  futures),..     
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c490: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000c4a0: 7368 6f77 2829 0d0a 0d0a 2020 2020 2020  show()....      
-0000c4b0: 2020 2020 2020 2020 2020 666f 7220 7220            for r 
-0000c4c0: 696e 2063 6f6e 6375 7272 656e 742e 6675  in concurrent.fu
-0000c4d0: 7475 7265 732e 6173 5f63 6f6d 706c 6574  tures.as_complet
-0000c4e0: 6564 2866 7574 7572 6573 293a 0d0a 2020  ed(futures):..  
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c500: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c510: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000c520: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c540: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000c550: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000c560: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c590: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000c5a0: 6261 722e 7661 6c75 6520 3d20 2073 656c  bar.value =  sel
-0000c5b0: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 2020 2020 2020 2020 2072 2e72 6573 756c           r.resul
-0000c5e0: 7428 2920 2020 200d 0a0d 0a20 2020 2020  t()    ....     
-0000c5f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c600: 2020 2020 2070 7269 6e74 2866 2749 7465       print(f'Ite
-0000c610: 7261 7469 6e67 206f 7665 7220 7472 6163  rating over trac
-0000c620: 6b73 207b 6c65 6e28 7365 6c66 2e66 696c  ks {len(self.fil
-0000c630: 7465 7265 645f 7472 6163 6b5f 6964 7329  tered_track_ids)
-0000c640: 7d27 2920 200d 0a20 2020 2020 2020 2020  }')  ..         
-0000c650: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-0000c660: 300d 0a20 2020 2020 2020 2020 2020 2066  0..            f
-0000c670: 7574 7572 6573 203d 205b 5d0d 0a20 2020  utures = []..   
-0000c680: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-0000c690: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-0000c6a0: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
-0000c6b0: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
-0000c6c0: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
-0000c6d0: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
-0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c700: 2020 666f 7220 7472 6163 6b20 696e 2073    for track in s
-0000c710: 656c 662e 7472 6163 6b73 2e66 696e 6461  elf.tracks.finda
-0000c720: 6c6c 2827 5472 6163 6b27 293a 0d0a 2020  ll('Track'):..  
-0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c740: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c760: 7472 6163 6b5f 6964 203d 2069 6e74 2874  track_id = int(t
-0000c770: 7261 636b 2e67 6574 2873 656c 662e 7472  rack.get(self.tr
-0000c780: 6163 6b69 645f 6b65 7929 290d 0a20 2020  ackid_key))..   
-0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2020 2069 6620 7472 6163 6b5f 6964       if track_id
-0000c7b0: 2069 6e20 7365 6c66 2e66 696c 7465 7265   in self.filtere
-0000c7c0: 645f 7472 6163 6b5f 6964 733a 0d0a 2020  d_track_ids:..  
-0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7e0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-0000c7f0: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
-0000c800: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
-0000c810: 662e 5f6d 6173 7465 725f 7472 6163 6b5f  f._master_track_
-0000c820: 636f 6d70 7574 6572 2c20 7472 6163 6b2c  computer, track,
-0000c830: 2074 7261 636b 5f69 6429 290d 0a20 2020   track_id))..   
-0000c840: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000c850: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000c860: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8b0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000c8c0: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
-0000c8d0: 6c65 6374 696e 6720 5472 6163 6b73 220d  lecting Tracks".
-0000c8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c900: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000c910: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
-0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c940: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c960: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
-0000c970: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
-0000c980: 6b5f 6964 7329 2c0d 0a20 2020 2020 2020  k_ids),..       
-0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9a0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c9d0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000c9e0: 6f77 2829 0d0a 0d0a 0d0a 2020 2020 2020  ow()......      
-0000c9f0: 2020 2020 2020 2020 2020 666f 7220 7220            for r 
-0000ca00: 696e 2063 6f6e 6375 7272 656e 742e 6675  in concurrent.fu
-0000ca10: 7475 7265 732e 6173 5f63 6f6d 706c 6574  tures.as_complet
-0000ca20: 6564 2866 7574 7572 6573 293a 0d0a 2020  ed(futures):..  
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ca50: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000ca60: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca80: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000ca90: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000caa0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cad0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000cae0: 6261 722e 7661 6c75 6520 3d20 7365 6c66  bar.value = self
-0000caf0: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
-0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb10: 2020 2020 2020 2020 722e 7265 7375 6c74          r.result
-0000cb20: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000cb30: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000cb40: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-0000cb50: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-0000cb60: 6f6e 653a 2020 0d0a 2020 2020 2020 2020  one:  ..        
-0000cb70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000cb80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cb90: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
-0000cba0: 6561 7465 5f73 6563 6f6e 645f 6368 616e  eate_second_chan
-0000cbb0: 6e65 6c5f 786d 6c28 290d 0a20 2020 2020  nel_xml()..     
-0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbd0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-0000cbe0: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-0000cbf0: 6e20 7365 6c66 2e67 7261 7068 5f73 706c  n self.graph_spl
-0000cc00: 6974 2e69 7465 6d73 2829 3a0d 0a20 2020  it.items():..   
-0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc40: 2020 2020 2020 6461 7567 6874 6572 5f74        daughter_t
-0000cc50: 7261 636b 5f69 6420 3d20 2069 6e74 2866  rack_id =  int(f
-0000cc60: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
-0000cc70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000cc80: 7469 6573 5b69 6e74 2866 6c6f 6174 286b  ties[int(float(k
-0000cc90: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
-0000cca0: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
+0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8d0: 2020 2020 2020 544f 5441 4c5f 494e 5445        TOTAL_INTE
+0000b8e0: 4e53 4954 5920 3d20 2d31 0d0a 2020 2020  NSITY = -1..    
+0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b910: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
+0000b920: 5920 3d20 2d31 2020 2020 2020 200d 0a20  Y = -1       .. 
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 2020 2020 2020 2065 6c73 653a 2020 2020         else:    
+0000b950: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b970: 2020 2020 2020 6966 2053 706f 746f 626a        if Spotobj
+0000b980: 6563 742e 6765 7428 7365 6c66 2e74 6f74  ect.get(self.tot
+0000b990: 616c 5f69 6e74 656e 7369 7479 5f63 6831  al_intensity_ch1
+0000b9a0: 5f6b 6579 2920 6973 206e 6f74 204e 6f6e  _key) is not Non
+0000b9b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9d0: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
+0000b9e0: 4c5f 494e 5445 4e53 4954 5920 3d20 666c  L_INTENSITY = fl
+0000b9f0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000ba00: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
+0000ba10: 7465 6e73 6974 795f 6368 315f 6b65 7929  tensity_ch1_key)
+0000ba20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba40: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
+0000ba50: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000ba60: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000ba70: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
+0000ba80: 7369 7479 5f63 6831 5f6b 6579 2929 0d0a  sity_ch1_key))..
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bab0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0000bae0: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
+0000baf0: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
+0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb10: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
+0000bb20: 4e5f 494e 5445 4e53 4954 5920 3d20 2d31  N_INTENSITY = -1
+0000bb30: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb50: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb70: 2020 2020 2020 2052 4144 4955 5320 3d20         RADIUS = 
+0000bb80: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000bb90: 2e67 6574 2873 656c 662e 7261 6469 7573  .get(self.radius
+0000bba0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbc0: 5155 414c 4954 5920 3d20 666c 6f61 7428  QUALITY = float(
+0000bbd0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000bbe0: 656c 662e 7175 616c 6974 795f 6b65 7929  elf.quality_key)
+0000bbf0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000bc00: 2020 2020 2020 2020 2020 2074 6573 746c             testl
+0000bc10: 6f63 6174 696f 6e20 3d20 2866 6c6f 6174  ocation = (float
+0000bc20: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000bc30: 7365 6c66 2e7a 706f 7369 645f 6b65 7929  self.zposid_key)
+0000bc40: 292c 2066 6c6f 6174 2853 706f 746f 626a  ), float(Spotobj
+0000bc50: 6563 742e 6765 7428 7365 6c66 2e79 706f  ect.get(self.ypo
+0000bc60: 7369 645f 6b65 7929 292c 2020 666c 6f61  sid_key)),  floa
+0000bc70: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000bc80: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
+0000bc90: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000bca0: 2020 2020 2020 2020 2020 2020 2066 7261               fra
+0000bcb0: 6d65 203d 2053 706f 746f 626a 6563 742e  me = Spotobject.
+0000bcc0: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
+0000bcd0: 5f6b 6579 290d 0a20 2020 2020 2020 2020  _key)..         
+0000bce0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000bcf0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0000bd00: 6b2c 206d 6173 6b63 656e 7472 6f69 6420  k, maskcentroid 
+0000bd10: 3d20 7365 6c66 2e5f 6765 745f 626f 756e  = self._get_boun
+0000bd20: 6461 7279 5f64 6973 7428 6672 616d 652c  dary_dist(frame,
+0000bd30: 2074 6573 746c 6f63 6174 696f 6e29 0d0a   testlocation)..
+0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd50: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd70: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+0000bd80: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000bd90: 6c6c 5f69 645d 203d 207b 0d0a 2020 2020  ll_id] = {..    
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
+0000bdc0: 6c69 645f 6b65 793a 2069 6e74 2863 656c  lid_key: int(cel
+0000bdd0: 6c5f 6964 292c 200d 0a20 2020 2020 2020  l_id), ..       
+0000bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdf0: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
+0000be00: 645f 6b65 7920 3a20 696e 7428 666c 6f61  d_key : int(floa
+0000be10: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000be20: 2873 656c 662e 6672 616d 6569 645f 6b65  (self.frameid_ke
+0000be30: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
+0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be50: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
+0000be60: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000be70: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
+0000be80: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bea0: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
+0000beb0: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
+0000bec0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000bed0: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
+0000bee0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf00: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+0000bf10: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000bf20: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
+0000bf30: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf50: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+0000bf60: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
+0000bf70: 203a 2054 4f54 414c 5f49 4e54 454e 5349   : TOTAL_INTENSI
+0000bf80: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
+0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfa0: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+0000bfb0: 7369 7479 5f6b 6579 203a 204d 4541 4e5f  sity_key : MEAN_
+0000bfc0: 494e 5445 4e53 4954 592c 0d0a 2020 2020  INTENSITY,..    
+0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfe0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+0000bff0: 6975 735f 6b65 7920 3a20 5241 4449 5553  ius_key : RADIUS
+0000c000: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c010: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c020: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
+0000c030: 3a20 5155 414c 4954 592c 0d0a 2020 2020  : QUALITY,..    
+0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c050: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
+0000c060: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
+0000c070: 6b65 793a 2066 6c6f 6174 2864 6973 7461  key: float(dista
+0000c080: 6e63 655f 6365 6c6c 5f6d 6173 6b29 2c0d  nce_cell_mask),.
+0000c090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c0a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c0b0: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
+0000c0c0: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
+0000c0d0: 6365 6e74 726f 6964 5b30 5d29 2c0d 0a20  centroid[0]),.. 
+0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c100: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
+0000c110: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+0000c120: 6e74 726f 6964 5b31 5d29 2c0d 0a20 2020  ntroid[1]),..   
+0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c140: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000c150: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
+0000c160: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+0000c170: 726f 6964 5b32 5d29 200d 0a20 2020 2020  roid[2]) ..     
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2020 207d 0d0a 2020 2020 2020 200d 0a20     }..       .. 
+0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000c1c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000c1d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000c1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 2020 2020 200d 0a0d 0a20 2020 200d 0a20       ....    .. 
+0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c220: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
+0000c230: 6566 205f 6765 745f 6d61 7374 6572 5f78  ef _get_master_x
+0000c240: 6d6c 5f64 6174 6128 7365 6c66 293a 0d0a  ml_data(self):..
+0000c250: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000c260: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
+0000c270: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+0000c280: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000c290: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000c2a0: 6861 6e6e 656c 5f78 6d6c 5f63 6f6e 7465  hannel_xml_conte
+0000c2b0: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
+0000c2c0: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
+0000c2d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c2e0: 662e 786d 6c5f 7472 6565 203d 2065 742e  f.xml_tree = et.
+0000c2f0: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
+0000c300: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000c310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c320: 2e78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  .xml_root = self
+0000c330: 2e78 6d6c 5f74 7265 652e 6765 7472 6f6f  .xml_tree.getroo
+0000c340: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+0000c350: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c360: 6368 616e 6e65 6c5f 786d 6c5f 6e61 6d65  channel_xml_name
+0000c370: 203d 2027 7365 636f 6e64 5f63 6861 6e6e   = 'second_chann
+0000c380: 656c 5f27 202b 206f 732e 7061 7468 2e73  el_' + os.path.s
+0000c390: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
+0000c3a0: 6261 7365 6e61 6d65 2873 656c 662e 786d  basename(self.xm
+0000c3b0: 6c5f 7061 7468 2929 5b30 5d20 2b20 272e  l_path))[0] + '.
+0000c3c0: 786d 6c27 0d0a 2020 2020 2020 2020 2020  xml'..          
+0000c3d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c3e0: 2e63 6861 6e6e 656c 5f78 6d6c 5f70 6174  .channel_xml_pat
+0000c3f0: 6820 3d20 6f73 2e70 6174 682e 6469 726e  h = os.path.dirn
+0000c400: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
+0000c410: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+0000c420: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000c430: 6372 6561 7465 5f63 6861 6e6e 656c 5f74  create_channel_t
+0000c440: 7265 6528 290d 0a0d 0a20 2020 2020 2020  ree()....       
+0000c450: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+0000c460: 5f6f 626a 6563 7473 203d 207b 7d0d 0a20  _objects = {}.. 
+0000c470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c480: 756e 6971 7565 5f70 726f 7065 7274 6965  unique_propertie
+0000c490: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+0000c4a0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+0000c4b0: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
+0000c4c0: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
+0000c4d0: 6469 6e67 5472 6163 6b49 6473 203d 205b  dingTrackIds = [
+0000c4e0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+0000c4f0: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+0000c500: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
+0000c510: 2020 2020 2073 656c 662e 616c 6c5f 7472       self.all_tr
+0000c520: 6163 6b5f 7072 6f70 6572 7469 6573 203d  ack_properties =
+0000c530: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000c540: 2073 656c 662e 7370 6c69 745f 706f 696e   self.split_poin
+0000c550: 7473 5f74 696d 6573 203d 205b 5d0d 0a0d  ts_times = []...
+0000c560: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000c570: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000c580: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
+0000c590: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000c5a0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000c5b0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000c5c0: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
+0000c5d0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000c5e0: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
+0000c5f0: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
+0000c600: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+0000c610: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000c620: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
+0000c630: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
+0000c640: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
+0000c650: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+0000c660: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+0000c670: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
+0000c680: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
+0000c690: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+0000c6a0: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
+0000c6b0: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
+0000c6c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000c6d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000c6e0: 2020 2020 2020 7365 6c66 2e53 706f 746f        self.Spoto
+0000c6f0: 626a 6563 7473 203d 2073 656c 662e 786d  bjects = self.xm
+0000c700: 6c5f 636f 6e74 656e 742e 6669 6e64 2827  l_content.find('
+0000c710: 4d6f 6465 6c27 292e 6669 6e64 2827 416c  Model').find('Al
+0000c720: 6c53 706f 7473 2729 0d0a 2020 2020 2020  lSpots')..      
+0000c730: 2020 2020 2020 2320 4578 7472 6163 7420        # Extract 
+0000c740: 7468 6520 7472 6163 6b73 2066 726f 6d20  the tracks from 
+0000c750: 786d 6c0d 0a20 2020 2020 2020 2020 2020  xml..           
+0000c760: 2073 656c 662e 7472 6163 6b73 203d 2073   self.tracks = s
+0000c770: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000c780: 6669 6e64 2822 4d6f 6465 6c22 292e 6669  find("Model").fi
+0000c790: 6e64 2822 416c 6c54 7261 636b 7322 290d  nd("AllTracks").
+0000c7a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c7b0: 662e 7365 7474 696e 6773 203d 2073 656c  f.settings = sel
+0000c7c0: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000c7d0: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000c7e0: 696e 6428 2249 6d61 6765 4461 7461 2229  ind("ImageData")
+0000c7f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000c800: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
+0000c810: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
+0000c820: 7469 6e67 732e 6765 7428 2270 6978 656c  tings.get("pixel
+0000c830: 7769 6474 6822 2929 0d0a 2020 2020 2020  width"))..      
+0000c840: 2020 2020 2020 7365 6c66 2e79 6361 6c69        self.ycali
+0000c850: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
+0000c860: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000c870: 7428 2270 6978 656c 6865 6967 6874 2229  t("pixelheight")
+0000c880: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000c890: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+0000c8a0: 203d 2066 6c6f 6174 2873 656c 662e 7365   = float(self.se
+0000c8b0: 7474 696e 6773 2e67 6574 2822 766f 7865  ttings.get("voxe
+0000c8c0: 6c64 6570 7468 2229 290d 0a20 2020 2020  ldepth"))..     
+0000c8d0: 2020 2020 2020 2073 656c 662e 7463 616c         self.tcal
+0000c8e0: 6962 7261 7469 6f6e 203d 2069 6e74 2866  ibration = int(f
+0000c8f0: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+0000c900: 6773 2e67 6574 2822 7469 6d65 696e 7465  gs.get("timeinte
+0000c910: 7276 616c 2229 2929 0d0a 2020 2020 2020  rval")))..      
+0000c920: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
+0000c930: 746f 7273 6574 7469 6e67 7320 3d20 7365  torsettings = se
+0000c940: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000c950: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
+0000c960: 6669 6e64 2822 4465 7465 6374 6f72 5365  find("DetectorSe
+0000c970: 7474 696e 6773 2229 0d0a 2020 2020 2020  ttings")..      
+0000c980: 2020 2020 2020 7365 6c66 2e62 6173 6963        self.basic
+0000c990: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
+0000c9a0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000c9b0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
+0000c9c0: 6428 2242 6173 6963 5365 7474 696e 6773  d("BasicSettings
+0000c9d0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000c9e0: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
+0000c9f0: 6e6e 656c 203d 2069 6e74 2866 6c6f 6174  nnel = int(float
+0000ca00: 2873 656c 662e 6465 7465 6374 6f72 7365  (self.detectorse
+0000ca10: 7474 696e 6773 2e67 6574 2822 5441 5247  ttings.get("TARG
+0000ca20: 4554 5f43 4841 4e4e 454c 2229 2929 0d0a  ET_CHANNEL")))..
+0000ca30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ca40: 2e74 7374 6172 7420 3d20 696e 7428 666c  .tstart = int(fl
+0000ca50: 6f61 7428 7365 6c66 2e62 6173 6963 7365  oat(self.basicse
+0000ca60: 7474 696e 6773 2e67 6574 2822 7473 7461  ttings.get("tsta
+0000ca70: 7274 2229 2929 0d0a 2020 2020 2020 2020  rt")))..        
+0000ca80: 2020 2020 7365 6c66 2e74 656e 6420 3d20      self.tend = 
+0000ca90: 696e 7428 666c 6f61 7428 7365 6c66 2e62  int(float(self.b
+0000caa0: 6173 6963 7365 7474 696e 6773 2e67 6574  asicsettings.get
+0000cab0: 2822 7465 6e64 2229 2929 2020 2020 2020  ("tend")))      
+0000cac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000cad0: 7072 696e 7428 2749 7465 7261 7469 6e67  print('Iterating
+0000cae0: 206f 7665 7220 7370 6f74 7320 696e 2066   over spots in f
+0000caf0: 7261 6d65 2729 0d0a 2020 2020 2020 2020  rame')..        
+0000cb00: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+0000cb10: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+0000cb20: 6675 7475 7265 7320 3d20 5b5d 0d0a 0d0a  futures = []....
+0000cb30: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000cb40: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+0000cb50: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
+0000cb60: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
+0000cb70: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
+0000cb80: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
+0000cb90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000cba0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000cbb0: 2020 2020 2066 6f72 2066 7261 6d65 2069       for frame i
+0000cbc0: 6e20 7365 6c66 2e53 706f 746f 626a 6563  n self.Spotobjec
+0000cbd0: 7473 2e66 696e 6461 6c6c 2827 5370 6f74  ts.findall('Spot
+0000cbe0: 7349 6e46 7261 6d65 2729 3a0d 0a20 2020  sInFrame'):..   
+0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc00: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+0000cc10: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
+0000cc20: 2e73 7562 6d69 7428 7365 6c66 2e5f 6d61  .submit(self._ma
+0000cc30: 7374 6572 5f73 706f 745f 636f 6d70 7574  ster_spot_comput
+0000cc40: 6572 2c20 6672 616d 6529 290d 0a20 2020  er, frame))..   
+0000cc50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000cc60: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000cc70: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccc0: 2020 2020 2020 2070 6172 656e 745f 7472         parent_tr
-0000ccd0: 6163 6b5f 6964 203d 2069 6e74 2866 6c6f  ack_id = int(flo
-0000cce0: 6174 2873 7472 2873 656c 662e 756e 6971  at(str(self.uniq
-0000ccf0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000cd00: 6573 5b69 6e74 2866 6c6f 6174 2876 2929  es[int(float(v))
-0000cd10: 5d5b 7365 6c66 2e75 6e69 7175 6569 645f  ][self.uniqueid_
-0000cd20: 6b65 795d 2929 290d 0a20 2020 2020 2020  key])))..       
+0000ccc0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000ccd0: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
+0000cce0: 6c65 6374 696e 6720 5370 6f74 7322 0d0a  lecting Spots"..
+0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd10: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000cd20: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
 0000cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd40: 2020 2020 2073 656c 662e 6772 6170 685f       self.graph_
-0000cd50: 7472 6163 6b73 5b64 6175 6768 7465 725f  tracks[daughter_
-0000cd60: 7472 6163 6b5f 6964 5d20 3d20 7061 7265  track_id] = pare
-0000cd70: 6e74 5f74 7261 636b 5f69 640d 0a0d 0a20  nt_track_id.... 
-0000cd80: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000cd90: 2827 6765 7474 696e 6720 6174 7472 6962  ('getting attrib
-0000cda0: 7574 6573 2729 2020 2020 2020 2020 2020  utes')          
-0000cdb0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000cdc0: 2020 2020 7365 6c66 2e5f 6765 745f 6174      self._get_at
-0000cdd0: 7472 6962 7574 6573 2829 0d0a 2020 2020  tributes()..    
-0000cde0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000cdf0: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-0000ce00: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
-0000ce10: 2066 6f72 2074 7261 636b 5f69 6420 696e   for track_id in
-0000ce20: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
-0000ce30: 7261 636b 5f69 6473 3a0d 0a20 2020 2020  rack_ids:..     
-0000ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000ce60: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-0000ce70: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-0000ce80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cea0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000ceb0: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-0000cec0: 6c20 3d20 224a 7573 7420 6f6e 6520 6d6f  l = "Just one mo
-0000ced0: 7265 2074 6869 6e67 220d 0a20 2020 2020  re thing"..     
-0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf00: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000cf10: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf50: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf80: 2020 2020 6c65 6e28 7365 6c66 2e66 696c      len(self.fil
-0000cf90: 7465 7265 645f 7472 6163 6b5f 6964 7329  tered_track_ids)
-0000cfa0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000cfd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cff0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000d000: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
-0000d010: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d030: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d040: 2e63 6f75 6e74 203d 2073 656c 662e 636f  .count = self.co
-0000d050: 756e 7420 2b20 310d 0a20 2020 2020 2020  unt + 1..       
-0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd50: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 2020 2020 2020 206c 656e 2866 7574           len(fut
+0000cd80: 7572 6573 292c 0d0a 2020 2020 2020 2020  ures),..        
+0000cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cda0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cdd0: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
+0000cde0: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
+0000cdf0: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
+0000ce00: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+0000ce10: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
+0000ce20: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
+0000ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ce50: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+0000ce60: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ce90: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000cea0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ced0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000cee0: 2e76 616c 7565 203d 2020 7365 6c66 2e63  .value =  self.c
+0000cef0: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf10: 2020 2020 2020 722e 7265 7375 6c74 2829        r.result()
+0000cf20: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0000cf30: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000cf40: 2020 7072 696e 7428 6627 4974 6572 6174    print(f'Iterat
+0000cf50: 696e 6720 6f76 6572 2074 7261 636b 7320  ing over tracks 
+0000cf60: 7b6c 656e 2873 656c 662e 6669 6c74 6572  {len(self.filter
+0000cf70: 6564 5f74 7261 636b 5f69 6473 297d 2729  ed_track_ids)}')
+0000cf80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000cf90: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
+0000cfa0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
+0000cfb0: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
+0000cfc0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
+0000cfd0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
+0000cfe0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
+0000cff0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
+0000d000: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
+0000d010: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
+0000d020: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000d030: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d040: 6f72 2074 7261 636b 2069 6e20 7365 6c66  or track in self
+0000d050: 2e74 7261 636b 732e 6669 6e64 616c 6c28  .tracks.findall(
+0000d060: 2754 7261 636b 2729 3a0d 0a20 2020 2020  'Track'):..     
 0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d080: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000d090: 6172 2e76 616c 7565 203d 2073 656c 662e  ar.value = self.
-0000d0a0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d0d0: 5f66 696e 616c 5f74 7261 636b 7328 7472  _final_tracks(tr
-0000d0e0: 6163 6b5f 6964 2920 0d0a 0d0a 2020 2020  ack_id) ....    
-0000d0f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d100: 666f 7572 6965 723a 0d0a 2020 2020 2020  fourier:..      
-0000d110: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000d120: 6e74 2827 636f 6d70 7574 696e 6720 466f  nt('computing Fo
-0000d130: 7572 6965 7227 290d 0a20 2020 2020 2020  urier')..       
-0000d140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d150: 2e5f 636f 6d70 7574 655f 7068 656e 6f74  ._compute_phenot
-0000d160: 7970 6573 2829 2020 2020 2020 2020 2020  ypes()          
-0000d170: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000d180: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d190: 2e5f 7465 6d70 6f72 616c 5f70 6c6f 7473  ._temporal_plots
-0000d1a0: 5f74 7261 636b 6d61 7465 2829 2020 2020  _trackmate()    
-0000d1b0: 2020 2020 0d0a 0d0a 0d0a 2020 2020 6465      ......    de
-0000d1c0: 6620 5f63 7265 6174 655f 7365 636f 6e64  f _create_second
-0000d1d0: 5f63 6861 6e6e 656c 5f78 6d6c 2873 656c  _channel_xml(sel
-0000d1e0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-0000d1f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d200: 2020 2020 2020 7072 696e 7428 2754 7261        print('Tra
-0000d210: 6e73 6665 7272 696e 6720 584d 4c27 2920  nsferring XML') 
-0000d220: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d230: 2020 2020 2020 2020 6368 616e 6e65 6c5f          channel_
-0000d240: 6669 6c74 6572 6564 5f74 7261 636b 7320  filtered_tracks 
-0000d250: 3d20 5b5d 2020 2020 2020 2020 2020 2020  = []            
-0000d260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d270: 2020 2020 2020 666f 7220 5370 6f74 6f62        for Spotob
-0000d280: 6a65 6374 2069 6e20 7365 6c66 2e78 6d6c  ject in self.xml
-0000d290: 5f72 6f6f 742e 6974 6572 2827 5370 6f74  _root.iter('Spot
-0000d2a0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2c0: 2063 656c 6c5f 6964 203d 2069 6e74 2853   cell_id = int(S
-0000d2d0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000d2e0: 6c66 2e73 706f 7469 645f 6b65 7929 290d  lf.spotid_key)).
-0000d2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d300: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d310: 6365 6c6c 5f69 6420 696e 2073 656c 662e  cell_id in self.
-0000d320: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000d330: 706f 745f 7072 6f70 6572 7469 6573 2e6b  pot_properties.k
-0000d340: 6579 7328 293a 2020 2020 2020 2020 0d0a  eys():        ..
-0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d360: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000d080: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000d090: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0000d0a0: 636b 5f69 6420 3d20 696e 7428 7472 6163  ck_id = int(trac
+0000d0b0: 6b2e 6765 7428 7365 6c66 2e74 7261 636b  k.get(self.track
+0000d0c0: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 6966 2074 7261 636b 5f69 6420 696e    if track_id in
+0000d0f0: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
+0000d100: 7261 636b 5f69 6473 3a0d 0a20 2020 2020  rack_ids:..     
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+0000d130: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
+0000d140: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
+0000d150: 6d61 7374 6572 5f74 7261 636b 5f63 6f6d  master_track_com
+0000d160: 7075 7465 722c 2074 7261 636b 2c20 7472  puter, track, tr
+0000d170: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
+0000d180: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000d190: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000d1a0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1c0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d1f0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000d200: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
+0000d210: 7469 6e67 2054 7261 636b 7322 0d0a 2020  ting Tracks"..  
+0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d230: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d240: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000d250: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
+0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0000d280: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2a0: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
+0000d2b0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+0000d2c0: 6473 292c 0d0a 2020 2020 2020 2020 2020  ds),..          
+0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2e0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000d310: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+0000d320: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+0000d330: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
+0000d340: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+0000d350: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
+0000d360: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
 0000d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2020 6e65 775f 706f 7369 7469 6f6e 7820    new_positionx 
-0000d3a0: 3d20 2073 656c 662e 6368 616e 6e65 6c5f  =  self.channel_
-0000d3b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000d3c0: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
-0000d3d0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-0000d3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d390: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+0000d3a0: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+0000d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d3d0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000d3e0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
 0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d400: 2020 2020 2020 6e65 775f 706f 7369 7469        new_positi
-0000d410: 6f6e 7920 3d20 2073 656c 662e 6368 616e  ony =  self.chan
-0000d420: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000d430: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-0000d440: 6964 5d5b 7365 6c66 2e79 706f 7369 645f  id][self.yposid_
-0000d450: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
-0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d470: 2020 2020 2020 2020 2020 6e65 775f 706f            new_po
-0000d480: 7369 7469 6f6e 7a20 3d20 2073 656c 662e  sitionz =  self.
-0000d490: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000d4a0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000d4b0: 656c 6c5f 6964 5d5b 7365 6c66 2e7a 706f  ell_id][self.zpo
-0000d4c0: 7369 645f 6b65 795d 0d0a 0d0a 2020 2020  sid_key]....    
-0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4f0: 6e65 775f 746f 7461 6c5f 696e 7465 6e73  new_total_intens
-0000d500: 6974 7920 3d20 7365 6c66 2e63 6861 6e6e  ity = self.chann
-0000d510: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-0000d520: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-0000d530: 645d 5b73 656c 662e 746f 7461 6c5f 696e  d][self.total_in
-0000d540: 7465 6e73 6974 795f 6b65 795d 0d0a 2020  tensity_key]..  
+0000d400: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d410: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000d420: 2e76 616c 7565 203d 2073 656c 662e 636f  .value = self.co
+0000d430: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 2020 2020 2072 2e72 6573 756c 7428 290d       r.result().
+0000d460: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000d470: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000d480: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+0000d490: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+0000d4a0: 3a20 200d 0a20 2020 2020 2020 2020 2020  :  ..           
+0000d4b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
+0000d4e0: 655f 7365 636f 6e64 5f63 6861 6e6e 656c  e_second_channel
+0000d4f0: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
+0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d510: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000d520: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+0000d530: 656c 662e 6772 6170 685f 7370 6c69 742e  elf.graph_split.
+0000d540: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
 0000d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d570: 2020 6e65 775f 6d65 616e 5f69 6e74 656e    new_mean_inten
-0000d580: 7369 7479 203d 2073 656c 662e 6368 616e  sity = self.chan
-0000d590: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000d5a0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-0000d5b0: 6964 5d5b 7365 6c66 2e6d 6561 6e5f 696e  id][self.mean_in
-0000d5c0: 7465 6e73 6974 795f 6b65 795d 0d0a 0d0a  tensity_key]....
-0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5f0: 2020 2020 6e65 775f 7261 6469 7573 203d      new_radius =
-0000d600: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000d610: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000d620: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000d630: 6c66 2e72 6164 6975 735f 6b65 795d 0d0a  lf.radius_key]..
-0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d660: 2020 2020 6e65 775f 7175 616c 6974 7920      new_quality 
-0000d670: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f75  = self.channel_u
-0000d680: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000d690: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
-0000d6a0: 656c 662e 7175 616c 6974 795f 6b65 795d  elf.quality_key]
-0000d6b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6d0: 2020 2020 2020 6e65 775f 6469 7374 616e        new_distan
-0000d6e0: 6365 5f63 656c 6c5f 6d61 736b 203d 2073  ce_cell_mask = s
-0000d6f0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-0000d700: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000d710: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
-0000d720: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-0000d730: 6173 6b5f 6b65 795d 0d0a 0d0a 2020 2020  ask_key]....    
-0000d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 5370 6f74 6f62 6a65 6374 2e73 6574 2873  Spotobject.set(s
-0000d770: 656c 662e 7870 6f73 6964 5f6b 6579 2c20  elf.xposid_key, 
-0000d780: 7374 7228 6e65 775f 706f 7369 7469 6f6e  str(new_position
-0000d790: 7829 2920 2020 2020 0d0a 2020 2020 2020  x))     ..      
-0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7b0: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-0000d7c0: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
-0000d7d0: 662e 7970 6f73 6964 5f6b 6579 2c20 7374  f.yposid_key, st
-0000d7e0: 7228 6e65 775f 706f 7369 7469 6f6e 7929  r(new_positiony)
-0000d7f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d810: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
-0000d820: 742e 7365 7428 7365 6c66 2e7a 706f 7369  t.set(self.zposi
-0000d830: 645f 6b65 792c 2073 7472 286e 6577 5f70  d_key, str(new_p
-0000d840: 6f73 6974 696f 6e7a 2929 0d0a 0d0a 2020  ositionz))....  
-0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d560: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d580: 2020 2064 6175 6768 7465 725f 7472 6163     daughter_trac
+0000d590: 6b5f 6964 203d 2020 696e 7428 666c 6f61  k_id =  int(floa
+0000d5a0: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
+0000d5b0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000d5c0: 735b 696e 7428 666c 6f61 7428 6b29 295d  s[int(float(k))]
+0000d5d0: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
+0000d5e0: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
+0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d600: 2020 2020 7061 7265 6e74 5f74 7261 636b      parent_track
+0000d610: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
+0000d620: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
+0000d630: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000d640: 696e 7428 666c 6f61 7428 7629 295d 5b73  int(float(v))][s
+0000d650: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000d660: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d680: 2020 7365 6c66 2e67 7261 7068 5f74 7261    self.graph_tra
+0000d690: 636b 735b 6461 7567 6874 6572 5f74 7261  cks[daughter_tra
+0000d6a0: 636b 5f69 645d 203d 2070 6172 656e 745f  ck_id] = parent_
+0000d6b0: 7472 6163 6b5f 6964 0d0a 0d0a 2020 2020  track_id....    
+0000d6c0: 2020 2020 2020 2020 7072 696e 7428 2767          print('g
+0000d6d0: 6574 7469 6e67 2061 7474 7269 6275 7465  etting attribute
+0000d6e0: 7327 2920 2020 2020 2020 2020 2020 2020  s')             
+0000d6f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000d700: 2073 656c 662e 5f67 6574 5f61 7474 7269   self._get_attri
+0000d710: 6275 7465 7328 290d 0a20 2020 2020 2020  butes()..       
+0000d720: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d730: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
+0000d740: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000d750: 7220 7472 6163 6b5f 6964 2069 6e20 7365  r track_id in se
+0000d760: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
+0000d770: 6b5f 6964 733a 0d0a 2020 2020 2020 2020  k_ids:..        
+0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d790: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000d7a0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000d7b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000d7f0: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
+0000d800: 2022 4a75 7374 206f 6e65 206d 6f72 6520   "Just one more 
+0000d810: 7468 696e 6722 0d0a 2020 2020 2020 2020  thing"..        
+0000d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d840: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000d850: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
 0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d870: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
-0000d880: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
-0000d890: 6e73 6974 795f 6b65 792c 2073 7472 286e  nsity_key, str(n
-0000d8a0: 6577 5f74 6f74 616c 5f69 6e74 656e 7369  ew_total_intensi
-0000d8b0: 7479 2929 2020 2020 200d 0a20 2020 2020  ty))     ..     
-0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000d8e0: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
-0000d8f0: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-0000d900: 795f 6b65 792c 2073 7472 286e 6577 5f6d  y_key, str(new_m
-0000d910: 6561 6e5f 696e 7465 6e73 6974 7929 290d  ean_intensity)).
-0000d920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d940: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-0000d950: 7365 7428 7365 6c66 2e72 6164 6975 735f  set(self.radius_
-0000d960: 6b65 792c 2073 7472 286e 6577 5f72 6164  key, str(new_rad
-0000d970: 6975 7329 2920 2020 2020 0d0a 2020 2020  ius))     ..    
-0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 5370 6f74 6f62 6a65 6374 2e73 6574 2873  Spotobject.set(s
-0000d9b0: 656c 662e 7175 616c 6974 795f 6b65 792c  elf.quality_key,
-0000d9c0: 2073 7472 286e 6577 5f71 7561 6c69 7479   str(new_quality
-0000d9d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
-0000da00: 6374 2e73 6574 2873 656c 662e 6469 7374  ct.set(self.dist
-0000da10: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
-0000da20: 6579 2c20 7374 7228 6e65 775f 6469 7374  ey, str(new_dist
-0000da30: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-0000da40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da60: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
-0000da70: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000da80: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000da90: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-0000daa0: 295d 5b73 656c 662e 7472 6163 6b69 645f  )][self.trackid_
-0000dab0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
-0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dad0: 2020 2020 2020 2020 2020 6368 616e 6e65            channe
-0000dae0: 6c5f 6669 6c74 6572 6564 5f74 7261 636b  l_filtered_track
-0000daf0: 732e 6170 7065 6e64 2874 7261 636b 5f69  s.append(track_i
-0000db00: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000db30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000db40: 6c66 2e78 6d6c 5f74 7265 652e 7772 6974  lf.xml_tree.writ
-0000db50: 6528 6f73 2e70 6174 682e 6a6f 696e 2873  e(os.path.join(s
-0000db60: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000db70: 7061 7468 2c20 7365 6c66 2e63 6861 6e6e  path, self.chann
-0000db80: 656c 5f78 6d6c 5f6e 616d 6529 2920 0d0a  el_xml_name)) ..
-0000db90: 0d0a 2020 2020 6465 6620 5f67 6574 5f78  ..    def _get_x
-0000dba0: 6d6c 5f64 6174 6128 7365 6c66 293a 0d0a  ml_data(self):..
-0000dbb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dbc0: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-0000dbd0: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-0000dbe0: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
-0000dbf0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc10: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-0000dc20: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
-0000dc30: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
-0000dc40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc50: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
-0000dc60: 7472 6565 203d 2065 742e 7061 7273 6528  tree = et.parse(
-0000dc70: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2020 2020 7365 6c66 2e78 6d6c 5f72        self.xml_r
-0000dca0: 6f6f 7420 3d20 7365 6c66 2e78 6d6c 5f74  oot = self.xml_t
-0000dcb0: 7265 652e 6765 7472 6f6f 7428 290d 0a20  ree.getroot().. 
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-0000dce0: 6c5f 786d 6c5f 6e61 6d65 203d 2027 7365  l_xml_name = 'se
-0000dcf0: 636f 6e64 5f63 6861 6e6e 656c 5f27 202b  cond_channel_' +
-0000dd00: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-0000dd10: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
-0000dd20: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
-0000dd30: 2929 5b30 5d20 2b20 272e 786d 6c27 0d0a  ))[0] + '.xml'..
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd50: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
-0000dd60: 656c 5f78 6d6c 5f70 6174 6820 3d20 6f73  el_xml_path = os
-0000dd70: 2e70 6174 682e 6469 726e 616d 6528 7365  .path.dirname(se
-0000dd80: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
-0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dda0: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
-0000ddb0: 5f63 6861 6e6e 656c 5f74 7265 6528 290d  _channel_tree().
-0000ddc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ddd0: 2069 6620 7365 6c66 2e61 7574 6f65 6e63   if self.autoenc
-0000dde0: 6f64 6572 5f6d 6f64 656c 2069 7320 6e6f  oder_model is no
-0000ddf0: 7420 4e6f 6e65 2061 6e64 2073 656c 662e  t None and self.
-0000de00: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-0000de10: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000de20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000de30: 656c 662e 6d61 7374 6572 5f78 6d6c 5f63  elf.master_xml_c
-0000de40: 6f6e 7465 6e74 203d 2073 656c 662e 786d  ontent = self.xm
-0000de50: 6c5f 636f 6e74 656e 740d 0a20 2020 2020  l_content..     
-0000de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de70: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
-0000de80: 6c5f 7472 6565 203d 2065 742e 7061 7273  l_tree = et.pars
-0000de90: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
-0000dea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000deb0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000dec0: 7374 6572 5f78 6d6c 5f72 6f6f 7420 3d20  ster_xml_root = 
-0000ded0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-0000dee0: 7472 6565 2e67 6574 726f 6f74 2829 0d0a  tree.getroot()..
-0000def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df00: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
-0000df10: 6572 5f78 6d6c 5f6e 616d 6520 3d20 276d  er_xml_name = 'm
-0000df20: 6173 7465 725f 2720 2b20 7365 6c66 2e6d  aster_' + self.m
-0000df30: 6173 7465 725f 6578 7472 615f 6e61 6d65  aster_extra_name
-0000df40: 2020 2b20 6f73 2e70 6174 682e 7370 6c69    + os.path.spli
-0000df50: 7465 7874 286f 732e 7061 7468 2e62 6173  text(os.path.bas
-0000df60: 656e 616d 6528 7365 6c66 2e78 6d6c 5f70  ename(self.xml_p
-0000df70: 6174 6829 295b 305d 202b 2027 2e78 6d6c  ath))[0] + '.xml
-0000df80: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-0000df90: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000dfa0: 6173 7465 725f 786d 6c5f 7061 7468 203d  aster_xml_path =
-0000dfb0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-0000dfc0: 2873 656c 662e 786d 6c5f 7061 7468 2920  (self.xml_path) 
-0000dfd0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000dfe0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d880: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
+0000d890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8c0: 206c 656e 2873 656c 662e 6669 6c74 6572   len(self.filter
+0000d8d0: 6564 5f74 7261 636b 5f69 6473 292c 0d0a  ed_track_ids),..
+0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d900: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d930: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000d940: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
+0000d950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d970: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000d980: 756e 7420 3d20 7365 6c66 2e63 6f75 6e74  unt = self.count
+0000d990: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
+0000d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d9c0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000d9d0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f75  value = self.cou
+0000d9e0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da00: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
+0000da10: 6e61 6c5f 7472 6163 6b73 2874 7261 636b  nal_tracks(track
+0000da20: 5f69 6429 200d 0a0d 0a20 2020 2020 2020  _id) ....       
+0000da30: 2020 2020 2069 6620 7365 6c66 2e66 6f75       if self.fou
+0000da40: 7269 6572 3a0d 0a20 2020 2020 2020 2020  rier:..         
+0000da50: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000da60: 2763 6f6d 7075 7469 6e67 2046 6f75 7269  'computing Fouri
+0000da70: 6572 2729 0d0a 2020 2020 2020 2020 2020  er')..          
+0000da80: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+0000da90: 6f6d 7075 7465 5f70 6865 6e6f 7479 7065  ompute_phenotype
+0000daa0: 7328 2920 2020 2020 2020 2020 2020 2020  s()             
+0000dab0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000dac0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+0000dad0: 656d 706f 7261 6c5f 706c 6f74 735f 7472  emporal_plots_tr
+0000dae0: 6163 6b6d 6174 6528 2920 2020 2020 2020  ackmate()       
+0000daf0: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
+0000db00: 6372 6561 7465 5f73 6563 6f6e 645f 6368  create_second_ch
+0000db10: 616e 6e65 6c5f 786d 6c28 7365 6c66 293a  annel_xml(self):
+0000db20: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
+0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db40: 2020 2070 7269 6e74 2827 5472 616e 7366     print('Transf
+0000db50: 6572 7269 6e67 2058 4d4c 2729 2020 200d  erring XML')   .
+0000db60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000db70: 2020 2020 2063 6861 6e6e 656c 5f66 696c       channel_fil
+0000db80: 7465 7265 645f 7472 6163 6b73 203d 205b  tered_tracks = [
+0000db90: 5d20 2020 2020 2020 2020 2020 200d 0a20  ]            .. 
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbb0: 2020 2066 6f72 2053 706f 746f 626a 6563     for Spotobjec
+0000dbc0: 7420 696e 2073 656c 662e 786d 6c5f 726f  t in self.xml_ro
+0000dbd0: 6f74 2e69 7465 7228 2753 706f 7427 293a  ot.iter('Spot'):
+0000dbe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dbf0: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+0000dc00: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
+0000dc10: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000dc20: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
+0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc40: 2020 2020 2020 2020 2020 6966 2063 656c            if cel
+0000dc50: 6c5f 6964 2069 6e20 7365 6c66 2e63 6861  l_id in self.cha
+0000dc60: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000dc70: 5f70 726f 7065 7274 6965 732e 6b65 7973  _properties.keys
+0000dc80: 2829 3a20 2020 2020 2020 200d 0a20 2020  ():        ..   
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcc0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000dcd0: 6577 5f70 6f73 6974 696f 6e78 203d 2020  ew_positionx =  
+0000dce0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+0000dcf0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000dd00: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
+0000dd10: 662e 7870 6f73 6964 5f6b 6579 5d0d 0a20  f.xposid_key].. 
+0000dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd40: 2020 206e 6577 5f70 6f73 6974 696f 6e79     new_positiony
+0000dd50: 203d 2020 7365 6c66 2e63 6861 6e6e 656c   =  self.channel
+0000dd60: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000dd70: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000dd80: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+0000dd90: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddb0: 2020 2020 2020 206e 6577 5f70 6f73 6974         new_posit
+0000ddc0: 696f 6e7a 203d 2020 7365 6c66 2e63 6861  ionz =  self.cha
+0000ddd0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000dde0: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000ddf0: 5f69 645d 5b73 656c 662e 7a70 6f73 6964  _id][self.zposid
+0000de00: 5f6b 6579 5d0d 0a0d 0a20 2020 2020 2020  _key]....       
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000de30: 5f74 6f74 616c 5f69 6e74 656e 7369 7479  _total_intensity
+0000de40: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
+0000de50: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000de60: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000de70: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000de80: 7369 7479 5f6b 6579 5d0d 0a20 2020 2020  sity_key]..     
+0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dea0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000deb0: 6577 5f6d 6561 6e5f 696e 7465 6e73 6974  ew_mean_intensit
+0000dec0: 7920 3d20 7365 6c66 2e63 6861 6e6e 656c  y = self.channel
+0000ded0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000dee0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000def0: 5b73 656c 662e 6d65 616e 5f69 6e74 656e  [self.mean_inten
+0000df00: 7369 7479 5f6b 6579 5d0d 0a0d 0a20 2020  sity_key]....   
+0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df30: 206e 6577 5f72 6164 6975 7320 3d20 7365   new_radius = se
+0000df40: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000df50: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000df60: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000df70: 7261 6469 7573 5f6b 6579 5d0d 0a20 2020  radius_key]..   
+0000df80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfa0: 206e 6577 5f71 7561 6c69 7479 203d 2073   new_quality = s
+0000dfb0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+0000dfc0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000dfd0: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
+0000dfe0: 2e71 7561 6c69 7479 5f6b 6579 5d0d 0a20  .quality_key].. 
 0000dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e000: 7365 6c66 2e75 6e69 7175 655f 6f62 6a65  self.unique_obje
-0000e010: 6374 7320 3d20 7b7d 0d0a 2020 2020 2020  cts = {}..      
-0000e020: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000e030: 6e69 7175 655f 7072 6f70 6572 7469 6573  nique_properties
-0000e040: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-0000e050: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
-0000e060: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
-0000e070: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e080: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
-0000e090: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
-0000e0a0: 2020 2020 2020 2020 2020 7365 6c66 2e4e            self.N
-0000e0b0: 6f72 6d61 6c54 7261 636b 4964 7320 3d20  ormalTrackIds = 
-0000e0c0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000e0d0: 2020 2020 7365 6c66 2e61 6c6c 5f74 7261      self.all_tra
-0000e0e0: 636b 5f70 726f 7065 7274 6965 7320 3d20  ck_properties = 
-0000e0f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000e100: 2020 2020 7365 6c66 2e73 706c 6974 5f70      self.split_p
-0000e110: 6f69 6e74 735f 7469 6d65 7320 3d20 5b5d  oints_times = []
-0000e120: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000e130: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000e140: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000e150: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-0000e160: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000e170: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000e180: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
-0000e190: 6469 6e67 5472 6163 6b49 6473 2e61 7070  dingTrackIds.app
-0000e1a0: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
-0000e1b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e1c0: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
-0000e1d0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000e1e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e200: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-0000e210: 6170 7065 6e64 2873 656c 662e 5472 6163  append(self.Trac
-0000e220: 6b69 6442 6f78 290d 0a20 2020 2020 2020  kidBox)..       
-0000e230: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-0000e240: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
-0000e250: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
-0000e260: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
-0000e270: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
-0000e280: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
-0000e290: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
-0000e2a0: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
-0000e2b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000e2c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000e2d0: 2020 2020 2020 2020 2073 656c 662e 5370           self.Sp
-0000e2e0: 6f74 6f62 6a65 6374 7320 3d20 7365 6c66  otobjects = self
-0000e2f0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000e300: 6428 274d 6f64 656c 2729 2e66 696e 6428  d('Model').find(
-0000e310: 2741 6c6c 5370 6f74 7327 290d 0a20 2020  'AllSpots')..   
-0000e320: 2020 2020 2020 2020 2020 2020 2023 2045               # E
-0000e330: 7874 7261 6374 2074 6865 2074 7261 636b  xtract the track
-0000e340: 7320 6672 6f6d 2078 6d6c 0d0a 2020 2020  s from xml..    
-0000e350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e360: 2e74 7261 636b 7320 3d20 7365 6c66 2e78  .tracks = self.x
-0000e370: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
-0000e380: 224d 6f64 656c 2229 2e66 696e 6428 2241  "Model").find("A
-0000e390: 6c6c 5472 6163 6b73 2229 0d0a 2020 2020  llTracks")..    
-0000e3a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e3b0: 2e73 6574 7469 6e67 7320 3d20 7365 6c66  .settings = self
-0000e3c0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000e3d0: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
-0000e3e0: 6e64 2822 496d 6167 6544 6174 6122 290d  nd("ImageData").
-0000e3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e400: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-0000e410: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
-0000e420: 7365 7474 696e 6773 2e67 6574 2822 7069  settings.get("pi
-0000e430: 7865 6c77 6964 7468 2229 290d 0a20 2020  xelwidth"))..   
-0000e440: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e450: 662e 7963 616c 6962 7261 7469 6f6e 203d  f.ycalibration =
-0000e460: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
-0000e470: 696e 6773 2e67 6574 2822 7069 7865 6c68  ings.get("pixelh
-0000e480: 6569 6768 7422 2929 0d0a 2020 2020 2020  eight"))..      
-0000e490: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
-0000e4a0: 6361 6c69 6272 6174 696f 6e20 3d20 666c  calibration = fl
-0000e4b0: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
-0000e4c0: 732e 6765 7428 2276 6f78 656c 6465 7074  s.get("voxeldept
-0000e4d0: 6822 2929 0d0a 2020 2020 2020 2020 2020  h"))..          
-0000e4e0: 2020 2020 2020 7365 6c66 2e74 6361 6c69        self.tcali
-0000e4f0: 6272 6174 696f 6e20 3d20 696e 7428 666c  bration = int(fl
-0000e500: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
-0000e510: 732e 6765 7428 2274 696d 6569 6e74 6572  s.get("timeinter
-0000e520: 7661 6c22 2929 290d 0a20 2020 2020 2020  val")))..       
-0000e530: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-0000e540: 7465 6374 6f72 7365 7474 696e 6773 203d  tectorsettings =
-0000e550: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000e560: 742e 6669 6e64 2822 5365 7474 696e 6773  t.find("Settings
-0000e570: 2229 2e66 696e 6428 2244 6574 6563 746f  ").find("Detecto
-0000e580: 7253 6574 7469 6e67 7322 290d 0a20 2020  rSettings")..   
-0000e590: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e5a0: 662e 6261 7369 6373 6574 7469 6e67 7320  f.basicsettings 
-0000e5b0: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000e5c0: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
-0000e5d0: 7322 292e 6669 6e64 2822 4261 7369 6353  s").find("BasicS
-0000e5e0: 6574 7469 6e67 7322 290d 0a20 2020 2020  ettings")..     
-0000e5f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e600: 6465 7465 6374 6f72 6368 616e 6e65 6c20  detectorchannel 
-0000e610: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
-0000e620: 2e64 6574 6563 746f 7273 6574 7469 6e67  .detectorsetting
-0000e630: 732e 6765 7428 2254 4152 4745 545f 4348  s.get("TARGET_CH
-0000e640: 414e 4e45 4c22 2929 290d 0a20 2020 2020  ANNEL")))..     
-0000e650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e660: 7473 7461 7274 203d 2069 6e74 2866 6c6f  tstart = int(flo
-0000e670: 6174 2873 656c 662e 6261 7369 6373 6574  at(self.basicset
-0000e680: 7469 6e67 732e 6765 7428 2274 7374 6172  tings.get("tstar
-0000e690: 7422 2929 290d 0a20 2020 2020 2020 2020  t")))..         
-0000e6a0: 2020 2020 2020 2073 656c 662e 7465 6e64         self.tend
-0000e6b0: 203d 2069 6e74 2866 6c6f 6174 2873 656c   = int(float(sel
-0000e6c0: 662e 6261 7369 6373 6574 7469 6e67 732e  f.basicsettings.
-0000e6d0: 6765 7428 2274 656e 6422 2929 290d 0a20  get("tend"))).. 
-0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e6f0: 656c 662e 5f67 6574 5f62 6f75 6e64 6172  elf._get_boundar
-0000e700: 795f 706f 696e 7473 2829 0d0a 2020 2020  y_points()..    
-0000e710: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000e720: 7428 2749 7465 7261 7469 6e67 206f 7665  t('Iterating ove
-0000e730: 7220 7370 6f74 7320 696e 2066 7261 6d65  r spots in frame
-0000e740: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-0000e750: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-0000e760: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
-0000e770: 2020 2020 6675 7475 7265 7320 3d20 5b5d      futures = []
-0000e780: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000e790: 2020 2020 7769 7468 2063 6f6e 6375 7272      with concurr
-0000e7a0: 656e 742e 6675 7475 7265 732e 5468 7265  ent.futures.Thre
-0000e7b0: 6164 506f 6f6c 4578 6563 7574 6f72 286d  adPoolExecutor(m
-0000e7c0: 6178 5f77 6f72 6b65 7273 203d 206f 732e  ax_workers = os.
-0000e7d0: 6370 755f 636f 756e 7428 2929 2061 7320  cpu_count()) as 
-0000e7e0: 6578 6563 7574 6f72 3a0d 0a20 2020 2020  executor:..     
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000e800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e810: 2020 2020 2066 6f72 2066 7261 6d65 2069       for frame i
-0000e820: 6e20 7365 6c66 2e53 706f 746f 626a 6563  n self.Spotobjec
-0000e830: 7473 2e66 696e 6461 6c6c 2827 5370 6f74  ts.findall('Spot
-0000e840: 7349 6e46 7261 6d65 2729 3a0d 0a20 2020  sInFrame'):..   
-0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e860: 2020 2020 2020 2020 2020 6675 7475 7265            future
-0000e870: 732e 6170 7065 6e64 2865 7865 6375 746f  s.append(executo
-0000e880: 722e 7375 626d 6974 2873 656c 662e 5f73  r.submit(self._s
-0000e890: 706f 745f 636f 6d70 7574 6572 2c20 6672  pot_computer, fr
-0000e8a0: 616d 6529 290d 0a20 2020 2020 2020 2020  ame))..         
-0000e8b0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000e8c0: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000e8d0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000e900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e920: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000e930: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
-0000e940: 436f 6c6c 6563 7469 6e67 2053 706f 7473  Collecting Spots
-0000e950: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e970: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000e980: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
-0000e990: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
-0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9e0: 2020 2020 2020 2020 6c65 6e28 6675 7475          len(futu
-0000e9f0: 7265 7329 2c0d 0a20 2020 2020 2020 2020  res),..         
-0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea10: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea40: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000ea50: 6261 722e 7368 6f77 2829 0d0a 0d0a 2020  bar.show()....  
-0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea70: 2020 666f 7220 7220 696e 2063 6f6e 6375    for r in concu
-0000ea80: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
-0000ea90: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
-0000eaa0: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
-0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eac0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000ead0: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
-0000eae0: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
-0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb00: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000eb10: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000eb20: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb50: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000eb60: 735f 6261 722e 7661 6c75 6520 3d20 2073  s_bar.value =  s
-0000eb70: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
-0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000eba0: 2e72 6573 756c 7428 290d 0a0d 0a20 2020  .result()....   
-0000ebb0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000ebc0: 6e74 2866 2749 7465 7261 7469 6e67 206f  nt(f'Iterating o
-0000ebd0: 7665 7220 7472 6163 6b73 207b 6c65 6e28  ver tracks {len(
-0000ebe0: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-0000ebf0: 6163 6b5f 6964 7329 7d27 2920 200d 0a20  ack_ids)}')  .. 
-0000ec00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ec10: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ec30: 7574 7572 6573 203d 205b 5d0d 0a20 2020  utures = []..   
-0000ec40: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-0000ec50: 6820 636f 6e63 7572 7265 6e74 2e66 7574  h concurrent.fut
-0000ec60: 7572 6573 2e54 6872 6561 6450 6f6f 6c45  ures.ThreadPoolE
-0000ec70: 7865 6375 746f 7228 6d61 785f 776f 726b  xecutor(max_work
-0000ec80: 6572 7320 3d20 6f73 2e63 7075 5f63 6f75  ers = os.cpu_cou
-0000ec90: 6e74 2829 2920 6173 2065 7865 6375 746f  nt()) as executo
-0000eca0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-0000ecb0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000ecc0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000ecd0: 7220 7472 6163 6b20 696e 2073 656c 662e  r track in self.
-0000ece0: 7472 6163 6b73 2e66 696e 6461 6c6c 2827  tracks.findall('
-0000ecf0: 5472 6163 6b27 293a 0d0a 2020 2020 2020  Track'):..      
-0000ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed30: 2020 2020 7472 6163 6b5f 6964 203d 2069      track_id = i
-0000ed40: 6e74 2874 7261 636b 2e67 6574 2873 656c  nt(track.get(sel
-0000ed50: 662e 7472 6163 6b69 645f 6b65 7929 290d  f.trackid_key)).
-0000ed60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ed70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000ed80: 7472 6163 6b5f 6964 2069 6e20 7365 6c66  track_id in self
-0000ed90: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
-0000eda0: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
-0000edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edc0: 2020 2020 2020 2020 6675 7475 7265 732e          futures.
-0000edd0: 6170 7065 6e64 2865 7865 6375 746f 722e  append(executor.
-0000ede0: 7375 626d 6974 2873 656c 662e 5f74 7261  submit(self._tra
-0000edf0: 636b 5f63 6f6d 7075 7465 722c 2074 7261  ck_computer, tra
-0000ee00: 636b 2c20 7472 6163 6b5f 6964 2929 0d0a  ck, track_id))..
-0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee20: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-0000ee30: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-0000ee40: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee60: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ee90: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000eea0: 6c61 6265 6c20 3d20 2243 6f6c 6c65 6374  label = "Collect
-0000eeb0: 696e 6720 5472 6163 6b73 220d 0a20 2020  ing Tracks"..   
-0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eee0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000eef0: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
-0000ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef20: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
-0000ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef50: 2020 6c65 6e28 7365 6c66 2e66 696c 7465    len(self.filte
-0000ef60: 7265 645f 7472 6163 6b5f 6964 7329 2c0d  red_track_ids),.
-0000ef70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef90: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000efc0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000efd0: 6f77 2829 0d0a 0d0a 0d0a 2020 2020 2020  ow()......      
-0000efe0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000eff0: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
-0000f000: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
-0000f010: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
-0000f020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f040: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000f050: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
-0000f060: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f080: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000f090: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000f0a0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0d0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000f0e0: 6172 2e76 616c 7565 203d 2073 656c 662e  ar.value = self.
-0000f0f0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f110: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
-0000f120: 756c 7428 290d 0a20 2020 2020 2020 2020  ult()..         
-0000f130: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000f140: 6861 6e6e 656c 5f73 6567 5f69 6d61 6765  hannel_seg_image
-0000f150: 2069 7320 6e6f 7420 4e6f 6e65 3a20 200d   is not None:  .
-0000f160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f170: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
-0000f180: 6561 7465 5f73 6563 6f6e 645f 6368 616e  eate_second_chan
-0000f190: 6e65 6c5f 786d 6c28 290d 0a20 2020 2020  nel_xml()..     
-0000f1a0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-0000f1b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f1c0: 6f72 2028 6b2c 7629 2069 6e20 7365 6c66  or (k,v) in self
-0000f1d0: 2e67 7261 7068 5f73 706c 6974 2e69 7465  .graph_split.ite
-0000f1e0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f200: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 6461 7567 6874 6572 5f74 7261 636b 5f69  daughter_track_i
-0000f230: 6420 3d20 2069 6e74 2866 6c6f 6174 2873  d =  int(float(s
-0000f240: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
-0000f250: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-0000f260: 6e74 2866 6c6f 6174 286b 2929 5d5b 7365  nt(float(k))][se
-0000f270: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
-0000f280: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e010: 2020 206e 6577 5f64 6973 7461 6e63 655f     new_distance_
+0000e020: 6365 6c6c 5f6d 6173 6b20 3d20 7365 6c66  cell_mask = self
+0000e030: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000e040: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000e050: 6365 6c6c 5f69 645d 5b73 656c 662e 6469  cell_id][self.di
+0000e060: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000e070: 5f6b 6579 5d0d 0a0d 0a20 2020 2020 2020  _key]....       
+0000e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e090: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000e0a0: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000e0b0: 2e78 706f 7369 645f 6b65 792c 2073 7472  .xposid_key, str
+0000e0c0: 286e 6577 5f70 6f73 6974 696f 6e78 2929  (new_positionx))
+0000e0d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0f0: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000e100: 626a 6563 742e 7365 7428 7365 6c66 2e79  bject.set(self.y
+0000e110: 706f 7369 645f 6b65 792c 2073 7472 286e  posid_key, str(n
+0000e120: 6577 5f70 6f73 6974 696f 6e79 2929 0d0a  ew_positiony))..
+0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e150: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000e160: 6574 2873 656c 662e 7a70 6f73 6964 5f6b  et(self.zposid_k
+0000e170: 6579 2c20 7374 7228 6e65 775f 706f 7369  ey, str(new_posi
+0000e180: 7469 6f6e 7a29 290d 0a0d 0a20 2020 2020  tionz))....     
+0000e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000e1b0: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
+0000e1c0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000e1d0: 7479 5f6b 6579 2c20 7374 7228 6e65 775f  ty_key, str(new_
+0000e1e0: 746f 7461 6c5f 696e 7465 6e73 6974 7929  total_intensity)
+0000e1f0: 2920 2020 2020 0d0a 2020 2020 2020 2020  )     ..        
+0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e210: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+0000e220: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+0000e230: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
+0000e240: 6579 2c20 7374 7228 6e65 775f 6d65 616e  ey, str(new_mean
+0000e250: 5f69 6e74 656e 7369 7479 2929 0d0a 2020  _intensity))..  
+0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e280: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+0000e290: 2873 656c 662e 7261 6469 7573 5f6b 6579  (self.radius_key
+0000e2a0: 2c20 7374 7228 6e65 775f 7261 6469 7573  , str(new_radius
+0000e2b0: 2929 2020 2020 200d 0a20 2020 2020 2020  ))     ..       
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2d0: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000e2e0: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000e2f0: 2e71 7561 6c69 7479 5f6b 6579 2c20 7374  .quality_key, st
+0000e300: 7228 6e65 775f 7175 616c 6974 7929 290d  r(new_quality)).
+0000e310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e330: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
+0000e340: 7365 7428 7365 6c66 2e64 6973 7461 6e63  set(self.distanc
+0000e350: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 792c  e_cell_mask_key,
+0000e360: 2073 7472 286e 6577 5f64 6973 7461 6e63   str(new_distanc
+0000e370: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
+0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3a0: 2020 2074 7261 636b 5f69 6420 3d20 7365     track_id = se
+0000e3b0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000e3c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000e3d0: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+0000e3e0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+0000e3f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e410: 2020 2020 2020 2063 6861 6e6e 656c 5f66         channel_f
+0000e420: 696c 7465 7265 645f 7472 6163 6b73 2e61  iltered_tracks.a
+0000e430: 7070 656e 6428 7472 6163 6b5f 6964 290d  ppend(track_id).
+0000e440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e460: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e480: 786d 6c5f 7472 6565 2e77 7269 7465 286f  xml_tree.write(o
+0000e490: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
+0000e4a0: 2e63 6861 6e6e 656c 5f78 6d6c 5f70 6174  .channel_xml_pat
+0000e4b0: 682c 2073 656c 662e 6368 616e 6e65 6c5f  h, self.channel_
+0000e4c0: 786d 6c5f 6e61 6d65 2929 200d 0a0d 0a20  xml_name)) .... 
+0000e4d0: 2020 2064 6566 205f 6765 745f 786d 6c5f     def _get_xml_
+0000e4e0: 6461 7461 2873 656c 6629 3a0d 0a0d 0a20  data(self):.... 
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000e500: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000e510: 2020 2069 6620 7365 6c66 2e63 6861 6e6e     if self.chann
+0000e520: 656c 5f73 6567 5f69 6d61 6765 2069 7320  el_seg_image is 
+0000e530: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e550: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+0000e560: 6c5f 636f 6e74 656e 7420 3d20 7365 6c66  l_content = self
+0000e570: 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a 2020  .xml_content..  
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2020 7365 6c66 2e78 6d6c 5f74 7265      self.xml_tre
+0000e5a0: 6520 3d20 6574 2e70 6172 7365 2873 656c  e = et.parse(sel
+0000e5b0: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 2020 2073 656c 662e 786d 6c5f 726f 6f74     self.xml_root
+0000e5e0: 203d 2073 656c 662e 786d 6c5f 7472 6565   = self.xml_tree
+0000e5f0: 2e67 6574 726f 6f74 2829 0d0a 2020 2020  .getroot()..    
+0000e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e610: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
+0000e620: 6d6c 5f6e 616d 6520 3d20 2773 6563 6f6e  ml_name = 'secon
+0000e630: 645f 6368 616e 6e65 6c5f 2720 2b20 6f73  d_channel_' + os
+0000e640: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
+0000e650: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+0000e660: 7365 6c66 2e78 6d6c 5f70 6174 6829 295b  self.xml_path))[
+0000e670: 305d 202b 2027 2e78 6d6c 270d 0a20 2020  0] + '.xml'..   
+0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e690: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+0000e6a0: 786d 6c5f 7061 7468 203d 206f 732e 7061  xml_path = os.pa
+0000e6b0: 7468 2e64 6972 6e61 6d65 2873 656c 662e  th.dirname(self.
+0000e6c0: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6e0: 2073 656c 662e 5f63 7265 6174 655f 6368   self._create_ch
+0000e6f0: 616e 6e65 6c5f 7472 6565 2829 0d0a 2020  annel_tree()..  
+0000e700: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000e710: 2073 656c 662e 6175 746f 656e 636f 6465   self.autoencode
+0000e720: 725f 6d6f 6465 6c20 6973 206e 6f74 204e  r_model is not N
+0000e730: 6f6e 6520 616e 6420 7365 6c66 2e73 6567  one and self.seg
+0000e740: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+0000e750: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000e760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e770: 2e6d 6173 7465 725f 786d 6c5f 636f 6e74  .master_xml_cont
+0000e780: 656e 7420 3d20 7365 6c66 2e78 6d6c 5f63  ent = self.xml_c
+0000e790: 6f6e 7465 6e74 0d0a 2020 2020 2020 2020  ontent..        
+0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e7b0: 656c 662e 6d61 7374 6572 5f78 6d6c 5f74  elf.master_xml_t
+0000e7c0: 7265 6520 3d20 6574 2e70 6172 7365 2873  ree = et.parse(s
+0000e7d0: 656c 662e 786d 6c5f 7061 7468 290d 0a20  elf.xml_path).. 
+0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7f0: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
+0000e800: 725f 786d 6c5f 726f 6f74 203d 2073 656c  r_xml_root = sel
+0000e810: 662e 6d61 7374 6572 5f78 6d6c 5f74 7265  f.master_xml_tre
+0000e820: 652e 6765 7472 6f6f 7428 290d 0a20 2020  e.getroot()..   
+0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e840: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
+0000e850: 786d 6c5f 6e61 6d65 203d 2027 6d61 7374  xml_name = 'mast
+0000e860: 6572 5f27 202b 2073 656c 662e 6d61 7374  er_' + self.mast
+0000e870: 6572 5f65 7874 7261 5f6e 616d 6520 202b  er_extra_name  +
+0000e880: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+0000e890: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
+0000e8a0: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
+0000e8b0: 2929 5b30 5d20 2b20 272e 786d 6c27 0d0a  ))[0] + '.xml'..
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8d0: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
+0000e8e0: 6572 5f78 6d6c 5f70 6174 6820 3d20 6f73  er_xml_path = os
+0000e8f0: 2e70 6174 682e 6469 726e 616d 6528 7365  .path.dirname(se
+0000e900: 6c66 2e78 6d6c 5f70 6174 6829 2020 2020  lf.xml_path)    
+0000e910: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000e920: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000e930: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e940: 662e 756e 6971 7565 5f6f 626a 6563 7473  f.unique_objects
+0000e950: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+0000e960: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000e970: 7565 5f70 726f 7065 7274 6965 7320 3d20  ue_properties = 
+0000e980: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+0000e990: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+0000e9a0: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
+0000e9b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e9c0: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+0000e9d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000e9e0: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
+0000e9f0: 616c 5472 6163 6b49 6473 203d 205b 5d0d  alTrackIds = [].
+0000ea00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea10: 2073 656c 662e 616c 6c5f 7472 6163 6b5f   self.all_track_
+0000ea20: 7072 6f70 6572 7469 6573 203d 205b 5d0d  properties = [].
+0000ea30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea40: 2073 656c 662e 7370 6c69 745f 706f 696e   self.split_poin
+0000ea50: 7473 5f74 696d 6573 203d 205b 5d0d 0a0d  ts_times = []...
+0000ea60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000ea80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ea90: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+0000eaa0: 636b 4964 732e 6170 7065 6e64 284e 6f6e  ckIds.append(Non
+0000eab0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+0000eac0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000ead0: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
+0000eae0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000eaf0: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
+0000eb00: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
+0000eb10: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000eb20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000eb30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000eb40: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
+0000eb50: 656e 6428 7365 6c66 2e54 7261 636b 6964  end(self.Trackid
+0000eb60: 426f 7829 0d0a 2020 2020 2020 2020 2020  Box)..          
+0000eb70: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+0000eb80: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+0000eb90: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
+0000eba0: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
+0000ebb0: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
+0000ebc0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+0000ebd0: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
+0000ebe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ebf0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ec00: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000ec10: 2020 2020 2020 7365 6c66 2e53 706f 746f        self.Spoto
+0000ec20: 626a 6563 7473 203d 2073 656c 662e 786d  bjects = self.xm
+0000ec30: 6c5f 636f 6e74 656e 742e 6669 6e64 2827  l_content.find('
+0000ec40: 4d6f 6465 6c27 292e 6669 6e64 2827 416c  Model').find('Al
+0000ec50: 6c53 706f 7473 2729 0d0a 2020 2020 2020  lSpots')..      
+0000ec60: 2020 2020 2020 2020 2020 2320 4578 7472            # Extr
+0000ec70: 6163 7420 7468 6520 7472 6163 6b73 2066  act the tracks f
+0000ec80: 726f 6d20 786d 6c0d 0a20 2020 2020 2020  rom xml..       
+0000ec90: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000eca0: 6163 6b73 203d 2073 656c 662e 786d 6c5f  acks = self.xml_
+0000ecb0: 636f 6e74 656e 742e 6669 6e64 2822 4d6f  content.find("Mo
+0000ecc0: 6465 6c22 292e 6669 6e64 2822 416c 6c54  del").find("AllT
+0000ecd0: 7261 636b 7322 290d 0a20 2020 2020 2020  racks")..       
+0000ece0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000ecf0: 7474 696e 6773 203d 2073 656c 662e 786d  ttings = self.xm
+0000ed00: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
+0000ed10: 5365 7474 696e 6773 2229 2e66 696e 6428  Settings").find(
+0000ed20: 2249 6d61 6765 4461 7461 2229 0d0a 2020  "ImageData")..  
+0000ed30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ed40: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
+0000ed50: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
+0000ed60: 7469 6e67 732e 6765 7428 2270 6978 656c  tings.get("pixel
+0000ed70: 7769 6474 6822 2929 0d0a 2020 2020 2020  width"))..      
+0000ed80: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
+0000ed90: 6361 6c69 6272 6174 696f 6e20 3d20 666c  calibration = fl
+0000eda0: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
+0000edb0: 732e 6765 7428 2270 6978 656c 6865 6967  s.get("pixelheig
+0000edc0: 6874 2229 290d 0a20 2020 2020 2020 2020  ht"))..         
+0000edd0: 2020 2020 2020 2073 656c 662e 7a63 616c         self.zcal
+0000ede0: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
+0000edf0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000ee00: 6574 2822 766f 7865 6c64 6570 7468 2229  et("voxeldepth")
+0000ee10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ee20: 2020 2073 656c 662e 7463 616c 6962 7261     self.tcalibra
+0000ee30: 7469 6f6e 203d 2069 6e74 2866 6c6f 6174  tion = int(float
+0000ee40: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000ee50: 6574 2822 7469 6d65 696e 7465 7276 616c  et("timeinterval
+0000ee60: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
+0000ee70: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
+0000ee80: 746f 7273 6574 7469 6e67 7320 3d20 7365  torsettings = se
+0000ee90: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000eea0: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
+0000eeb0: 6669 6e64 2822 4465 7465 6374 6f72 5365  find("DetectorSe
+0000eec0: 7474 696e 6773 2229 0d0a 2020 2020 2020  ttings")..      
+0000eed0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+0000eee0: 6173 6963 7365 7474 696e 6773 203d 2073  asicsettings = s
+0000eef0: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000ef00: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
+0000ef10: 2e66 696e 6428 2242 6173 6963 5365 7474  .find("BasicSett
+0000ef20: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
+0000ef30: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+0000ef40: 6563 746f 7263 6861 6e6e 656c 203d 2069  ectorchannel = i
+0000ef50: 6e74 2866 6c6f 6174 2873 656c 662e 6465  nt(float(self.de
+0000ef60: 7465 6374 6f72 7365 7474 696e 6773 2e67  tectorsettings.g
+0000ef70: 6574 2822 5441 5247 4554 5f43 4841 4e4e  et("TARGET_CHANN
+0000ef80: 454c 2229 2929 0d0a 2020 2020 2020 2020  EL")))..        
+0000ef90: 2020 2020 2020 2020 7365 6c66 2e74 7374          self.tst
+0000efa0: 6172 7420 3d20 696e 7428 666c 6f61 7428  art = int(float(
+0000efb0: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
+0000efc0: 6773 2e67 6574 2822 7473 7461 7274 2229  gs.get("tstart")
+0000efd0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000efe0: 2020 2020 7365 6c66 2e74 656e 6420 3d20      self.tend = 
+0000eff0: 696e 7428 666c 6f61 7428 7365 6c66 2e62  int(float(self.b
+0000f000: 6173 6963 7365 7474 696e 6773 2e67 6574  asicsettings.get
+0000f010: 2822 7465 6e64 2229 2929 0d0a 2020 2020  ("tend")))..    
+0000f020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f030: 2e5f 6765 745f 626f 756e 6461 7279 5f70  ._get_boundary_p
+0000f040: 6f69 6e74 7328 290d 0a20 2020 2020 2020  oints()..       
+0000f050: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+0000f060: 4974 6572 6174 696e 6720 6f76 6572 2073  Iterating over s
+0000f070: 706f 7473 2069 6e20 6672 616d 6527 290d  pots in frame').
+0000f080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f090: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
+0000f0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f0b0: 2066 7574 7572 6573 203d 205b 5d0d 0a0d   futures = []...
+0000f0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f0d0: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
+0000f0e0: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
+0000f0f0: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
+0000f100: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
+0000f110: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
+0000f120: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
+0000f130: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f150: 2020 666f 7220 6672 616d 6520 696e 2073    for frame in s
+0000f160: 656c 662e 5370 6f74 6f62 6a65 6374 732e  elf.Spotobjects.
+0000f170: 6669 6e64 616c 6c28 2753 706f 7473 496e  findall('SpotsIn
+0000f180: 4672 616d 6527 293a 0d0a 2020 2020 2020  Frame'):..      
+0000f190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1a0: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
+0000f1b0: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
+0000f1c0: 7562 6d69 7428 7365 6c66 2e5f 7370 6f74  ubmit(self._spot
+0000f1d0: 5f63 6f6d 7075 7465 722c 2066 7261 6d65  _computer, frame
+0000f1e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000f1f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f200: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000f210: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f230: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f260: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000f270: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
+0000f280: 6c65 6374 696e 6720 5370 6f74 7322 0d0a  lecting Spots"..
 0000f290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2a0: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
-0000f2b0: 203d 2069 6e74 2866 6c6f 6174 2873 7472   = int(float(str
-0000f2c0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-0000f2d0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-0000f2e0: 2866 6c6f 6174 2876 2929 5d5b 7365 6c66  (float(v))][self
-0000f2f0: 2e75 6e69 7175 6569 645f 6b65 795d 2929  .uniqueid_key]))
-0000f300: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f310: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f320: 656c 662e 6772 6170 685f 7472 6163 6b73  elf.graph_tracks
-0000f330: 5b64 6175 6768 7465 725f 7472 6163 6b5f  [daughter_track_
-0000f340: 6964 5d20 3d20 7061 7265 6e74 5f74 7261  id] = parent_tra
-0000f350: 636b 5f69 640d 0a20 2020 2020 2020 2020  ck_id..         
-0000f360: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
-0000f370: 5f61 7474 7269 6275 7465 7328 290d 0a20  _attributes().. 
-0000f380: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f390: 6620 7365 6c66 2e61 7574 6f65 6e63 6f64  f self.autoencod
-0000f3a0: 6572 5f6d 6f64 656c 2061 6e64 2073 656c  er_model and sel
-0000f3b0: 662e 7365 675f 696d 6167 6520 6973 206e  f.seg_image is n
-0000f3c0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3e0: 2070 7269 6e74 2827 4765 7474 696e 6720   print('Getting 
-0000f3f0: 6175 746f 656e 636f 6465 7220 636c 6f75  autoencoder clou
-0000f400: 6473 2729 0d0a 2020 2020 2020 2020 2020  ds')..          
-0000f410: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f420: 662e 5f61 7373 6967 6e5f 636c 7573 7465  f._assign_cluste
-0000f430: 725f 636c 6173 7328 290d 0a20 2020 2020  r_class()..     
-0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f450: 2020 7072 696e 7428 2743 7265 6174 696e    print('Creatin
-0000f460: 6720 6d61 7374 6572 2078 6d6c 2729 0d0a  g master xml')..
+0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2b0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000f2c0: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
+0000f2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2f0: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
+0000f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f320: 2020 2020 206c 656e 2866 7574 7572 6573       len(futures
+0000f330: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f350: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f380: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000f390: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f3b0: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
+0000f3c0: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
+0000f3d0: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
+0000f3e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f400: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+0000f410: 7420 3d20 7365 6c66 2e63 6f75 6e74 202b  t = self.count +
+0000f420: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f440: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f450: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000f460: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
 0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f480: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
-0000f490: 6174 655f 6d61 7374 6572 5f78 6d6c 2829  ate_master_xml()
-0000f4a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f4b0: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
-0000f4c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000f4d0: 2020 2066 6f72 2074 7261 636b 5f69 6420     for track_id 
-0000f4e0: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
-0000f4f0: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
-0000f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f520: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-0000f530: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-0000f540: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f570: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-0000f580: 6265 6c20 3d20 224a 7573 7420 6f6e 6520  bel = "Just one 
-0000f590: 6d6f 7265 2074 6869 6e67 220d 0a20 2020  more thing"..   
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5c0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000f5d0: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-0000f5e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f610: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f640: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
-0000f650: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-0000f660: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f690: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f490: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000f4a0: 6172 2e76 616c 7565 203d 2020 7365 6c66  ar.value =  self
+0000f4b0: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
+0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4d0: 2020 2020 2020 2020 2020 2020 722e 7265              r.re
+0000f4e0: 7375 6c74 2829 0d0a 0d0a 2020 2020 2020  sult()....      
+0000f4f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000f500: 6627 4974 6572 6174 696e 6720 6f76 6572  f'Iterating over
+0000f510: 2074 7261 636b 7320 7b6c 656e 2873 656c   tracks {len(sel
+0000f520: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+0000f530: 5f69 6473 297d 2729 2020 0d0a 2020 2020  _ids)}')  ..    
+0000f540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f550: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
+0000f560: 2020 2020 2020 2020 2020 2020 6675 7475              futu
+0000f570: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
+0000f580: 2020 2020 2020 2020 2020 7769 7468 2063            with c
+0000f590: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+0000f5a0: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
+0000f5b0: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
+0000f5c0: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
+0000f5d0: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
+0000f5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f5f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f600: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+0000f610: 7261 636b 2069 6e20 7365 6c66 2e74 7261  rack in self.tra
+0000f620: 636b 732e 6669 6e64 616c 6c28 2754 7261  cks.findall('Tra
+0000f630: 636b 2729 3a0d 0a20 2020 2020 2020 2020  ck'):..         
+0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f650: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f670: 2074 7261 636b 5f69 6420 3d20 696e 7428   track_id = int(
+0000f680: 7472 6163 6b2e 6765 7428 7365 6c66 2e74  track.get(self.t
+0000f690: 7261 636b 6964 5f6b 6579 2929 0d0a 2020  rackid_key))..  
 0000f6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f6c0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000f6d0: 6f77 2829 0d0a 2020 2020 2020 2020 2020  ow()..          
-0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f700: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000f710: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f740: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000f750: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
-0000f760: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
-0000f770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f780: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f790: 662e 5f66 696e 616c 5f74 7261 636b 7328  f._final_tracks(
-0000f7a0: 7472 6163 6b5f 6964 2920 0d0a 0d0a 2020  track_id) ....  
-0000f7b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000f7c0: 2073 656c 662e 666f 7572 6965 723a 0d0a   self.fourier:..
-0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7e0: 2020 2070 7269 6e74 2827 636f 6d70 7574     print('comput
-0000f7f0: 696e 6720 466f 7572 6965 7227 290d 0a20  ing Fourier').. 
+0000f6b0: 2020 2020 2020 2020 2020 6966 2074 7261            if tra
+0000f6c0: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
+0000f6d0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+0000f6e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f700: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
+0000f710: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
+0000f720: 6d69 7428 7365 6c66 2e5f 7472 6163 6b5f  mit(self._track_
+0000f730: 636f 6d70 7574 6572 2c20 7472 6163 6b2c  computer, track,
+0000f740: 2074 7261 636b 5f69 6429 290d 0a20 2020   track_id))..   
+0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f760: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+0000f770: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+0000f780: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f7d0: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
+0000f7e0: 656c 203d 2022 436f 6c6c 6563 7469 6e67  el = "Collecting
+0000f7f0: 2054 7261 636b 7322 0d0a 2020 2020 2020   Tracks"..      
 0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f810: 2020 7365 6c66 2e5f 636f 6d70 7574 655f    self._compute_
-0000f820: 7068 656e 6f74 7970 6573 2829 2020 2020  phenotypes()    
-0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f840: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000f850: 2020 2020 2020 7365 6c66 2e5f 7465 6d70        self._temp
-0000f860: 6f72 616c 5f70 6c6f 7473 5f74 7261 636b  oral_plots_track
-0000f870: 6d61 7465 2829 0d0a 2020 2020 2020 2020  mate()..        
-0000f880: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-0000f890: 6465 6620 5f63 7265 6174 655f 6d61 7374  def _create_mast
-0000f8a0: 6572 5f78 6d6c 2873 656c 6629 3a0d 0a20  er_xml(self):.. 
-0000f8b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000f8c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000f8d0: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
-0000f8e0: 696e 2073 656c 662e 6d61 7374 6572 5f78  in self.master_x
-0000f8f0: 6d6c 5f72 6f6f 742e 6974 6572 2827 5370  ml_root.iter('Sp
-0000f900: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
-0000f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f920: 2020 2020 2020 2063 656c 6c5f 6964 203d         cell_id =
-0000f930: 2069 6e74 2853 706f 746f 626a 6563 742e   int(Spotobject.
-0000f940: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
-0000f950: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000f810: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f820: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000f830: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
+0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f860: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f880: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000f890: 656e 2873 656c 662e 6669 6c74 6572 6564  en(self.filtered
+0000f8a0: 5f74 7261 636b 5f69 6473 292c 0d0a 2020  _track_ids),..  
+0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8d0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8f0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000f900: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+0000f910: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+0000f920: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
+0000f930: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+0000f940: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
+0000f950: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
 0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f970: 2020 2020 2020 2069 6620 6365 6c6c 5f69         if cell_i
-0000f980: 6420 696e 2073 656c 662e 756e 6971 7565  d in self.unique
-0000f990: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000f9a0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f980: 656c 662e 636f 756e 7420 3d20 7365 6c66  elf.count = self
+0000f990: 2e63 6f75 6e74 202b 2031 0d0a 2020 2020  .count + 1..    
+0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000f9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9f0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-0000fa00: 696e 2073 656c 662e 756e 6971 7565 5f73  in self.unique_s
-0000fa10: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000fa20: 656c 6c5f 6964 5d2e 6b65 7973 2829 3a0d  ell_id].keys():.
-0000fa30: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000f9c0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
+0000f9d0: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
+0000f9e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa00: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000fa10: 726f 6772 6573 735f 6261 722e 7661 6c75  rogress_bar.valu
+0000fa20: 6520 3d20 7365 6c66 2e63 6f75 6e74 0d0a  e = self.count..
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa50: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-0000fa60: 6f74 6f62 6a65 6374 2e73 6574 286b 2c20  otobject.set(k, 
-0000fa70: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
-0000fa80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000fa90: 6365 6c6c 5f69 645d 5b6b 5d29 2920 2020  cell_id][k]))   
-0000faa0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000fab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fac0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-0000fad0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000fae0: 7374 6572 5f78 6d6c 5f74 7265 652e 7772  ster_xml_tree.wr
-0000faf0: 6974 6528 6f73 2e70 6174 682e 6a6f 696e  ite(os.path.join
-0000fb00: 2873 656c 662e 6d61 7374 6572 5f78 6d6c  (self.master_xml
-0000fb10: 5f70 6174 682c 2073 656c 662e 6d61 7374  _path, self.mast
-0000fb20: 6572 5f78 6d6c 5f6e 616d 6529 290d 0a20  er_xml_name)).. 
-0000fb30: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000fa50: 2020 2020 722e 7265 7375 6c74 2829 0d0a      r.result()..
+0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa70: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
+0000fa80: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
+0000fa90: 204e 6f6e 653a 2020 0d0a 2020 2020 2020   None:  ..      
+0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fab0: 2073 656c 662e 5f63 7265 6174 655f 7365   self._create_se
+0000fac0: 636f 6e64 5f63 6861 6e6e 656c 5f78 6d6c  cond_channel_xml
+0000fad0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000fae0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0000faf0: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+0000fb00: 2920 696e 2073 656c 662e 6772 6170 685f  ) in self.graph_
+0000fb10: 7370 6c69 742e 6974 656d 7328 293a 0d0a  split.items():..
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 0000fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb80: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-0000fb90: 2020 2020 6465 6620 5f61 7373 6967 6e5f      def _assign_
-0000fba0: 636c 7573 7465 725f 636c 6173 7328 7365  cluster_class(se
-0000fbb0: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
-0000fbc0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000fbd0: 2020 2020 2020 2073 656c 662e 6178 6573         self.axes
-0000fbe0: 203d 2073 656c 662e 6178 6573 2e72 6570   = self.axes.rep
-0000fbf0: 6c61 6365 2822 5422 2c20 2222 290d 0a20  lace("T", "").. 
-0000fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000fc20: 2020 2020 2020 2020 2066 6f72 2063 6f75           for cou
-0000fc30: 6e74 2c20 7469 6d65 5f6b 6579 2069 6e20  nt, time_key in 
-0000fc40: 656e 756d 6572 6174 6528 7365 6c66 2e5f  enumerate(self._
-0000fc50: 7469 6d65 645f 6365 6e74 726f 6964 2e6b  timed_centroid.k
-0000fc60: 6579 7328 2929 3a0d 0a20 2020 2020 2020  eys()):..       
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000fb50: 2020 2020 2020 2020 2064 6175 6768 7465           daughte
+0000fb60: 725f 7472 6163 6b5f 6964 203d 2020 696e  r_track_id =  in
+0000fb70: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
+0000fb80: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+0000fb90: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
+0000fba0: 7428 6b29 295d 5b73 656c 662e 756e 6971  t(k))][self.uniq
+0000fbb0: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
+0000fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbd0: 2020 2020 2020 2020 2020 7061 7265 6e74            parent
+0000fbe0: 5f74 7261 636b 5f69 6420 3d20 696e 7428  _track_id = int(
+0000fbf0: 666c 6f61 7428 7374 7228 7365 6c66 2e75  float(str(self.u
+0000fc00: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000fc10: 7274 6965 735b 696e 7428 666c 6f61 7428  rties[int(float(
+0000fc20: 7629 295d 5b73 656c 662e 756e 6971 7565  v))][self.unique
+0000fc30: 6964 5f6b 6579 5d29 2929 0d0a 2020 2020  id_key])))..    
+0000fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc50: 2020 2020 2020 2020 7365 6c66 2e67 7261          self.gra
+0000fc60: 7068 5f74 7261 636b 735b 6461 7567 6874  ph_tracks[daught
+0000fc70: 6572 5f74 7261 636b 5f69 645d 203d 2070  er_track_id] = p
+0000fc80: 6172 656e 745f 7472 6163 6b5f 6964 0d0a  arent_track_id..
 0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fca0: 2074 7265 652c 2073 706f 745f 6365 6e74   tree, spot_cent
-0000fcb0: 726f 6964 7320 3d20 7365 6c66 2e5f 7469  roids = self._ti
-0000fcc0: 6d65 645f 6365 6e74 726f 6964 5b74 696d  med_centroid[tim
-0000fcd0: 655f 6b65 795d 0d0a 2020 2020 2020 2020  e_key]..        
-0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcf0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-0000fd00: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-0000fd10: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd30: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000fd40: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
-0000fd50: 2241 7574 6f65 6e63 6f64 6572 2066 6f72  "Autoencoder for
-0000fd60: 2072 6566 696e 696e 6720 706f 696e 7420   refining point 
-0000fd70: 636c 6f75 6473 220d 0a20 2020 2020 2020  clouds"..       
-0000fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd90: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000fda0: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
-0000fdb0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdf0: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
-0000fe00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe30: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
-0000fe40: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
-0000fe50: 6964 2e6b 6579 7328 2929 202b 2031 2c0d  id.keys()) + 1,.
-0000fe60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fe70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fca0: 7365 6c66 2e5f 6765 745f 6174 7472 6962  self._get_attrib
+0000fcb0: 7574 6573 2829 0d0a 2020 2020 2020 2020  utes()..        
+0000fcc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000fcd0: 6175 746f 656e 636f 6465 725f 6d6f 6465  autoencoder_mode
+0000fce0: 6c20 616e 6420 7365 6c66 2e73 6567 5f69  l and self.seg_i
+0000fcf0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+0000fd00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000fd10: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000fd20: 2747 6574 7469 6e67 2061 7574 6f65 6e63  'Getting autoenc
+0000fd30: 6f64 6572 2063 6c6f 7564 7327 290d 0a20  oder clouds').. 
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd50: 2020 2020 2020 7365 6c66 2e5f 6173 7369        self._assi
+0000fd60: 676e 5f63 6c75 7374 6572 5f63 6c61 7373  gn_cluster_class
+0000fd70: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000fd80: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000fd90: 2827 4372 6561 7469 6e67 206d 6173 7465  ('Creating maste
+0000fda0: 7220 786d 6c27 290d 0a20 2020 2020 2020  r xml')..       
+0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdc0: 7365 6c66 2e5f 6372 6561 7465 5f6d 6173  self._create_mas
+0000fdd0: 7465 725f 786d 6c28 290d 0a20 2020 2020  ter_xml()..     
+0000fde0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fdf0: 636f 756e 7420 3d20 3020 0d0a 2020 2020  count = 0 ..    
+0000fe00: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000fe10: 7472 6163 6b5f 6964 2069 6e20 7365 6c66  track_id in self
+0000fe20: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+0000fe30: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+0000fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe50: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000fe60: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000fe70: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
 0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe90: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0000fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000feb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fec0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000fed0: 722e 7661 6c75 6520 3d20 2063 6f75 6e74  r.value =  count
-0000fee0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff00: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000ff10: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
+0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fea0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000feb0: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
+0000fec0: 4a75 7374 206f 6e65 206d 6f72 6520 7468  Just one more th
+0000fed0: 696e 6722 0d0a 2020 2020 2020 2020 2020  ing"..          
+0000fee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fef0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ff00: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000ff10: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
 0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff30: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-0000ff40: 725f 6576 616c 203d 2043 6c75 7374 6572  r_eval = Cluster
-0000ff50: 696e 6728 7365 6c66 2e61 6363 656c 6572  ing(self.acceler
-0000ff60: 6174 6f72 2c20 7365 6c66 2e64 6576 6963  ator, self.devic
-0000ff70: 6573 2c20 7365 6c66 2e73 6567 5f69 6d61  es, self.seg_ima
-0000ff80: 6765 5b69 6e74 2874 696d 655f 6b65 7929  ge[int(time_key)
-0000ff90: 2c3a 5d2c 2020 7365 6c66 2e61 7865 732c  ,:],  self.axes,
-0000ffa0: 2073 656c 662e 6e75 6d5f 706f 696e 7473   self.num_points
-0000ffb0: 2c20 7365 6c66 2e61 7574 6f65 6e63 6f64  , self.autoencod
-0000ffc0: 6572 5f6d 6f64 656c 2c20 6b65 7920 3d20  er_model, key = 
-0000ffd0: 7469 6d65 5f6b 6579 2c20 7072 6f67 7265  time_key, progre
-0000ffe0: 7373 5f62 6172 3d73 656c 662e 7072 6f67  ss_bar=self.prog
-0000fff0: 7265 7373 5f62 6172 2c20 6261 7463 685f  ress_bar, batch_
-00010000: 7369 7a65 203d 2073 656c 662e 6261 7463  size = self.batc
-00010010: 685f 7369 7a65 2c20 7363 616c 655f 7a3d  h_size, scale_z=
-00010020: 7365 6c66 2e73 6361 6c65 5f7a 2c20 7363  self.scale_z, sc
-00010030: 616c 655f 7879 3d20 7365 6c66 2e73 6361  ale_xy= self.sca
-00010040: 6c65 5f78 792c 2063 656e 7465 7220 3d20  le_xy, center = 
-00010050: 7365 6c66 2e63 656e 7465 7229 2020 2020  self.center)    
-00010060: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00010070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010080: 636c 7573 7465 725f 6576 616c 2e5f 6372  cluster_eval._cr
-00010090: 6561 7465 5f63 6c75 7374 6572 5f6c 6162  eate_cluster_lab
-000100a0: 656c 7328 290d 0a20 2020 2020 2020 2020  els()..         
+0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff40: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
+0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff70: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000ff80: 656e 2873 656c 662e 6669 6c74 6572 6564  en(self.filtered
+0000ff90: 5f74 7261 636b 5f69 6473 292c 0d0a 2020  _track_ids),..  
+0000ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffc0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fff0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00010000: 7373 5f62 6172 2e73 686f 7728 290d 0a20  ss_bar.show().. 
+00010010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010030: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+00010040: 7420 3d20 7365 6c66 2e63 6f75 6e74 202b  t = self.count +
+00010050: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010070: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010080: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
+00010090: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
+000100a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000100b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100c0: 2020 7469 6d65 645f 636c 7573 7465 725f    timed_cluster_
-000100d0: 6c61 6265 6c20 3d20 636c 7573 7465 725f  label = cluster_
-000100e0: 6576 616c 2e74 696d 6564 5f63 6c75 7374  eval.timed_clust
-000100f0: 6572 5f6c 6162 656c 200d 0a20 2020 2020  er_label ..     
-00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010110: 2020 2020 2020 6f75 7470 7574 5f6c 6162        output_lab
-00010120: 656c 732c 2020 6f75 7470 7574 5f63 6c75  els,  output_clu
-00010130: 7374 6572 5f63 656e 7472 6f69 642c 206f  ster_centroid, o
-00010140: 7574 7075 745f 636c 6f75 645f 6563 6365  utput_cloud_ecce
-00010150: 6e74 7269 6369 7479 2c20 6f75 7470 7574  ntricity, output
-00010160: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
-00010170: 6374 6f72 2c20 6f75 7470 7574 5f6c 6172  ctor, output_lar
-00010180: 6765 7374 5f65 6967 656e 7661 6c75 652c  gest_eigenvalue,
-00010190: 206f 7574 7075 745f 6469 6d65 6e73 696f   output_dimensio
-000101a0: 6e73 2c20 6f75 7470 7574 5f63 6c6f 7564  ns, output_cloud
-000101b0: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
-000101c0: 7469 6d65 645f 636c 7573 7465 725f 6c61  timed_cluster_la
-000101d0: 6265 6c5b 7469 6d65 5f6b 6579 5d0d 0a20  bel[time_key].. 
-000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101f0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00010200: 3120 3d20 310d 0a20 2020 2020 2020 2020  1 = 1..         
-00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010220: 2020 7363 616c 655f 3220 3d20 310d 0a20    scale_2 = 1.. 
-00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010240: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00010250: 696e 2072 616e 6765 286c 656e 286f 7574  in range(len(out
-00010260: 7075 745f 636c 7573 7465 725f 6365 6e74  put_cluster_cent
-00010270: 726f 6964 2929 3a0d 0a20 2020 2020 2020  roid)):..       
-00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010290: 2020 2020 2020 2020 2020 2020 2063 656e               cen
-000102a0: 7472 6f69 6420 3d20 6f75 7470 7574 5f63  troid = output_c
-000102b0: 6c75 7374 6572 5f63 656e 7472 6f69 645b  luster_centroid[
-000102c0: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
-000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102e0: 2020 2020 2020 2020 7175 616c 6974 7920          quality 
-000102f0: 3d20 6f75 7470 7574 5f6c 6172 6765 7374  = output_largest
-00010300: 5f65 6967 656e 7661 6c75 655b 695d 0d0a  _eigenvalue[i]..
+000100c0: 2020 2020 2020 7365 6c66 2e5f 6669 6e61        self._fina
+000100d0: 6c5f 7472 6163 6b73 2874 7261 636b 5f69  l_tracks(track_i
+000100e0: 6429 200d 0a0d 0a20 2020 2020 2020 2020  d) ....         
+000100f0: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+00010100: 6f75 7269 6572 3a0d 0a20 2020 2020 2020  ourier:..       
+00010110: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00010120: 7428 2763 6f6d 7075 7469 6e67 2046 6f75  t('computing Fou
+00010130: 7269 6572 2729 0d0a 2020 2020 2020 2020  rier')..        
+00010140: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010150: 5f63 6f6d 7075 7465 5f70 6865 6e6f 7479  _compute_phenoty
+00010160: 7065 7328 2920 2020 2020 2020 2020 2020  pes()           
+00010170: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00010180: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010190: 656c 662e 5f74 656d 706f 7261 6c5f 706c  elf._temporal_pl
+000101a0: 6f74 735f 7472 6163 6b6d 6174 6528 290d  ots_trackmate().
+000101b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101c0: 200d 0a0d 0a20 2020 2064 6566 205f 6372   ....    def _cr
+000101d0: 6561 7465 5f6d 6173 7465 725f 786d 6c28  eate_master_xml(
+000101e0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000101f0: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+00010200: 2020 2020 2020 2020 2020 666f 7220 5370            for Sp
+00010210: 6f74 6f62 6a65 6374 2069 6e20 7365 6c66  otobject in self
+00010220: 2e6d 6173 7465 725f 786d 6c5f 726f 6f74  .master_xml_root
+00010230: 2e69 7465 7228 2753 706f 7427 293a 0d0a  .iter('Spot'):..
+00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010260: 6365 6c6c 5f69 6420 3d20 696e 7428 5370  cell_id = int(Sp
+00010270: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+00010280: 662e 7370 6f74 6964 5f6b 6579 2929 0d0a  f.spotid_key))..
+00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 6966 2063 656c 6c5f 6964 2069 6e20 7365  if cell_id in se
+000102c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000102d0: 726f 7065 7274 6965 732e 6b65 7973 2829  roperties.keys()
+000102e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010300: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010330: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
-00010340: 5f63 6f6d 705f 6669 7273 7479 7a20 3d20  _comp_firstyz = 
-00010350: 6f75 7470 7574 5f63 6c6f 7564 5f65 6363  output_cloud_ecc
-00010360: 656e 7472 6963 6974 795b 695d 0d0a 2020  entricity[i]..  
+00010330: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
+00010340: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00010350: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00010360: 2e6b 6579 7328 293a 0d0a 0d0a 2020 2020  .keys():....    
 00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2020 6573 7365 6e74 7269 6369 7479 5f64    essentricity_d
-000103a0: 696d 656e 7369 6f6e 203d 206f 7574 7075  imension = outpu
-000103b0: 745f 6469 6d65 6e73 696f 6e73 5b69 5d20  t_dimensions[i] 
-000103c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
-000103f0: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
-00010400: 305d 203d 3d20 323a 0d0a 2020 2020 2020  0] == 2:..      
-00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010430: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
-00010440: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-00010450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010470: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010480: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-00010490: 656e 7369 6f6e 5b31 5d20 3d3d 2031 3a0d  ension[1] == 1:.
-000104a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010390: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
+000103a0: 742e 7365 7428 6b2c 2073 7472 2873 656c  t.set(k, str(sel
+000103b0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000103c0: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+000103d0: 5d5b 6b5d 2929 2020 200d 0a0d 0a20 2020  ][k]))   ....   
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010400: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00010410: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
+00010420: 6c5f 7472 6565 2e77 7269 7465 286f 732e  l_tree.write(os.
+00010430: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e6d  path.join(self.m
+00010440: 6173 7465 725f 786d 6c5f 7061 7468 2c20  aster_xml_path, 
+00010450: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+00010460: 6e61 6d65 2929 0d0a 2020 2020 2020 2020  name))..        
+00010470: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010490: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
-000104e0: 662e 7963 616c 6962 7261 7469 6f6e 0d0a  f.ycalibration..
-000104f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000104c0: 2020 2020 200d 0a0d 0a20 2020 2064 6566       ....    def
+000104d0: 205f 6173 7369 676e 5f63 6c75 7374 6572   _assign_cluster
+000104e0: 5f63 6c61 7373 2873 656c 6629 3a0d 0a20  _class(self):.. 
+000104f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010510: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
-00010520: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
-00010530: 305d 203d 3d20 323a 0d0a 2020 2020 2020  0] == 2:..      
-00010540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 7365 6c66 2e61 7865 7320 3d20 7365 6c66  self.axes = self
+00010520: 2e61 7865 732e 7265 706c 6163 6528 2254  .axes.replace("T
+00010530: 222c 2022 2229 0d0a 2020 2020 2020 2020  ", "")..        
+00010540: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
-00010570: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-00010580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000105b0: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-000105c0: 656e 7369 6f6e 5b31 5d20 3d3d 2030 3a0d  ension[1] == 0:.
-000105d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
-00010610: 662e 7863 616c 6962 7261 7469 6f6e 2020  f.xcalibration  
-00010620: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010640: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
-00010650: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
-00010660: 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20 2020  on[0] == 1:..   
-00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010690: 2020 2020 2020 2020 7363 616c 655f 3120          scale_1 
-000106a0: 3d20 7365 6c66 2e79 6361 6c69 6272 6174  = self.ycalibrat
-000106b0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00010560: 2020 666f 7220 636f 756e 742c 2074 696d    for count, tim
+00010570: 655f 6b65 7920 696e 2065 6e75 6d65 7261  e_key in enumera
+00010580: 7465 2873 656c 662e 5f74 696d 6564 5f63  te(self._timed_c
+00010590: 656e 7472 6f69 642e 6b65 7973 2829 293a  entroid.keys()):
+000105a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000105b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105d0: 2020 2020 2020 2020 2020 7472 6565 2c20            tree, 
+000105e0: 7370 6f74 5f63 656e 7472 6f69 6473 203d  spot_centroids =
+000105f0: 2073 656c 662e 5f74 696d 6564 5f63 656e   self._timed_cen
+00010600: 7472 6f69 645b 7469 6d65 5f6b 6579 5d0d  troid[time_key].
+00010610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010620: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00010630: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00010640: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010660: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010670: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00010680: 2e6c 6162 656c 203d 2022 4175 746f 656e  .label = "Autoen
+00010690: 636f 6465 7220 666f 7220 7265 6669 6e69  coder for refini
+000106a0: 6e67 2070 6f69 6e74 2063 6c6f 7564 7322  ng point clouds"
+000106b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000106c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106e0: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
-000106f0: 6469 6d65 6e73 696f 6e5b 315d 203d 3d20  dimension[1] == 
-00010700: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+000106d0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+000106e0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+000106f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010730: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
-00010740: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00010750: 6e20 200d 0a0d 0a20 2020 2020 2020 2020  n  ....         
+00010720: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00010730: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00010740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2020 2020 2020 2020 2020 2069 6620 6573             if es
-00010780: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
-00010790: 7369 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20  sion[0] == 1:.. 
+00010770: 2020 206c 656e 2873 656c 662e 5f74 696d     len(self._tim
+00010780: 6564 5f63 656e 7472 6f69 642e 6b65 7973  ed_centroid.keys
+00010790: 2829 2920 2b20 312c 0d0a 2020 2020 2020  ()) + 1,..      
 000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000107b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107c0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-000107d0: 3120 3d20 7365 6c66 2e79 6361 6c69 6272  1 = self.ycalibr
-000107e0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010810: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
-00010820: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
-00010830: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
-00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010860: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
-00010870: 3d20 7365 6c66 2e7a 6361 6c69 6272 6174  = self.zcalibrat
-00010880: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-00010890: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108b0: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-000108c0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-000108d0: 696f 6e5b 305d 203d 3d20 303a 0d0a 2020  ion[0] == 0:..  
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010900: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-00010910: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
-00010920: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00010930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010950: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-00010960: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-00010970: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109a0: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-000109b0: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-000109c0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-000109f0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00010a00: 696f 6e5b 305d 203d 3d20 303a 0d0a 2020  ion[0] == 0:..  
-00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a30: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-00010a40: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
-00010a50: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00010a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a80: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-00010a90: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-00010aa0: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
-00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ad0: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-00010ae0: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
-00010af0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107d0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107f0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00010800: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+00010810: 203d 2020 636f 756e 7420 0d0a 2020 2020   =  count ..    
+00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010840: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
+00010850: 6f77 2829 0d0a 0d0a 2020 2020 2020 2020  ow()....        
+00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010870: 2020 2063 6c75 7374 6572 5f65 7661 6c20     cluster_eval 
+00010880: 3d20 436c 7573 7465 7269 6e67 2873 656c  = Clustering(sel
+00010890: 662e 6163 6365 6c65 7261 746f 722c 2073  f.accelerator, s
+000108a0: 656c 662e 6465 7669 6365 732c 2073 656c  elf.devices, sel
+000108b0: 662e 7365 675f 696d 6167 655b 696e 7428  f.seg_image[int(
+000108c0: 7469 6d65 5f6b 6579 292c 3a5d 2c20 2073  time_key),:],  s
+000108d0: 656c 662e 6178 6573 2c20 7365 6c66 2e6e  elf.axes, self.n
+000108e0: 756d 5f70 6f69 6e74 732c 2073 656c 662e  um_points, self.
+000108f0: 6175 746f 656e 636f 6465 725f 6d6f 6465  autoencoder_mode
+00010900: 6c2c 206b 6579 203d 2074 696d 655f 6b65  l, key = time_ke
+00010910: 792c 2070 726f 6772 6573 735f 6261 723d  y, progress_bar=
+00010920: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00010930: 722c 2062 6174 6368 5f73 697a 6520 3d20  r, batch_size = 
+00010940: 7365 6c66 2e62 6174 6368 5f73 697a 652c  self.batch_size,
+00010950: 2073 6361 6c65 5f7a 3d73 656c 662e 7363   scale_z=self.sc
+00010960: 616c 655f 7a2c 2073 6361 6c65 5f78 793d  ale_z, scale_xy=
+00010970: 2073 656c 662e 7363 616c 655f 7879 2c20   self.scale_xy, 
+00010980: 6365 6e74 6572 203d 2073 656c 662e 6365  center = self.ce
+00010990: 6e74 6572 2920 2020 2020 2020 0d0a 2020  nter)       ..  
+000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109b0: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
+000109c0: 5f65 7661 6c2e 5f63 7265 6174 655f 636c  _eval._create_cl
+000109d0: 7573 7465 725f 6c61 6265 6c73 2829 0d0a  uster_labels()..
+000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109f0: 2020 2020 2020 2020 2020 2074 696d 6564             timed
+00010a00: 5f63 6c75 7374 6572 5f6c 6162 656c 203d  _cluster_label =
+00010a10: 2063 6c75 7374 6572 5f65 7661 6c2e 7469   cluster_eval.ti
+00010a20: 6d65 645f 636c 7573 7465 725f 6c61 6265  med_cluster_labe
+00010a30: 6c20 0d0a 2020 2020 2020 2020 2020 2020  l ..            
+00010a40: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00010a50: 7574 7075 745f 6c61 6265 6c73 2c20 206f  utput_labels,  o
+00010a60: 7574 7075 745f 636c 7573 7465 725f 6365  utput_cluster_ce
+00010a70: 6e74 726f 6964 2c20 6f75 7470 7574 5f63  ntroid, output_c
+00010a80: 6c6f 7564 5f65 6363 656e 7472 6963 6974  loud_eccentricit
+00010a90: 792c 206f 7574 7075 745f 6c61 7267 6573  y, output_larges
+00010aa0: 745f 6569 6765 6e76 6563 746f 722c 206f  t_eigenvector, o
+00010ab0: 7574 7075 745f 6c61 7267 6573 745f 6569  utput_largest_ei
+00010ac0: 6765 6e76 616c 7565 2c20 6f75 7470 7574  genvalue, output
+00010ad0: 5f64 696d 656e 7369 6f6e 732c 206f 7574  _dimensions, out
+00010ae0: 7075 745f 636c 6f75 645f 7375 7266 6163  put_cloud_surfac
+00010af0: 655f 6172 6561 203d 2074 696d 6564 5f63  e_area = timed_c
+00010b00: 6c75 7374 6572 5f6c 6162 656c 5b74 696d  luster_label[tim
+00010b10: 655f 6b65 795d 0d0a 2020 2020 2020 2020  e_key]..        
 00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b30: 2020 2073 6361 6c65 5f31 203d 2031 0d0a     scale_1 = 1..
 00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b50: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00010b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b50: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00010b60: 5f32 203d 2031 0d0a 2020 2020 2020 2020  _2 = 1..        
 00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ba0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00010bb0: 6c5f 6178 6973 203d 206f 7574 7075 745f  l_axis = output_
-00010bc0: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
-00010bd0: 746f 725b 695d 0d0a 2020 2020 2020 2020  tor[i]..        
-00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bf0: 2020 2020 2020 2020 2020 2020 7375 7266              surf
-00010c00: 6163 655f 6172 6561 203d 206f 7574 7075  ace_area = outpu
-00010c10: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
-00010c20: 6172 6561 5b69 5d20 2a20 7365 6c66 2e7a  area[i] * self.z
-00010c30: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
-00010c40: 6c66 2e79 6361 6c69 6272 6174 696f 6e20  lf.ycalibration 
-00010c50: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
-00010c60: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c80: 2020 2020 2020 2020 2064 6973 742c 2069           dist, i
-00010c90: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
-00010ca0: 7928 6365 6e74 726f 6964 290d 0a20 2020  y(centroid)..   
+00010b80: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00010b90: 6528 6c65 6e28 6f75 7470 7574 5f63 6c75  e(len(output_clu
+00010ba0: 7374 6572 5f63 656e 7472 6f69 6429 293a  ster_centroid)):
+00010bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bd0: 2020 2020 2020 6365 6e74 726f 6964 203d        centroid =
+00010be0: 206f 7574 7075 745f 636c 7573 7465 725f   output_cluster_
+00010bf0: 6365 6e74 726f 6964 5b69 5d0d 0a20 2020  centroid[i]..   
+00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c20: 2071 7561 6c69 7479 203d 206f 7574 7075   quality = outpu
+00010c30: 745f 6c61 7267 6573 745f 6569 6765 6e76  t_largest_eigenv
+00010c40: 616c 7565 5b69 5d0d 0a20 2020 2020 2020  alue[i]..       
+00010c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c60: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+00010c70: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00010c80: 6972 7374 797a 203d 206f 7574 7075 745f  irstyz = output_
+00010c90: 636c 6f75 645f 6563 6365 6e74 7269 6369  cloud_eccentrici
+00010ca0: 7479 5b69 5d0d 0a20 2020 2020 2020 2020  ty[i]..         
 00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cd0: 2072 6164 6975 7320 3d20 7175 616c 6974   radius = qualit
-00010ce0: 7920 2a20 6d61 7468 2e70 6f77 2873 656c  y * math.pow(sel
-00010cf0: 662e 7a63 616c 6962 7261 7469 6f6e 202a  f.zcalibration *
-00010d00: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-00010d10: 6f6e 202a 2073 656c 662e 7963 616c 6962  on * self.ycalib
-00010d20: 7261 7469 6f6e 2c20 312e 302f 332e 3029  ration, 1.0/3.0)
-00010d30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d50: 2020 2020 2020 6966 2064 6973 7420 3c20        if dist < 
-00010d60: 7175 616c 6974 793a 0d0a 2020 2020 2020  quality:..      
-00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d90: 2020 2020 2020 636c 6f73 6573 745f 6365        closest_ce
-00010da0: 6e74 726f 6964 203d 2073 706f 745f 6365  ntroid = spot_ce
-00010db0: 6e74 726f 6964 735b 696e 6465 785d 0d0a  ntroids[index]..
-00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010de0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00010df0: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
-00010e00: 3d20 2869 6e74 2874 696d 655f 6b65 7929  = (int(time_key)
-00010e10: 2c63 6c6f 7365 7374 5f63 656e 7472 6f69  ,closest_centroi
-00010e20: 645b 305d 2c20 636c 6f73 6573 745f 6365  d[0], closest_ce
-00010e30: 6e74 726f 6964 5b31 5d2c 2063 6c6f 7365  ntroid[1], close
-00010e40: 7374 5f63 656e 7472 6f69 645b 325d 290d  st_centroid[2]).
-00010e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e70: 2020 2020 2020 2020 2020 2020 2063 6c6f               clo
-00010e80: 7365 7374 5f63 656c 6c5f 6964 203d 2073  sest_cell_id = s
-00010e90: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00010ea0: 6365 6e74 726f 6964 5b66 7261 6d65 5f73  centroid[frame_s
-00010eb0: 706f 745f 6365 6e74 726f 6964 5d0d 0a20  pot_centroid].. 
+00010cc0: 2020 2020 2020 2020 2020 2065 7373 656e             essen
+00010cd0: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
+00010ce0: 6e20 3d20 6f75 7470 7574 5f64 696d 656e  n = output_dimen
+00010cf0: 7369 6f6e 735b 695d 200d 0a20 2020 2020  sions[i] ..     
+00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010d20: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
+00010d30: 696d 656e 7369 6f6e 5b30 5d20 3d3d 2032  imension[0] == 2
+00010d40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d60: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00010d70: 616c 655f 3120 3d20 7365 6c66 2e7a 6361  ale_1 = self.zca
+00010d80: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010db0: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
+00010dc0: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
+00010dd0: 315d 203d 3d20 313a 0d0a 2020 2020 2020  1] == 1:..      
+00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00010e10: 655f 3220 3d20 7365 6c66 2e79 6361 6c69  e_2 = self.ycali
+00010e20: 6272 6174 696f 6e0d 0a0d 0a20 2020 2020  bration....     
+00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010e50: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
+00010e60: 696d 656e 7369 6f6e 5b30 5d20 3d3d 2032  imension[0] == 2
+00010e70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e90: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00010ea0: 616c 655f 3120 3d20 7365 6c66 2e7a 6361  ale_1 = self.zca
+00010eb0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
 00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ee0: 2020 2020 2020 2020 2020 206d 6173 6b5f             mask_
-00010ef0: 7665 6374 6f72 203d 205b 2066 6c6f 6174  vector = [ float
-00010f00: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00010f10: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00010f20: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00010f30: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-00010f40: 726f 6964 5f78 5f6b 6579 5d29 2c20 666c  roid_x_key]), fl
-00010f50: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00010f60: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00010f70: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00010f80: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
-00010f90: 656e 7472 6f69 645f 795f 6b65 795d 292c  entroid_y_key]),
-00010fa0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00010fb0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00010fc0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00010fd0: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-00010fe0: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
-00010ff0: 5d29 205d 0d0a 2020 2020 2020 2020 2020  ]) ]..          
+00010ee0: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
+00010ef0: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
+00010f00: 315d 203d 3d20 303a 0d0a 2020 2020 2020  1] == 0:..      
+00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00010f40: 655f 3220 3d20 7365 6c66 2e78 6361 6c69  e_2 = self.xcali
+00010f50: 6272 6174 696f 6e20 2020 0d0a 0d0a 2020  bration   ....  
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+00010f90: 795f 6469 6d65 6e73 696f 6e5b 305d 203d  y_dimension[0] =
+00010fa0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fd0: 2073 6361 6c65 5f31 203d 2073 656c 662e   scale_1 = self.
+00010fe0: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011020: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
-00011030: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
-00011040: 6528 6365 6c6c 5f61 7869 732c 206d 6173  e(cell_axis, mas
-00011050: 6b5f 7665 6374 6f72 290d 0a20 2020 2020  k_vector)..     
-00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00011010: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
+00011020: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
+00011030: 6f6e 5b31 5d20 3d3d 2030 3a0d 0a20 2020  on[1] == 0:..   
+00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011060: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011070: 6361 6c65 5f32 203d 2073 656c 662e 7863  cale_2 = self.xc
+00011080: 616c 6962 7261 7469 6f6e 2020 0d0a 0d0a  alibration  ....
 00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000110c0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000110d0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-000110e0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-000110f0: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
-00011100: 6b5f 6b65 7920 3a20 6365 6c6c 5f61 7869  k_key : cell_axi
-00011110: 735f 6d61 736b 7d29 0d0a 2020 2020 2020  s_mask})..      
+000110b0: 2020 2020 6966 2065 7373 656e 7472 6963      if essentric
+000110c0: 6974 795f 6469 6d65 6e73 696f 6e5b 305d  ity_dimension[0]
+000110d0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011100: 2020 2073 6361 6c65 5f31 203d 2073 656c     scale_1 = sel
+00011110: 662e 7963 616c 6962 7261 7469 6f6e 0d0a  f.ycalibration..
 00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011140: 2020 2020 2020 6966 2073 656c 662e 756e        if self.un
-00011150: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011160: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00011170: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
-00011180: 7261 6469 7573 5f6b 6579 5d20 3e20 303a  radius_key] > 0:
-00011190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000111d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000111e0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-000111f0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00011200: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-00011210: 795f 636f 6d70 5f66 6972 7374 6b65 7920  y_comp_firstkey 
-00011220: 3a20 6563 6365 6e74 7269 6369 7479 5f63  : eccentricity_c
-00011230: 6f6d 705f 6669 7273 7479 7a5b 305d 202a  omp_firstyz[0] *
-00011240: 2073 6361 6c65 5f31 7d29 0d0a 2020 2020   scale_1})..    
-00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011140: 2020 2020 2020 2020 2020 2069 6620 6573             if es
+00011150: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
+00011160: 7369 6f6e 5b31 5d20 3d3d 2032 3a0d 0a20  sion[1] == 2:.. 
+00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111a0: 2073 6361 6c65 5f32 203d 2073 656c 662e   scale_2 = self.
+000111b0: 7a63 616c 6962 7261 7469 6f6e 2020 2020  zcalibration    
+000111c0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111f0: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+00011200: 7479 5f64 696d 656e 7369 6f6e 5b30 5d20  ty_dimension[0] 
+00011210: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011240: 2020 7363 616c 655f 3120 3d20 7365 6c66    scale_1 = self
+00011250: 2e78 6361 6c69 6272 6174 696f 6e0d 0a20  .xcalibration.. 
 00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011280: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00011290: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000112a0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-000112b0: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
-000112c0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000112d0: 5f73 6563 6f6e 646b 6579 203a 2065 6363  _secondkey : ecc
-000112e0: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-000112f0: 6972 7374 797a 5b31 5d20 2a20 7363 616c  irstyz[1] * scal
-00011300: 655f 327d 290d 0a20 2020 2020 2020 2020  e_2})..         
+00011280: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+00011290: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+000112a0: 696f 6e5b 315d 203d 3d20 313a 0d0a 2020  ion[1] == 1:..  
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112e0: 7363 616c 655f 3220 3d20 7365 6c66 2e79  scale_2 = self.y
+000112f0: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
+00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011340: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00011350: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00011360: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
-00011370: 6174 6528 7b73 656c 662e 7375 7266 6163  ate({self.surfac
-00011380: 655f 6172 6561 5f6b 6579 203a 2073 7572  e_area_key : sur
-00011390: 6661 6365 5f61 7265 617d 290d 0a20 2020  face_area})..   
+00011320: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+00011330: 7479 5f64 696d 656e 7369 6f6e 5b30 5d20  ty_dimension[0] 
+00011340: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011370: 2020 7363 616c 655f 3120 3d20 7365 6c66    scale_1 = self
+00011380: 2e78 6361 6c69 6272 6174 696f 6e0d 0a20  .xcalibration.. 
+00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113d0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000113e0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000113f0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00011400: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00011410: 7175 616c 6974 795f 6b65 7920 3a20 7175  quality_key : qu
-00011420: 616c 6974 797d 290d 0a20 2020 2020 2020  ality})..       
+000113b0: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+000113c0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+000113d0: 696f 6e5b 315d 203d 3d20 323a 0d0a 2020  ion[1] == 2:..  
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011410: 7363 616c 655f 3220 3d20 7365 6c66 2e7a  scale_2 = self.z
+00011420: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
 00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011450: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011460: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00011470: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00011480: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-00011490: 7064 6174 6528 7b73 656c 662e 7261 6469  pdate({self.radi
-000114a0: 7573 5f6b 6579 203a 2072 6164 6975 7320  us_key : radius 
-000114b0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114e0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011510: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000114e0: 2020 2020 2020 6365 6c6c 5f61 7869 7320        cell_axis 
+000114f0: 3d20 6f75 7470 7574 5f6c 6172 6765 7374  = output_largest
+00011500: 5f65 6967 656e 7665 6374 6f72 5b69 5d0d  _eigenvector[i].
+00011510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00011560: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00011570: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00011580: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
-00011590: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000115a0: 5f66 6972 7374 6b65 7920 3a20 2d31 7d29  _firstkey : -1})
-000115b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000115f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00011600: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00011610: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00011620: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-00011630: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
-00011640: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
-00011650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011670: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011680: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00011690: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-000116a0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-000116b0: 7064 6174 6528 7b73 656c 662e 7375 7266  pdate({self.surf
-000116c0: 6163 655f 6172 6561 5f6b 6579 203a 202d  ace_area_key : -
-000116d0: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
-000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00011710: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011720: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00011730: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
-00011740: 6528 7b73 656c 662e 7175 616c 6974 795f  e({self.quality_
-00011750: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
-00011760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011790: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000117a0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000117b0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-000117c0: 5d2e 7570 6461 7465 287b 7365 6c66 2e72  ].update({self.r
-000117d0: 6164 6975 735f 6b65 7920 3a20 2d31 207d  adius_key : -1 }
-000117e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011530: 2020 2020 2073 7572 6661 6365 5f61 7265       surface_are
+00011540: 6120 3d20 6f75 7470 7574 5f63 6c6f 7564  a = output_cloud
+00011550: 5f73 7572 6661 6365 5f61 7265 615b 695d  _surface_area[i]
+00011560: 202a 2073 656c 662e 7a63 616c 6962 7261   * self.zcalibra
+00011570: 7469 6f6e 202a 2073 656c 662e 7963 616c  tion * self.ycal
+00011580: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
+00011590: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115c0: 2020 6469 7374 2c20 696e 6465 7820 3d20    dist, index = 
+000115d0: 7472 6565 2e71 7565 7279 2863 656e 7472  tree.query(centr
+000115e0: 6f69 6429 0d0a 2020 2020 2020 2020 2020  oid)..          
+000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011600: 2020 2020 2020 2020 2020 7261 6469 7573            radius
+00011610: 203d 2071 7561 6c69 7479 202a 206d 6174   = quality * mat
+00011620: 682e 706f 7728 7365 6c66 2e7a 6361 6c69  h.pow(self.zcali
+00011630: 6272 6174 696f 6e20 2a20 7365 6c66 2e78  bration * self.x
+00011640: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
+00011650: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
+00011660: 2031 2e30 2f33 2e30 290d 0a20 2020 2020   1.0/3.0)..     
+00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011680: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011690: 6620 6469 7374 203c 2071 7561 6c69 7479  f dist < quality
+000116a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000116d0: 6c6f 7365 7374 5f63 656e 7472 6f69 6420  losest_centroid 
+000116e0: 3d20 7370 6f74 5f63 656e 7472 6f69 6473  = spot_centroids
+000116f0: 5b69 6e64 6578 5d0d 0a20 2020 2020 2020  [index]..       
+00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011720: 2020 2020 2066 7261 6d65 5f73 706f 745f       frame_spot_
+00011730: 6365 6e74 726f 6964 203d 2028 696e 7428  centroid = (int(
+00011740: 7469 6d65 5f6b 6579 292c 636c 6f73 6573  time_key),closes
+00011750: 745f 6365 6e74 726f 6964 5b30 5d2c 2063  t_centroid[0], c
+00011760: 6c6f 7365 7374 5f63 656e 7472 6f69 645b  losest_centroid[
+00011770: 315d 2c20 636c 6f73 6573 745f 6365 6e74  1], closest_cent
+00011780: 726f 6964 5b32 5d29 0d0a 2020 2020 2020  roid[2])..      
+00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117b0: 2020 2020 2020 636c 6f73 6573 745f 6365        closest_ce
+000117c0: 6c6c 5f69 6420 3d20 7365 6c66 2e75 6e69  ll_id = self.uni
+000117d0: 7175 655f 7370 6f74 5f63 656e 7472 6f69  que_spot_centroi
+000117e0: 645b 6672 616d 655f 7370 6f74 5f63 656e  d[frame_spot_cen
+000117f0: 7472 6f69 645d 0d0a 2020 2020 2020 2020  troid]..        
 00011800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011810: 2020 2020 2020 0d0a 0d0a 0d0a 0d0a 0d0a        ..........
-00011820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011840: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011860: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-00011870: 6c66 2e72 6f6f 745f 7370 6f74 732e 6974  lf.root_spots.it
-00011880: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000118b0: 6f6f 745f 7370 6f74 735b 6b5d 203d 2073  oot_spots[k] = s
-000118c0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000118d0: 7072 6f70 6572 7469 6573 5b6b 5d20 2020  properties[k]   
-000118e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000118f0: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00011900: 6620 5f63 6f6d 7075 7465 5f70 6865 6e6f  f _compute_pheno
-00011910: 7479 7065 7328 7365 6c66 293a 0d0a 0d0a  types(self):....
-00011920: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
-00011930: 2c76 2920 696e 2073 656c 662e 756e 6971  ,v) in self.uniq
-00011940: 7565 5f74 7261 636b 732e 6974 656d 7328  ue_tracks.items(
-00011950: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00011960: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00011970: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
-00011980: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
-00011990: 2020 2020 7472 6163 6b6c 6574 5f70 726f      tracklet_pro
-000119a0: 7065 7274 6965 7320 3d20 7365 6c66 2e75  perties = self.u
-000119b0: 6e69 7175 655f 7472 6163 6b5f 7072 6f70  nique_track_prop
-000119c0: 6572 7469 6573 5b6b 5d0d 0a20 2020 2020  erties[k]..     
-000119d0: 2020 2020 2020 2020 2020 2074 7261 636b             track
-000119e0: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
-000119f0: 7472 6163 6b73 5b6b 5d0d 0a20 2020 2020  tracks[k]..     
-00011a00: 2020 2020 2020 2020 2020 205a 203d 2074             Z = t
-00011a10: 7261 636b 735b 3a2c 325d 0d0a 2020 2020  racks[:,2]..    
-00011a20: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
-00011a30: 7472 6163 6b73 5b3a 2c33 5d0d 0a20 2020  tracks[:,3]..   
-00011a40: 2020 2020 2020 2020 2020 2020 2058 203d               X =
-00011a50: 2074 7261 636b 735b 3a2c 345d 0d0a 2020   tracks[:,4]..  
-00011a60: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00011a70: 6d65 203d 2074 7261 636b 6c65 745f 7072  me = tracklet_pr
-00011a80: 6f70 6572 7469 6573 5b3a 2c30 5d0d 0a20  operties[:,0].. 
-00011a90: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00011aa0: 6e69 7175 655f 6964 7320 3d20 7472 6163  nique_ids = trac
-00011ab0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00011ac0: 3a2c 315d 0d0a 2020 2020 2020 2020 2020  :,1]..          
-00011ad0: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
-00011ae0: 5f73 6574 203d 2073 6574 2875 6e69 7175  _set = set(uniqu
-00011af0: 655f 6964 7329 0d0a 2020 2020 2020 2020  e_ids)..        
-00011b00: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
-00011b10: 6f6e 5f69 6473 203d 2074 7261 636b 6c65  on_ids = trackle
-00011b20: 745f 7072 6f70 6572 7469 6573 5b3a 2c32  t_properties[:,2
-00011b30: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00011b40: 2020 2072 6164 6975 7320 3d20 7472 6163     radius = trac
-00011b50: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00011b60: 3a2c 335d 0d0a 2020 2020 2020 2020 2020  :,3]..          
-00011b70: 2020 2020 2020 766f 6c75 6d65 203d 2074        volume = t
-00011b80: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-00011b90: 6573 5b3a 2c34 5d0d 0a20 2020 2020 2020  es[:,4]..       
-00011ba0: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-00011bb0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00011bc0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00011bd0: 6572 7469 6573 5b3a 2c35 5d0d 0a20 2020  erties[:,5]..   
-00011be0: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
-00011bf0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00011c00: 6563 6f6e 6420 3d20 7472 6163 6b6c 6574  econd = tracklet
-00011c10: 5f70 726f 7065 7274 6965 735b 3a2c 365d  _properties[:,6]
-00011c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011c30: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
-00011c40: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00011c50: 7469 6573 5b3a 2c37 5d0d 0a20 2020 2020  ties[:,7]..     
-00011c60: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00011c70: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-00011c80: 6e73 6974 7920 3d20 7472 6163 6b6c 6574  nsity = tracklet
-00011c90: 5f70 726f 7065 7274 6965 735b 3a2c 385d  _properties[:,8]
-00011ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011cb0: 2020 7370 6565 6420 3d20 7472 6163 6b6c    speed = trackl
-00011cc0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00011cd0: 395d 0d0a 2020 2020 2020 2020 2020 2020  9]..            
-00011ce0: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
-00011cf0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00011d00: 6572 7469 6573 5b3a 2c31 305d 0d0a 2020  erties[:,10]..  
-00011d10: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-00011d20: 6365 6c65 7261 7469 6f6e 203d 2074 7261  celeration = tra
-00011d30: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00011d40: 5b3a 2c31 315d 0d0a 2020 2020 2020 2020  [:,11]..        
-00011d50: 2020 2020 2020 2020 6469 7374 616e 6365          distance
-00011d60: 5f63 656c 6c5f 6d61 736b 203d 2074 7261  _cell_mask = tra
-00011d70: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00011d80: 5b3a 2c31 325d 0d0a 2020 2020 2020 2020  [:,12]..        
-00011d90: 2020 2020 2020 2020 7261 6469 616c 5f61          radial_a
-00011da0: 6e67 6c65 203d 2074 7261 636b 6c65 745f  ngle = tracklet_
-00011db0: 7072 6f70 6572 7469 6573 5b3a 2c31 335d  properties[:,13]
-00011dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011dd0: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
-00011de0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00011df0: 6572 7469 6573 5b3a 2c31 345d 0d0a 0d0a  erties[:,14]....
-00011e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011e10: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00011e20: 2020 2020 756e 6971 7565 5f66 6674 5f70      unique_fft_p
-00011e30: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00011e40: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
-00011e50: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-00011e60: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
-00011e70: 6573 5f74 7261 636b 6c65 7420 3d20 7b7d  es_tracklet = {}
-00011e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011e90: 2020 7365 6c66 2e75 6e69 7175 655f 6666    self.unique_ff
-00011ea0: 745f 7072 6f70 6572 7469 6573 5b74 7261  t_properties[tra
-00011eb0: 636b 5f69 645d 203d 207b 7d0d 0a20 2020  ck_id] = {}..   
-00011ec0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011ed0: 662e 756e 6971 7565 5f63 6c75 7374 6572  f.unique_cluster
-00011ee0: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
-00011ef0: 6b5f 6964 5d20 3d20 7b7d 0d0a 0d0a 2020  k_id] = {}....  
-00011f00: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00011f10: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
-00011f20: 7274 6965 735f 7472 6163 6b6c 6574 203d  rties_tracklet =
-00011f30: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00011f40: 2020 2020 2075 6e69 7175 655f 6479 6e61       unique_dyna
-00011f50: 6d69 635f 7072 6f70 6572 7469 6573 5f74  mic_properties_t
-00011f60: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
-00011f70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011f80: 6c66 2e75 6e69 7175 655f 7368 6170 655f  lf.unique_shape_
-00011f90: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
-00011fa0: 5f69 645d 203d 207b 7d0d 0a20 2020 2020  _id] = {}..     
-00011fb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011fc0: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
-00011fd0: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
-00011fe0: 6964 5d20 3d20 7b7d 0d0a 2020 2020 2020  id] = {}..      
-00011ff0: 2020 2020 2020 2020 2020 6578 7061 6e64            expand
-00012000: 6564 5f74 696d 6520 3d20 6e70 2e7a 6572  ed_time = np.zer
-00012010: 6f73 2873 656c 662e 7465 6e64 202d 2073  os(self.tend - s
-00012020: 656c 662e 7473 7461 7274 202b 2031 290d  elf.tstart + 1).
-00012030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012040: 2070 6f69 6e74 5f73 616d 706c 6520 3d20   point_sample = 
-00012050: 6578 7061 6e64 6564 5f74 696d 652e 7368  expanded_time.sh
-00012060: 6170 655b 305d 0d0a 2020 2020 2020 2020  ape[0]..        
-00012070: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00012080: 2072 616e 6765 286c 656e 2865 7870 616e   range(len(expan
-00012090: 6465 645f 7469 6d65 2929 3a0d 0a20 2020  ded_time)):..   
+00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011820: 2020 2020 6d61 736b 5f76 6563 746f 7220      mask_vector 
+00011830: 3d20 5b20 666c 6f61 7428 7365 6c66 2e75  = [ float(self.u
+00011840: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00011850: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00011860: 745f 6365 6c6c 5f69 6429 5d5b 7365 6c66  t_cell_id)][self
+00011870: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
+00011880: 6b65 795d 292c 2066 6c6f 6174 2873 656c  key]), float(sel
+00011890: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000118a0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+000118b0: 7365 7374 5f63 656c 6c5f 6964 295d 5b73  sest_cell_id)][s
+000118c0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+000118d0: 5f79 5f6b 6579 5d29 2c20 666c 6f61 7428  _y_key]), float(
+000118e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000118f0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00011900: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00011910: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
+00011920: 6f69 645f 7a5f 6b65 795d 2920 5d0d 0a20  oid_z_key]) ].. 
+00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011950: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+00011960: 6178 6973 5f6d 6173 6b20 3d20 616e 6775  axis_mask = angu
+00011970: 6c61 725f 6368 616e 6765 2863 656c 6c5f  lar_change(cell_
+00011980: 6178 6973 2c20 6d61 736b 5f76 6563 746f  axis, mask_vecto
+00011990: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000119f0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00011a00: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00011a10: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00011a20: 7570 6461 7465 287b 7365 6c66 2e63 656c  update({self.cel
+00011a30: 6c61 7869 735f 6d61 736b 5f6b 6579 203a  laxis_mask_key :
+00011a40: 2063 656c 6c5f 6178 6973 5f6d 6173 6b7d   cell_axis_mask}
+00011a50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011a80: 6620 7365 6c66 2e75 6e69 7175 655f 7370  f self.unique_sp
+00011a90: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00011aa0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00011ab0: 6429 5d5b 7365 6c66 2e72 6164 6975 735f  d)][self.radius_
+00011ac0: 6b65 795d 203e 2030 3a0d 0a20 2020 2020  key] > 0:..     
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011b00: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00011b10: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00011b20: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00011b30: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
+00011b40: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00011b50: 6669 7273 746b 6579 203a 2065 6363 656e  firstkey : eccen
+00011b60: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00011b70: 7374 797a 5b30 5d20 2a20 7363 616c 655f  styz[0] * scale_
+00011b80: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
+00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bb0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00011bc0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00011bd0: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00011be0: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
+00011bf0: 6528 7b73 656c 662e 6563 6365 6e74 7269  e({self.eccentri
+00011c00: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00011c10: 6b65 7920 3a20 6563 6365 6e74 7269 6369  key : eccentrici
+00011c20: 7479 5f63 6f6d 705f 6669 7273 7479 7a5b  ty_comp_firstyz[
+00011c30: 315d 202a 2073 6361 6c65 5f32 7d29 0d0a  1] * scale_2})..
+00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00011c80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00011c90: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
+00011ca0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00011cb0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+00011cc0: 6b65 7920 3a20 7375 7266 6163 655f 6172  key : surface_ar
+00011cd0: 6561 7d29 0d0a 2020 2020 2020 2020 2020  ea})..          
+00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d00: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00011d10: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00011d20: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00011d30: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+00011d40: 7465 287b 7365 6c66 2e71 7561 6c69 7479  te({self.quality
+00011d50: 5f6b 6579 203a 2071 7561 6c69 7479 7d29  _key : quality})
+00011d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d90: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00011da0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011db0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00011dc0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00011dd0: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
+00011de0: 3a20 7261 6469 7573 207d 290d 0a20 2020  : radius })..   
+00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e10: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e80: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00011e90: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00011ea0: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00011eb0: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
+00011ec0: 6528 7b73 656c 662e 6563 6365 6e74 7269  e({self.eccentri
+00011ed0: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
+00011ee0: 6579 203a 202d 317d 290d 0a20 2020 2020  ey : -1})..     
+00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011f20: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00011f30: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00011f40: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00011f50: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
+00011f60: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00011f70: 7365 636f 6e64 6b65 7920 3a20 2d31 7d29  secondkey : -1})
+00011f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fb0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00011fc0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011fd0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00011fe0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00011ff0: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
+00012000: 615f 6b65 7920 3a20 2d31 7d29 0d0a 2020  a_key : -1})..  
+00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012040: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00012050: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00012060: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00012070: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00012080: 2e71 7561 6c69 7479 5f6b 6579 203a 202d  .quality_key : -
+00012090: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
 000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 2020 2020 6578 7061 6e64 6564 5f74 696d      expanded_tim
-000120c0: 655b 695d 203d 2069 200d 0a20 2020 2020  e[i] = i ..     
-000120d0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-000120e0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-000120f0: 2069 6e20 756e 6971 7565 5f69 6473 5f73   in unique_ids_s
-00012100: 6574 3a0d 0a20 2020 2020 2020 2020 2020  et:..           
-00012110: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00012120: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-00012130: 616e 6465 645f 696e 7465 6e73 6974 7920  anded_intensity 
-00012140: 3d20 6e70 2e7a 6572 6f73 2873 656c 662e  = np.zeros(self.
-00012150: 7465 6e64 202d 2073 656c 662e 7473 7461  tend - self.tsta
-00012160: 7274 202b 2031 290d 0a20 2020 2020 2020  rt + 1)..       
-00012170: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120c0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000120d0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000120e0: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+000120f0: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
+00012100: 6528 7b73 656c 662e 7261 6469 7573 5f6b  e({self.radius_k
+00012110: 6579 203a 202d 3120 7d29 0d0a 2020 2020  ey : -1 })..    
+00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012140: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00012150: 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020 2020  .........       
+00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012170: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012190: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000121a0: 2020 2020 2020 6375 7272 656e 745f 7469        current_ti
-000121b0: 6d65 203d 205b 5d0d 0a20 2020 2020 2020  me = []..       
-000121c0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000121d0: 656e 745f 7a20 3d20 5b5d 0d0a 2020 2020  ent_z = []..    
-000121e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000121f0: 7572 7265 6e74 5f79 203d 205b 5d0d 0a20  urrent_y = [].. 
-00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012210: 2020 6375 7272 656e 745f 7820 3d20 5b5d    current_x = []
-00012220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012230: 2020 2020 2063 7572 7265 6e74 5f69 6e74       current_int
-00012240: 656e 7369 7479 203d 205b 5d0d 0a20 2020  ensity = []..   
-00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012260: 6375 7272 656e 745f 7261 6469 7573 203d  current_radius =
-00012270: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012280: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012290: 766f 6c75 6d65 203d 205b 5d0d 0a20 2020  volume = []..   
-000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122b0: 6375 7272 656e 745f 7370 6565 6420 3d20  current_speed = 
-000122c0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000122d0: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
-000122e0: 6f74 696f 6e5f 616e 676c 6520 3d20 5b5d  otion_angle = []
-000122f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012300: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
-00012310: 656c 6572 6174 696f 6e20 3d20 5b5d 0d0a  eleration = []..
-00012320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012330: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
-00012340: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
-00012350: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012360: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
-00012370: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00012380: 5f66 6972 7374 203d 205b 5d0d 0a20 2020  _first = []..   
-00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123a0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-000123b0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-000123c0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000123d0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000123e0: 745f 7375 7266 6163 655f 6172 6561 203d  t_surface_area =
-000123f0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00012400: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012410: 745f 7261 6469 616c 5f61 6e67 6c65 203d  t_radial_angle =
-00012420: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012430: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012440: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
-00012450: 205b 5d20 0d0a 2020 2020 2020 2020 2020   [] ..          
-00012460: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012470: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00012480: 7220 6a20 696e 2072 616e 6765 2874 696d  r j in range(tim
-00012490: 652e 7368 6170 655b 305d 293a 0d0a 2020  e.shape[0]):..  
-000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124b0: 2020 2020 2020 2020 6966 2063 7572 7265          if curre
-000124c0: 6e74 5f75 6e69 7175 655f 6964 203d 3d20  nt_unique_id == 
-000124d0: 756e 6971 7565 5f69 6473 5b6a 5d3a 0d0a  unique_ids[j]:..
-000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012500: 2063 7572 7265 6e74 5f74 696d 652e 6170   current_time.ap
-00012510: 7065 6e64 2874 696d 655b 6a5d 290d 0a20  pend(time[j]).. 
-00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012540: 6375 7272 656e 745f 7a2e 6170 7065 6e64  current_z.append
-00012550: 285a 5b6a 5d29 0d0a 2020 2020 2020 2020  (Z[j])..        
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012580: 5f79 2e61 7070 656e 6428 595b 6a5d 290d  _y.append(Y[j]).
-00012590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 2020 6375 7272 656e 745f 782e 6170 7065    current_x.appe
-000125c0: 6e64 2858 5b6a 5d29 0d0a 2020 2020 2020  nd(X[j])..      
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 2020 2020 2020 2065 7870 616e             expan
-000125f0: 6465 645f 696e 7465 6e73 6974 795b 696e  ded_intensity[in
-00012600: 7428 7469 6d65 5b6a 5d29 5d20 3d20 696e  t(time[j])] = in
-00012610: 7465 6e73 6974 795b 6a5d 0d0a 2020 2020  tensity[j]..    
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012640: 7265 6e74 5f69 6e74 656e 7369 7479 2e61  rent_intensity.a
-00012650: 7070 656e 6428 696e 7465 6e73 6974 795b  ppend(intensity[
-00012660: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012680: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
-00012690: 6469 7573 2e61 7070 656e 6428 7261 6469  dius.append(radi
-000126a0: 7573 5b6a 5d29 0d0a 2020 2020 2020 2020  us[j])..        
-000126b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126c0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000126d0: 5f76 6f6c 756d 652e 6170 7065 6e64 2876  _volume.append(v
-000126e0: 6f6c 756d 655b 6a5d 290d 0a20 2020 2020  olume[j])..     
-000126f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012700: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012710: 656e 745f 7370 6565 642e 6170 7065 6e64  ent_speed.append
-00012720: 2873 7065 6564 5b6a 5d29 0d0a 2020 2020  (speed[j])..    
-00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012740: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012750: 7265 6e74 5f6d 6f74 696f 6e5f 616e 676c  rent_motion_angl
-00012760: 652e 6170 7065 6e64 286d 6f74 696f 6e5f  e.append(motion_
-00012770: 616e 676c 655b 6a5d 290d 0a20 2020 2020  angle[j])..     
-00012780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012790: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000127a0: 656e 745f 6163 6365 6c65 7261 7469 6f6e  ent_acceleration
-000127b0: 2e61 7070 656e 6428 6163 6365 6c65 7261  .append(accelera
-000127c0: 7469 6f6e 5b6a 5d29 0d0a 2020 2020 2020  tion[j])..      
-000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127e0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000127f0: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
-00012800: 5f6d 6173 6b2e 6170 7065 6e64 2864 6973  _mask.append(dis
-00012810: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5b  tance_cell_mask[
-00012820: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012840: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
-00012850: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00012860: 6669 7273 742e 6170 7065 6e64 2865 6363  first.append(ecc
-00012870: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00012880: 6972 7374 5b6a 5d29 0d0a 2020 2020 2020  irst[j])..      
-00012890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128a0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000128b0: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
-000128c0: 636f 6d70 5f73 6563 6f6e 642e 6170 7065  comp_second.appe
-000128d0: 6e64 2865 6363 656e 7472 6963 6974 795f  nd(eccentricity_
-000128e0: 636f 6d70 5f73 6563 6f6e 645b 6a5d 290d  comp_second[j]).
-000128f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012910: 2020 6375 7272 656e 745f 7375 7266 6163    current_surfac
-00012920: 655f 6172 6561 2e61 7070 656e 6428 7375  e_area.append(su
-00012930: 7266 6163 655f 6172 6561 5b6a 5d29 0d0a  rface_area[j])..
-00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012960: 2063 7572 7265 6e74 5f72 6164 6961 6c5f   current_radial_
-00012970: 616e 676c 652e 6170 7065 6e64 2872 6164  angle.append(rad
-00012980: 6961 6c5f 616e 676c 655b 6a5d 290d 0a20  ial_angle[j]).. 
-00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129b0: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
-000129c0: 735f 6d61 736b 2e61 7070 656e 6428 6365  s_mask.append(ce
-000129d0: 6c6c 5f61 7869 735f 6d61 736b 5b6a 5d29  ll_axis_mask[j])
-000129e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000129f0: 2020 2020 2063 7572 7265 6e74 5f74 696d       current_tim
-00012a00: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
-00012a10: 7572 7265 6e74 5f74 696d 652c 2064 7479  urrent_time, dty
-00012a20: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a40: 2020 2063 7572 7265 6e74 5f69 6e74 656e     current_inten
-00012a50: 7369 7479 203d 206e 702e 6173 6172 7261  sity = np.asarra
-00012a60: 7928 6375 7272 656e 745f 696e 7465 6e73  y(current_intens
-00012a70: 6974 792c 2064 7479 7065 3d6e 702e 666c  ity, dtype=np.fl
-00012a80: 6f61 7433 3229 0d0a 0d0a 0d0a 0d0a 2020  oat32)........  
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 2063 7572 7265 6e74 5f72 6164 6975 7320   current_radius 
-00012ab0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-00012ac0: 7265 6e74 5f72 6164 6975 732c 2064 7479  rent_radius, dty
-00012ad0: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012af0: 2020 2063 7572 7265 6e74 5f76 6f6c 756d     current_volum
-00012b00: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
-00012b10: 7572 7265 6e74 5f76 6f6c 756d 652c 2064  urrent_volume, d
-00012b20: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00012b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012b40: 2020 2020 2063 7572 7265 6e74 5f65 6363       current_ecc
-00012b50: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00012b60: 6972 7374 203d 206e 702e 6173 6172 7261  irst = np.asarra
-00012b70: 7928 6375 7272 656e 745f 6563 6365 6e74  y(current_eccent
-00012b80: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00012b90: 742c 2064 7479 7065 3d6e 702e 666c 6f61  t, dtype=np.floa
-00012ba0: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
-00012bb0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012bc0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00012bd0: 6d70 5f73 6563 6f6e 6420 3d20 6e70 2e61  mp_second = np.a
-00012be0: 7361 7272 6179 2863 7572 7265 6e74 5f65  sarray(current_e
-00012bf0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00012c00: 5f73 6563 6f6e 642c 2064 7479 7065 3d6e  _second, dtype=n
-00012c10: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
-00012c20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012c30: 7572 7265 6e74 5f73 7572 6661 6365 5f61  urrent_surface_a
-00012c40: 7265 6120 3d20 6e70 2e61 7361 7272 6179  rea = np.asarray
-00012c50: 2863 7572 7265 6e74 5f73 7572 6661 6365  (current_surface
-00012c60: 5f61 7265 612c 2064 7479 7065 3d6e 702e  _area, dtype=np.
-00012c70: 666c 6f61 7433 3229 0d0a 0d0a 2020 2020  float32)....    
-00012c80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012c90: 7572 7265 6e74 5f73 7065 6564 203d 206e  urrent_speed = n
-00012ca0: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-00012cb0: 745f 7370 6565 642c 2064 7479 7065 3d6e  t_speed, dtype=n
-00012cc0: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012ce0: 7572 7265 6e74 5f6d 6f74 696f 6e5f 616e  urrent_motion_an
-00012cf0: 676c 6520 3d20 6e70 2e61 7361 7272 6179  gle = np.asarray
-00012d00: 2863 7572 7265 6e74 5f6d 6f74 696f 6e5f  (current_motion_
-00012d10: 616e 676c 652c 2064 7479 7065 3d6e 702e  angle, dtype=np.
-00012d20: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-00012d30: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012d40: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
-00012d50: 6e20 3d20 6e70 2e61 7361 7272 6179 2863  n = np.asarray(c
-00012d60: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
-00012d70: 696f 6e2c 2064 7479 7065 3d6e 702e 666c  ion, dtype=np.fl
-00012d80: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00012d90: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012da0: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
-00012db0: 5f6d 6173 6b20 3d20 6e70 2e61 7361 7272  _mask = np.asarr
-00012dc0: 6179 2863 7572 7265 6e74 5f64 6973 7461  ay(current_dista
-00012dd0: 6e63 655f 6365 6c6c 5f6d 6173 6b2c 2064  nce_cell_mask, d
-00012de0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00012df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012e00: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
-00012e10: 6961 6c5f 616e 676c 6520 3d20 6e70 2e61  ial_angle = np.a
-00012e20: 7361 7272 6179 2863 7572 7265 6e74 5f72  sarray(current_r
-00012e30: 6164 6961 6c5f 616e 676c 652c 2064 7479  adial_angle, dty
-00012e40: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00012e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e60: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00012e70: 6178 6973 5f6d 6173 6b20 3d20 6e70 2e61  axis_mask = np.a
-00012e80: 7361 7272 6179 2863 7572 7265 6e74 5f63  sarray(current_c
-00012e90: 656c 6c5f 6178 6973 5f6d 6173 6b2c 2064  ell_axis_mask, d
-00012ea0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00012eb0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-00012ec0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012ed0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ef0: 2020 2069 6620 706f 696e 745f 7361 6d70     if point_samp
-00012f00: 6c65 203e 2030 3a0d 0a20 2020 2020 2020  le > 0:..       
+00012190: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+000121a0: 2c76 2920 696e 2073 656c 662e 726f 6f74  ,v) in self.root
+000121b0: 5f73 706f 7473 2e69 7465 6d73 2829 3a0d  _spots.items():.
+000121c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121e0: 2020 2073 656c 662e 726f 6f74 5f73 706f     self.root_spo
+000121f0: 7473 5b6b 5d20 3d20 7365 6c66 2e75 6e69  ts[k] = self.uni
+00012200: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00012210: 6965 735b 6b5d 2020 2020 2020 2020 200d  ies[k]         .
+00012220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012230: 200d 0a20 2020 2064 6566 205f 636f 6d70   ..    def _comp
+00012240: 7574 655f 7068 656e 6f74 7970 6573 2873  ute_phenotypes(s
+00012250: 656c 6629 3a0d 0a0d 0a20 2020 2020 2020  elf):....       
+00012260: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+00012270: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
+00012280: 6b73 2e69 7465 6d73 2829 3a0d 0a20 2020  ks.items():..   
+00012290: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000122a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000122b0: 7261 636b 5f69 6420 3d20 6b0d 0a20 2020  rack_id = k..   
+000122c0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000122d0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+000122e0: 203d 2073 656c 662e 756e 6971 7565 5f74   = self.unique_t
+000122f0: 7261 636b 5f70 726f 7065 7274 6965 735b  rack_properties[
+00012300: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
+00012310: 2020 2020 7472 6163 6b73 203d 2073 656c      tracks = sel
+00012320: 662e 756e 6971 7565 5f74 7261 636b 735b  f.unique_tracks[
+00012330: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
+00012340: 2020 2020 5a20 3d20 7472 6163 6b73 5b3a      Z = tracks[:
+00012350: 2c32 5d0d 0a20 2020 2020 2020 2020 2020  ,2]..           
+00012360: 2020 2020 2059 203d 2074 7261 636b 735b       Y = tracks[
+00012370: 3a2c 335d 0d0a 2020 2020 2020 2020 2020  :,3]..          
+00012380: 2020 2020 2020 5820 3d20 7472 6163 6b73        X = tracks
+00012390: 5b3a 2c34 5d0d 0a20 2020 2020 2020 2020  [:,4]..         
+000123a0: 2020 2020 2020 2074 696d 6520 3d20 7472         time = tr
+000123b0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+000123c0: 735b 3a2c 305d 0d0a 2020 2020 2020 2020  s[:,0]..        
+000123d0: 2020 2020 2020 2020 756e 6971 7565 5f69          unique_i
+000123e0: 6473 203d 2074 7261 636b 6c65 745f 7072  ds = tracklet_pr
+000123f0: 6f70 6572 7469 6573 5b3a 2c31 5d0d 0a20  operties[:,1].. 
+00012400: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00012410: 6e69 7175 655f 6964 735f 7365 7420 3d20  nique_ids_set = 
+00012420: 7365 7428 756e 6971 7565 5f69 6473 290d  set(unique_ids).
+00012430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012440: 2067 656e 6572 6174 696f 6e5f 6964 7320   generation_ids 
+00012450: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00012460: 7274 6965 735b 3a2c 325d 0d0a 2020 2020  rties[:,2]..    
+00012470: 2020 2020 2020 2020 2020 2020 7261 6469              radi
+00012480: 7573 203d 2074 7261 636b 6c65 745f 7072  us = tracklet_pr
+00012490: 6f70 6572 7469 6573 5b3a 2c33 5d0d 0a20  operties[:,3].. 
+000124a0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000124b0: 6f6c 756d 6520 3d20 7472 6163 6b6c 6574  olume = tracklet
+000124c0: 5f70 726f 7065 7274 6965 735b 3a2c 345d  _properties[:,4]
+000124d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000124e0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
+000124f0: 6f6d 705f 6669 7273 7420 3d20 7472 6163  omp_first = trac
+00012500: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012510: 3a2c 355d 0d0a 2020 2020 2020 2020 2020  :,5]..          
+00012520: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
+00012530: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
+00012540: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00012550: 7469 6573 5b3a 2c36 5d0d 0a20 2020 2020  ties[:,6]..     
+00012560: 2020 2020 2020 2020 2020 2073 7572 6661             surfa
+00012570: 6365 5f61 7265 6120 3d20 7472 6163 6b6c  ce_area = trackl
+00012580: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00012590: 375d 0d0a 2020 2020 2020 2020 2020 2020  7]..            
+000125a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000125b0: 2020 2020 2069 6e74 656e 7369 7479 203d       intensity =
+000125c0: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+000125d0: 7469 6573 5b3a 2c38 5d0d 0a20 2020 2020  ties[:,8]..     
+000125e0: 2020 2020 2020 2020 2020 2073 7065 6564             speed
+000125f0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00012600: 6572 7469 6573 5b3a 2c39 5d0d 0a20 2020  erties[:,9]..   
+00012610: 2020 2020 2020 2020 2020 2020 206d 6f74               mot
+00012620: 696f 6e5f 616e 676c 6520 3d20 7472 6163  ion_angle = trac
+00012630: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012640: 3a2c 3130 5d0d 0a20 2020 2020 2020 2020  :,10]..         
+00012650: 2020 2020 2020 2061 6363 656c 6572 6174         accelerat
+00012660: 696f 6e20 3d20 7472 6163 6b6c 6574 5f70  ion = tracklet_p
+00012670: 726f 7065 7274 6965 735b 3a2c 3131 5d0d  roperties[:,11].
+00012680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012690: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+000126a0: 6173 6b20 3d20 7472 6163 6b6c 6574 5f70  ask = tracklet_p
+000126b0: 726f 7065 7274 6965 735b 3a2c 3132 5d0d  roperties[:,12].
+000126c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000126d0: 2072 6164 6961 6c5f 616e 676c 6520 3d20   radial_angle = 
+000126e0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+000126f0: 6965 735b 3a2c 3133 5d0d 0a20 2020 2020  ies[:,13]..     
+00012700: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+00012710: 6178 6973 5f6d 6173 6b20 3d20 7472 6163  axis_mask = trac
+00012720: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012730: 3a2c 3134 5d0d 0a0d 0a0d 0a20 2020 2020  :,14]......     
+00012740: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012750: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00012760: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
+00012770: 6573 5f74 7261 636b 6c65 7420 3d20 7b7d  es_tracklet = {}
+00012780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012790: 2020 756e 6971 7565 5f63 6c75 7374 6572    unique_cluster
+000127a0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+000127b0: 6b6c 6574 203d 207b 7d0d 0a20 2020 2020  klet = {}..     
+000127c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000127d0: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
+000127e0: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
+000127f0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00012800: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00012810: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
+00012820: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
+00012830: 207b 7d0d 0a0d 0a20 2020 2020 2020 2020   {}....         
+00012840: 2020 2020 2020 2075 6e69 7175 655f 7368         unique_sh
+00012850: 6170 655f 7072 6f70 6572 7469 6573 5f74  ape_properties_t
+00012860: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
+00012870: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00012880: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
+00012890: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+000128a0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+000128b0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000128c0: 7565 5f73 6861 7065 5f70 726f 7065 7274  ue_shape_propert
+000128d0: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
+000128e0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+000128f0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00012900: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
+00012910: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
+00012920: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00012930: 2020 2065 7870 616e 6465 645f 7469 6d65     expanded_time
+00012940: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
+00012950: 2e74 656e 6420 2d20 7365 6c66 2e74 7374  .tend - self.tst
+00012960: 6172 7420 2b20 3129 0d0a 2020 2020 2020  art + 1)..      
+00012970: 2020 2020 2020 2020 2020 706f 696e 745f            point_
+00012980: 7361 6d70 6c65 203d 2065 7870 616e 6465  sample = expande
+00012990: 645f 7469 6d65 2e73 6861 7065 5b30 5d0d  d_time.shape[0].
+000129a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000129b0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000129c0: 6c65 6e28 6578 7061 6e64 6564 5f74 696d  len(expanded_tim
+000129d0: 6529 293a 0d0a 2020 2020 2020 2020 2020  e)):..          
+000129e0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+000129f0: 616e 6465 645f 7469 6d65 5b69 5d20 3d20  anded_time[i] = 
+00012a00: 6920 0d0a 2020 2020 2020 2020 2020 2020  i ..            
+00012a10: 2020 2020 666f 7220 6375 7272 656e 745f      for current_
+00012a20: 756e 6971 7565 5f69 6420 696e 2075 6e69  unique_id in uni
+00012a30: 7175 655f 6964 735f 7365 743a 0d0a 2020  que_ids_set:..  
+00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012a60: 2020 2020 2020 6578 7061 6e64 6564 5f69        expanded_i
+00012a70: 6e74 656e 7369 7479 203d 206e 702e 7a65  ntensity = np.ze
+00012a80: 726f 7328 7365 6c66 2e74 656e 6420 2d20  ros(self.tend - 
+00012a90: 7365 6c66 2e74 7374 6172 7420 2b20 3129  self.tstart + 1)
+00012aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012ab0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00012ac0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012ae0: 7572 7265 6e74 5f74 696d 6520 3d20 5b5d  urrent_time = []
+00012af0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012b00: 2020 2020 2063 7572 7265 6e74 5f7a 203d       current_z =
+00012b10: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00012b20: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012b30: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00012b40: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012b50: 6e74 5f78 203d 205b 5d0d 0a20 2020 2020  nt_x = []..     
+00012b60: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012b70: 7272 656e 745f 696e 7465 6e73 6974 7920  rrent_intensity 
+00012b80: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012b90: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012ba0: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bc0: 2063 7572 7265 6e74 5f76 6f6c 756d 6520   current_volume 
+00012bd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012be0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012bf0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c10: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
+00012c20: 6e67 6c65 203d 205b 5d0d 0a20 2020 2020  ngle = []..     
+00012c30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012c40: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
+00012c50: 6f6e 203d 205b 5d0d 0a20 2020 2020 2020  on = []..       
+00012c60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012c70: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00012c80: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
+00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ca0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+00012cb0: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
+00012cc0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012cd0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012ce0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00012cf0: 6d70 5f73 6563 6f6e 6420 3d20 5b5d 0d0a  mp_second = []..
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
+00012d20: 6365 5f61 7265 6120 3d20 5b5d 0d0a 0d0a  ce_area = []....
+00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d40: 2020 2063 7572 7265 6e74 5f72 6164 6961     current_radia
+00012d50: 6c5f 616e 676c 6520 3d20 5b5d 0d0a 2020  l_angle = []..  
+00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d70: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
+00012d80: 6973 5f6d 6173 6b20 3d20 5b5d 200d 0a20  is_mask = [] .. 
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00012db0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00012dc0: 7261 6e67 6528 7469 6d65 2e73 6861 7065  range(time.shape
+00012dd0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
+00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012df0: 2069 6620 6375 7272 656e 745f 756e 6971   if current_uniq
+00012e00: 7565 5f69 6420 3d3d 2075 6e69 7175 655f  ue_id == unique_
+00012e10: 6964 735b 6a5d 3a0d 0a20 2020 2020 2020  ids[j]:..       
+00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012e40: 745f 7469 6d65 2e61 7070 656e 6428 7469  t_time.append(ti
+00012e50: 6d65 5b6a 5d29 0d0a 2020 2020 2020 2020  me[j])..        
+00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e70: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012e80: 5f7a 2e61 7070 656e 6428 5a5b 6a5d 290d  _z.append(Z[j]).
+00012e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012eb0: 2020 6375 7272 656e 745f 792e 6170 7065    current_y.appe
+00012ec0: 6e64 2859 5b6a 5d29 0d0a 2020 2020 2020  nd(Y[j])..      
+00012ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ee0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012ef0: 6e74 5f78 2e61 7070 656e 6428 585b 6a5d  nt_x.append(X[j]
+00012f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 2020 2020 2020 2020 2078 665f 7361 6d70           xf_samp
-00012f30: 6c65 203d 2066 6674 6672 6571 2870 6f69  le = fftfreq(poi
-00012f40: 6e74 5f73 616d 706c 652c 2073 656c 662e  nt_sample, self.
-00012f50: 7463 616c 6962 7261 7469 6f6e 290d 0a20  tcalibration).. 
+00012f20: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
+00012f30: 656e 7369 7479 5b69 6e74 2874 696d 655b  ensity[int(time[
+00012f40: 6a5d 295d 203d 2069 6e74 656e 7369 7479  j])] = intensity
+00012f50: 5b6a 5d0d 0a20 2020 2020 2020 2020 2020  [j]..           
 00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012f80: 6674 7374 7269 705f 7361 6d70 6c65 203d  ftstrip_sample =
-00012f90: 2066 6674 2865 7870 616e 6465 645f 696e   fft(expanded_in
-00012fa0: 7465 6e73 6974 7929 0d0a 2020 2020 2020  tensity)..      
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fc0: 2020 2020 2020 2020 2020 6666 7474 6f74            ffttot
-00012fd0: 616c 5f73 616d 706c 6520 3d20 6e70 2e61  al_sample = np.a
-00012fe0: 6273 2866 6674 7374 7269 705f 7361 6d70  bs(fftstrip_samp
-00012ff0: 6c65 290d 0a20 2020 2020 2020 2020 2020  le)..           
-00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013010: 2020 2020 2078 665f 7361 6d70 6c65 203d       xf_sample =
-00013020: 2078 665f 7361 6d70 6c65 5b30 203a 206c   xf_sample[0 : l
-00013030: 656e 2878 665f 7361 6d70 6c65 2920 2f2f  en(xf_sample) //
-00013040: 2032 5d0d 0a20 2020 2020 2020 2020 2020   2]..           
-00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013060: 2020 2020 2066 6674 746f 7461 6c5f 7361       ffttotal_sa
-00013070: 6d70 6c65 203d 2066 6674 746f 7461 6c5f  mple = ffttotal_
-00013080: 7361 6d70 6c65 5b30 203a 206c 656e 2866  sample[0 : len(f
-00013090: 6674 746f 7461 6c5f 7361 6d70 6c65 2920  fttotal_sample) 
-000130a0: 2f2f 2032 5d0d 0a0d 0a20 2020 2020 2020  // 2]....       
-000130b0: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-000130c0: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
-000130d0: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
-000130e0: 6e74 5f75 6e69 7175 655f 6964 5d20 3d20  nt_unique_id] = 
-000130f0: 6578 7061 6e64 6564 5f74 696d 652c 2065  expanded_time, e
-00013100: 7870 616e 6465 645f 696e 7465 6e73 6974  xpanded_intensit
-00013110: 792c 2078 665f 7361 6d70 6c65 2c20 6666  y, xf_sample, ff
-00013120: 7474 6f74 616c 5f73 616d 706c 650d 0a20  ttotal_sample.. 
-00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013140: 2020 756e 6971 7565 5f63 6c75 7374 6572    unique_cluster
-00013150: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013160: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00013170: 7175 655f 6964 5d20 3d20 2063 7572 7265  que_id] =  curre
-00013180: 6e74 5f74 696d 650d 0a20 2020 2020 2020  nt_time..       
-00013190: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-000131a0: 7565 5f73 6861 7065 5f70 726f 7065 7274  ue_shape_propert
-000131b0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
-000131c0: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
-000131d0: 3d20 6375 7272 656e 745f 7469 6d65 2c20  = current_time, 
-000131e0: 6375 7272 656e 745f 7a2c 2063 7572 7265  current_z, curre
-000131f0: 6e74 5f79 2c20 6375 7272 656e 745f 782c  nt_y, current_x,
-00013200: 2063 7572 7265 6e74 5f72 6164 6975 732c   current_radius,
-00013210: 2063 7572 7265 6e74 5f76 6f6c 756d 652c   current_volume,
-00013220: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
-00013230: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00013240: 2c20 6375 7272 656e 745f 6563 6365 6e74  , current_eccent
-00013250: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00013260: 6e64 2c20 6375 7272 656e 745f 7375 7266  nd, current_surf
-00013270: 6163 655f 6172 6561 0d0a 2020 2020 2020  ace_area..      
-00013280: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-00013290: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
-000132a0: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
-000132b0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-000132c0: 645d 203d 2063 7572 7265 6e74 5f74 696d  d] = current_tim
-000132d0: 652c 2063 7572 7265 6e74 5f73 7065 6564  e, current_speed
-000132e0: 2c20 6375 7272 656e 745f 6d6f 7469 6f6e  , current_motion
-000132f0: 5f61 6e67 6c65 2c20 6375 7272 656e 745f  _angle, current_
-00013300: 6163 6365 6c65 7261 7469 6f6e 2c20 6375  acceleration, cu
-00013310: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
-00013320: 656c 6c5f 6d61 736b 2c20 6375 7272 656e  ell_mask, curren
-00013330: 745f 7261 6469 616c 5f61 6e67 6c65 2c20  t_radial_angle, 
-00013340: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
-00013350: 735f 6d61 736b 0d0a 2020 2020 2020 2020  s_mask..        
-00013360: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013370: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
-00013380: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
-00013390: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
-000133a0: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
-000133b0: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
-000133c0: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-000133d0: 5f75 6e69 7175 655f 6964 5d7d 290d 0a20  _unique_id]}).. 
-000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133f0: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
-00013400: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
-00013410: 5b74 7261 636b 5f69 645d 2e75 7064 6174  [track_id].updat
-00013420: 6528 7b63 7572 7265 6e74 5f75 6e69 7175  e({current_uniqu
-00013430: 655f 6964 3a75 6e69 7175 655f 636c 7573  e_id:unique_clus
-00013440: 7465 725f 7072 6f70 6572 7469 6573 5f74  ter_properties_t
-00013450: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
-00013460: 756e 6971 7565 5f69 645d 7d29 0d0a 0d0a  unique_id]})....
-00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013480: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00013490: 6861 7065 5f70 726f 7065 7274 6965 735b  hape_properties[
-000134a0: 7472 6163 6b5f 6964 5d2e 7570 6461 7465  track_id].update
-000134b0: 287b 6375 7272 656e 745f 756e 6971 7565  ({current_unique
-000134c0: 5f69 643a 756e 6971 7565 5f73 6861 7065  _id:unique_shape
-000134d0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-000134e0: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-000134f0: 7175 655f 6964 5d7d 290d 0a20 2020 2020  que_id]})..     
-00013500: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013510: 6c66 2e75 6e69 7175 655f 6479 6e61 6d69  lf.unique_dynami
-00013520: 635f 7072 6f70 6572 7469 6573 5b74 7261  c_properties[tra
-00013530: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
-00013540: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00013550: 3a75 6e69 7175 655f 6479 6e61 6d69 635f  :unique_dynamic_
-00013560: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00013570: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-00013580: 7565 5f69 645d 7d29 0d0a 0d0a 2020 2020  ue_id]})....    
-00013590: 6465 6620 5f73 6563 6f6e 645f 6368 616e  def _second_chan
-000135a0: 6e65 6c5f 7370 6f74 7328 7365 6c66 2c20  nel_spots(self, 
-000135b0: 6672 616d 652c 207a 2c20 792c 2078 2c20  frame, z, y, x, 
-000135c0: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
-000135d0: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
-000135e0: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-000135f0: 6565 2c20 6365 6e74 726f 6964 732c 206c  ee, centroids, l
-00013600: 6162 656c 732c 2076 6f6c 756d 652c 2069  abels, volume, i
-00013610: 6e74 656e 7369 7479 5f6d 6561 6e2c 2069  ntensity_mean, i
-00013620: 6e74 656e 7369 7479 5f74 6f74 616c 2c20  ntensity_total, 
-00013630: 626f 756e 6469 6e67 5f62 6f78 6573 203d  bounding_boxes =
-00013640: 2073 656c 662e 5f74 696d 6564 5f63 6861   self._timed_cha
-00013650: 6e6e 656c 5f73 6567 5f69 6d61 6765 5b73  nnel_seg_image[s
-00013660: 7472 2869 6e74 2866 6c6f 6174 2866 7261  tr(int(float(fra
-00013670: 6d65 2929 295d 0d0a 2020 2020 2020 2020  me)))]..        
-00013680: 2020 2020 7069 7865 6c74 6573 746c 6f63      pixeltestloc
-00013690: 6174 696f 6e20 3d20 287a 2c79 2c78 290d  ation = (z,y,x).
-000136a0: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-000136b0: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
-000136c0: 7175 6572 7928 7069 7865 6c74 6573 746c  query(pixeltestl
-000136d0: 6f63 6174 696f 6e29 0d0a 0d0a 0d0a 2020  ocation)......  
-000136e0: 2020 2020 2020 2020 2020 6262 6f78 203d            bbox =
-000136f0: 2062 6f75 6e64 696e 675f 626f 7865 735b   bounding_boxes[
-00013700: 696e 6465 785d 0d0a 2020 2020 2020 2020  index]..        
-00013710: 2020 2020 7369 7a65 7a20 3d20 6162 7328      sizez = abs(
-00013720: 6262 6f78 5b30 5d20 2d20 6262 6f78 5b33  bbox[0] - bbox[3
-00013730: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00013740: 7369 7a65 7920 3d20 6162 7328 6262 6f78  sizey = abs(bbox
-00013750: 5b31 5d20 2d20 6262 6f78 5b34 5d29 0d0a  [1] - bbox[4])..
-00013760: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00013770: 7820 3d20 6162 7328 6262 6f78 5b32 5d20  x = abs(bbox[2] 
-00013780: 2d20 6262 6f78 5b35 5d29 200d 0a20 2020  - bbox[5]) ..   
-00013790: 2020 2020 2020 2020 2076 6574 6f5f 766f           veto_vo
-000137a0: 6c75 6d65 203d 2073 697a 6578 202a 2073  lume = sizex * s
-000137b0: 697a 6579 202a 2073 697a 657a 0d0a 2020  izey * sizez..  
-000137c0: 2020 2020 2020 2020 2020 7665 746f 5f72            veto_r
-000137d0: 6164 6975 7320 3d20 6d61 7468 2e70 6f77  adius = math.pow
-000137e0: 2833 202a 2076 6574 6f5f 766f 6c75 6d65  (3 * veto_volume
-000137f0: 202f 2028 3420 2a20 6d61 7468 2e70 6929   / (4 * math.pi)
-00013800: 2c20 312e 3020 2f20 332e 3029 0d0a 0d0a  , 1.0 / 3.0)....
-00013810: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00013820: 7469 6f6e 203d 2028 6365 6e74 726f 6964  tion = (centroid
-00013830: 735b 696e 6465 785d 5b30 5d20 2a20 7365  s[index][0] * se
-00013840: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-00013850: 2063 656e 7472 6f69 6473 5b69 6e64 6578   centroids[index
-00013860: 5d5b 315d 2a73 656c 662e 7963 616c 6962  ][1]*self.ycalib
-00013870: 7261 7469 6f6e 2c20 6365 6e74 726f 6964  ration, centroid
-00013880: 735b 696e 6465 785d 5b32 5d2a 7365 6c66  s[index][2]*self
-00013890: 2e78 6361 6c69 6272 6174 696f 6e29 0d0a  .xcalibration)..
-000138a0: 2020 2020 2020 2020 2020 2020 5155 414c              QUAL
-000138b0: 4954 5920 3d20 6d61 7468 2e70 6f77 2876  ITY = math.pow(v
-000138c0: 6f6c 756d 655b 696e 6465 785d 2c20 312e  olume[index], 1.
-000138d0: 302f 332e 3029 0d0a 2020 2020 2020 2020  0/3.0)..        
-000138e0: 2020 2020 5241 4449 5553 203d 206d 6174      RADIUS = mat
-000138f0: 682e 706f 7728 766f 6c75 6d65 5b69 6e64  h.pow(volume[ind
-00013900: 6578 5d20 2a20 7365 6c66 2e78 6361 6c69  ex] * self.xcali
-00013910: 6272 6174 696f 6e20 2a20 7365 6c66 2e79  bration * self.y
-00013920: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
-00013930: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-00013940: 2031 2e30 2f33 2e30 2920 0d0a 0d0a 2020   1.0/3.0) ....  
-00013950: 2020 2020 2020 2020 2020 6469 7374 616e            distan
-00013960: 6365 5f63 656c 6c5f 6d61 736b 2c20 6d61  ce_cell_mask, ma
-00013970: 736b 6365 6e74 726f 6964 203d 2073 656c  skcentroid = sel
-00013980: 662e 5f67 6574 5f62 6f75 6e64 6172 795f  f._get_boundary_
-00013990: 6469 7374 2866 7261 6d65 2c20 6c6f 6361  dist(frame, loca
-000139a0: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-000139b0: 2020 2069 6620 6469 7374 203c 3d20 3220     if dist <= 2 
-000139c0: 2a20 7665 746f 5f72 6164 6975 733a 0d0a  * veto_radius:..
-000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139e0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-000139f0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00013a00: 6965 735b 6365 6c6c 5f69 645d 203d 207b  ies[cell_id] = {
-00013a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013a20: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00013a30: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
-00013a40: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
-00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a60: 2020 2073 656c 662e 6672 616d 6569 645f     self.frameid_
-00013a70: 6b65 7920 3a20 696e 7428 6672 616d 6529  key : int(frame)
-00013a80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00013a90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013aa0: 7a70 6f73 6964 5f6b 6579 203a 2066 6c6f  zposid_key : flo
-00013ab0: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
-00013ac0: 6578 5d5b 305d 2a20 7365 6c66 2e7a 6361  ex][0]* self.zca
-00013ad0: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
-00013ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013af0: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
-00013b00: 5f6b 6579 203a 2066 6c6f 6174 2863 656e  _key : float(cen
-00013b10: 7472 6f69 6473 5b69 6e64 6578 5d5b 315d  troids[index][1]
-00013b20: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
-00013b30: 696f 6e29 2c0d 0a20 2020 2020 2020 2020  ion),..         
-00013b40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013b50: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
-00013b60: 2066 6c6f 6174 2863 656e 7472 6f69 6473   float(centroids
-00013b70: 5b69 6e64 6578 5d5b 325d 2a20 7365 6c66  [index][2]* self
-00013b80: 2e78 6361 6c69 6272 6174 696f 6e29 2c0d  .xcalibration),.
-00013b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ba0: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-00013bb0: 6163 6b69 645f 6b65 793a 2069 6e74 2874  ackid_key: int(t
-00013bc0: 7261 636b 5f69 6429 2c0d 0a20 2020 2020  rack_id),..     
-00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013be0: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
-00013bf0: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
-00013c00: 6c6f 6174 2869 6e74 656e 7369 7479 5f74  loat(intensity_t
-00013c10: 6f74 616c 5b69 6e64 6578 5d29 292c 0d0a  otal[index])),..
-00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c30: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
-00013c40: 6e5f 696e 7465 6e73 6974 795f 6b65 7920  n_intensity_key 
-00013c50: 3a20 2866 6c6f 6174 2869 6e74 656e 7369  : (float(intensi
-00013c60: 7479 5f6d 6561 6e5b 696e 6465 785d 2929  ty_mean[index]))
-00013c70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00013c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013c90: 7261 6469 7573 5f6b 6579 203a 2028 666c  radius_key : (fl
-00013ca0: 6f61 7428 5241 4449 5553 2929 2c0d 0a20  oat(RADIUS)),.. 
-00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cc0: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
-00013cd0: 6974 795f 6b65 7920 3a20 2866 6c6f 6174  ity_key : (float
-00013ce0: 2851 5541 4c49 5459 2929 2c0d 0a20 2020  (QUALITY)),..   
-00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d00: 2020 2020 2073 656c 662e 6469 7374 616e       self.distan
-00013d10: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-00013d20: 3a20 666c 6f61 7428 6469 7374 616e 6365  : float(distance
-00013d30: 5f63 656c 6c5f 6d61 736b 292c 0d0a 2020  _cell_mask),..  
-00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d50: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
-00013d60: 656e 7472 6f69 645f 7a5f 6b65 793a 2066  entroid_z_key: f
-00013d70: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
-00013d80: 645b 305d 292c 0d0a 2020 2020 2020 2020  d[0]),..        
-00013d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013da0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-00013db0: 645f 795f 6b65 793a 2066 6c6f 6174 286d  d_y_key: float(m
-00013dc0: 6173 6b63 656e 7472 6f69 645b 315d 292c  askcentroid[1]),
-00013dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013de0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00013df0: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
-00013e00: 793a 2066 6c6f 6174 286d 6173 6b63 656e  y: float(maskcen
-00013e10: 7472 6f69 645b 325d 2920 0d0a 0d0a 2020  troid[2]) ....  
-00013e20: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-00013e30: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00013e40: 6620 6365 6c6c 5f69 6420 696e 2073 656c  f cell_id in sel
-00013e50: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
-00013e60: 6f6b 7570 2e6b 6579 7328 293a 0d0a 2020  okup.keys():..  
-00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00013e90: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00013ea0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-00013eb0: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-00013ec0: 5f69 645d 203d 2073 656c 662e 756e 6971  _id] = self.uniq
-00013ed0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00013ee0: 6573 5b63 656c 6c5f 6964 5d0d 0a20 2020  es[cell_id]..   
-00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f00: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-00013f10: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00013f20: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
-00013f30: 6461 7465 287b 7365 6c66 2e74 6f74 616c  date({self.total
-00013f40: 5f69 6e74 656e 7369 7479 5f6b 6579 3a20  _intensity_key: 
-00013f50: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
-00013f60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00013f70: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-00013f80: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-00013f90: 6c6c 5f69 645d 2e75 7064 6174 6528 7b73  ll_id].update({s
-00013fa0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-00013fb0: 7479 5f6b 6579 3a20 2d31 7d29 0d0a 2020  ty_key: -1})..  
-00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fd0: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
-00013fe0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00013ff0: 7274 6965 735b 6365 6c6c 5f69 645d 2e75  rties[cell_id].u
-00014000: 7064 6174 6528 7b73 656c 662e 7261 6469  pdate({self.radi
-00014010: 7573 5f6b 6579 3a20 2d31 7d29 0d0a 2020  us_key: -1})..  
-00014020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014030: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
-00014040: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014050: 7274 6965 735b 6365 6c6c 5f69 645d 2e75  rties[cell_id].u
-00014060: 7064 6174 6528 7b73 656c 662e 7175 616c  pdate({self.qual
-00014070: 6974 795f 6b65 793a 202d 317d 290d 0a0d  ity_key: -1})...
-00014080: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140a0: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-000140b0: 5f64 6963 745f 7570 6461 7465 2873 656c  _dict_update(sel
-000140c0: 662c 2075 6e69 7175 655f 7472 6163 6b6c  f, unique_trackl
-000140d0: 6574 5f69 6473 3a20 4c69 7374 2c20 2063  et_ids: List,  c
-000140e0: 656c 6c5f 6964 3a20 696e 742c 2074 7261  ell_id: int, tra
-000140f0: 636b 5f69 643a 2069 6e74 2c20 736f 7572  ck_id: int, sour
-00014100: 6365 5f69 643a 2069 6e74 2c20 7461 7267  ce_id: int, targ
-00014110: 6574 5f69 643a 2069 6e74 293a 0d0a 0d0a  et_id: int):....
-00014120: 200d 0a20 2020 2020 2020 2067 656e 6572   ..        gener
-00014130: 6174 696f 6e5f 6964 203d 2073 656c 662e  ation_id = self.
-00014140: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
-00014150: 6365 6c6c 5f69 645d 0d0a 2020 2020 2020  cell_id]..      
-00014160: 2020 7472 6163 6b6c 6574 5f69 6420 3d20    tracklet_id = 
-00014170: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
-00014180: 6374 5b63 656c 6c5f 6964 5d0d 0a0d 0a20  ct[cell_id].... 
-00014190: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
-000141a0: 203d 2073 7472 2874 7261 636b 5f69 6429   = str(track_id)
-000141b0: 202b 2020 7374 7228 6765 6e65 7261 7469   +  str(generati
-000141c0: 6f6e 5f69 6429 202b 2073 7472 2874 7261  on_id) + str(tra
-000141d0: 636b 6c65 745f 6964 290d 0a20 2020 2020  cklet_id)..     
-000141e0: 2020 200d 0a20 2020 2020 2020 2076 6563     ..        vec
-000141f0: 5f6d 6173 6b20 3d20 5b66 6c6f 6174 2873  _mask = [float(s
-00014200: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014210: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014220: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-00014230: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-00014240: 5d29 2c20 666c 6f61 7428 7365 6c66 2e75  ]), float(self.u
-00014250: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014260: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014270: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
-00014280: 7472 6f69 645f 795f 6b65 795d 292c 2066  troid_y_key]), f
-00014290: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-000142a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000142b0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-000142c0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-000142d0: 5f7a 5f6b 6579 5d29 205d 0d0a 0d0a 2020  _z_key]) ]....  
-000142e0: 2020 2020 2020 7665 635f 6365 6c6c 203d        vec_cell =
-000142f0: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
-00014300: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014310: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014320: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-00014330: 795d 2920 2c20 0d0a 2020 2020 2020 2020  y]) , ..        
-00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014350: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-00014360: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014370: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014380: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
-00014390: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
-000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143b0: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
-000143c0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000143d0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000143e0: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-000143f0: 5f6b 6579 5d29 5d0d 0a0d 0a20 2020 2020  _key])]....     
-00014400: 2020 2061 6e67 6c65 203d 2061 6e67 756c     angle = angul
-00014410: 6172 5f63 6861 6e67 6528 7665 635f 6d61  ar_change(vec_ma
-00014420: 736b 2c20 7665 635f 6365 6c6c 290d 0a0d  sk, vec_cell)...
-00014430: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00014440: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014450: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014460: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014470: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
-00014480: 203a 2061 6e67 6c65 7d29 2020 2020 2020   : angle})      
-00014490: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000144a0: 0d0a 2020 2020 2020 2020 756e 6971 7565  ..        unique
-000144b0: 5f74 7261 636b 6c65 745f 6964 732e 6170  _tracklet_ids.ap
-000144c0: 7065 6e64 2873 7472 2875 6e69 7175 655f  pend(str(unique_
-000144d0: 6964 2929 0d0a 2020 2020 2020 2020 7365  id))..        se
-000144e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000144f0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014500: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00014510: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
-00014520: 7920 3a20 7374 7228 756e 6971 7565 5f69  y : str(unique_i
-00014530: 6429 7d29 0d0a 2020 2020 2020 2020 7365  d)})..        se
-00014540: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014550: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014560: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00014570: 7365 6c66 2e74 7261 636b 6c65 7469 645f  self.trackletid_
-00014580: 6b65 7920 3a20 7374 7228 7472 6163 6b6c  key : str(trackl
-00014590: 6574 5f69 6429 7d29 200d 0a20 2020 2020  et_id)}) ..     
-000145a0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000145b0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000145c0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-000145d0: 6174 6528 7b73 656c 662e 6765 6e65 7261  ate({self.genera
-000145e0: 7469 6f6e 6964 5f6b 6579 203a 2073 7472  tionid_key : str
-000145f0: 2867 656e 6572 6174 696f 6e5f 6964 297d  (generation_id)}
-00014600: 2920 0d0a 2020 2020 2020 2020 7365 6c66  ) ..        self
-00014610: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014620: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014630: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00014640: 6c66 2e74 7261 636b 6964 5f6b 6579 203a  lf.trackid_key :
-00014650: 2073 7472 2874 7261 636b 5f69 6429 7d29   str(track_id)})
-00014660: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00014670: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014680: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014690: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-000146a0: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
-000146b0: 7920 3a20 302e 307d 290d 0a20 2020 2020  y : 0.0})..     
-000146c0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000146d0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000146e0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-000146f0: 6174 6528 7b73 656c 662e 7370 6565 645f  ate({self.speed_
-00014700: 6b65 7920 3a20 302e 307d 290d 0a20 2020  key : 0.0})..   
-00014710: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00014720: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014730: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00014740: 7064 6174 6528 7b73 656c 662e 6163 6365  pdate({self.acce
-00014750: 6c65 7261 7469 6f6e 5f6b 6579 203a 2030  leration_key : 0
-00014760: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
-00014770: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014780: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014790: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-000147a0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-000147b0: 795f 636f 6d70 5f66 6972 7374 6b65 7920  y_comp_firstkey 
-000147c0: 3a20 2d31 7d29 0d0a 2020 2020 2020 2020  : -1})..        
-000147d0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000147e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000147f0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00014800: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
-00014810: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
-00014820: 6579 203a 202d 317d 290d 0a20 2020 2020  ey : -1})..     
-00014830: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00014840: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014850: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00014860: 6174 6528 7b73 656c 662e 7375 7266 6163  ate({self.surfac
-00014870: 655f 6172 6561 5f6b 6579 203a 202d 317d  e_area_key : -1}
-00014880: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00014890: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000148a0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000148b0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000148c0: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
-000148d0: 6b65 7920 3a20 2d31 7d29 0d0a 0d0a 2020  key : -1})....  
-000148e0: 2020 2020 2020 6966 2073 6f75 7263 655f        if source_
-000148f0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0d  id is not None:.
-00014900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014910: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014920: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014930: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014940: 656c 662e 6265 666f 7265 6964 5f6b 6579  elf.beforeid_key
-00014950: 203a 2069 6e74 2873 6f75 7263 655f 6964   : int(source_id
-00014960: 297d 290d 0a20 2020 2020 2020 2020 2020  )})..           
-00014970: 2076 6563 5f31 203d 205b 666c 6f61 7428   vec_1 = [float(
-00014980: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014990: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000149a0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-000149b0: 706f 7369 645f 6b65 795d 2920 2d20 666c  posid_key]) - fl
-000149c0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000149d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000149e0: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
-000149f0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-00014a00: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
-00014a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a20: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00014a30: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014a40: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014a50: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-00014a60: 5d29 202d 2066 6c6f 6174 2873 656c 662e  ]) - float(self.
-00014a70: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014a80: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00014a90: 655f 6964 295d 5b73 656c 662e 7970 6f73  e_id)][self.ypos
-00014aa0: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
-00014ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ac0: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-00014ad0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014ae0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014af0: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
-00014b00: 7369 645f 6b65 795d 2920 2d20 2066 6c6f  sid_key]) -  flo
-00014b10: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014b20: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014b30: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-00014b40: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00014b50: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-00014b60: 7065 6564 203d 206e 702e 7371 7274 286e  peed = np.sqrt(n
-00014b70: 702e 646f 7428 7665 635f 312c 2076 6563  p.dot(vec_1, vec
-00014b80: 5f31 2929 2f73 656c 662e 7463 616c 6962  _1))/self.tcalib
-00014b90: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00014ba0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00014bb0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014bc0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00014bd0: 6461 7465 287b 7365 6c66 2e73 7065 6564  date({self.speed
-00014be0: 5f6b 6579 203a 2073 7065 6564 7d29 0d0a  _key : speed})..
-00014bf0: 0d0a 2020 2020 2020 2020 2020 2020 6d6f  ..            mo
-00014c00: 7469 6f6e 5f61 6e67 6c65 203d 2061 6e67  tion_angle = ang
-00014c10: 756c 6172 5f63 6861 6e67 6528 7665 635f  ular_change(vec_
-00014c20: 6d61 736b 2c20 7665 635f 3129 0d0a 0d0a  mask, vec_1)....
-00014c30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014c40: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014c50: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014c60: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00014c70: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
-00014c80: 6b65 7920 3a20 6d6f 7469 6f6e 5f61 6e67  key : motion_ang
-00014c90: 6c65 7d29 200d 0a0d 0a20 2020 2020 2020  le}) ....       
-00014ca0: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
-00014cb0: 6420 696e 2073 656c 662e 6564 6765 5f73  d in self.edge_s
-00014cc0: 6f75 7263 655f 6c6f 6f6b 7570 3a0d 0a20  ource_lookup:.. 
-00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ce0: 2020 2070 7265 5f73 6f75 7263 655f 6964     pre_source_id
-00014cf0: 203d 2073 656c 662e 6564 6765 5f73 6f75   = self.edge_sou
-00014d00: 7263 655f 6c6f 6f6b 7570 5b73 6f75 7263  rce_lookup[sourc
-00014d10: 655f 6964 5d0d 0a20 2020 2020 2020 2020  e_id]..         
-00014d20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d40: 2076 6563 5f32 203d 205b 666c 6f61 7428   vec_2 = [float(
-00014d50: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014d60: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014d70: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-00014d80: 706f 7369 645f 6b65 795d 2920 2d20 3220  posid_key]) - 2 
-00014d90: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
-00014da0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014db0: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
-00014dc0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
-00014dd0: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
-00014de0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014df0: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
-00014e00: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
-00014e10: 6c66 2e78 706f 7369 645f 6b65 795d 292c  lf.xposid_key]),
-00014e20: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00014e30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00014e40: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00014e50: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014e60: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00014e70: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00014e80: 202d 2032 202a 2066 6c6f 6174 2873 656c   - 2 * float(sel
-00014e90: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014ea0: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
-00014eb0: 7263 655f 6964 295d 5b73 656c 662e 7970  rce_id)][self.yp
-00014ec0: 6f73 6964 5f6b 6579 5d29 202b 2066 6c6f  osid_key]) + flo
-00014ed0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014ee0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014ef0: 6e74 2870 7265 5f73 6f75 7263 655f 6964  nt(pre_source_id
-00014f00: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
-00014f10: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
-00014f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f30: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-00014f40: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014f50: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014f60: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
-00014f70: 6b65 795d 2920 2d20 2032 202a 2066 6c6f  key]) -  2 * flo
-00014f80: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014f90: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014fa0: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-00014fb0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00014fc0: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
-00014fd0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014fe0: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
-00014ff0: 7263 655f 6964 295d 5b73 656c 662e 7a70  rce_id)][self.zp
-00015000: 6f73 6964 5f6b 6579 5d29 5d0d 0a20 2020  osid_key])]..   
-00015010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015020: 2061 6363 203d 206e 702e 7371 7274 286e   acc = np.sqrt(n
-00015030: 702e 646f 7428 7665 635f 322c 2076 6563  p.dot(vec_2, vec
-00015040: 5f32 2929 2f73 656c 662e 7463 616c 6962  _2))/self.tcalib
-00015050: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00015060: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015080: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00015090: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000150a0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-000150b0: 7465 287b 7365 6c66 2e61 6363 656c 6572  te({self.acceler
-000150c0: 6174 696f 6e5f 6b65 7920 3a20 6163 637d  ation_key : acc}
-000150d0: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-000150e0: 736f 7572 6365 5f69 6420 6973 204e 6f6e  source_id is Non
-000150f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00015100: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015110: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015120: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00015130: 287b 7365 6c66 2e62 6566 6f72 6569 645f  ({self.beforeid_
-00015140: 6b65 7920 3a20 4e6f 6e65 7d29 200d 0a20  key : None}) .. 
-00015150: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-00015160: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00015170: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00015180: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00015190: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000151a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000151b0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-000151c0: 7064 6174 6528 7b73 656c 662e 6166 7465  pdate({self.afte
-000151d0: 7269 645f 6b65 7920 3a20 696e 7428 7461  rid_key : int(ta
-000151e0: 7267 6574 5f69 6429 7d29 200d 0a20 2020  rget_id)}) ..   
-000151f0: 2020 2020 2065 6c69 6620 7461 7267 6574       elif target
-00015200: 5f69 6420 6973 204e 6f6e 653a 0d0a 2020  _id is None:..  
-00015210: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00015220: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015230: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00015240: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00015250: 2e61 6674 6572 6964 5f6b 6579 203a 204e  .afterid_key : N
-00015260: 6f6e 657d 290d 0a20 2020 2020 2020 2020  one})..         
-00015270: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
-00015280: 662e 5f73 6563 6f6e 645f 6368 616e 6e65  f._second_channe
-00015290: 6c5f 7570 6461 7465 2863 656c 6c5f 6964  l_update(cell_id
-000152a0: 2c20 7472 6163 6b5f 6964 2920 2020 200d  , track_id)    .
-000152b0: 0a0d 0a0d 0a20 2020 2064 6566 205f 7465  .....    def _te
-000152c0: 6d70 6f72 616c 5f70 6c6f 7473 5f74 7261  mporal_plots_tra
-000152d0: 636b 6d61 7465 2873 656c 6629 3a0d 0a20  ckmate(self):.. 
-000152e0: 2020 200d 0a20 2020 200d 0a20 2020 200d     ..    ..    .
-000152f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015300: 2073 656c 662e 4174 7472 203d 207b 7d0d   self.Attr = {}.
-00015310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015320: 2073 7461 7274 7469 6d65 203d 2069 6e74   starttime = int
-00015330: 286d 696e 2873 656c 662e 416c 6c56 616c  (min(self.AllVal
-00015340: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
-00015350: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
-00015360: 2020 2020 2020 2020 2065 6e64 7469 6d65           endtime
-00015370: 203d 2069 6e74 286d 6178 2873 656c 662e   = int(max(self.
-00015380: 416c 6c56 616c 7565 735b 7365 6c66 2e66  AllValues[self.f
-00015390: 7261 6d65 6964 5f6b 6579 5d29 290d 0a20  rameid_key])).. 
-000153a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000153c0: 2020 7365 6c66 2e74 696d 6520 3d20 5b5d    self.time = []
-000153d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000153e0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-000153f0: 6561 6e5f 6469 7370 5f7a 203d 205b 5d0d  ean_disp_z = [].
-00015400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015410: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00015420: 725f 6469 7370 5f7a 203d 205b 5d0d 0a0d  r_disp_z = []...
-00015430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015440: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00015450: 616e 5f64 6973 705f 7920 3d20 5b5d 0d0a  an_disp_y = []..
-00015460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015470: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00015480: 5f64 6973 705f 7920 3d20 5b5d 0d0a 0d0a  _disp_y = []....
-00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154a0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-000154b0: 6e5f 6469 7370 5f78 203d 205b 5d0d 0a20  n_disp_x = [].. 
-000154c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000154d0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-000154e0: 6469 7370 5f78 203d 205b 5d0d 0a0d 0a20  disp_x = [].... 
-000154f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015500: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00015510: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
-00015520: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015530: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f72  lf.mitotic_var_r
-00015540: 6164 6975 7320 3d20 5b5d 0d0a 0d0a 2020  adius = []....  
-00015550: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015560: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00015570: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
-00015580: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015590: 2e6d 6974 6f74 6963 5f76 6172 5f73 7065  .mitotic_var_spe
-000155a0: 6564 203d 205b 5d0d 0a0d 0a20 2020 2020  ed = []....     
-000155b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000155c0: 6d69 746f 7469 635f 6d65 616e 5f61 6363  mitotic_mean_acc
-000155d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000155e0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-000155f0: 7469 635f 7661 725f 6163 6320 3d20 5b5d  tic_var_acc = []
-00015600: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015610: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00015620: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
-00015630: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
-00015640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015650: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00015660: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00015670: 6765 203d 205b 5d0d 0a0d 0a20 2020 2020  ge = []....     
-00015680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015690: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-000156a0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-000156b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000156c0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-000156d0: 6963 5f76 6172 5f64 6973 7461 6e63 655f  ic_var_distance_
-000156e0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-000156f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015700: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00015710: 6963 5f6d 6561 6e5f 6469 7370 5f7a 203d  ic_mean_disp_z =
-00015720: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015730: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00015740: 746f 7469 635f 7661 725f 6469 7370 5f7a  totic_var_disp_z
-00015750: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015760: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00015770: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-00015780: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
-00015790: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000157a0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-000157b0: 5f64 6973 705f 7920 3d20 5b5d 0d0a 0d0a  _disp_y = []....
-000157c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157d0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-000157e0: 5f6d 6561 6e5f 6469 7370 5f78 203d 205b  _mean_disp_x = [
-000157f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015800: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015810: 7469 635f 7661 725f 6469 7370 5f78 203d  tic_var_disp_x =
-00015820: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015830: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015840: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
-00015850: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
-00015860: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015870: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f72  on_mitotic_var_r
-00015880: 6164 6975 7320 3d20 5b5d 0d0a 0d0a 2020  adius = []....  
-00015890: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000158a0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-000158b0: 6561 6e5f 7370 6565 6420 3d20 5b5d 0d0a  ean_speed = []..
-000158c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158d0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-000158e0: 5f76 6172 5f73 7065 6564 203d 205b 5d0d  _var_speed = [].
-000158f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015900: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015910: 7469 635f 6d65 616e 5f61 6363 203d 205b  tic_mean_acc = [
-00015920: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015930: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015940: 7469 635f 7661 725f 6163 6320 3d20 5b5d  tic_var_acc = []
-00015950: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015960: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00015970: 6f74 6963 5f6d 6561 6e5f 6469 7265 6374  otic_mean_direct
-00015980: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
-00015990: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000159a0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-000159b0: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
-000159c0: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-000159d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000159e0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-000159f0: 7469 635f 6d65 616e 5f64 6973 7461 6e63  tic_mean_distanc
-00015a00: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
-00015a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015a20: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00015a30: 6963 5f76 6172 5f64 6973 7461 6e63 655f  ic_var_distance_
-00015a40: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-00015a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015a60: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00015a70: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
-00015a80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015a90: 662e 616c 6c5f 7661 725f 6469 7370 5f7a  f.all_var_disp_z
-00015aa0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015ab0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00015ac0: 6c5f 6d65 616e 5f64 6973 705f 7920 3d20  l_mean_disp_y = 
-00015ad0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00015ae0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00015af0: 5f64 6973 705f 7920 3d20 5b5d 0d0a 0d0a  _disp_y = []....
-00015b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b10: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00015b20: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
-00015b30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015b40: 616c 6c5f 7661 725f 6469 7370 5f78 203d  all_var_disp_x =
-00015b50: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015b60: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00015b70: 6d65 616e 5f72 6164 6975 7320 3d20 5b5d  mean_radius = []
-00015b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015b90: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f72    self.all_var_r
-00015ba0: 6164 6975 7320 3d20 5b5d 0d0a 0d0a 2020  adius = []....  
-00015bb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015bc0: 6c66 2e61 6c6c 5f6d 6561 6e5f 7370 6565  lf.all_mean_spee
-00015bd0: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
-00015be0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00015bf0: 5f76 6172 5f73 7065 6564 203d 205b 5d0d  _var_speed = [].
-00015c00: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015c10: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00015c20: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00015c30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015c40: 616c 6c5f 7661 725f 6163 6320 3d20 5b5d  all_var_acc = []
-00015c50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015c60: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00015c70: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
-00015c80: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
-00015c90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015ca0: 616c 6c5f 7661 725f 6469 7265 6374 696f  all_var_directio
-00015cb0: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00015cc0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015cd0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00015ce0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00015cf0: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
-00015d00: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00015d10: 6c6c 5f76 6172 5f64 6973 7461 6e63 655f  ll_var_distance_
-00015d20: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-00015d30: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015d40: 2020 2020 616c 6c5f 7370 6f74 735f 7472      all_spots_tr
-00015d50: 6163 6b73 203d 207b 7d0d 0a20 2020 2020  acks = {}..     
-00015d60: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-00015d70: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
-00015d80: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015d90: 6965 732e 6974 656d 7328 293a 0d0a 2020  ies.items():..  
-00015da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015db0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00015dc0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00015dd0: 7370 6f74 7320 3d20 7365 6c66 2e75 6e69  spots = self.uni
-00015de0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015df0: 6965 735b 6b5d 0d0a 2020 2020 2020 2020  ies[k]..        
-00015e00: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00015e10: 2073 656c 662e 7472 6163 6b69 645f 6b65   self.trackid_ke
-00015e20: 7920 696e 2061 6c6c 5f73 706f 7473 3a0d  y in all_spots:.
-00015e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e40: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
-00015e50: 706f 7473 5f74 7261 636b 735b 6b5d 203d  pots_tracks[k] =
-00015e60: 2061 6c6c 5f73 706f 7473 0d0a 2020 2020   all_spots..    
-00015e70: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015ea0: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
-00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ec0: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
-00015ed0: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
-00015ee0: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
-00015ef0: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
-00015f00: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
-00015f10: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
-00015f20: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 2020 2066 6f72 2069 2069 6e20 7471 646d     for i in tqdm
-00015f50: 2872 616e 6765 2873 7461 7274 7469 6d65  (range(starttime
-00015f60: 2c20 656e 6474 696d 6529 2c20 746f 7461  , endtime), tota
-00015f70: 6c3d 656e 6474 696d 6520 2d20 7374 6172  l=endtime - star
-00015f80: 7474 696d 6529 3a0d 0a20 2020 2020 2020  ttime):..       
-00015f90: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00015fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015fb0: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-00015fc0: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
-00015fd0: 2e73 7562 6d69 7428 7365 6c66 2e5f 636f  .submit(self._co
-00015fe0: 6d70 7574 655f 7465 6d70 6f72 616c 2c20  mpute_temporal, 
-00015ff0: 692c 2061 6c6c 5f73 706f 7473 5f74 7261  i, all_spots_tra
-00016000: 636b 7329 290d 0a20 0d0a 2020 2020 2020  cks)).. ..      
-00016010: 2020 2020 2020 2020 2020 2020 2020 5b72                [r
-00016020: 2e72 6573 756c 7428 2920 666f 7220 7220  .result() for r 
-00016030: 696e 2063 6f6e 6375 7272 656e 742e 6675  in concurrent.fu
-00016040: 7475 7265 732e 6173 5f63 6f6d 706c 6574  tures.as_complet
-00016050: 6564 2866 7574 7572 6573 295d 0d0a 0d0a  ed(futures)]....
-00016060: 0d0a 2020 2020 6465 6620 5f63 6f6d 7075  ..    def _compu
-00016070: 7465 5f74 656d 706f 7261 6c28 7365 6c66  te_temporal(self
-00016080: 2c20 692c 2061 6c6c 5f73 706f 7473 5f74  , i, all_spots_t
-00016090: 7261 636b 7329 3a20 2020 2020 2020 2020  racks):         
-000160a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000160b0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-000160c0: 6f74 6963 5f64 6973 705f 7a20 3d20 5b5d  otic_disp_z = []
-000160d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000160e0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-000160f0: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00016100: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016110: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-00016120: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016130: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00016140: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016160: 206d 6974 6f74 6963 5f73 7065 6564 203d   mitotic_speed =
-00016170: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016180: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016190: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-000161a0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000161b0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-000161c0: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161e0: 2020 2020 6d69 746f 7469 635f 6469 7374      mitotic_dist
-000161f0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00016200: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016210: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016220: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
-00016230: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016240: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00016250: 7469 635f 6469 7370 5f79 203d 205b 5d0d  tic_disp_y = [].
-00016260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016270: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016280: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162a0: 2020 6e6f 6e5f 6d69 746f 7469 635f 7261    non_mitotic_ra
-000162b0: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-000162c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000162d0: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
-000162e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000162f0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016300: 6974 6f74 6963 5f61 6363 203d 205b 5d0d  itotic_acc = [].
-00016310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016320: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016330: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00016340: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00016350: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00016360: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-00016370: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00016380: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016390: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000163a0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000163b0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-000163c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163d0: 2020 616c 6c5f 6469 7370 5f79 203d 205b    all_disp_y = [
-000163e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000163f0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00016400: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00016410: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00016420: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00016430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016440: 2061 6c6c 5f73 7065 6564 203d 205b 5d0d   all_speed = [].
-00016450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016460: 2020 2020 2061 6c6c 5f61 6363 203d 205b       all_acc = [
-00016470: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016480: 2020 2020 2020 2061 6c6c 5f64 6972 6563         all_direc
-00016490: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-000164a0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000164b0: 2020 2020 2020 2020 616c 6c5f 6469 7374          all_dist
-000164c0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-000164d0: 205b 5d0d 0a0d 0a0d 0a0d 0a0d 0a20 2020   []..........   
-000164e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164f0: 2066 6f72 2028 6b2c 7629 2069 6e20 616c   for (k,v) in al
-00016500: 6c5f 7370 6f74 735f 7472 6163 6b73 2e69  l_spots_tracks.i
-00016510: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00016520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016530: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00016540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016550: 2020 2063 7572 7265 6e74 5f74 696d 6520     current_time 
-00016560: 3d20 616c 6c5f 7370 6f74 735f 7472 6163  = all_spots_trac
-00016570: 6b73 5b6b 5d5b 7365 6c66 2e66 7261 6d65  ks[k][self.frame
-00016580: 6964 5f6b 6579 5d0d 0a20 2020 2020 2020  id_key]..       
-00016590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165a0: 2020 2020 206d 6974 6f74 6963 203d 2061       mitotic = a
-000165b0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000165c0: 6b5d 5b73 656c 662e 6469 7669 6469 6e67  k][self.dividing
-000165d0: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-000165e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00016600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016610: 6966 2069 203d 3d20 696e 7428 6375 7272  if i == int(curr
-00016620: 656e 745f 7469 6d65 293a 0d0a 2020 2020  ent_time):..    
-00016630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016640: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016650: 206d 6974 6f74 6963 3a0d 0a20 2020 2020   mitotic:..     
-00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016680: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-00016690: 7a2e 6170 7065 6e64 2861 6c6c 5f73 706f  z.append(all_spo
-000166a0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-000166b0: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
-000166c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166e0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-000166f0: 6469 7370 5f79 2e61 7070 656e 6428 616c  disp_y.append(al
-00016700: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00016710: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-00016720: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016740: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016750: 6f74 6963 5f64 6973 705f 782e 6170 7065  otic_disp_x.appe
-00016760: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00016770: 636b 735b 6b5d 5b73 656c 662e 7870 6f73  cks[k][self.xpos
-00016780: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00016790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167b0: 2020 6966 2061 6c6c 5f73 706f 7473 5f74    if all_spots_t
-000167c0: 7261 636b 735b 6b5d 5b73 656c 662e 7261  racks[k][self.ra
-000167d0: 6469 7573 5f6b 6579 5d20 3e20 303a 0d0a  dius_key] > 0:..
-000167e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016800: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016810: 6963 5f72 6164 6975 732e 6170 7065 6e64  ic_radius.append
-00016820: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00016830: 735b 6b5d 5b73 656c 662e 7261 6469 7573  s[k][self.radius
-00016840: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00012f70: 2020 2020 2020 6375 7272 656e 745f 696e        current_in
+00012f80: 7465 6e73 6974 792e 6170 7065 6e64 2869  tensity.append(i
+00012f90: 6e74 656e 7369 7479 5b6a 5d29 0d0a 2020  ntensity[j])..  
+00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012fc0: 7572 7265 6e74 5f72 6164 6975 732e 6170  urrent_radius.ap
+00012fd0: 7065 6e64 2872 6164 6975 735b 6a5d 290d  pend(radius[j]).
+00012fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013000: 2020 6375 7272 656e 745f 766f 6c75 6d65    current_volume
+00013010: 2e61 7070 656e 6428 766f 6c75 6d65 5b6a  .append(volume[j
+00013020: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013040: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
+00013050: 6564 2e61 7070 656e 6428 7370 6565 645b  ed.append(speed[
+00013060: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013080: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
+00013090: 7469 6f6e 5f61 6e67 6c65 2e61 7070 656e  tion_angle.appen
+000130a0: 6428 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a  d(motion_angle[j
+000130b0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130d0: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
+000130e0: 656c 6572 6174 696f 6e2e 6170 7065 6e64  eleration.append
+000130f0: 2861 6363 656c 6572 6174 696f 6e5b 6a5d  (acceleration[j]
+00013100: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013120: 2020 2020 6375 7272 656e 745f 6469 7374      current_dist
+00013130: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00013140: 7070 656e 6428 6469 7374 616e 6365 5f63  ppend(distance_c
+00013150: 656c 6c5f 6d61 736b 5b6a 5d29 0d0a 2020  ell_mask[j])..  
+00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013170: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013180: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013190: 6974 795f 636f 6d70 5f66 6972 7374 2e61  ity_comp_first.a
+000131a0: 7070 656e 6428 6563 6365 6e74 7269 6369  ppend(eccentrici
+000131b0: 7479 5f63 6f6d 705f 6669 7273 745b 6a5d  ty_comp_first[j]
+000131c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131e0: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
+000131f0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+00013200: 636f 6e64 2e61 7070 656e 6428 6563 6365  cond.append(ecce
+00013210: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+00013220: 636f 6e64 5b6a 5d29 0d0a 2020 2020 2020  cond[j])..      
+00013230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013240: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013250: 6e74 5f73 7572 6661 6365 5f61 7265 612e  nt_surface_area.
+00013260: 6170 7065 6e64 2873 7572 6661 6365 5f61  append(surface_a
+00013270: 7265 615b 6a5d 290d 0a20 2020 2020 2020  rea[j])..       
+00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013290: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000132a0: 745f 7261 6469 616c 5f61 6e67 6c65 2e61  t_radial_angle.a
+000132b0: 7070 656e 6428 7261 6469 616c 5f61 6e67  ppend(radial_ang
+000132c0: 6c65 5b6a 5d29 0d0a 2020 2020 2020 2020  le[j])..        
+000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000132f0: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b2e  _cell_axis_mask.
+00013300: 6170 7065 6e64 2863 656c 6c5f 6178 6973  append(cell_axis
+00013310: 5f6d 6173 6b5b 6a5d 290d 0a20 2020 2020  _mask[j])..     
+00013320: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013330: 7272 656e 745f 7469 6d65 203d 206e 702e  rrent_time = np.
+00013340: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00013350: 7469 6d65 2c20 6474 7970 653d 6e70 2e66  time, dtype=np.f
+00013360: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00013370: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013380: 656e 745f 696e 7465 6e73 6974 7920 3d20  ent_intensity = 
+00013390: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+000133a0: 6e74 5f69 6e74 656e 7369 7479 2c20 6474  nt_intensity, dt
+000133b0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+000133c0: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
+000133d0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000133e0: 745f 7261 6469 7573 203d 206e 702e 6173  t_radius = np.as
+000133f0: 6172 7261 7928 6375 7272 656e 745f 7261  array(current_ra
+00013400: 6469 7573 2c20 6474 7970 653d 6e70 2e66  dius, dtype=np.f
+00013410: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00013420: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013430: 656e 745f 766f 6c75 6d65 203d 206e 702e  ent_volume = np.
+00013440: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00013450: 766f 6c75 6d65 2c20 6474 7970 653d 6e70  volume, dtype=np
+00013460: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+00013470: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013480: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00013490: 7479 5f63 6f6d 705f 6669 7273 7420 3d20  ty_comp_first = 
+000134a0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+000134b0: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+000134c0: 636f 6d70 5f66 6972 7374 2c20 6474 7970  comp_first, dtyp
+000134d0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
+000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134f0: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
+00013500: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00013510: 6e64 203d 206e 702e 6173 6172 7261 7928  nd = np.asarray(
+00013520: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+00013530: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00013540: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00013550: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00013560: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013570: 7375 7266 6163 655f 6172 6561 203d 206e  surface_area = n
+00013580: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+00013590: 745f 7375 7266 6163 655f 6172 6561 2c20  t_surface_area, 
+000135a0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+000135b0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+000135c0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000135d0: 7370 6565 6420 3d20 6e70 2e61 7361 7272  speed = np.asarr
+000135e0: 6179 2863 7572 7265 6e74 5f73 7065 6564  ay(current_speed
+000135f0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00013600: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00013610: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013620: 6d6f 7469 6f6e 5f61 6e67 6c65 203d 206e  motion_angle = n
+00013630: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+00013640: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  t_motion_angle, 
+00013650: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00013660: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013670: 2020 2020 2020 6375 7272 656e 745f 6163        current_ac
+00013680: 6365 6c65 7261 7469 6f6e 203d 206e 702e  celeration = np.
+00013690: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+000136a0: 6163 6365 6c65 7261 7469 6f6e 2c20 6474  acceleration, dt
+000136b0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+000136c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000136d0: 2020 2020 6375 7272 656e 745f 6469 7374      current_dist
+000136e0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+000136f0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00013700: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00013710: 6c5f 6d61 736b 2c20 6474 7970 653d 6e70  l_mask, dtype=np
+00013720: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+00013730: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013740: 7272 656e 745f 7261 6469 616c 5f61 6e67  rrent_radial_ang
+00013750: 6c65 203d 206e 702e 6173 6172 7261 7928  le = np.asarray(
+00013760: 6375 7272 656e 745f 7261 6469 616c 5f61  current_radial_a
+00013770: 6e67 6c65 2c20 6474 7970 653d 6e70 2e66  ngle, dtype=np.f
+00013780: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00013790: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000137a0: 656e 745f 6365 6c6c 5f61 7869 735f 6d61  ent_cell_axis_ma
+000137b0: 736b 203d 206e 702e 6173 6172 7261 7928  sk = np.asarray(
+000137c0: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
+000137d0: 735f 6d61 736b 2c20 6474 7970 653d 6e70  s_mask, dtype=np
+000137e0: 2e66 6c6f 6174 3332 290d 0a0d 0a0d 0a20  .float32)...... 
+000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013800: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00013810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00013820: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00013830: 6f69 6e74 5f73 616d 706c 6520 3e20 303a  oint_sample > 0:
+00013840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013860: 2020 7866 5f73 616d 706c 6520 3d20 6666    xf_sample = ff
+00013870: 7466 7265 7128 706f 696e 745f 7361 6d70  tfreq(point_samp
+00013880: 6c65 2c20 7365 6c66 2e74 6361 6c69 6272  le, self.tcalibr
+00013890: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+000138a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138b0: 2020 2020 2020 2020 6666 7473 7472 6970          fftstrip
+000138c0: 5f73 616d 706c 6520 3d20 6666 7428 6578  _sample = fft(ex
+000138d0: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
+000138e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000138f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013900: 2020 2066 6674 746f 7461 6c5f 7361 6d70     ffttotal_samp
+00013910: 6c65 203d 206e 702e 6162 7328 6666 7473  le = np.abs(ffts
+00013920: 7472 6970 5f73 616d 706c 6529 0d0a 2020  trip_sample)..  
+00013930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013940: 2020 2020 2020 2020 2020 2020 2020 7866                xf
+00013950: 5f73 616d 706c 6520 3d20 7866 5f73 616d  _sample = xf_sam
+00013960: 706c 655b 3020 3a20 6c65 6e28 7866 5f73  ple[0 : len(xf_s
+00013970: 616d 706c 6529 202f 2f20 325d 0d0a 2020  ample) // 2]..  
+00013980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013990: 2020 2020 2020 2020 2020 2020 2020 6666                ff
+000139a0: 7474 6f74 616c 5f73 616d 706c 6520 3d20  ttotal_sample = 
+000139b0: 6666 7474 6f74 616c 5f73 616d 706c 655b  ffttotal_sample[
+000139c0: 3020 3a20 6c65 6e28 6666 7474 6f74 616c  0 : len(ffttotal
+000139d0: 5f73 616d 706c 6529 202f 2f20 325d 0d0a  _sample) // 2]..
+000139e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000139f0: 2020 2020 2075 6e69 7175 655f 6666 745f       unique_fft_
+00013a00: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+00013a10: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
+00013a20: 7565 5f69 645d 203d 2065 7870 616e 6465  ue_id] = expande
+00013a30: 645f 7469 6d65 2c20 6578 7061 6e64 6564  d_time, expanded
+00013a40: 5f69 6e74 656e 7369 7479 2c20 7866 5f73  _intensity, xf_s
+00013a50: 616d 706c 652c 2066 6674 746f 7461 6c5f  ample, ffttotal_
+00013a60: 7361 6d70 6c65 0d0a 2020 2020 2020 2020  sample..        
+00013a70: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00013a80: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
+00013a90: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
+00013aa0: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
+00013ab0: 203d 2020 6375 7272 656e 745f 7469 6d65   =  current_time
+00013ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013ad0: 2020 2020 2075 6e69 7175 655f 7368 6170       unique_shap
+00013ae0: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
+00013af0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00013b00: 6971 7565 5f69 645d 203d 2063 7572 7265  ique_id] = curre
+00013b10: 6e74 5f74 696d 652c 2063 7572 7265 6e74  nt_time, current
+00013b20: 5f7a 2c20 6375 7272 656e 745f 792c 2063  _z, current_y, c
+00013b30: 7572 7265 6e74 5f78 2c20 6375 7272 656e  urrent_x, curren
+00013b40: 745f 7261 6469 7573 2c20 6375 7272 656e  t_radius, curren
+00013b50: 745f 766f 6c75 6d65 2c20 6375 7272 656e  t_volume, curren
+00013b60: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00013b70: 6f6d 705f 6669 7273 742c 2063 7572 7265  omp_first, curre
+00013b80: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+00013b90: 636f 6d70 5f73 6563 6f6e 642c 2063 7572  comp_second, cur
+00013ba0: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
+00013bb0: 610d 0a20 2020 2020 2020 2020 2020 2020  a..             
+00013bc0: 2020 2020 2020 756e 6971 7565 5f64 796e        unique_dyn
+00013bd0: 616d 6963 5f70 726f 7065 7274 6965 735f  amic_properties_
+00013be0: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
+00013bf0: 5f75 6e69 7175 655f 6964 5d20 3d20 6375  _unique_id] = cu
+00013c00: 7272 656e 745f 7469 6d65 2c20 6375 7272  rrent_time, curr
+00013c10: 656e 745f 7370 6565 642c 2063 7572 7265  ent_speed, curre
+00013c20: 6e74 5f6d 6f74 696f 6e5f 616e 676c 652c  nt_motion_angle,
+00013c30: 2063 7572 7265 6e74 5f61 6363 656c 6572   current_acceler
+00013c40: 6174 696f 6e2c 2063 7572 7265 6e74 5f64  ation, current_d
+00013c50: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00013c60: 6b2c 2063 7572 7265 6e74 5f72 6164 6961  k, current_radia
+00013c70: 6c5f 616e 676c 652c 2063 7572 7265 6e74  l_angle, current
+00013c80: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b0d  _cell_axis_mask.
+00013c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ca0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00013cb0: 6666 745f 7072 6f70 6572 7469 6573 5b74  fft_properties[t
+00013cc0: 7261 636b 5f69 645d 2e75 7064 6174 6528  rack_id].update(
+00013cd0: 7b63 7572 7265 6e74 5f75 6e69 7175 655f  {current_unique_
+00013ce0: 6964 3a75 6e69 7175 655f 6666 745f 7072  id:unique_fft_pr
+00013cf0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00013d00: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00013d10: 5f69 645d 7d29 0d0a 2020 2020 2020 2020  _id]})..        
+00013d20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013d30: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
+00013d40: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
+00013d50: 6964 5d2e 7570 6461 7465 287b 6375 7272  id].update({curr
+00013d60: 656e 745f 756e 6971 7565 5f69 643a 756e  ent_unique_id:un
+00013d70: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
+00013d80: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00013d90: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+00013da0: 6964 5d7d 290d 0a0d 0a20 2020 2020 2020  id]})....       
+00013db0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013dc0: 2e75 6e69 7175 655f 7368 6170 655f 7072  .unique_shape_pr
+00013dd0: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
+00013de0: 645d 2e75 7064 6174 6528 7b63 7572 7265  d].update({curre
+00013df0: 6e74 5f75 6e69 7175 655f 6964 3a75 6e69  nt_unique_id:uni
+00013e00: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
+00013e10: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
+00013e20: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
+00013e30: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00013e40: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00013e50: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
+00013e60: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
+00013e70: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
+00013e80: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
+00013e90: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
+00013ea0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+00013eb0: 7265 6e74 5f75 6e69 7175 655f 6964 5d7d  rent_unique_id]}
+00013ec0: 290d 0a0d 0a20 2020 2064 6566 205f 7365  )....    def _se
+00013ed0: 636f 6e64 5f63 6861 6e6e 656c 5f73 706f  cond_channel_spo
+00013ee0: 7473 2873 656c 662c 2066 7261 6d65 2c20  ts(self, frame, 
+00013ef0: 7a2c 2079 2c20 782c 2063 656c 6c5f 6964  z, y, x, cell_id
+00013f00: 2c20 7472 6163 6b5f 6964 293a 0d0a 2020  , track_id):..  
+00013f10: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00013f20: 2020 2020 2020 2074 7265 652c 2063 656e         tree, cen
+00013f30: 7472 6f69 6473 2c20 6c61 6265 6c73 2c20  troids, labels, 
+00013f40: 766f 6c75 6d65 2c20 696e 7465 6e73 6974  volume, intensit
+00013f50: 795f 6d65 616e 2c20 696e 7465 6e73 6974  y_mean, intensit
+00013f60: 795f 746f 7461 6c2c 2062 6f75 6e64 696e  y_total, boundin
+00013f70: 675f 626f 7865 7320 3d20 7365 6c66 2e5f  g_boxes = self._
+00013f80: 7469 6d65 645f 6368 616e 6e65 6c5f 7365  timed_channel_se
+00013f90: 675f 696d 6167 655b 7374 7228 696e 7428  g_image[str(int(
+00013fa0: 666c 6f61 7428 6672 616d 6529 2929 5d0d  float(frame)))].
+00013fb0: 0a20 2020 2020 2020 2020 2020 2070 6978  .            pix
+00013fc0: 656c 7465 7374 6c6f 6361 7469 6f6e 203d  eltestlocation =
+00013fd0: 2028 7a2c 792c 7829 0d0a 2020 2020 2020   (z,y,x)..      
+00013fe0: 2020 2020 2020 6469 7374 2c20 696e 6465        dist, inde
+00013ff0: 7820 3d20 7472 6565 2e71 7565 7279 2870  x = tree.query(p
+00014000: 6978 656c 7465 7374 6c6f 6361 7469 6f6e  ixeltestlocation
+00014010: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+00014020: 2020 2062 626f 7820 3d20 626f 756e 6469     bbox = boundi
+00014030: 6e67 5f62 6f78 6573 5b69 6e64 6578 5d0d  ng_boxes[index].
+00014040: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00014050: 657a 203d 2061 6273 2862 626f 785b 305d  ez = abs(bbox[0]
+00014060: 202d 2062 626f 785b 335d 290d 0a20 2020   - bbox[3])..   
+00014070: 2020 2020 2020 2020 2073 697a 6579 203d           sizey =
+00014080: 2061 6273 2862 626f 785b 315d 202d 2062   abs(bbox[1] - b
+00014090: 626f 785b 345d 290d 0a20 2020 2020 2020  box[4])..       
+000140a0: 2020 2020 2073 697a 6578 203d 2061 6273       sizex = abs
+000140b0: 2862 626f 785b 325d 202d 2062 626f 785b  (bbox[2] - bbox[
+000140c0: 355d 2920 0d0a 2020 2020 2020 2020 2020  5]) ..          
+000140d0: 2020 7665 746f 5f76 6f6c 756d 6520 3d20    veto_volume = 
+000140e0: 7369 7a65 7820 2a20 7369 7a65 7920 2a20  sizex * sizey * 
+000140f0: 7369 7a65 7a0d 0a20 2020 2020 2020 2020  sizez..         
+00014100: 2020 2076 6574 6f5f 7261 6469 7573 203d     veto_radius =
+00014110: 206d 6174 682e 706f 7728 3320 2a20 7665   math.pow(3 * ve
+00014120: 746f 5f76 6f6c 756d 6520 2f20 2834 202a  to_volume / (4 *
+00014130: 206d 6174 682e 7069 292c 2031 2e30 202f   math.pi), 1.0 /
+00014140: 2033 2e30 290d 0a0d 0a20 2020 2020 2020   3.0)....       
+00014150: 2020 2020 206c 6f63 6174 696f 6e20 3d20       location = 
+00014160: 2863 656e 7472 6f69 6473 5b69 6e64 6578  (centroids[index
+00014170: 5d5b 305d 202a 2073 656c 662e 7a63 616c  ][0] * self.zcal
+00014180: 6962 7261 7469 6f6e 2c20 6365 6e74 726f  ibration, centro
+00014190: 6964 735b 696e 6465 785d 5b31 5d2a 7365  ids[index][1]*se
+000141a0: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
+000141b0: 2063 656e 7472 6f69 6473 5b69 6e64 6578   centroids[index
+000141c0: 5d5b 325d 2a73 656c 662e 7863 616c 6962  ][2]*self.xcalib
+000141d0: 7261 7469 6f6e 290d 0a20 2020 2020 2020  ration)..       
+000141e0: 2020 2020 2051 5541 4c49 5459 203d 206d       QUALITY = m
+000141f0: 6174 682e 706f 7728 766f 6c75 6d65 5b69  ath.pow(volume[i
+00014200: 6e64 6578 5d2c 2031 2e30 2f33 2e30 290d  ndex], 1.0/3.0).
+00014210: 0a20 2020 2020 2020 2020 2020 2052 4144  .            RAD
+00014220: 4955 5320 3d20 6d61 7468 2e70 6f77 2876  IUS = math.pow(v
+00014230: 6f6c 756d 655b 696e 6465 785d 202a 2073  olume[index] * s
+00014240: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00014250: 202a 2073 656c 662e 7963 616c 6962 7261   * self.ycalibra
+00014260: 7469 6f6e 202a 2073 656c 662e 7a63 616c  tion * self.zcal
+00014270: 6962 7261 7469 6f6e 2c20 312e 302f 332e  ibration, 1.0/3.
+00014280: 3029 200d 0a0d 0a20 2020 2020 2020 2020  0) ....         
+00014290: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
+000142a0: 5f6d 6173 6b2c 206d 6173 6b63 656e 7472  _mask, maskcentr
+000142b0: 6f69 6420 3d20 7365 6c66 2e5f 6765 745f  oid = self._get_
+000142c0: 626f 756e 6461 7279 5f64 6973 7428 6672  boundary_dist(fr
+000142d0: 616d 652c 206c 6f63 6174 696f 6e29 0d0a  ame, location)..
+000142e0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+000142f0: 6973 7420 3c3d 2032 202a 2076 6574 6f5f  ist <= 2 * veto_
+00014300: 7261 6469 7573 3a0d 0a20 2020 2020 2020  radius:..       
+00014310: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00014320: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+00014330: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+00014340: 6c5f 6964 5d20 3d20 7b0d 0a20 2020 2020  l_id] = {..     
+00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014360: 2020 2073 656c 662e 6365 6c6c 6964 5f6b     self.cellid_k
+00014370: 6579 3a20 696e 7428 6365 6c6c 5f69 6429  ey: int(cell_id)
+00014380: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00014390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000143a0: 2e66 7261 6d65 6964 5f6b 6579 203a 2069  .frameid_key : i
+000143b0: 6e74 2866 7261 6d65 292c 0d0a 2020 2020  nt(frame),..    
+000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143d0: 2020 2020 7365 6c66 2e7a 706f 7369 645f      self.zposid_
+000143e0: 6b65 7920 3a20 666c 6f61 7428 6365 6e74  key : float(cent
+000143f0: 726f 6964 735b 696e 6465 785d 5b30 5d2a  roids[index][0]*
+00014400: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+00014410: 6f6e 292c 0d0a 2020 2020 2020 2020 2020  on),..          
+00014420: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014430: 6c66 2e79 706f 7369 645f 6b65 7920 3a20  lf.yposid_key : 
+00014440: 666c 6f61 7428 6365 6e74 726f 6964 735b  float(centroids[
+00014450: 696e 6465 785d 5b31 5d2a 2073 656c 662e  index][1]* self.
+00014460: 7963 616c 6962 7261 7469 6f6e 292c 0d0a  ycalibration),..
+00014470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014480: 2020 2020 2020 2020 7365 6c66 2e78 706f          self.xpo
+00014490: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+000144a0: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+000144b0: 5b32 5d2a 2073 656c 662e 7863 616c 6962  [2]* self.xcalib
+000144c0: 7261 7469 6f6e 292c 0d0a 2020 2020 2020  ration),..      
+000144d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144e0: 2020 7365 6c66 2e74 7261 636b 6964 5f6b    self.trackid_k
+000144f0: 6579 3a20 696e 7428 7472 6163 6b5f 6964  ey: int(track_id
+00014500: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00014510: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014520: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+00014530: 5f6b 6579 203a 2028 666c 6f61 7428 696e  _key : (float(in
+00014540: 7465 6e73 6974 795f 746f 7461 6c5b 696e  tensity_total[in
+00014550: 6465 785d 2929 2c0d 0a20 2020 2020 2020  dex])),..       
+00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014570: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
+00014580: 7369 7479 5f6b 6579 203a 2028 666c 6f61  sity_key : (floa
+00014590: 7428 696e 7465 6e73 6974 795f 6d65 616e  t(intensity_mean
+000145a0: 5b69 6e64 6578 5d29 292c 0d0a 2020 2020  [index])),..    
+000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145c0: 2020 2020 7365 6c66 2e72 6164 6975 735f      self.radius_
+000145d0: 6b65 7920 3a20 2866 6c6f 6174 2852 4144  key : (float(RAD
+000145e0: 4955 5329 292c 0d0a 2020 2020 2020 2020  IUS)),..        
+000145f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014600: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
+00014610: 203a 2028 666c 6f61 7428 5155 414c 4954   : (float(QUALIT
+00014620: 5929 292c 0d0a 2020 2020 2020 2020 2020  Y)),..          
+00014630: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014640: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+00014650: 5f6d 6173 6b5f 6b65 793a 2066 6c6f 6174  _mask_key: float
+00014660: 2864 6973 7461 6e63 655f 6365 6c6c 5f6d  (distance_cell_m
+00014670: 6173 6b29 2c0d 0a20 2020 2020 2020 2020  ask),..         
+00014680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014690: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+000146a0: 5f7a 5f6b 6579 3a20 666c 6f61 7428 6d61  _z_key: float(ma
+000146b0: 736b 6365 6e74 726f 6964 5b30 5d29 2c0d  skcentroid[0]),.
+000146c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000146d0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+000146e0: 736b 6365 6e74 726f 6964 5f79 5f6b 6579  skcentroid_y_key
+000146f0: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+00014700: 726f 6964 5b31 5d29 2c0d 0a20 2020 2020  roid[1]),..     
+00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014720: 2020 2073 656c 662e 6d61 736b 6365 6e74     self.maskcent
+00014730: 726f 6964 5f78 5f6b 6579 3a20 666c 6f61  roid_x_key: floa
+00014740: 7428 6d61 736b 6365 6e74 726f 6964 5b32  t(maskcentroid[2
+00014750: 5d29 200d 0a0d 0a20 2020 2020 2020 2020  ]) ....         
+00014760: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00014770: 2020 2020 2020 656c 6966 2063 656c 6c5f        elif cell_
+00014780: 6964 2069 6e20 7365 6c66 2e65 6467 655f  id in self.edge_
+00014790: 736f 7572 6365 5f6c 6f6f 6b75 702e 6b65  source_lookup.ke
+000147a0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+000147b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147d0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+000147e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000147f0: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
+00014800: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014810: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+00014820: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
+00014830: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00014840: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+00014850: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+00014860: 6c6c 5f69 645d 2e75 7064 6174 6528 7b73  ll_id].update({s
+00014870: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+00014880: 6974 795f 6b65 793a 202d 317d 290d 0a20  ity_key: -1}).. 
+00014890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148a0: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+000148b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000148c0: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+000148d0: 7570 6461 7465 287b 7365 6c66 2e6d 6561  update({self.mea
+000148e0: 6e5f 696e 7465 6e73 6974 795f 6b65 793a  n_intensity_key:
+000148f0: 202d 317d 290d 0a20 2020 2020 2020 2020   -1})..         
+00014900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014910: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+00014920: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+00014930: 656c 6c5f 6964 5d2e 7570 6461 7465 287b  ell_id].update({
+00014940: 7365 6c66 2e72 6164 6975 735f 6b65 793a  self.radius_key:
+00014950: 202d 317d 290d 0a20 2020 2020 2020 2020   -1})..         
+00014960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014970: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+00014980: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+00014990: 656c 6c5f 6964 5d2e 7570 6461 7465 287b  ell_id].update({
+000149a0: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
+000149b0: 3a20 2d31 7d29 0d0a 0d0a 0d0a 0d0a 2020  : -1})........  
+000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000149e0: 0a20 2020 2064 6566 205f 6469 6374 5f75  .    def _dict_u
+000149f0: 7064 6174 6528 7365 6c66 2c20 756e 6971  pdate(self, uniq
+00014a00: 7565 5f74 7261 636b 6c65 745f 6964 733a  ue_tracklet_ids:
+00014a10: 204c 6973 742c 2020 6365 6c6c 5f69 643a   List,  cell_id:
+00014a20: 2069 6e74 2c20 7472 6163 6b5f 6964 3a20   int, track_id: 
+00014a30: 696e 742c 2073 6f75 7263 655f 6964 3a20  int, source_id: 
+00014a40: 696e 742c 2074 6172 6765 745f 6964 3a20  int, target_id: 
+00014a50: 696e 7429 3a0d 0a0d 0a20 0d0a 2020 2020  int):.... ..    
+00014a60: 2020 2020 6765 6e65 7261 7469 6f6e 5f69      generation_i
+00014a70: 6420 3d20 7365 6c66 2e67 656e 6572 6174  d = self.generat
+00014a80: 696f 6e5f 6469 6374 5b63 656c 6c5f 6964  ion_dict[cell_id
+00014a90: 5d0d 0a20 2020 2020 2020 2074 7261 636b  ]..        track
+00014aa0: 6c65 745f 6964 203d 2073 656c 662e 7472  let_id = self.tr
+00014ab0: 6163 6b6c 6574 5f64 6963 745b 6365 6c6c  acklet_dict[cell
+00014ac0: 5f69 645d 0d0a 0d0a 2020 2020 2020 2020  _id]....        
+00014ad0: 756e 6971 7565 5f69 6420 3d20 7374 7228  unique_id = str(
+00014ae0: 7472 6163 6b5f 6964 2920 2b20 2073 7472  track_id) +  str
+00014af0: 2867 656e 6572 6174 696f 6e5f 6964 2920  (generation_id) 
+00014b00: 2b20 7374 7228 7472 6163 6b6c 6574 5f69  + str(tracklet_i
+00014b10: 6429 0d0a 2020 2020 2020 2020 0d0a 2020  d)..        ..  
+00014b20: 2020 2020 2020 7665 635f 6d61 736b 203d        vec_mask =
+00014b30: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
+00014b40: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014b50: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014b60: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
+00014b70: 6f69 645f 785f 6b65 795d 292c 2066 6c6f  oid_x_key]), flo
+00014b80: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014b90: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014ba0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00014bb0: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
+00014bc0: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
+00014bd0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014be0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014bf0: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
+00014c00: 6b63 656e 7472 6f69 645f 7a5f 6b65 795d  kcentroid_z_key]
+00014c10: 2920 5d0d 0a0d 0a20 2020 2020 2020 2076  ) ]....        v
+00014c20: 6563 5f63 656c 6c20 3d20 5b66 6c6f 6174  ec_cell = [float
+00014c30: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014c40: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014c50: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00014c60: 7870 6f73 6964 5f6b 6579 5d29 202c 200d  xposid_key]) , .
+00014c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c80: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+00014c90: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014ca0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014cb0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00014cc0: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
+00014cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014ce0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+00014cf0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014d00: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014d10: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014d20: 6c66 2e7a 706f 7369 645f 6b65 795d 295d  lf.zposid_key])]
+00014d30: 0d0a 0d0a 2020 2020 2020 2020 616e 676c  ....        angl
+00014d40: 6520 3d20 616e 6775 6c61 725f 6368 616e  e = angular_chan
+00014d50: 6765 2876 6563 5f6d 6173 6b2c 2076 6563  ge(vec_mask, vec
+00014d60: 5f63 656c 6c29 0d0a 0d0a 2020 2020 2020  _cell)....      
+00014d70: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00014d80: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014d90: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00014da0: 7465 287b 7365 6c66 2e72 6164 6961 6c5f  te({self.radial_
+00014db0: 616e 676c 655f 6b65 7920 3a20 616e 676c  angle_key : angl
+00014dc0: 657d 2920 2020 2020 2020 2020 2020 2020  e})             
+00014dd0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00014de0: 2020 2075 6e69 7175 655f 7472 6163 6b6c     unique_trackl
+00014df0: 6574 5f69 6473 2e61 7070 656e 6428 7374  et_ids.append(st
+00014e00: 7228 756e 6971 7565 5f69 6429 290d 0a20  r(unique_id)).. 
+00014e10: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00014e20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014e30: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00014e40: 2e75 7064 6174 6528 7b73 656c 662e 756e  .update({self.un
+00014e50: 6971 7565 6964 5f6b 6579 203a 2073 7472  iqueid_key : str
+00014e60: 2875 6e69 7175 655f 6964 297d 290d 0a20  (unique_id)}).. 
+00014e70: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00014e80: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014e90: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00014ea0: 2e75 7064 6174 6528 7b73 656c 662e 7472  .update({self.tr
+00014eb0: 6163 6b6c 6574 6964 5f6b 6579 203a 2073  ackletid_key : s
+00014ec0: 7472 2874 7261 636b 6c65 745f 6964 297d  tr(tracklet_id)}
+00014ed0: 2920 0d0a 2020 2020 2020 2020 7365 6c66  ) ..        self
+00014ee0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014ef0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00014f00: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00014f10: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
+00014f20: 6b65 7920 3a20 7374 7228 6765 6e65 7261  key : str(genera
+00014f30: 7469 6f6e 5f69 6429 7d29 200d 0a20 2020  tion_id)}) ..   
+00014f40: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00014f50: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014f60: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00014f70: 7064 6174 6528 7b73 656c 662e 7472 6163  pdate({self.trac
+00014f80: 6b69 645f 6b65 7920 3a20 7374 7228 7472  kid_key : str(tr
+00014f90: 6163 6b5f 6964 297d 290d 0a20 2020 2020  ack_id)})..     
+00014fa0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014fb0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014fc0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00014fd0: 6174 6528 7b73 656c 662e 6d6f 7469 6f6e  ate({self.motion
+00014fe0: 5f61 6e67 6c65 5f6b 6579 203a 2030 2e30  _angle_key : 0.0
+00014ff0: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
+00015000: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015010: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015020: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015030: 6c66 2e73 7065 6564 5f6b 6579 203a 2030  lf.speed_key : 0
+00015040: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
+00015050: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015060: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015070: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015080: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+00015090: 6e5f 6b65 7920 3a20 302e 307d 290d 0a20  n_key : 0.0}).. 
+000150a0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000150b0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000150c0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+000150d0: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
+000150e0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+000150f0: 6669 7273 746b 6579 203a 202d 317d 290d  firstkey : -1}).
+00015100: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00015110: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015120: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015130: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015140: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00015150: 705f 7365 636f 6e64 6b65 7920 3a20 2d31  p_secondkey : -1
+00015160: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
+00015170: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015180: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015190: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+000151a0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+000151b0: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
+000151c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000151d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000151e0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000151f0: 6461 7465 287b 7365 6c66 2e63 656c 6c61  date({self.cella
+00015200: 7869 735f 6d61 736b 5f6b 6579 203a 202d  xis_mask_key : -
+00015210: 317d 290d 0a0d 0a20 2020 2020 2020 2069  1})....        i
+00015220: 6620 736f 7572 6365 5f69 6420 6973 206e  f source_id is n
+00015230: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00015240: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00015250: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015260: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00015270: 7570 6461 7465 287b 7365 6c66 2e62 6566  update({self.bef
+00015280: 6f72 6569 645f 6b65 7920 3a20 696e 7428  oreid_key : int(
+00015290: 736f 7572 6365 5f69 6429 7d29 0d0a 2020  source_id)})..  
+000152a0: 2020 2020 2020 2020 2020 7665 635f 3120            vec_1 
+000152b0: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
+000152c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000152d0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000152e0: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
+000152f0: 6579 5d29 202d 2066 6c6f 6174 2873 656c  ey]) - float(sel
+00015300: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015310: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
+00015320: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
+00015330: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
+00015340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015350: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00015360: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015370: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015380: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
+00015390: 706f 7369 645f 6b65 795d 2920 2d20 666c  posid_key]) - fl
+000153a0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000153b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000153c0: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
+000153d0: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+000153e0: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
+000153f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015400: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00015410: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015420: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015430: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
+00015440: 5d29 202d 2020 666c 6f61 7428 7365 6c66  ]) -  float(self
+00015450: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015460: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+00015470: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
+00015480: 7369 645f 6b65 795d 295d 0d0a 2020 2020  sid_key])]..    
+00015490: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
+000154a0: 6e70 2e73 7172 7428 6e70 2e64 6f74 2876  np.sqrt(np.dot(v
+000154b0: 6563 5f31 2c20 7665 635f 3129 292f 7365  ec_1, vec_1))/se
+000154c0: 6c66 2e74 6361 6c69 6272 6174 696f 6e0d  lf.tcalibration.
+000154d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000154e0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000154f0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015500: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00015510: 656c 662e 7370 6565 645f 6b65 7920 3a20  elf.speed_key : 
+00015520: 7370 6565 647d 290d 0a0d 0a20 2020 2020  speed})....     
+00015530: 2020 2020 2020 206d 6f74 696f 6e5f 616e         motion_an
+00015540: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
+00015550: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
+00015560: 6563 5f31 290d 0a0d 0a20 2020 2020 2020  ec_1)....       
+00015570: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015580: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015590: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+000155a0: 7064 6174 6528 7b73 656c 662e 6d6f 7469  pdate({self.moti
+000155b0: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 206d  on_angle_key : m
+000155c0: 6f74 696f 6e5f 616e 676c 657d 2920 0d0a  otion_angle}) ..
+000155d0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000155e0: 2073 6f75 7263 655f 6964 2069 6e20 7365   source_id in se
+000155f0: 6c66 2e65 6467 655f 736f 7572 6365 5f6c  lf.edge_source_l
+00015600: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
+00015610: 2020 2020 2020 2020 2020 2020 7072 655f              pre_
+00015620: 736f 7572 6365 5f69 6420 3d20 7365 6c66  source_id = self
+00015630: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
+00015640: 6b75 705b 736f 7572 6365 5f69 645d 0d0a  kup[source_id]..
+00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015660: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00015670: 2020 2020 2020 2020 2020 7665 635f 3220            vec_2 
+00015680: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
+00015690: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000156a0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000156b0: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
+000156c0: 6579 5d29 202d 2032 202a 2066 6c6f 6174  ey]) - 2 * float
+000156d0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+000156e0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000156f0: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
+00015700: 662e 7870 6f73 6964 5f6b 6579 5d29 202b  f.xposid_key]) +
+00015710: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00015720: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015730: 6573 5b69 6e74 2870 7265 5f73 6f75 7263  es[int(pre_sourc
+00015740: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
+00015750: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
+00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015770: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
+00015780: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015790: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000157a0: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
+000157b0: 7369 645f 6b65 795d 2920 2d20 3220 2a20  sid_key]) - 2 * 
+000157c0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+000157d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000157e0: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
+000157f0: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+00015800: 795d 2920 2b20 666c 6f61 7428 7365 6c66  y]) + float(self
+00015810: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015820: 7065 7274 6965 735b 696e 7428 7072 655f  perties[int(pre_
+00015830: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
+00015840: 2e79 706f 7369 645f 6b65 795d 292c 200d  .yposid_key]), .
+00015850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015860: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+00015870: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015880: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015890: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+000158a0: 662e 7a70 6f73 6964 5f6b 6579 5d29 202d  f.zposid_key]) -
+000158b0: 2020 3220 2a20 666c 6f61 7428 7365 6c66    2 * float(self
+000158c0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000158d0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+000158e0: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
+000158f0: 7369 645f 6b65 795d 2920 2b20 666c 6f61  sid_key]) + floa
+00015900: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015910: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015920: 7428 7072 655f 736f 7572 6365 5f69 6429  t(pre_source_id)
+00015930: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
+00015940: 795d 295d 0d0a 2020 2020 2020 2020 2020  y])]..          
+00015950: 2020 2020 2020 2020 2020 6163 6320 3d20            acc = 
+00015960: 6e70 2e73 7172 7428 6e70 2e64 6f74 2876  np.sqrt(np.dot(v
+00015970: 6563 5f32 2c20 7665 635f 3229 292f 7365  ec_2, vec_2))/se
+00015980: 6c66 2e74 6361 6c69 6272 6174 696f 6e0d  lf.tcalibration.
+00015990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000159a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000159b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000159c0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000159d0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+000159e0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+000159f0: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+00015a00: 6579 203a 2061 6363 7d29 0d0a 2020 2020  ey : acc})..    
+00015a10: 2020 2020 656c 6966 2073 6f75 7263 655f      elif source_
+00015a20: 6964 2069 7320 4e6f 6e65 3a0d 0a20 2020  id is None:..   
+00015a30: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00015a40: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015a50: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015a60: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015a70: 6265 666f 7265 6964 5f6b 6579 203a 204e  beforeid_key : N
+00015a80: 6f6e 657d 2920 0d0a 2020 2020 2020 2020  one}) ..        
+00015a90: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00015aa0: 6966 2074 6172 6765 745f 6964 2069 7320  if target_id is 
+00015ab0: 6e6f 7420 4e6f 6e65 3a20 2020 2020 2020  not None:       
+00015ac0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00015ad0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015ae0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015af0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015b00: 7365 6c66 2e61 6674 6572 6964 5f6b 6579  self.afterid_key
+00015b10: 203a 2069 6e74 2874 6172 6765 745f 6964   : int(target_id
+00015b20: 297d 2920 0d0a 2020 2020 2020 2020 656c  )}) ..        el
+00015b30: 6966 2074 6172 6765 745f 6964 2069 7320  if target_id is 
+00015b40: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00015b50: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00015b60: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015b70: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00015b80: 6174 6528 7b73 656c 662e 6166 7465 7269  ate({self.afteri
+00015b90: 645f 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  d_key : None})..
+00015ba0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00015bb0: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
+00015bc0: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
+00015bd0: 6528 6365 6c6c 5f69 642c 2074 7261 636b  e(cell_id, track
+00015be0: 5f69 6429 2020 2020 0d0a 0d0a 0d0a 2020  _id)    ......  
+00015bf0: 2020 6465 6620 5f74 656d 706f 7261 6c5f    def _temporal_
+00015c00: 706c 6f74 735f 7472 6163 6b6d 6174 6528  plots_trackmate(
+00015c10: 7365 6c66 293a 0d0a 2020 2020 0d0a 2020  self):..    ..  
+00015c20: 2020 0d0a 2020 2020 0d0a 2020 2020 2020    ..    ..      
+00015c30: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+00015c40: 7474 7220 3d20 7b7d 0d0a 2020 2020 2020  ttr = {}..      
+00015c50: 2020 2020 2020 2020 2020 7374 6172 7474            startt
+00015c60: 696d 6520 3d20 696e 7428 6d69 6e28 7365  ime = int(min(se
+00015c70: 6c66 2e41 6c6c 5661 6c75 6573 5b73 656c  lf.AllValues[sel
+00015c80: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
+00015c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015ca0: 2020 656e 6474 696d 6520 3d20 696e 7428    endtime = int(
+00015cb0: 6d61 7828 7365 6c66 2e41 6c6c 5661 6c75  max(self.AllValu
+00015cc0: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
+00015cd0: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
+00015ce0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00015cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015d00: 7469 6d65 203d 205b 5d0d 0a20 2020 2020  time = []..     
+00015d10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015d20: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00015d30: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
+00015d40: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015d50: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00015d60: 7a20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  z = []....      
+00015d70: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015d80: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00015d90: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00015da0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015db0: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
+00015dc0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015dd0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015de0: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00015df0: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
+00015e00: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015e10: 6f74 6963 5f76 6172 5f64 6973 705f 7820  otic_var_disp_x 
+00015e20: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015e30: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015e40: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
+00015e50: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015e60: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015e70: 7469 635f 7661 725f 7261 6469 7573 203d  tic_var_radius =
+00015e80: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015e90: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015ea0: 7469 635f 6d65 616e 5f73 7065 6564 203d  tic_mean_speed =
+00015eb0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00015ec0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015ed0: 635f 7661 725f 7370 6565 6420 3d20 5b5d  c_var_speed = []
+00015ee0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015ef0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00015f00: 5f6d 6561 6e5f 6163 6320 3d20 5b5d 0d0a  _mean_acc = []..
+00015f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f20: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00015f30: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
+00015f40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015f50: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+00015f60: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00015f70: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+00015f80: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015f90: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+00015fa0: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+00015fb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015fc0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00015fd0: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
+00015fe0: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
+00015ff0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016000: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+00016010: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00016020: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
+00016030: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016040: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00016050: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
+00016060: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016070: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00016080: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
+00016090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000160a0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+000160b0: 6963 5f6d 6561 6e5f 6469 7370 5f79 203d  ic_mean_disp_y =
+000160c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000160d0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+000160e0: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
+000160f0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016100: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00016110: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+00016120: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
+00016130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016140: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00016150: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
+00016160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016170: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00016180: 5f6d 6561 6e5f 7261 6469 7573 203d 205b  _mean_radius = [
+00016190: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000161a0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+000161b0: 7469 635f 7661 725f 7261 6469 7573 203d  tic_var_radius =
+000161c0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+000161d0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+000161e0: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
+000161f0: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
+00016200: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00016210: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
+00016220: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
+00016230: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016240: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00016250: 6e5f 6163 6320 3d20 5b5d 0d0a 2020 2020  n_acc = []..    
+00016260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016270: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00016280: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
+00016290: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000162a0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+000162b0: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
+000162c0: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
+000162d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000162e0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+000162f0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00016300: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
+00016310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016320: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00016330: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
+00016340: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
+00016350: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016360: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00016370: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00016380: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
+00016390: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000163a0: 616c 6c5f 6d65 616e 5f64 6973 705f 7a20  all_mean_disp_z 
+000163b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000163c0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+000163d0: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
+000163e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000163f0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00016400: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
+00016410: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016420: 662e 616c 6c5f 7661 725f 6469 7370 5f79  f.all_var_disp_y
+00016430: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016440: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00016450: 6c5f 6d65 616e 5f64 6973 705f 7820 3d20  l_mean_disp_x = 
+00016460: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016470: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00016480: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
+00016490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000164a0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7261  self.all_mean_ra
+000164b0: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
+000164c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000164d0: 616c 6c5f 7661 725f 7261 6469 7573 203d  all_var_radius =
+000164e0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+000164f0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00016500: 6d65 616e 5f73 7065 6564 203d 205b 5d0d  mean_speed = [].
+00016510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016520: 2073 656c 662e 616c 6c5f 7661 725f 7370   self.all_var_sp
+00016530: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
+00016540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016550: 2e61 6c6c 5f6d 6561 6e5f 6163 6320 3d20  .all_mean_acc = 
+00016560: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016570: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00016580: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
+00016590: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000165a0: 662e 616c 6c5f 6d65 616e 5f64 6972 6563  f.all_mean_direc
+000165b0: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+000165c0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000165d0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+000165e0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000165f0: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
+00016600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016610: 2e61 6c6c 5f6d 6561 6e5f 6469 7374 616e  .all_mean_distan
+00016620: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+00016630: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016640: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00016650: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00016660: 736b 203d 205b 5d0d 0a0d 0a0d 0a20 2020  sk = []......   
+00016670: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00016680: 5f73 706f 7473 5f74 7261 636b 7320 3d20  _spots_tracks = 
+00016690: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+000166a0: 2020 2020 666f 7220 286b 2c76 2920 696e      for (k,v) in
+000166b0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+000166c0: 745f 7072 6f70 6572 7469 6573 2e69 7465  t_properties.ite
+000166d0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+000166e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000166f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016700: 2020 2020 2061 6c6c 5f73 706f 7473 203d       all_spots =
+00016710: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00016720: 745f 7072 6f70 6572 7469 6573 5b6b 5d0d  t_properties[k].
+00016730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016740: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00016750: 7261 636b 6964 5f6b 6579 2069 6e20 616c  rackid_key in al
+00016760: 6c5f 7370 6f74 733a 0d0a 2020 2020 2020  l_spots:..      
+00016770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016780: 2020 2020 616c 6c5f 7370 6f74 735f 7472      all_spots_tr
+00016790: 6163 6b73 5b6b 5d20 3d20 616c 6c5f 7370  acks[k] = all_sp
+000167a0: 6f74 730d 0a20 2020 2020 2020 2020 2020  ots..           
+000167b0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+000167c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000167d0: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+000167e0: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+000167f0: 2020 2020 2020 2020 2077 6974 6820 636f           with co
+00016800: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+00016810: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
+00016820: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
+00016830: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
+00016840: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
 00016850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016870: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00016880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168a0: 2020 6d69 746f 7469 635f 7261 6469 7573    mitotic_radius
-000168b0: 2e61 7070 656e 6428 4e6f 6e65 2920 2020  .append(None)   
-000168c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168e0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000168f0: 746f 7469 635f 7370 6565 642e 6170 7065  totic_speed.appe
-00016900: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00016910: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
-00016920: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016950: 206d 6974 6f74 6963 5f61 6363 2e61 7070   mitotic_acc.app
-00016960: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00016970: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
-00016980: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
-00016990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000169a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169b0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-000169c0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000169d0: 6e67 652e 6170 7065 6e64 2861 6c6c 5f73  nge.append(all_s
-000169e0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-000169f0: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-00016a00: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00016a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a30: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-00016a40: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-00016a50: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00016a60: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
-00016a70: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-00016a80: 795d 290d 0a0d 0a0d 0a20 2020 2020 2020  y])......       
-00016a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016aa0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00016ab0: 7420 6d69 746f 7469 633a 0d0a 2020 2020  t mitotic:..    
-00016ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ae0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00016af0: 6469 7370 5f7a 2e61 7070 656e 6428 616c  disp_z.append(al
-00016b00: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00016b10: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-00016b20: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b40: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00016b50: 5f6d 6974 6f74 6963 5f64 6973 705f 792e  _mitotic_disp_y.
-00016b60: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00016b70: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00016b80: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
-00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bb0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00016bc0: 635f 6469 7370 5f78 2e61 7070 656e 6428  c_disp_x.append(
-00016bd0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016be0: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
-00016bf0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00016c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016c20: 6620 616c 6c5f 7370 6f74 735f 7472 6163  f all_spots_trac
-00016c30: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
-00016c40: 735f 6b65 795d 203e 2030 3a0d 0a20 2020  s_key] > 0:..   
-00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c70: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00016c80: 6f74 6963 5f72 6164 6975 732e 6170 7065  otic_radius.appe
-00016c90: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00016ca0: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
-00016cb0: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
+00016860: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00016870: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00016880: 6920 696e 2074 7164 6d28 7261 6e67 6528  i in tqdm(range(
+00016890: 7374 6172 7474 696d 652c 2065 6e64 7469  starttime, endti
+000168a0: 6d65 292c 2074 6f74 616c 3d65 6e64 7469  me), total=endti
+000168b0: 6d65 202d 2073 7461 7274 7469 6d65 293a  me - starttime):
+000168c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000168d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168f0: 2020 6675 7475 7265 732e 6170 7065 6e64    futures.append
+00016900: 2865 7865 6375 746f 722e 7375 626d 6974  (executor.submit
+00016910: 2873 656c 662e 5f63 6f6d 7075 7465 5f74  (self._compute_t
+00016920: 656d 706f 7261 6c2c 2069 2c20 616c 6c5f  emporal, i, all_
+00016930: 7370 6f74 735f 7472 6163 6b73 2929 0d0a  spots_tracks))..
+00016940: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00016950: 2020 2020 2020 205b 722e 7265 7375 6c74         [r.result
+00016960: 2829 2066 6f72 2072 2069 6e20 636f 6e63  () for r in conc
+00016970: 7572 7265 6e74 2e66 7574 7572 6573 2e61  urrent.futures.a
+00016980: 735f 636f 6d70 6c65 7465 6428 6675 7475  s_completed(futu
+00016990: 7265 7329 5d0d 0a0d 0a0d 0a20 2020 2064  res)]......    d
+000169a0: 6566 205f 636f 6d70 7574 655f 7465 6d70  ef _compute_temp
+000169b0: 6f72 616c 2873 656c 662c 2069 2c20 616c  oral(self, i, al
+000169c0: 6c5f 7370 6f74 735f 7472 6163 6b73 293a  l_spots_tracks):
+000169d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000169f0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016a00: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+00016a10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016a20: 6974 6f74 6963 5f64 6973 705f 7920 3d20  itotic_disp_y = 
+00016a30: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016a40: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016a50: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
+00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a70: 206d 6974 6f74 6963 5f72 6164 6975 7320   mitotic_radius 
+00016a80: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016a90: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00016aa0: 635f 7370 6565 6420 3d20 5b5d 0d0a 2020  c_speed = []..  
+00016ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ac0: 2020 6d69 746f 7469 635f 6163 6320 3d20    mitotic_acc = 
+00016ad0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016ae0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016af0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00016b00: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+00016b10: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016b20: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
+00016b30: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a  ll_mask = []....
+00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b50: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00016b60: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
+00016b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b80: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00016b90: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
+00016ba0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016bb0: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+00016bc0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016bd0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00016be0: 6974 6f74 6963 5f72 6164 6975 7320 3d20  itotic_radius = 
+00016bf0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016c00: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00016c10: 7469 635f 7370 6565 6420 3d20 5b5d 0d0a  tic_speed = []..
+00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c30: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00016c40: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
+00016c50: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016c60: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
+00016c70: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
+00016c80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016c90: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016ca0: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+00016cb0: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
 00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ce0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d10: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016d20: 5f72 6164 6975 732e 6170 7065 6e64 284e  _radius.append(N
-00016d30: 6f6e 6529 2020 2020 2020 2020 2020 0d0a  one)          ..
-00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d60: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00016d70: 7469 635f 7370 6565 642e 6170 7065 6e64  tic_speed.append
-00016d80: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00016d90: 735b 6b5d 5b73 656c 662e 7370 6565 645f  s[k][self.speed_
-00016da0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00016cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016ce0: 2020 2020 2020 616c 6c5f 6469 7370 5f7a        all_disp_z
+00016cf0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016d00: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00016d10: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
+00016d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d30: 616c 6c5f 6469 7370 5f78 203d 205b 5d0d  all_disp_x = [].
+00016d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d50: 2020 2020 2061 6c6c 5f72 6164 6975 7320       all_radius 
+00016d60: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016d70: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
+00016d80: 6565 6420 3d20 5b5d 0d0a 2020 2020 2020  eed = []..      
+00016d90: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00016da0: 6c5f 6163 6320 3d20 5b5d 0d0a 2020 2020  l_acc = []..    
 00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dc0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016dd0: 6f6e 5f6d 6974 6f74 6963 5f61 6363 2e61  on_mitotic_acc.a
-00016de0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00016df0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e61  tracks[k][self.a
-00016e00: 6363 656c 6572 6174 696f 6e5f 6b65 795d  cceleration_key]
-00016e10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00016e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e30: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016e40: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-00016e50: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-00016e60: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00016e70: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
-00016e80: 5f61 6e67 6c65 5f6b 6579 5d29 0d0a 2020  _angle_key])..  
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016eb0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00016ec0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00016ed0: 6d61 736b 2e61 7070 656e 6428 616c 6c5f  mask.append(all_
-00016ee0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00016ef0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-00016f00: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a0d  ll_mask_key])...
-00016f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f30: 2020 2061 6c6c 5f64 6973 705f 7a2e 6170     all_disp_z.ap
-00016f40: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00016f50: 7261 636b 735b 6b5d 5b73 656c 662e 7a70  racks[k][self.zp
-00016f60: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00016dc0: 616c 6c5f 6469 7265 6374 696f 6e61 6c5f  all_directional_
+00016dd0: 6368 616e 6765 203d 205b 5d0d 0a20 2020  change = []..   
+00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016df0: 2061 6c6c 5f64 6973 7461 6e63 655f 6365   all_distance_ce
+00016e00: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a  ll_mask = []....
+00016e10: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00016e20: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+00016e30: 2c76 2920 696e 2061 6c6c 5f73 706f 7473  ,v) in all_spots
+00016e40: 5f74 7261 636b 732e 6974 656d 7328 293a  _tracks.items():
+00016e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016e60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00016e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e80: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00016e90: 656e 745f 7469 6d65 203d 2061 6c6c 5f73  ent_time = all_s
+00016ea0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00016eb0: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+00016ec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016ed0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00016ee0: 746f 7469 6320 3d20 616c 6c5f 7370 6f74  totic = all_spot
+00016ef0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00016f00: 2e64 6976 6964 696e 675f 6b65 795d 0d0a  .dividing_key]..
+00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00016f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f40: 2020 2020 2020 2020 2069 6620 6920 3d3d           if i ==
+00016f50: 2069 6e74 2863 7572 7265 6e74 5f74 696d   int(current_tim
+00016f60: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
 00016f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f80: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00016f90: 6c5f 6469 7370 5f79 2e61 7070 656e 6428  l_disp_y.append(
-00016fa0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016fb0: 5b6b 5d5b 7365 6c66 2e79 706f 7369 645f  [k][self.yposid_
-00016fc0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fe0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00016ff0: 705f 782e 6170 7065 6e64 2861 6c6c 5f73  p_x.append(all_s
-00017000: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017010: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
-00017020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 2020 6966 2061 6c6c 5f73 706f 7473      if all_spots
-00017050: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017060: 7261 6469 7573 5f6b 6579 5d20 3e20 303a  radius_key] > 0:
-00017070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017090: 2020 2020 2020 2020 616c 6c5f 7261 6469          all_radi
-000170a0: 7573 2e61 7070 656e 6428 616c 6c5f 7370  us.append(all_sp
-000170b0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-000170c0: 6c66 2e72 6164 6975 735f 6b65 795d 290d  lf.radius_key]).
-000170d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170f0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017120: 616c 6c5f 7261 6469 7573 2e61 7070 656e  all_radius.appen
-00017130: 6428 4e6f 6e65 2920 2020 2020 2020 0d0a  d(None)       ..
-00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017160: 2020 616c 6c5f 7370 6565 642e 6170 7065    all_speed.appe
-00017170: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017180: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
-00017190: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-000171a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171b0: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
-000171c0: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
-000171d0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-000171e0: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-000171f0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00016f80: 2020 2020 2020 2069 6620 6d69 746f 7469         if mitoti
+00016f90: 633a 0d0a 2020 2020 2020 2020 2020 2020  c:..            
+00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fb0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00016fc0: 7469 635f 6469 7370 5f7a 2e61 7070 656e  tic_disp_z.appen
+00016fd0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00016fe0: 6b73 5b6b 5d5b 7365 6c66 2e7a 706f 7369  ks[k][self.zposi
+00016ff0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00017000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017020: 206d 6974 6f74 6963 5f64 6973 705f 792e   mitotic_disp_y.
+00017030: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017040: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017050: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
+00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017080: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00017090: 7370 5f78 2e61 7070 656e 6428 616c 6c5f  sp_x.append(all_
+000170a0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000170b0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+000170c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170e0: 2020 2020 2020 2020 2020 2069 6620 616c             if al
+000170f0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017100: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
+00017110: 795d 203e 2030 3a0d 0a20 2020 2020 2020  y] > 0:..       
+00017120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017140: 2020 2020 6d69 746f 7469 635f 7261 6469      mitotic_radi
+00017150: 7573 2e61 7070 656e 6428 616c 6c5f 7370  us.append(all_sp
+00017160: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017170: 6c66 2e72 6164 6975 735f 6b65 795d 290d  lf.radius_key]).
+00017180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171a0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171d0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+000171e0: 6963 5f72 6164 6975 732e 6170 7065 6e64  ic_radius.append
+000171f0: 284e 6f6e 6529 2020 2020 2020 200d 0a20  (None)       .. 
 00017200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017210: 2020 2020 2020 2020 2061 6c6c 5f64 6972           all_dir
-00017220: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00017230: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017240: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017250: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
-00017260: 5d29 2020 200d 0a20 2020 2020 2020 2020  ])   ..         
+00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017220: 2020 2020 2020 206d 6974 6f74 6963 5f73         mitotic_s
+00017230: 7065 6564 2e61 7070 656e 6428 616c 6c5f  peed.append(all_
+00017240: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017250: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
+00017260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017280: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00017290: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-000172a0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-000172b0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-000172c0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000172d0: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
+00017280: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00017290: 635f 6163 632e 6170 7065 6e64 2861 6c6c  c_acc.append(all
+000172a0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+000172b0: 5b73 656c 662e 6163 6365 6c65 7261 7469  [self.accelerati
+000172c0: 6f6e 5f6b 6579 5d29 0d0a 2020 2020 2020  on_key])..      
+000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017300: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017320: 6d69 746f 7469 635f 6469 7370 5f7a 203d  mitotic_disp_z =
-00017330: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-00017340: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
-00017350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017360: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00017370: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
-00017380: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
-00017390: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-000173a0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-000173b0: 7469 635f 6469 7370 5f78 203d 206e 702e  tic_disp_x = np.
-000173c0: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
-000173d0: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017400: 6469 7370 5f7a 203d 206e 702e 6162 7328  disp_z = np.abs(
-00017410: 6e70 2e64 6966 6628 6e6f 6e5f 6d69 746f  np.diff(non_mito
-00017420: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
-00017430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017440: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00017450: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
-00017460: 2e64 6966 6628 6e6f 6e5f 6d69 746f 7469  .diff(non_mitoti
-00017470: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
-00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017490: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-000174a0: 5f78 203d 206e 702e 6162 7328 6e70 2e64  _x = np.abs(np.d
-000174b0: 6966 6628 6e6f 6e5f 6d69 746f 7469 635f  iff(non_mitotic_
-000174c0: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
+000172f0: 2020 6d69 746f 7469 635f 6469 7265 6374    mitotic_direct
+00017300: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
+00017310: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017320: 6163 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74  acks[k][self.mot
+00017330: 696f 6e5f 616e 676c 655f 6b65 795d 290d  ion_angle_key]).
+00017340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017360: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00017370: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00017380: 6173 6b2e 6170 7065 6e64 2861 6c6c 5f73  ask.append(all_s
+00017390: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000173a0: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
+000173b0: 6c5f 6d61 736b 5f6b 6579 5d29 0d0a 0d0a  l_mask_key])....
+000173c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173e0: 2020 2020 6966 206e 6f74 206d 6974 6f74      if not mitot
+000173f0: 6963 3a0d 0a20 2020 2020 2020 2020 2020  ic:..           
+00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017410: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00017420: 5f6d 6974 6f74 6963 5f64 6973 705f 7a2e  _mitotic_disp_z.
+00017430: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017440: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017450: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
+00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017480: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017490: 635f 6469 7370 5f79 2e61 7070 656e 6428  c_disp_y.append(
+000174a0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000174b0: 5b6b 5d5b 7365 6c66 2e79 706f 7369 645f  [k][self.yposid_
+000174c0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
 000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 616c 6c5f 6469 7370 5f7a 203d 206e 702e  all_disp_z = np.
-000174f0: 6162 7328 6e70 2e64 6966 6628 616c 6c5f  abs(np.diff(all_
-00017500: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00017510: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00017520: 6c5f 6469 7370 5f79 203d 206e 702e 6162  l_disp_y = np.ab
-00017530: 7328 6e70 2e64 6966 6628 616c 6c5f 6469  s(np.diff(all_di
-00017540: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-00017550: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017560: 6469 7370 5f78 203d 206e 702e 6162 7328  disp_x = np.abs(
-00017570: 6e70 2e64 6966 6628 616c 6c5f 6469 7370  np.diff(all_disp
-00017580: 5f78 2929 0d0a 0d0a 0d0a 2020 2020 2020  _x))......      
+000174e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000174f0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00017500: 782e 6170 7065 6e64 2861 6c6c 5f73 706f  x.append(all_spo
+00017510: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017520: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
+00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017550: 2020 2020 2020 2020 6966 2061 6c6c 5f73          if all_s
+00017560: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017570: 656c 662e 7261 6469 7573 5f6b 6579 5d20  elf.radius_key] 
+00017580: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
 00017590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000175c0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-000175d0: 652e 6170 7065 6e64 2869 202a 2073 656c  e.append(i * sel
-000175e0: 662e 7463 616c 6962 7261 7469 6f6e 290d  f.tcalibration).
-000175f0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00017600: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00017610: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00017620: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
-00017630: 286d 6974 6f74 6963 5f64 6973 705f 7a29  (mitotic_disp_z)
-00017640: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017650: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00017660: 7469 635f 7661 725f 6469 7370 5f7a 2e61  tic_var_disp_z.a
-00017670: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00017680: 6f74 6963 5f64 6973 705f 7a29 290d 0a0d  otic_disp_z))...
-00017690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000176a0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000176b0: 635f 6d65 616e 5f64 6973 705f 792e 6170  c_mean_disp_y.ap
-000176c0: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-000176d0: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
+000175b0: 2020 6e6f 6e5f 6d69 746f 7469 635f 7261    non_mitotic_ra
+000175c0: 6469 7573 2e61 7070 656e 6428 616c 6c5f  dius.append(all_
+000175d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000175e0: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+000175f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017610: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00017620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00017650: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
+00017660: 2e61 7070 656e 6428 4e6f 6e65 2920 2020  .append(None)   
+00017670: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176a0: 206e 6f6e 5f6d 6974 6f74 6963 5f73 7065   non_mitotic_spe
+000176b0: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
+000176c0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000176d0: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
 000176e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176f0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00017700: 7661 725f 6469 7370 5f79 2e61 7070 656e  var_disp_y.appen
-00017710: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00017720: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
-00017730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017740: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00017750: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
-00017760: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-00017770: 5f64 6973 705f 7829 290d 0a20 2020 2020  _disp_x))..     
-00017780: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017790: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-000177a0: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
-000177b0: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
-000177c0: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
-000177d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000177e0: 662e 6d69 746f 7469 635f 6d65 616e 5f72  f.mitotic_mean_r
-000177f0: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00017800: 6d65 616e 286d 6974 6f74 6963 5f72 6164  mean(mitotic_rad
-00017810: 6975 7329 290d 0a20 2020 2020 2020 2020  ius))..         
-00017820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017830: 6d69 746f 7469 635f 7661 725f 7261 6469  mitotic_var_radi
-00017840: 7573 2e61 7070 656e 6428 6e70 2e73 7464  us.append(np.std
-00017850: 286d 6974 6f74 6963 5f72 6164 6975 7329  (mitotic_radius)
-00017860: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017870: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00017880: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017890: 662e 6d69 746f 7469 635f 6d65 616e 5f73  f.mitotic_mean_s
-000178a0: 7065 6564 2e61 7070 656e 6428 6e70 2e6d  peed.append(np.m
-000178b0: 6561 6e28 6d69 746f 7469 635f 7370 6565  ean(mitotic_spee
-000178c0: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-000178d0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000178e0: 746f 7469 635f 7661 725f 7370 6565 642e  totic_var_speed.
-000178f0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
-00017900: 746f 7469 635f 7370 6565 6429 290d 0a0d  totic_speed))...
-00017910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017920: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00017930: 635f 6d65 616e 5f61 6363 2e61 7070 656e  c_mean_acc.appen
-00017940: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
-00017950: 635f 6163 6329 290d 0a20 2020 2020 2020  c_acc))..       
-00017960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017970: 662e 6d69 746f 7469 635f 7661 725f 6163  f.mitotic_var_ac
-00017980: 632e 6170 7065 6e64 286e 702e 7374 6428  c.append(np.std(
-00017990: 6d69 746f 7469 635f 6163 6329 290d 0a0d  mitotic_acc))...
-000179a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000179b0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000179c0: 635f 6d65 616e 5f64 6972 6563 7469 6f6e  c_mean_direction
-000179d0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-000179e0: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-000179f0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00017a00: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
-00017a10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017a20: 6d69 746f 7469 635f 7661 725f 6469 7265  mitotic_var_dire
-00017a30: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
-00017a40: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00017a50: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-00017a60: 5f63 6861 6e67 6529 290d 0a0d 0a20 2020  _change))....   
-00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a80: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00017a90: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
-00017aa0: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
-00017ab0: 6d65 616e 286d 6974 6f74 6963 5f64 6973  mean(mitotic_dis
-00017ac0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
-00017ad0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017ae0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00017af0: 7469 635f 7661 725f 6469 7374 616e 6365  tic_var_distance
-00017b00: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-00017b10: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00017b20: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00017b30: 6173 6b29 290d 0a0d 0a20 2020 2020 2020  ask))....       
-00017b40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017b50: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00017b60: 616e 5f64 6973 705f 7a2e 6170 7065 6e64  an_disp_z.append
-00017b70: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00017b80: 6f74 6963 5f64 6973 705f 7a29 290d 0a20  otic_disp_z)).. 
-00017b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ba0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00017bb0: 7469 635f 7661 725f 6469 7370 5f7a 2e61  tic_var_disp_z.a
-00017bc0: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
-00017bd0: 5f6d 6974 6f74 6963 5f64 6973 705f 7a29  _mitotic_disp_z)
-00017be0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00017bf0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00017c00: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-00017c10: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-00017c20: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00017c30: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
-00017c40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017c50: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00017c60: 7661 725f 6469 7370 5f79 2e61 7070 656e  var_disp_y.appen
-00017c70: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-00017c80: 6f74 6963 5f64 6973 705f 7929 290d 0a0d  otic_disp_y))...
-00017c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017ca0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00017cb0: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00017cc0: 782e 6170 7065 6e64 286e 702e 6d65 616e  x.append(np.mean
-00017cd0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-00017ce0: 705f 7829 290d 0a20 2020 2020 2020 2020  p_x))..         
-00017cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017d00: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00017d10: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
-00017d20: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-00017d30: 5f64 6973 705f 7829 290d 0a0d 0a20 2020  _disp_x))....   
-00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d50: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00017d60: 635f 6d65 616e 5f72 6164 6975 732e 6170  c_mean_radius.ap
-00017d70: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00017d80: 5f6d 6974 6f74 6963 5f72 6164 6975 7329  _mitotic_radius)
-00017d90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017da0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00017db0: 6d69 746f 7469 635f 7661 725f 7261 6469  mitotic_var_radi
-00017dc0: 7573 2e61 7070 656e 6428 6e70 2e73 7464  us.append(np.std
-00017dd0: 286e 6f6e 5f6d 6974 6f74 6963 5f72 6164  (non_mitotic_rad
-00017de0: 6975 7329 290d 0a0d 0a20 2020 2020 2020  ius))....       
-00017df0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017e00: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00017e10: 616e 5f73 7065 6564 2e61 7070 656e 6428  an_speed.append(
-00017e20: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
-00017e30: 7469 635f 7370 6565 6429 290d 0a20 2020  tic_speed))..   
-00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e50: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00017e60: 635f 7661 725f 7370 6565 642e 6170 7065  c_var_speed.appe
-00017e70: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-00017e80: 746f 7469 635f 7370 6565 6429 290d 0a0d  totic_speed))...
-00017e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017ea0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00017eb0: 746f 7469 635f 6d65 616e 5f61 6363 2e61  totic_mean_acc.a
-00017ec0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-00017ed0: 6e5f 6d69 746f 7469 635f 6163 6329 290d  n_mitotic_acc)).
-00017ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017ef0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00017f00: 746f 7469 635f 7661 725f 6163 632e 6170  totic_var_acc.ap
-00017f10: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-00017f20: 6d69 746f 7469 635f 6163 6329 290d 0a0d  mitotic_acc))...
-00017f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017f40: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00017f50: 746f 7469 635f 6d65 616e 5f64 6972 6563  totic_mean_direc
-00017f60: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-00017f70: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00017f80: 5f6d 6974 6f74 6963 5f64 6972 6563 7469  _mitotic_directi
-00017f90: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
-00017fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fb0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00017fc0: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
-00017fd0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
-00017fe0: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-00017ff0: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-00018000: 5f63 6861 6e67 6529 2920 0d0a 0d0a 2020  _change)) ....  
-00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018020: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00018030: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
-00018040: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-00018050: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-00018060: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-00018070: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
-00018080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018090: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-000180a0: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
-000180b0: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
-000180c0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-000180d0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-000180e0: 6d61 736b 2929 0d0a 0d0a 0d0a 2020 2020  mask))......    
-000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018100: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00018110: 7370 5f7a 2e61 7070 656e 6428 6e70 2e6d  sp_z.append(np.m
-00018120: 6561 6e28 616c 6c5f 6469 7370 5f7a 2929  ean(all_disp_z))
-00018130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018140: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00018150: 6172 5f64 6973 705f 7a2e 6170 7065 6e64  ar_disp_z.append
-00018160: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
-00018170: 5f7a 2929 0d0a 0d0a 2020 2020 2020 2020  _z))....        
-00018180: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018190: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f79  .all_mean_disp_y
-000181a0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-000181b0: 616c 6c5f 6469 7370 5f79 2929 0d0a 2020  all_disp_y))..  
-000181c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181d0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-000181e0: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-000181f0: 7374 6428 616c 6c5f 6469 7370 5f79 2929  std(all_disp_y))
-00018200: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018210: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018220: 5f6d 6561 6e5f 6469 7370 5f78 2e61 7070  _mean_disp_x.app
-00018230: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-00018240: 6469 7370 5f78 2929 0d0a 2020 2020 2020  disp_x))..      
+000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017700: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00017710: 7469 635f 6163 632e 6170 7065 6e64 2861  tic_acc.append(a
+00017720: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017730: 6b5d 5b73 656c 662e 6163 6365 6c65 7261  k][self.accelera
+00017740: 7469 6f6e 5f6b 6579 5d29 0d0a 2020 2020  tion_key])..    
+00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017770: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017780: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00017790: 6765 2e61 7070 656e 6428 616c 6c5f 7370  ge.append(all_sp
+000177a0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000177b0: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
+000177c0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000177d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000177f0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
+00017800: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+00017810: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017820: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
+00017830: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00017840: 5f6b 6579 5d29 0d0a 0d0a 2020 2020 2020  _key])....      
+00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017860: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017870: 6469 7370 5f7a 2e61 7070 656e 6428 616c  disp_z.append(al
+00017880: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017890: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
+000178a0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000178b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178c0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+000178d0: 792e 6170 7065 6e64 2861 6c6c 5f73 706f  y.append(all_spo
+000178e0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+000178f0: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
+00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017920: 2020 616c 6c5f 6469 7370 5f78 2e61 7070    all_disp_x.app
+00017930: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017940: 6163 6b73 5b6b 5d5b 7365 6c66 2e78 706f  acks[k][self.xpo
+00017950: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017970: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017980: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017990: 5b6b 5d5b 7365 6c66 2e72 6164 6975 735f  [k][self.radius_
+000179a0: 6b65 795d 203e 2030 3a0d 0a20 2020 2020  key] > 0:..     
+000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179d0: 2061 6c6c 5f72 6164 6975 732e 6170 7065   all_radius.appe
+000179e0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+000179f0: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
+00017a00: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
+00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a20: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00017a30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a50: 2020 2020 2020 2020 2061 6c6c 5f72 6164           all_rad
+00017a60: 6975 732e 6170 7065 6e64 284e 6f6e 6529  ius.append(None)
+00017a70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a90: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
+00017aa0: 7065 6564 2e61 7070 656e 6428 616c 6c5f  peed.append(all_
+00017ab0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017ac0: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
+00017ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017af0: 2020 2020 616c 6c5f 6163 632e 6170 7065      all_acc.appe
+00017b00: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017b10: 636b 735b 6b5d 5b73 656c 662e 6163 6365  cks[k][self.acce
+00017b20: 6c65 7261 7469 6f6e 5f6b 6579 5d29 0d0a  leration_key])..
+00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b50: 2020 616c 6c5f 6469 7265 6374 696f 6e61    all_directiona
+00017b60: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00017b70: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017b80: 5b6b 5d5b 7365 6c66 2e6d 6f74 696f 6e5f  [k][self.motion_
+00017b90: 616e 676c 655f 6b65 795d 2920 2020 0d0a  angle_key])   ..
+00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bc0: 2020 616c 6c5f 6469 7374 616e 6365 5f63    all_distance_c
+00017bd0: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+00017be0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017bf0: 5b6b 5d5b 7365 6c66 2e64 6973 7461 6e63  [k][self.distanc
+00017c00: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 795d  e_cell_mask_key]
+00017c10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c40: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00017c50: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00017c60: 5f64 6973 705f 7a20 3d20 6e70 2e61 6273  _disp_z = np.abs
+00017c70: 286e 702e 6469 6666 286d 6974 6f74 6963  (np.diff(mitotic
+00017c80: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
+00017c90: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017ca0: 6974 6f74 6963 5f64 6973 705f 7920 3d20  itotic_disp_y = 
+00017cb0: 6e70 2e61 6273 286e 702e 6469 6666 286d  np.abs(np.diff(m
+00017cc0: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
+00017cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017ce0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+00017cf0: 705f 7820 3d20 6e70 2e61 6273 286e 702e  p_x = np.abs(np.
+00017d00: 6469 6666 286d 6974 6f74 6963 5f64 6973  diff(mitotic_dis
+00017d10: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
+00017d20: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00017d30: 5f6d 6974 6f74 6963 5f64 6973 705f 7a20  _mitotic_disp_z 
+00017d40: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+00017d50: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+00017d60: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
+00017d70: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00017d80: 6974 6f74 6963 5f64 6973 705f 7920 3d20  itotic_disp_y = 
+00017d90: 6e70 2e61 6273 286e 702e 6469 6666 286e  np.abs(np.diff(n
+00017da0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00017db0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+00017dc0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00017dd0: 6f74 6963 5f64 6973 705f 7820 3d20 6e70  otic_disp_x = np
+00017de0: 2e61 6273 286e 702e 6469 6666 286e 6f6e  .abs(np.diff(non
+00017df0: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
+00017e00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00017e10: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+00017e20: 705f 7a20 3d20 6e70 2e61 6273 286e 702e  p_z = np.abs(np.
+00017e30: 6469 6666 2861 6c6c 5f64 6973 705f 7a29  diff(all_disp_z)
+00017e40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017e50: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+00017e60: 7920 3d20 6e70 2e61 6273 286e 702e 6469  y = np.abs(np.di
+00017e70: 6666 2861 6c6c 5f64 6973 705f 7929 290d  ff(all_disp_y)).
+00017e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017e90: 2020 2020 2061 6c6c 5f64 6973 705f 7820       all_disp_x 
+00017ea0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+00017eb0: 2861 6c6c 5f64 6973 705f 7829 290d 0a0d  (all_disp_x))...
+00017ec0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ee0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f00: 2073 656c 662e 7469 6d65 2e61 7070 656e   self.time.appen
+00017f10: 6428 6920 2a20 7365 6c66 2e74 6361 6c69  d(i * self.tcali
+00017f20: 6272 6174 696f 6e29 0d0a 0d0a 0d0a 2020  bration)......  
+00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f40: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00017f50: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
+00017f60: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+00017f70: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
+00017f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f90: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00017fa0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
+00017fb0: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
+00017fc0: 7370 5f7a 2929 0d0a 0d0a 2020 2020 2020  sp_z))....      
+00017fd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017fe0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00017ff0: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+00018000: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+00018010: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+00018020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018030: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+00018040: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
+00018050: 6428 6d69 746f 7469 635f 6469 7370 5f79  d(mitotic_disp_y
+00018060: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018070: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018080: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00018090: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
+000180a0: 6e28 6d69 746f 7469 635f 6469 7370 5f78  n(mitotic_disp_x
+000180b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000180c0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+000180d0: 6f74 6963 5f76 6172 5f64 6973 705f 782e  otic_var_disp_x.
+000180e0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+000180f0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+00018100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018110: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018120: 6963 5f6d 6561 6e5f 7261 6469 7573 2e61  ic_mean_radius.a
+00018130: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00018140: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
+00018150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018160: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018170: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
+00018180: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00018190: 635f 7261 6469 7573 2929 0d0a 2020 2020  c_radius))..    
+000181a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000181c0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000181d0: 6963 5f6d 6561 6e5f 7370 6565 642e 6170  ic_mean_speed.ap
+000181e0: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
+000181f0: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
+00018200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018210: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00018220: 6172 5f73 7065 6564 2e61 7070 656e 6428  ar_speed.append(
+00018230: 6e70 2e73 7464 286d 6974 6f74 6963 5f73  np.std(mitotic_s
+00018240: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
 00018250: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018260: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-00018270: 782e 6170 7065 6e64 286e 702e 7374 6428  x.append(np.std(
-00018280: 616c 6c5f 6469 7370 5f78 2929 0d0a 0d0a  all_disp_x))....
-00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182a0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-000182b0: 6e5f 7261 6469 7573 2e61 7070 656e 6428  n_radius.append(
-000182c0: 6e70 2e6d 6561 6e28 616c 6c5f 7261 6469  np.mean(all_radi
-000182d0: 7573 2929 0d0a 2020 2020 2020 2020 2020  us))..          
-000182e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000182f0: 6c6c 5f76 6172 5f72 6164 6975 732e 6170  ll_var_radius.ap
-00018300: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00018310: 7261 6469 7573 2929 0d0a 0d0a 2020 2020  radius))....    
-00018320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018330: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7370  self.all_mean_sp
-00018340: 6565 642e 6170 7065 6e64 286e 702e 6d65  eed.append(np.me
-00018350: 616e 2861 6c6c 5f73 7065 6564 2929 0d0a  an(all_speed))..
-00018360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018370: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00018380: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
-00018390: 2e73 7464 2861 6c6c 5f73 7065 6564 2929  .std(all_speed))
-000183a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000183b0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-000183c0: 5f6d 6561 6e5f 6163 632e 6170 7065 6e64  _mean_acc.append
-000183d0: 286e 702e 6d65 616e 2861 6c6c 5f61 6363  (np.mean(all_acc
-000183e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000183f0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018400: 5f76 6172 5f61 6363 2e61 7070 656e 6428  _var_acc.append(
-00018410: 6e70 2e73 7464 2861 6c6c 5f61 6363 2929  np.std(all_acc))
-00018420: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
-00018430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018440: 2e61 6c6c 5f6d 6561 6e5f 6469 7265 6374  .all_mean_direct
-00018450: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
-00018460: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-00018470: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018480: 6765 2929 0d0a 2020 2020 2020 2020 2020  ge))..          
-00018490: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000184a0: 6c6c 5f76 6172 5f64 6972 6563 7469 6f6e  ll_var_direction
-000184b0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-000184c0: 286e 702e 7374 6428 616c 6c5f 6469 7265  (np.std(all_dire
-000184d0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
-000184e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000184f0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00018500: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
-00018510: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
-00018520: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7374  np.mean(all_dist
-00018530: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-00018540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018550: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00018560: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
-00018570: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
-00018580: 7374 6428 616c 6c5f 6469 7374 616e 6365  std(all_distance
-00018590: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
-000185a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000185c0: 2020 2020 0d0a 6465 6620 626f 756e 6461      ..def bounda
-000185d0: 7279 5f70 6f69 6e74 7328 6d61 736b 2c20  ry_points(mask, 
-000185e0: 7863 616c 6962 7261 7469 6f6e 2c20 7963  xcalibration, yc
-000185f0: 616c 6962 7261 7469 6f6e 2c20 7a63 616c  alibration, zcal
-00018600: 6962 7261 7469 6f6e 293a 0d0a 0d0a 2020  ibration):....  
-00018610: 2020 6e64 696d 203d 206c 656e 286d 6173    ndim = len(mas
-00018620: 6b2e 7368 6170 6529 0d0a 2020 2020 7469  k.shape)..    ti
-00018630: 6d65 645f 6d61 736b 203d 207b 7d0d 0a20  med_mask = {}.. 
-00018640: 2020 206d 6173 6b20 3d20 6d61 736b 203e     mask = mask >
-00018650: 2030 0d0a 2020 2020 6d61 736b 203d 206d   0..    mask = m
-00018660: 6173 6b2e 6173 7479 7065 2827 7569 6e74  ask.astype('uint
-00018670: 3827 290d 0a20 2020 2023 2059 5820 7368  8')..    # YX sh
-00018680: 6170 6564 206f 626a 6563 740d 0a20 2020  aped object..   
-00018690: 2069 6620 6e64 696d 203d 3d20 323a 0d0a   if ndim == 2:..
-000186a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000186b0: 2020 626f 756e 6461 7279 203d 2066 696e    boundary = fin
-000186c0: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
-000186d0: 6b29 0d0a 2020 2020 2020 2020 7265 6769  k)..        regi
-000186e0: 6f6e 6365 6e74 726f 6964 203d 2028 302c  oncentroid = (0,
-000186f0: 2920 2b20 636f 6d70 7574 655f 6365 6e74  ) + compute_cent
-00018700: 726f 6964 2862 6f75 6e64 6172 7929 200d  roid(boundary) .
-00018710: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
-00018720: 203d 206e 702e 7768 6572 6528 626f 756e   = np.where(boun
-00018730: 6461 7279 203e 2030 290d 0a20 2020 2020  dary > 0)..     
-00018740: 2020 2072 6561 6c5f 696e 6469 6365 7320     real_indices 
-00018750: 3d20 6e70 2e74 7261 6e73 706f 7365 286e  = np.transpose(n
-00018760: 702e 6173 6172 7261 7928 696e 6469 6365  p.asarray(indice
-00018770: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
-00018780: 7433 3229 292e 636f 7079 2829 0d0a 0d0a  t32)).copy()....
-00018790: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
-000187a0: 2072 616e 6765 2830 2c20 6c65 6e28 7265   range(0, len(re
-000187b0: 616c 5f69 6e64 6963 6573 2929 3a0d 0a0d  al_indices)):...
-000187c0: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
-000187d0: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
-000187e0: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-000187f0: 5d5b 305d 202a 2079 6361 6c69 6272 6174  ][0] * ycalibrat
-00018800: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00018810: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00018820: 5b31 5d20 3d20 7265 616c 5f69 6e64 6963  [1] = real_indic
-00018830: 6573 5b6a 5d5b 315d 202a 2078 6361 6c69  es[j][1] * xcali
-00018840: 6272 6174 696f 6e0d 0a0d 0a20 2020 2020  bration....     
-00018850: 2020 2074 7265 6520 3d20 7370 6174 6961     tree = spatia
-00018860: 6c2e 634b 4454 7265 6528 7265 616c 5f69  l.cKDTree(real_i
-00018870: 6e64 6963 6573 290d 0a20 2020 2020 2020  ndices)..       
-00018880: 2023 2054 6869 7320 6f62 6a65 6374 2063   # This object c
-00018890: 6f6e 7461 696e 7320 6c69 7374 206f 6620  ontains list of 
-000188a0: 616c 6c20 7468 6520 706f 696e 7473 2066  all the points f
-000188b0: 6f72 2061 6c6c 2074 6865 206c 6162 656c  or all the label
-000188c0: 7320 696e 2074 6865 204d 6173 6b20 696d  s in the Mask im
-000188d0: 6167 6520 7769 7468 2074 6865 206c 6162  age with the lab
-000188e0: 656c 2069 6420 616e 6420 766f 6c75 6d65  el id and volume
-000188f0: 206f 6620 6561 6368 206c 6162 656c 0d0a   of each label..
-00018900: 2020 2020 2020 2020 7469 6d65 645f 6d61          timed_ma
-00018910: 736b 5b73 7472 2830 295d 203d 205b 7472  sk[str(0)] = [tr
-00018920: 6565 2c20 696e 6469 6365 732c 2072 6567  ee, indices, reg
-00018930: 696f 6e63 656e 7472 6f69 645d 0d0a 0d0a  ioncentroid]....
-00018940: 2020 2020 2320 5459 5820 7368 6170 6564      # TYX shaped
-00018950: 206f 626a 6563 740d 0a20 2020 2069 6620   object..    if 
-00018960: 6e64 696d 203d 3d20 333a 0d0a 0d0a 0d0a  ndim == 3:......
-00018970: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00018980: 2074 7164 6d28 7261 6e67 6528 302c 206d   tqdm(range(0, m
-00018990: 6173 6b2e 7368 6170 655b 305d 2929 3a0d  ask.shape[0])):.
-000189a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000189c0: 2020 2062 6f75 6e64 6172 7920 3d20 6669     boundary = fi
-000189d0: 6e64 5f62 6f75 6e64 6172 6965 7328 6d61  nd_boundaries(ma
-000189e0: 736b 5b69 2c3a 5d29 0d0a 2020 2020 2020  sk[i,:])..      
-000189f0: 2020 2020 2020 2020 2020 7265 6769 6f6e            region
-00018a00: 6365 6e74 726f 6964 203d 2028 302c 2920  centroid = (0,) 
-00018a10: 2b20 636f 6d70 7574 655f 6365 6e74 726f  + compute_centro
-00018a20: 6964 2862 6f75 6e64 6172 7929 200d 0a20  id(boundary) .. 
-00018a30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00018a40: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
-00018a50: 6528 626f 756e 6461 7279 203e 2030 290d  e(boundary > 0).
-00018a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018a70: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
-00018a80: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
-00018a90: 6173 6172 7261 7928 696e 6469 6365 732c  asarray(indices,
-00018aa0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00018ab0: 3229 292e 636f 7079 2829 0d0a 0d0a 2020  2)).copy()....  
-00018ac0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00018ad0: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
-00018ae0: 6c65 6e28 7265 616c 5f69 6e64 6963 6573  len(real_indices
-00018af0: 2929 3a0d 0a0d 0a20 2020 2020 2020 2020  )):....         
-00018b00: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-00018b10: 696e 6469 6365 735b 6a5d 5b30 5d20 3d20  indices[j][0] = 
-00018b20: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00018b30: 305d 202a 2079 6361 6c69 6272 6174 696f  0] * ycalibratio
-00018b40: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00018b50: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-00018b60: 6365 735b 6a5d 5b31 5d20 3d20 7265 616c  ces[j][1] = real
-00018b70: 5f69 6e64 6963 6573 5b6a 5d5b 315d 202a  _indices[j][1] *
-00018b80: 2078 6361 6c69 6272 6174 696f 6e0d 0a0d   xcalibration...
-00018b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ba0: 2074 7265 6520 3d20 7370 6174 6961 6c2e   tree = spatial.
-00018bb0: 634b 4454 7265 6528 7265 616c 5f69 6e64  cKDTree(real_ind
-00018bc0: 6963 6573 290d 0a0d 0a20 2020 2020 2020  ices)....       
-00018bd0: 2020 2020 2020 2020 2074 696d 6564 5f6d           timed_m
-00018be0: 6173 6b5b 7374 7228 6929 5d20 3d20 5b74  ask[str(i)] = [t
-00018bf0: 7265 652c 2069 6e64 6963 6573 2c20 7265  ree, indices, re
-00018c00: 6769 6f6e 6365 6e74 726f 6964 5d0d 0a20  gioncentroid].. 
-00018c10: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00018c20: 2023 2054 5a59 5820 7368 6170 6564 206f   # TZYX shaped o
-00018c30: 626a 6563 740d 0a20 2020 2069 6620 6e64  bject..    if nd
-00018c40: 696d 203d 3d20 343a 0d0a 2020 2020 2020  im == 4:..      
-00018c50: 2020 7072 696e 7428 274d 6173 6b73 206d    print('Masks m
-00018c60: 6164 6520 696e 746f 2061 2034 4420 6379  ade into a 4D cy
-00018c70: 6c69 6e64 6572 2c20 7570 2729 0d0a 2020  linder, up')..  
-00018c80: 2020 2020 2020 626f 756e 6461 7279 203d        boundary =
-00018c90: 206e 702e 7a65 726f 7328 0d0a 2020 2020   np.zeros(..    
-00018ca0: 2020 2020 2020 2020 5b6d 6173 6b2e 7368          [mask.sh
-00018cb0: 6170 655b 305d 2c20 6d61 736b 2e73 6861  ape[0], mask.sha
-00018cc0: 7065 5b31 5d2c 206d 6173 6b2e 7368 6170  pe[1], mask.shap
-00018cd0: 655b 325d 2c20 6d61 736b 2e73 6861 7065  e[2], mask.shape
-00018ce0: 5b33 5d5d 0d0a 2020 2020 2020 2020 290d  [3]]..        ).
-00018cf0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-00018d00: 6e20 7261 6e67 6528 302c 206d 6173 6b2e  n range(0, mask.
-00018d10: 7368 6170 655b 305d 293a 0d0a 2020 2020  shape[0]):..    
-00018d20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00018d30: 2020 2020 2020 626f 756e 6461 7279 5b69        boundary[i
-00018d40: 2c3a 5d20 3d20 6669 6e64 5f62 6f75 6e64  ,:] = find_bound
-00018d50: 6172 6965 7328 6d61 736b 5b69 2c3a 5d29  aries(mask[i,:])
-00018d60: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00018d70: 6769 6f6e 6365 6e74 726f 6964 203d 2063  gioncentroid = c
-00018d80: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
-00018d90: 626f 756e 6461 7279 5b69 2c3a 5d29 200d  boundary[i,:]) .
-00018da0: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
-00018db0: 6963 6573 203d 206e 702e 7768 6572 6528  ices = np.where(
-00018dc0: 626f 756e 6461 7279 5b69 2c3a 5d20 3e20  boundary[i,:] > 
-00018dd0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-00018de0: 7265 616c 5f69 6e64 6963 6573 203d 206e  real_indices = n
-00018df0: 702e 7472 616e 7370 6f73 6528 6e70 2e61  p.transpose(np.a
-00018e00: 7361 7272 6179 2869 6e64 6963 6573 2c20  sarray(indices, 
-00018e10: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00018e20: 2929 2e63 6f70 7928 290d 0a0d 0a20 2020  )).copy()....   
-00018e30: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00018e40: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
-00018e50: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
-00018e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018e70: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-00018e80: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
-00018e90: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
-00018ea0: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
-00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ec0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
-00018ed0: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
-00018ee0: 6365 735b 6a5d 5b31 5d20 2a20 7963 616c  ces[j][1] * ycal
-00018ef0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00018f00: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00018f10: 616c 5f69 6e64 6963 6573 5b6a 5d5b 325d  al_indices[j][2]
-00018f20: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-00018f30: 6a5d 5b32 5d20 2a20 7863 616c 6962 7261  j][2] * xcalibra
-00018f40: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
-00018f50: 2020 2020 7472 6565 203d 2073 7061 7469      tree = spati
-00018f60: 616c 2e63 4b44 5472 6565 2872 6561 6c5f  al.cKDTree(real_
-00018f70: 696e 6469 6365 7329 0d0a 2020 2020 2020  indices)..      
-00018f80: 2020 2020 2020 7469 6d65 645f 6d61 736b        timed_mask
-00018f90: 5b73 7472 2869 295d 203d 205b 7472 6565  [str(i)] = [tree
-00018fa0: 2c20 696e 6469 6365 732c 2072 6567 696f  , indices, regio
-00018fb0: 6e63 656e 7472 6f69 645d 0d0a 2020 2020  ncentroid]..    
-00018fc0: 7072 696e 7428 2743 6f6d 7075 7465 6420  print('Computed 
-00018fd0: 7468 6520 626f 756e 6461 7279 2070 6f69  the boundary poi
-00018fe0: 6e74 7327 290d 0a0d 0a20 2020 2072 6574  nts')....    ret
-00018ff0: 7572 6e20 7469 6d65 645f 6d61 736b 2c20  urn timed_mask, 
-00019000: 626f 756e 6461 7279 2020 2020 2020 2020  boundary        
-00019010: 0d0a 0d0a 6465 6620 636f 6d70 7574 655f  ....def compute_
-00019020: 6365 6e74 726f 6964 2862 696e 6172 795f  centroid(binary_
-00019030: 696d 6167 6529 3a0d 0a20 2020 2023 2045  image):..    # E
-00019040: 6e73 7572 6520 6269 6e61 7279 2069 6d61  nsure binary ima
-00019050: 6765 2069 7320 6120 4e75 6d50 7920 6172  ge is a NumPy ar
-00019060: 7261 790d 0a20 2020 2062 696e 6172 795f  ray..    binary_
-00019070: 696d 6167 6520 3d20 6e70 2e61 7272 6179  image = np.array
-00019080: 2862 696e 6172 795f 696d 6167 6529 0d0a  (binary_image)..
-00019090: 0d0a 2020 2020 7768 6974 655f 7069 7865  ..    white_pixe
-000190a0: 6c73 203d 206e 702e 7768 6572 6528 6269  ls = np.where(bi
-000190b0: 6e61 7279 5f69 6d61 6765 203d 3d20 3129  nary_image == 1)
-000190c0: 0d0a 2020 2020 6e75 6d5f 7069 7865 6c73  ..    num_pixels
-000190d0: 203d 206c 656e 2877 6869 7465 5f70 6978   = len(white_pix
-000190e0: 656c 735b 305d 290d 0a0d 0a20 2020 2023  els[0])....    #
-000190f0: 2043 6f6d 7075 7465 2074 6865 2063 656e   Compute the cen
-00019100: 7472 6f69 6420 6f66 2074 6865 2077 6869  troid of the whi
-00019110: 7465 2070 6978 656c 7320 696e 2074 6865  te pixels in the
-00019120: 2062 6f75 6e64 6172 7920 696d 6167 650d   boundary image.
-00019130: 0a20 2020 2063 656e 7472 6f69 6420 3d20  .    centroid = 
-00019140: 6e70 2e7a 6572 6f73 2862 696e 6172 795f  np.zeros(binary_
-00019150: 696d 6167 652e 6e64 696d 290d 0a20 2020  image.ndim)..   
-00019160: 2066 6f72 2064 696d 2069 6e20 7261 6e67   for dim in rang
-00019170: 6528 6269 6e61 7279 5f69 6d61 6765 2e6e  e(binary_image.n
-00019180: 6469 6d29 3a0d 0a20 2020 2020 2020 2063  dim):..        c
-00019190: 656e 7472 6f69 645b 6469 6d5d 203d 2077  entroid[dim] = w
-000191a0: 6869 7465 5f70 6978 656c 735b 6469 6d5d  hite_pixels[dim]
-000191b0: 2e73 756d 2829 202f 206e 756d 5f70 6978  .sum() / num_pix
-000191c0: 656c 730d 0a0d 0a20 2020 2072 6574 7572  els....    retur
-000191d0: 6e20 6365 6e74 726f 6964 0d0a 0d0a 0d0a  n centroid......
-000191e0: 0d0a 200d 0a0d 0a64 6566 2067 6574 5f63  .. ....def get_c
-000191f0: 7376 5f64 6174 6128 6373 7629 3a0d 0a0d  sv_data(csv):...
-00019200: 0a20 2020 2020 2020 2064 6174 6173 6574  .        dataset
-00019210: 203d 2070 642e 7265 6164 5f63 7376 280d   = pd.read_csv(.
-00019220: 0a20 2020 2020 2020 2020 2020 2063 7376  .            csv
-00019230: 2c20 6465 6c69 6d69 7465 723d 222c 222c  , delimiter=",",
-00019240: 2065 6e63 6f64 696e 673d 2275 6e69 636f   encoding="unico
-00019250: 6465 5f65 7363 6170 6522 2c20 6c6f 775f  de_escape", low_
-00019260: 6d65 6d6f 7279 3d46 616c 7365 0d0a 2020  memory=False..  
-00019270: 2020 2020 2020 295b 333a 5d0d 0a20 2020        )[3:]..   
-00019280: 2020 2020 2064 6174 6173 6574 5f69 6e64       dataset_ind
-00019290: 6578 203d 2064 6174 6173 6574 2e69 6e64  ex = dataset.ind
-000192a0: 6578 0d0a 2020 2020 2020 2020 7265 7475  ex..        retu
-000192b0: 726e 2064 6174 6173 6574 2c20 6461 7461  rn dataset, data
-000192c0: 7365 745f 696e 6465 780d 0a20 2020 200d  set_index..    .
-000192d0: 0a64 6566 2067 6574 5f73 706f 745f 6461  .def get_spot_da
-000192e0: 7461 7365 7428 7370 6f74 5f64 6174 6173  taset(spot_datas
-000192f0: 6574 2c20 7472 6163 6b5f 616e 616c 7973  et, track_analys
-00019300: 6973 5f73 706f 745f 6b65 7973 2c20 7863  is_spot_keys, xc
-00019310: 616c 6962 7261 7469 6f6e 2c20 7963 616c  alibration, ycal
-00019320: 6962 7261 7469 6f6e 2c20 7a63 616c 6962  ibration, zcalib
-00019330: 7261 7469 6f6e 2c20 4174 7472 6962 7574  ration, Attribut
-00019340: 6542 6f78 6e61 6d65 2c20 6465 7465 6374  eBoxname, detect
-00019350: 696f 6e63 6861 6e6e 656c 293a 0d0a 2020  ionchannel):..  
-00019360: 2020 2020 2020 416c 6c56 616c 7565 7320        AllValues 
-00019370: 3d20 7b7d 0d0a 2020 2020 2020 2020 706f  = {}..        po
-00019380: 7369 7820 3d20 7472 6163 6b5f 616e 616c  six = track_anal
-00019390: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-000193a0: 706f 7369 7822 5d0d 0a20 2020 2020 2020  posix"]..       
-000193b0: 2070 6f73 6979 203d 2074 7261 636b 5f61   posiy = track_a
-000193c0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-000193d0: 735b 2270 6f73 6979 225d 0d0a 2020 2020  s["posiy"]..    
-000193e0: 2020 2020 706f 7369 7a20 3d20 7472 6163      posiz = trac
-000193f0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00019400: 6b65 7973 5b22 706f 7369 7a22 5d0d 0a20  keys["posiz"].. 
-00019410: 2020 2020 2020 2066 7261 6d65 203d 2074         frame = t
-00019420: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00019430: 6f74 5f6b 6579 735b 2266 7261 6d65 225d  ot_keys["frame"]
-00019440: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00019450: 2020 2020 4c6f 6361 7469 6f6e 5820 3d20      LocationX = 
-00019460: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-00019470: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
-00019480: 785d 2e61 7374 7970 6528 2266 6c6f 6174  x].astype("float
-00019490: 2229 202f 2078 6361 6c69 6272 6174 696f  ") / xcalibratio
-000194a0: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
-000194b0: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
-000194c0: 2020 2020 4c6f 6361 7469 6f6e 5920 3d20      LocationY = 
-000194d0: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-000194e0: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
-000194f0: 795d 2e61 7374 7970 6528 2266 6c6f 6174  y].astype("float
-00019500: 2229 202f 2079 6361 6c69 6272 6174 696f  ") / ycalibratio
-00019510: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
-00019520: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
-00019530: 2020 2020 4c6f 6361 7469 6f6e 5a20 3d20      LocationZ = 
-00019540: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-00019550: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
-00019560: 7a5d 2e61 7374 7970 6528 2266 6c6f 6174  z].astype("float
-00019570: 2229 202f 207a 6361 6c69 6272 6174 696f  ") / zcalibratio
-00019580: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
-00019590: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
-000195a0: 2020 2020 4c6f 6361 7469 6f6e 5420 3d20      LocationT = 
-000195b0: 2873 706f 745f 6461 7461 7365 745b 6672  (spot_dataset[fr
-000195c0: 616d 655d 2e61 7374 7970 6528 2266 6c6f  ame].astype("flo
-000195d0: 6174 2229 292e 6173 7479 7065 2822 696e  at")).astype("in
-000195e0: 7422 290d 0a20 2020 2020 2020 200d 0a0d  t")..        ...
-000195f0: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
-00019600: 7661 6c75 6573 203d 205b 7472 6163 6b5f  values = [track_
-00019610: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-00019620: 7973 5b22 6d65 616e 5f69 6e74 656e 7369  ys["mean_intensi
-00019630: 7479 225d 2c74 7261 636b 5f61 6e61 6c79  ty"],track_analy
-00019640: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
-00019650: 6f74 616c 5f69 6e74 656e 7369 7479 225d  otal_intensity"]
-00019660: 5d0d 0a20 2020 2020 2020 2066 6f72 2028  ]..        for (
-00019670: 6b2c 7629 2069 6e20 7472 6163 6b5f 616e  k,v) in track_an
-00019680: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00019690: 2e69 7465 6d73 2829 3a0d 0a0d 0a20 2020  .items():....   
-000196a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000196b0: 6465 7465 6374 696f 6e63 6861 6e6e 656c  detectionchannel
-000196c0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
-000196d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000196e0: 6b20 3d3d 2022 6d65 616e 5f69 6e74 656e  k == "mean_inten
-000196f0: 7369 7479 5f63 6832 223a 0d0a 2020 2020  sity_ch2":..    
-00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019710: 2020 2020 2020 2076 616c 7565 203d 2074         value = t
-00019720: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00019730: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
-00019740: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
-00019750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019760: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-00019770: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
-00019780: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
-00019790: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
-000197a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000197b0: 6620 6b20 3d3d 2022 746f 7461 6c5f 696e  f k == "total_in
-000197c0: 7465 6e73 6974 795f 6368 3222 3a0d 0a20  tensity_ch2":.. 
-000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197e0: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
-000197f0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-00019800: 5f73 706f 745f 6b65 7973 5b22 746f 7461  _spot_keys["tota
-00019810: 6c5f 696e 7465 6e73 6974 7922 5d0d 0a20  l_intensity"].. 
-00019820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019830: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
-00019840: 7565 735b 7661 6c75 655d 203d 2073 706f  ues[value] = spo
-00019850: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
-00019860: 7970 6528 2266 6c6f 6174 2229 2020 2020  ype("float")    
-00019870: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-00019880: 2020 2020 2020 2069 6620 7620 6e6f 7420         if v not 
-00019890: 696e 2069 676e 6f72 655f 7661 6c75 6573  in ignore_values
-000198a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000198b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198d0: 2020 2041 6c6c 5661 6c75 6573 5b76 5d20     AllValues[v] 
-000198e0: 3d20 7370 6f74 5f64 6174 6173 6574 5b76  = spot_dataset[v
-000198f0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-00019900: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019910: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00019920: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
-00019930: 785d 203d 2072 6f75 6e64 284c 6f63 6174  x] = round(Locat
-00019940: 696f 6e58 2c33 290d 0a20 2020 2020 2020  ionX,3)..       
-00019950: 2041 6c6c 5661 6c75 6573 5b70 6f73 6979   AllValues[posiy
-00019960: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
-00019970: 6f6e 592c 3329 0d0a 2020 2020 2020 2020  onY,3)..        
-00019980: 416c 6c56 616c 7565 735b 706f 7369 7a5d  AllValues[posiz]
-00019990: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
-000199a0: 6e5a 2c33 290d 0a20 2020 2020 2020 2041  nZ,3)..        A
-000199b0: 6c6c 5661 6c75 6573 5b66 7261 6d65 5d20  llValues[frame] 
-000199c0: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
-000199d0: 542c 3329 0d0a 2020 2020 2020 2020 4174  T,3)..        At
-000199e0: 7472 6962 7574 6569 6473 203d 205b 5d0d  tributeids = [].
-000199f0: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
-00019a00: 7465 6964 732e 6170 7065 6e64 2841 7474  teids.append(Att
-00019a10: 7269 6275 7465 426f 786e 616d 6529 0d0a  ributeBoxname)..
-00019a20: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
-00019a30: 6962 7574 656e 616d 6520 696e 2041 6c6c  ibutename in All
-00019a40: 5661 6c75 6573 2e6b 6579 7328 293a 0d0a  Values.keys():..
-00019a50: 2020 2020 2020 2020 2020 2020 2020 4174                At
-00019a60: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
-00019a70: 6428 6174 7472 6962 7574 656e 616d 6529  d(attributename)
-00019a80: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00019a90: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
-00019aa0: 2020 2020 2020 7265 7475 726e 2041 7474        return Att
-00019ab0: 7269 6275 7465 6964 732c 2041 6c6c 5661  ributeids, AllVa
-00019ac0: 6c75 6573 2020 2020 200d 0a20 2020 200d  lues     ..    .
-00019ad0: 0a64 6566 2067 6574 5f74 7261 636b 5f64  .def get_track_d
-00019ae0: 6174 6173 6574 2874 7261 636b 5f64 6174  ataset(track_dat
-00019af0: 6173 6574 2c20 7472 6163 6b5f 616e 616c  aset, track_anal
-00019b00: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
-00019b10: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
-00019b20: 7261 636b 5f6b 6579 732c 2054 7261 636b  rack_keys, Track
-00019b30: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
-00019b40: 293a 0d0a 0d0a 2020 2020 2020 2020 416c  ):....        Al
-00019b50: 6c54 7261 636b 5661 6c75 6573 203d 207b  lTrackValues = {
-00019b60: 7d0d 0a20 2020 2020 2020 2074 7261 636b  }..        track
-00019b70: 5f69 6420 3d20 7472 6163 6b5f 616e 616c  _id = track_anal
-00019b80: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-00019b90: 7472 6163 6b5f 6964 225d 0d0a 2020 2020  track_id"]..    
-00019ba0: 2020 2020 5469 6420 3d20 7472 6163 6b5f      Tid = track_
-00019bb0: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
-00019bc0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-00019bd0: 290d 0a20 2020 2020 2020 0d0a 2020 2020  )..       ..    
-00019be0: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
-00019bf0: 6573 5b74 7261 636b 5f69 645d 203d 2054  es[track_id] = T
-00019c00: 6964 0d0a 2020 2020 2020 0d0a 2020 2020  id..      ..    
-00019c10: 2020 2020 666f 7220 286b 2c20 7629 2069      for (k, v) i
-00019c20: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
-00019c30: 5f74 7261 636b 5f6b 6579 732e 6974 656d  _track_keys.item
-00019c40: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
-00019c50: 2020 2020 2020 2020 7820 3d20 7472 6163          x = trac
-00019c60: 6b5f 6461 7461 7365 745b 765d 2e61 7374  k_dataset[v].ast
-00019c70: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-00019c80: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00019c90: 6e76 616c 203d 206d 696e 2878 290d 0a20  nval = min(x).. 
-00019ca0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00019cb0: 6178 7661 6c20 3d20 6d61 7828 7829 0d0a  axval = max(x)..
-00019cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019cd0: 2020 6966 206d 696e 7661 6c20 3e20 3020    if minval > 0 
-00019ce0: 616e 6420 6d61 7876 616c 203c 3d20 313a  and maxval <= 1:
-00019cf0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019d00: 2020 2020 2020 2020 7820 3d20 7820 2b20          x = x + 
-00019d10: 310d 0a0d 0a20 2020 2020 2020 2020 2020  1....           
-00019d20: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
-00019d30: 7565 735b 6b5d 203d 2072 6f75 6e64 2878  ues[k] = round(x
-00019d40: 2c20 3329 0d0a 0d0a 2020 2020 2020 2020  , 3)....        
-00019d50: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
-00019d60: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00019d70: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
-00019d80: 732e 6170 7065 6e64 2854 7261 636b 4174  s.append(TrackAt
-00019d90: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
-00019da0: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
-00019db0: 7269 6275 7465 6e61 6d65 2069 6e20 7472  ributename in tr
-00019dc0: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
-00019dd0: 636b 5f6b 6579 732e 6b65 7973 2829 3a0d  ck_keys.keys():.
-00019de0: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
-00019df0: 636b 4174 7472 6962 7574 6569 6473 2e61  ckAttributeids.a
-00019e00: 7070 656e 6428 6174 7472 6962 7574 656e  ppend(attributen
-00019e10: 616d 6529 2020 2020 0d0a 2020 2020 0d0a  ame)    ..    ..
-00019e20: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00019e30: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-00019e40: 2c20 416c 6c54 7261 636b 5661 6c75 6573  , AllTrackValues
-00019e50: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
-00019e60: 6564 6765 735f 6461 7461 7365 7428 6564  edges_dataset(ed
-00019e70: 6765 735f 6461 7461 7365 742c 2065 6467  ges_dataset, edg
-00019e80: 6573 5f64 6174 6173 6574 5f69 6e64 6578  es_dataset_index
-00019e90: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
-00019ea0: 5f73 706f 745f 6b65 7973 2c20 7472 6163  _spot_keys, trac
-00019eb0: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
-00019ec0: 5f6b 6579 7329 3a0d 0a0d 0a20 2020 2020  _keys):....     
-00019ed0: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
-00019ee0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-00019ef0: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
-00019f00: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00019f10: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
-00019f20: 0a20 2020 2020 2020 2054 6964 203d 2065  .        Tid = e
-00019f30: 6467 6573 5f64 6174 6173 6574 5b74 7261  dges_dataset[tra
-00019f40: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
-00019f50: 6c6f 6174 2229 0d0a 2020 2020 2020 2020  loat")..        
-00019f60: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
-00019f70: 7265 2854 6964 203d 3d20 3029 0d0a 2020  re(Tid == 0)..  
-00019f80: 2020 2020 2020 6d61 7874 7261 636b 5f69        maxtrack_i
-00019f90: 6420 3d20 6d61 7828 5469 6429 0d0a 2020  d = max(Tid)..  
-00019fa0: 2020 2020 2020 636f 6e64 6974 696f 6e5f        condition_
-00019fb0: 696e 6469 6365 7320 3d20 6564 6765 735f  indices = edges_
-00019fc0: 6461 7461 7365 745f 696e 6465 785b 696e  dataset_index[in
-00019fd0: 6469 6365 735d 0d0a 2020 2020 2020 2020  dices]..        
-00019fe0: 5469 645b 636f 6e64 6974 696f 6e5f 696e  Tid[condition_in
-00019ff0: 6469 6365 735d 203d 206d 6178 7472 6163  dices] = maxtrac
-0001a000: 6b5f 6964 202b 2031 0d0a 2020 2020 2020  k_id + 1..      
-0001a010: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
-0001a020: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
-0001a030: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
-0001a040: 6b20 696e 2074 7261 636b 5f61 6e61 6c79  k in track_analy
-0001a050: 7369 735f 6564 6765 735f 6b65 7973 2e76  sis_edges_keys.v
-0001a060: 616c 7565 7328 293a 0d0a 0d0a 2020 2020  alues():....    
-0001a070: 2020 2020 2020 2020 6966 206b 2021 3d20          if k != 
-0001a080: 7472 6163 6b5f 6964 3a0d 0a20 2020 2020  track_id:..     
-0001a090: 2020 2020 2020 2020 2020 2078 203d 2065             x = e
-0001a0a0: 6467 6573 5f64 6174 6173 6574 5b6b 5d2e  dges_dataset[k].
-0001a0b0: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-0001a0c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a0d0: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
-0001a0e0: 735b 6b5d 203d 2078 2020 200d 0a20 2020  s[k] = x   ..   
-0001a0f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001a100: 7265 7475 726e 2041 6c6c 4564 6765 7356  return AllEdgesV
-0001a110: 616c 7565 7320 2020 0d0a 2020 2020 0d0a  alues   ..    ..
-0001a120: 2020 2020 2020 200d 0a20 2020 200d 0a64         ..    ..d
-0001a130: 6566 2073 6361 6c65 5f76 616c 7565 2878  ef scale_value(x
-0001a140: 2c20 7363 616c 6520 3d20 3235 3520 2a20  , scale = 255 * 
-0001a150: 3235 3529 3a0d 0a0d 0a0d 0a20 2020 2020  255):......     
-0001a160: 7265 7475 726e 2078 202a 2073 6361 6c65  return x * scale
-0001a170: 2020 200d 0a20 2020 200d 0a0d 0a0d 0a64     ..    ......d
-0001a180: 6566 2070 726f 625f 7369 676d 6f69 6428  ef prob_sigmoid(
-0001a190: 7829 3a0d 0a20 2020 2072 6574 7572 6e20  x):..    return 
-0001a1a0: 3120 2d20 6d61 7468 2e65 7870 282d 7829  1 - math.exp(-x)
-0001a1b0: 0d0a 0d0a 0d0a 6465 6620 616e 6775 6c61  ......def angula
-0001a1c0: 725f 6368 616e 6765 2876 6563 5f30 2c20  r_change(vec_0, 
-0001a1d0: 7665 635f 3129 3a0d 0a20 2020 2020 2020  vec_1):..       
-0001a1e0: 200d 0a20 2020 2020 2020 2076 6563 5f30   ..        vec_0
-0001a1f0: 203d 2076 6563 5f30 202f 206e 702e 6c69   = vec_0 / np.li
-0001a200: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3029  nalg.norm(vec_0)
-0001a210: 0d0a 2020 2020 2020 2020 7665 635f 3120  ..        vec_1 
-0001a220: 3d20 7665 635f 3120 2f20 6e70 2e6c 696e  = vec_1 / np.lin
-0001a230: 616c 672e 6e6f 726d 2876 6563 5f31 290d  alg.norm(vec_1).
-0001a240: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
-0001a250: 206e 702e 6172 6363 6f73 286e 702e 636c   np.arccos(np.cl
-0001a260: 6970 286e 702e 646f 7428 7665 635f 302c  ip(np.dot(vec_0,
-0001a270: 2076 6563 5f31 292c 202d 312e 302c 2031   vec_1), -1.0, 1
-0001a280: 2e30 2929 0d0a 2020 2020 2020 2020 616e  .0))..        an
-0001a290: 676c 6520 3d20 616e 676c 6520 2a20 3138  gle = angle * 18
-0001a2a0: 3020 2f20 6e70 2e70 690d 0a20 2020 2020  0 / np.pi..     
-0001a2b0: 2020 2072 6574 7572 6e20 616e 676c 650d     return angle.
-0001a2c0: 0a20 2020 2020 0d0a 0d0a 6465 6620 6576  .     ....def ev
-0001a2d0: 616c 5f62 6f6f 6c28 7661 6c75 6529 3a0d  al_bool(value):.
-0001a2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a2f0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-0001a300: 7661 6c75 6520 203d 3d20 2754 7275 6527  value  == 'True'
-0001a310: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
-0001a320: 2020 2020 6469 765f 6b65 7920 3d20 5472      div_key = Tr
-0001a330: 7565 0d0a 2020 2020 2020 2020 656c 7365  ue..        else
-0001a340: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a350: 2020 2064 6976 5f6b 6579 203d 2046 616c     div_key = Fal
-0001a360: 7365 200d 0a0d 0a20 2020 2020 2020 2072  se ....        r
-0001a370: 6574 7572 6e20 6469 765f 6b65 7920 2020  eturn div_key   
-0001a380: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-0001a390: 0a64 6566 2063 6865 636b 5f61 6e64 5f75  .def check_and_u
-0001a3a0: 7064 6174 655f 6d61 736b 286d 6173 6b2c  pdate_mask(mask,
-0001a3b0: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
-0001a3c0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0001a3d0: 286d 6173 6b2e 7368 6170 6529 203c 206c  (mask.shape) < l
-0001a3e0: 656e 2869 6d61 6765 2e73 6861 7065 293a  en(image.shape):
-0001a3f0: 0d0a 2020 2020 2020 2020 2020 2020 7570  ..            up
-0001a400: 6461 7465 5f6d 6173 6b20 3d20 6e70 2e7a  date_mask = np.z
-0001a410: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
-0001a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a430: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
-0001a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a450: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
-0001a460: 655b 305d 2c0d 0a20 2020 2020 2020 2020  e[0],..         
-0001a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a480: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001a490: 7065 5b31 5d2c 0d0a 2020 2020 2020 2020  pe[1],..        
-0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4b0: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001a4c0: 6170 655b 325d 2c0d 0a20 2020 2020 2020  ape[2],..       
-0001a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4e0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
-0001a4f0: 6861 7065 5b33 5d2c 0d0a 2020 2020 2020  hape[3],..      
-0001a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a510: 2020 2020 2020 5d2c 2064 7479 7065 3d22        ], dtype="
-0001a520: 7569 6e74 3822 0d0a 2020 2020 2020 2020  uint8"..        
-0001a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a540: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-0001a550: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
-0001a560: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
-0001a570: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
-0001a580: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0001a590: 6e20 7261 6e67 6528 302c 2075 7064 6174  n range(0, updat
-0001a5a0: 655f 6d61 736b 2e73 6861 7065 5b31 5d29  e_mask.shape[1])
-0001a5b0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-0001a5c0: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-0001a5d0: 6d61 736b 5b69 2c20 6a2c 203a 2c20 3a5d  mask[i, j, :, :]
-0001a5e0: 203d 206d 6173 6b5b 692c 203a 2c20 3a5d   = mask[i, :, :]
-0001a5f0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0001a600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a610: 2075 7064 6174 655f 6d61 736b 203d 206d   update_mask = m
-0001a620: 6173 6b0d 0a0d 0a20 2020 2020 2020 2072  ask....        r
-0001a630: 6574 7572 6e20 7570 6461 7465 5f6d 6173  eturn update_mas
-0001a640: 6b20 2020 2020 2020 200d 0a20 2020 2020  k        ..     
-0001a650: 2020 0d0a                                  ..
+00018260: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00018270: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
+00018280: 616e 286d 6974 6f74 6963 5f61 6363 2929  an(mitotic_acc))
+00018290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000182a0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000182b0: 6963 5f76 6172 5f61 6363 2e61 7070 656e  ic_var_acc.appen
+000182c0: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
+000182d0: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
+000182e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000182f0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00018300: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00018310: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
+00018320: 6e28 6d69 746f 7469 635f 6469 7265 6374  n(mitotic_direct
+00018330: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018350: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018360: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
+00018370: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+00018380: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
+00018390: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+000183a0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000183b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000183c0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
+000183d0: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+000183e0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+000183f0: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
+00018400: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
+00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018420: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00018430: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00018440: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
+00018450: 6428 6d69 746f 7469 635f 6469 7374 616e  d(mitotic_distan
+00018460: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+00018470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018480: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018490: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+000184a0: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
+000184b0: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+000184c0: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+000184d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000184e0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+000184f0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
+00018500: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00018510: 635f 6469 7370 5f7a 2929 0d0a 0d0a 2020  c_disp_z))....  
+00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018530: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018540: 6963 5f6d 6561 6e5f 6469 7370 5f79 2e61  ic_mean_disp_y.a
+00018550: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00018560: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
+00018570: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018580: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018590: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+000185a0: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
+000185b0: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
+000185c0: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
+000185d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000185e0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+000185f0: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
+00018600: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
+00018610: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018630: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018640: 6f74 6963 5f76 6172 5f64 6973 705f 782e  otic_var_disp_x.
+00018650: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00018660: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+00018670: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018680: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018690: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+000186a0: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+000186b0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+000186c0: 635f 7261 6469 7573 2929 0d0a 2020 2020  c_radius))..    
+000186d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186e0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+000186f0: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
+00018700: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00018710: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
+00018720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018730: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018740: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
+00018750: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
+00018760: 286e 6f6e 5f6d 6974 6f74 6963 5f73 7065  (non_mitotic_spe
+00018770: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
+00018780: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018790: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f73  on_mitotic_var_s
+000187a0: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
+000187b0: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f73  td(non_mitotic_s
+000187c0: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
+000187d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000187e0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+000187f0: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
+00018800: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+00018810: 6963 5f61 6363 2929 0d0a 2020 2020 2020  ic_acc))..      
+00018820: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018830: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00018840: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
+00018850: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
+00018860: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
+00018870: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018880: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00018890: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
+000188a0: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
+000188b0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+000188c0: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+000188d0: 616e 6765 2929 0d0a 2020 2020 2020 2020  ange))..        
+000188e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000188f0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00018900: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018910: 6e67 652e 6170 7065 6e64 286e 702e 7374  nge.append(np.st
+00018920: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
+00018930: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00018940: 2929 200d 0a0d 0a20 2020 2020 2020 2020  )) ....         
+00018950: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018960: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00018970: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00018980: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
+00018990: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
+000189a0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000189b0: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
+000189c0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000189d0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+000189e0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+000189f0: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+00018a00: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
+00018a10: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+00018a20: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00018a30: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018a40: 6c5f 6d65 616e 5f64 6973 705f 7a2e 6170  l_mean_disp_z.ap
+00018a50: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+00018a60: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
+00018a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018a80: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+00018a90: 5f7a 2e61 7070 656e 6428 6e70 2e73 7464  _z.append(np.std
+00018aa0: 2861 6c6c 5f64 6973 705f 7a29 290d 0a0d  (all_disp_z))...
+00018ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018ac0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00018ad0: 616e 5f64 6973 705f 792e 6170 7065 6e64  an_disp_y.append
+00018ae0: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
+00018af0: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
+00018b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018b10: 616c 6c5f 7661 725f 6469 7370 5f79 2e61  all_var_disp_y.a
+00018b20: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00018b30: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
+00018b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b50: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+00018b60: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
+00018b70: 6d65 616e 2861 6c6c 5f64 6973 705f 7829  mean(all_disp_x)
+00018b80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018b90: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018ba0: 7661 725f 6469 7370 5f78 2e61 7070 656e  var_disp_x.appen
+00018bb0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
+00018bc0: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
+00018bd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018be0: 662e 616c 6c5f 6d65 616e 5f72 6164 6975  f.all_mean_radiu
+00018bf0: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
+00018c00: 2861 6c6c 5f72 6164 6975 7329 290d 0a20  (all_radius)).. 
+00018c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c20: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00018c30: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+00018c40: 2e73 7464 2861 6c6c 5f72 6164 6975 7329  .std(all_radius)
+00018c50: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018c60: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018c70: 6c5f 6d65 616e 5f73 7065 6564 2e61 7070  l_mean_speed.app
+00018c80: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
+00018c90: 7370 6565 6429 290d 0a20 2020 2020 2020  speed))..       
+00018ca0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018cb0: 662e 616c 6c5f 7661 725f 7370 6565 642e  f.all_var_speed.
+00018cc0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018cd0: 6c5f 7370 6565 6429 290d 0a0d 0a20 2020  l_speed))....   
+00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cf0: 2073 656c 662e 616c 6c5f 6d65 616e 5f61   self.all_mean_a
+00018d00: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
+00018d10: 6e28 616c 6c5f 6163 6329 290d 0a20 2020  n(all_acc))..   
+00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d30: 2073 656c 662e 616c 6c5f 7661 725f 6163   self.all_var_ac
+00018d40: 632e 6170 7065 6e64 286e 702e 7374 6428  c.append(np.std(
+00018d50: 616c 6c5f 6163 6329 290d 0a0d 0a0d 0a0d  all_acc)).......
+00018d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018d70: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00018d80: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
+00018d90: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+00018da0: 6d65 616e 2861 6c6c 5f64 6972 6563 7469  mean(all_directi
+00018db0: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
+00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018dd0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00018de0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00018df0: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
+00018e00: 2861 6c6c 5f64 6972 6563 7469 6f6e 616c  (all_directional
+00018e10: 5f63 6861 6e67 6529 290d 0a0d 0a20 2020  _change))....   
+00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e30: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+00018e40: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018e50: 6b2e 6170 7065 6e64 286e 702e 6d65 616e  k.append(np.mean
+00018e60: 2861 6c6c 5f64 6973 7461 6e63 655f 6365  (all_distance_ce
+00018e70: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
+00018e80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018e90: 656c 662e 616c 6c5f 7661 725f 6469 7374  elf.all_var_dist
+00018ea0: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00018eb0: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00018ec0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00018ed0: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
+00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ef0: 2020 200d 0a20 2020 2020 2020 200d 0a64     ..        ..d
+00018f00: 6566 2062 6f75 6e64 6172 795f 706f 696e  ef boundary_poin
+00018f10: 7473 286d 6173 6b2c 2078 6361 6c69 6272  ts(mask, xcalibr
+00018f20: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
+00018f30: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
+00018f40: 6e29 3a0d 0a0d 0a20 2020 206e 6469 6d20  n):....    ndim 
+00018f50: 3d20 6c65 6e28 6d61 736b 2e73 6861 7065  = len(mask.shape
+00018f60: 290d 0a20 2020 2074 696d 6564 5f6d 6173  )..    timed_mas
+00018f70: 6b20 3d20 7b7d 0d0a 2020 2020 6d61 736b  k = {}..    mask
+00018f80: 203d 206d 6173 6b20 3e20 300d 0a20 2020   = mask > 0..   
+00018f90: 206d 6173 6b20 3d20 6d61 736b 2e61 7374   mask = mask.ast
+00018fa0: 7970 6528 2775 696e 7438 2729 0d0a 2020  ype('uint8')..  
+00018fb0: 2020 2320 5958 2073 6861 7065 6420 6f62    # YX shaped ob
+00018fc0: 6a65 6374 0d0a 2020 2020 6966 206e 6469  ject..    if ndi
+00018fd0: 6d20 3d3d 2032 3a0d 0a20 2020 2020 2020  m == 2:..       
+00018fe0: 200d 0a20 2020 2020 2020 2062 6f75 6e64   ..        bound
+00018ff0: 6172 7920 3d20 6669 6e64 5f62 6f75 6e64  ary = find_bound
+00019000: 6172 6965 7328 6d61 736b 290d 0a20 2020  aries(mask)..   
+00019010: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
+00019020: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
+00019030: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
+00019040: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
+00019050: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
+00019060: 6865 7265 2862 6f75 6e64 6172 7920 3e20  here(boundary > 
+00019070: 3029 0d0a 2020 2020 2020 2020 7265 616c  0)..        real
+00019080: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
+00019090: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
+000190a0: 6179 2869 6e64 6963 6573 2c20 6474 7970  ay(indices, dtyp
+000190b0: 653d 6e70 2e66 6c6f 6174 3332 2929 2e63  e=np.float32)).c
+000190c0: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
+000190d0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+000190e0: 302c 206c 656e 2872 6561 6c5f 696e 6469  0, len(real_indi
+000190f0: 6365 7329 293a 0d0a 0d0a 2020 2020 2020  ces)):....      
+00019100: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+00019110: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
+00019120: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
+00019130: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+00019140: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
+00019150: 6e64 6963 6573 5b6a 5d5b 315d 203d 2072  ndices[j][1] = r
+00019160: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
+00019170: 5d20 2a20 7863 616c 6962 7261 7469 6f6e  ] * xcalibration
+00019180: 0d0a 0d0a 2020 2020 2020 2020 7472 6565  ....        tree
+00019190: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
+000191a0: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
+000191b0: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
+000191c0: 206f 626a 6563 7420 636f 6e74 6169 6e73   object contains
+000191d0: 206c 6973 7420 6f66 2061 6c6c 2074 6865   list of all the
+000191e0: 2070 6f69 6e74 7320 666f 7220 616c 6c20   points for all 
+000191f0: 7468 6520 6c61 6265 6c73 2069 6e20 7468  the labels in th
+00019200: 6520 4d61 736b 2069 6d61 6765 2077 6974  e Mask image wit
+00019210: 6820 7468 6520 6c61 6265 6c20 6964 2061  h the label id a
+00019220: 6e64 2076 6f6c 756d 6520 6f66 2065 6163  nd volume of eac
+00019230: 6820 6c61 6265 6c0d 0a20 2020 2020 2020  h label..       
+00019240: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
+00019250: 3029 5d20 3d20 5b74 7265 652c 2069 6e64  0)] = [tree, ind
+00019260: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
+00019270: 726f 6964 5d0d 0a0d 0a20 2020 2023 2054  roid]....    # T
+00019280: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
+00019290: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
+000192a0: 2033 3a0d 0a0d 0a0d 0a20 2020 2020 2020   3:......       
+000192b0: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
+000192c0: 616e 6765 2830 2c20 6d61 736b 2e73 6861  ange(0, mask.sha
+000192d0: 7065 5b30 5d29 293a 0d0a 2020 2020 2020  pe[0])):..      
+000192e0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000192f0: 2020 2020 2020 2020 2020 2020 626f 756e              boun
+00019300: 6461 7279 203d 2066 696e 645f 626f 756e  dary = find_boun
+00019310: 6461 7269 6573 286d 6173 6b5b 692c 3a5d  daries(mask[i,:]
+00019320: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019330: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
+00019340: 6420 3d20 2830 2c29 202b 2063 6f6d 7075  d = (0,) + compu
+00019350: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
+00019360: 6461 7279 2920 0d0a 2020 2020 2020 2020  dary) ..        
+00019370: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
+00019380: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
+00019390: 6172 7920 3e20 3029 0d0a 2020 2020 2020  ary > 0)..      
+000193a0: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
+000193b0: 6e64 6963 6573 203d 206e 702e 7472 616e  ndices = np.tran
+000193c0: 7370 6f73 6528 6e70 2e61 7361 7272 6179  spose(np.asarray
+000193d0: 2869 6e64 6963 6573 2c20 6474 7970 653d  (indices, dtype=
+000193e0: 6e70 2e66 6c6f 6174 3332 2929 2e63 6f70  np.float32)).cop
+000193f0: 7928 290d 0a0d 0a20 2020 2020 2020 2020  y()....         
+00019400: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00019410: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
+00019420: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
+00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019440: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+00019450: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
+00019460: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
+00019470: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00019480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019490: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+000194a0: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
+000194b0: 735b 6a5d 5b31 5d20 2a20 7863 616c 6962  s[j][1] * xcalib
+000194c0: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
+000194d0: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
+000194e0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+000194f0: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
+00019500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019510: 2020 7469 6d65 645f 6d61 736b 5b73 7472    timed_mask[str
+00019520: 2869 295d 203d 205b 7472 6565 2c20 696e  (i)] = [tree, in
+00019530: 6469 6365 732c 2072 6567 696f 6e63 656e  dices, regioncen
+00019540: 7472 6f69 645d 0d0a 2020 2020 2020 2020  troid]..        
+00019550: 2020 2020 0d0a 2020 2020 2320 545a 5958      ..    # TZYX
+00019560: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
+00019570: 2020 2020 6966 206e 6469 6d20 3d3d 2034      if ndim == 4
+00019580: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+00019590: 2827 4d61 736b 7320 6d61 6465 2069 6e74  ('Masks made int
+000195a0: 6f20 6120 3444 2063 796c 696e 6465 722c  o a 4D cylinder,
+000195b0: 2075 7027 290d 0a20 2020 2020 2020 2062   up')..        b
+000195c0: 6f75 6e64 6172 7920 3d20 6e70 2e7a 6572  oundary = np.zer
+000195d0: 6f73 280d 0a20 2020 2020 2020 2020 2020  os(..           
+000195e0: 205b 6d61 736b 2e73 6861 7065 5b30 5d2c   [mask.shape[0],
+000195f0: 206d 6173 6b2e 7368 6170 655b 315d 2c20   mask.shape[1], 
+00019600: 6d61 736b 2e73 6861 7065 5b32 5d2c 206d  mask.shape[2], m
+00019610: 6173 6b2e 7368 6170 655b 335d 5d0d 0a20  ask.shape[3]].. 
+00019620: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00019630: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00019640: 2830 2c20 6d61 736b 2e73 6861 7065 5b30  (0, mask.shape[0
+00019650: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+00019660: 200d 0a20 2020 2020 2020 2020 2020 2062   ..            b
+00019670: 6f75 6e64 6172 795b 692c 3a5d 203d 2066  oundary[i,:] = f
+00019680: 696e 645f 626f 756e 6461 7269 6573 286d  ind_boundaries(m
+00019690: 6173 6b5b 692c 3a5d 290d 0a20 2020 2020  ask[i,:])..     
+000196a0: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
+000196b0: 7472 6f69 6420 3d20 636f 6d70 7574 655f  troid = compute_
+000196c0: 6365 6e74 726f 6964 2862 6f75 6e64 6172  centroid(boundar
+000196d0: 795b 692c 3a5d 2920 0d0a 2020 2020 2020  y[i,:]) ..      
+000196e0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+000196f0: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
+00019700: 795b 692c 3a5d 203e 2030 290d 0a20 2020  y[i,:] > 0)..   
+00019710: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00019720: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
+00019730: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
+00019740: 696e 6469 6365 732c 2064 7479 7065 3d6e  indices, dtype=n
+00019750: 702e 666c 6f61 7433 3229 292e 636f 7079  p.float32)).copy
+00019760: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+00019770: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+00019780: 2830 2c20 6c65 6e28 7265 616c 5f69 6e64  (0, len(real_ind
+00019790: 6963 6573 2929 3a0d 0a0d 0a20 2020 2020  ices)):....     
+000197a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000197b0: 6561 6c5f 696e 6469 6365 735b 6a5d 5b30  eal_indices[j][0
+000197c0: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
+000197d0: 5b6a 5d5b 305d 202a 207a 6361 6c69 6272  [j][0] * zcalibr
+000197e0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+000197f0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
+00019800: 696e 6469 6365 735b 6a5d 5b31 5d20 3d20  indices[j][1] = 
+00019810: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+00019820: 315d 202a 2079 6361 6c69 6272 6174 696f  1] * ycalibratio
+00019830: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00019840: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+00019850: 6365 735b 6a5d 5b32 5d20 3d20 7265 616c  ces[j][2] = real
+00019860: 5f69 6e64 6963 6573 5b6a 5d5b 325d 202a  _indices[j][2] *
+00019870: 2078 6361 6c69 6272 6174 696f 6e0d 0a0d   xcalibration...
+00019880: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
+00019890: 6520 3d20 7370 6174 6961 6c2e 634b 4454  e = spatial.cKDT
+000198a0: 7265 6528 7265 616c 5f69 6e64 6963 6573  ree(real_indices
+000198b0: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
+000198c0: 696d 6564 5f6d 6173 6b5b 7374 7228 6929  imed_mask[str(i)
+000198d0: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
+000198e0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
+000198f0: 6964 5d0d 0a20 2020 2070 7269 6e74 2827  id]..    print('
+00019900: 436f 6d70 7574 6564 2074 6865 2062 6f75  Computed the bou
+00019910: 6e64 6172 7920 706f 696e 7473 2729 0d0a  ndary points')..
+00019920: 0d0a 2020 2020 7265 7475 726e 2074 696d  ..    return tim
+00019930: 6564 5f6d 6173 6b2c 2062 6f75 6e64 6172  ed_mask, boundar
+00019940: 7920 2020 2020 2020 200d 0a0d 0a64 6566  y        ....def
+00019950: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
+00019960: 6428 6269 6e61 7279 5f69 6d61 6765 293a  d(binary_image):
+00019970: 0d0a 2020 2020 2320 456e 7375 7265 2062  ..    # Ensure b
+00019980: 696e 6172 7920 696d 6167 6520 6973 2061  inary image is a
+00019990: 204e 756d 5079 2061 7272 6179 0d0a 2020   NumPy array..  
+000199a0: 2020 6269 6e61 7279 5f69 6d61 6765 203d    binary_image =
+000199b0: 206e 702e 6172 7261 7928 6269 6e61 7279   np.array(binary
+000199c0: 5f69 6d61 6765 290d 0a0d 0a20 2020 2077  _image)....    w
+000199d0: 6869 7465 5f70 6978 656c 7320 3d20 6e70  hite_pixels = np
+000199e0: 2e77 6865 7265 2862 696e 6172 795f 696d  .where(binary_im
+000199f0: 6167 6520 3d3d 2031 290d 0a20 2020 206e  age == 1)..    n
+00019a00: 756d 5f70 6978 656c 7320 3d20 6c65 6e28  um_pixels = len(
+00019a10: 7768 6974 655f 7069 7865 6c73 5b30 5d29  white_pixels[0])
+00019a20: 0d0a 0d0a 2020 2020 2320 436f 6d70 7574  ....    # Comput
+00019a30: 6520 7468 6520 6365 6e74 726f 6964 206f  e the centroid o
+00019a40: 6620 7468 6520 7768 6974 6520 7069 7865  f the white pixe
+00019a50: 6c73 2069 6e20 7468 6520 626f 756e 6461  ls in the bounda
+00019a60: 7279 2069 6d61 6765 0d0a 2020 2020 6365  ry image..    ce
+00019a70: 6e74 726f 6964 203d 206e 702e 7a65 726f  ntroid = np.zero
+00019a80: 7328 6269 6e61 7279 5f69 6d61 6765 2e6e  s(binary_image.n
+00019a90: 6469 6d29 0d0a 2020 2020 666f 7220 6469  dim)..    for di
+00019aa0: 6d20 696e 2072 616e 6765 2862 696e 6172  m in range(binar
+00019ab0: 795f 696d 6167 652e 6e64 696d 293a 0d0a  y_image.ndim):..
+00019ac0: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
+00019ad0: 5b64 696d 5d20 3d20 7768 6974 655f 7069  [dim] = white_pi
+00019ae0: 7865 6c73 5b64 696d 5d2e 7375 6d28 2920  xels[dim].sum() 
+00019af0: 2f20 6e75 6d5f 7069 7865 6c73 0d0a 0d0a  / num_pixels....
+00019b00: 2020 2020 7265 7475 726e 2063 656e 7472      return centr
+00019b10: 6f69 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a  oid........ ....
+00019b20: 6465 6620 6765 745f 6373 765f 6461 7461  def get_csv_data
+00019b30: 2863 7376 293a 0d0a 0d0a 2020 2020 2020  (csv):....      
+00019b40: 2020 6461 7461 7365 7420 3d20 7064 2e72    dataset = pd.r
+00019b50: 6561 645f 6373 7628 0d0a 2020 2020 2020  ead_csv(..      
+00019b60: 2020 2020 2020 6373 762c 2064 656c 696d        csv, delim
+00019b70: 6974 6572 3d22 2c22 2c20 656e 636f 6469  iter=",", encodi
+00019b80: 6e67 3d22 756e 6963 6f64 655f 6573 6361  ng="unicode_esca
+00019b90: 7065 222c 206c 6f77 5f6d 656d 6f72 793d  pe", low_memory=
+00019ba0: 4661 6c73 650d 0a20 2020 2020 2020 2029  False..        )
+00019bb0: 5b33 3a5d 0d0a 2020 2020 2020 2020 6461  [3:]..        da
+00019bc0: 7461 7365 745f 696e 6465 7820 3d20 6461  taset_index = da
+00019bd0: 7461 7365 742e 696e 6465 780d 0a20 2020  taset.index..   
+00019be0: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
+00019bf0: 7365 742c 2064 6174 6173 6574 5f69 6e64  set, dataset_ind
+00019c00: 6578 0d0a 2020 2020 0d0a 6465 6620 6765  ex..    ..def ge
+00019c10: 745f 7370 6f74 5f64 6174 6173 6574 2873  t_spot_dataset(s
+00019c20: 706f 745f 6461 7461 7365 742c 2074 7261  pot_dataset, tra
+00019c30: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00019c40: 5f6b 6579 732c 2078 6361 6c69 6272 6174  _keys, xcalibrat
+00019c50: 696f 6e2c 2079 6361 6c69 6272 6174 696f  ion, ycalibratio
+00019c60: 6e2c 207a 6361 6c69 6272 6174 696f 6e2c  n, zcalibration,
+00019c70: 2041 7474 7269 6275 7465 426f 786e 616d   AttributeBoxnam
+00019c80: 652c 2064 6574 6563 7469 6f6e 6368 616e  e, detectionchan
+00019c90: 6e65 6c29 3a0d 0a20 2020 2020 2020 2041  nel):..        A
+00019ca0: 6c6c 5661 6c75 6573 203d 207b 7d0d 0a20  llValues = {}.. 
+00019cb0: 2020 2020 2020 2070 6f73 6978 203d 2074         posix = t
+00019cc0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00019cd0: 6f74 5f6b 6579 735b 2270 6f73 6978 225d  ot_keys["posix"]
+00019ce0: 0d0a 2020 2020 2020 2020 706f 7369 7920  ..        posiy 
+00019cf0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+00019d00: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
+00019d10: 7922 5d0d 0a20 2020 2020 2020 2070 6f73  y"]..        pos
+00019d20: 697a 203d 2074 7261 636b 5f61 6e61 6c79  iz = track_analy
+00019d30: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
+00019d40: 6f73 697a 225d 0d0a 2020 2020 2020 2020  osiz"]..        
+00019d50: 6672 616d 6520 3d20 7472 6163 6b5f 616e  frame = track_an
+00019d60: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00019d70: 5b22 6672 616d 6522 5d0d 0a20 2020 2020  ["frame"]..     
+00019d80: 2020 200d 0a20 2020 2020 2020 204c 6f63     ..        Loc
+00019d90: 6174 696f 6e58 203d 2028 0d0a 2020 2020  ationX = (..    
+00019da0: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
+00019db0: 6173 6574 5b70 6f73 6978 5d2e 6173 7479  aset[posix].asty
+00019dc0: 7065 2822 666c 6f61 7422 2920 2f20 7863  pe("float") / xc
+00019dd0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00019de0: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
+00019df0: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
+00019e00: 6174 696f 6e59 203d 2028 0d0a 2020 2020  ationY = (..    
+00019e10: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
+00019e20: 6173 6574 5b70 6f73 6979 5d2e 6173 7479  aset[posiy].asty
+00019e30: 7065 2822 666c 6f61 7422 2920 2f20 7963  pe("float") / yc
+00019e40: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00019e50: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
+00019e60: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
+00019e70: 6174 696f 6e5a 203d 2028 0d0a 2020 2020  ationZ = (..    
+00019e80: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
+00019e90: 6173 6574 5b70 6f73 697a 5d2e 6173 7479  aset[posiz].asty
+00019ea0: 7065 2822 666c 6f61 7422 2920 2f20 7a63  pe("float") / zc
+00019eb0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00019ec0: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
+00019ed0: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
+00019ee0: 6174 696f 6e54 203d 2028 7370 6f74 5f64  ationT = (spot_d
+00019ef0: 6174 6173 6574 5b66 7261 6d65 5d2e 6173  ataset[frame].as
+00019f00: 7479 7065 2822 666c 6f61 7422 2929 2e61  type("float")).a
+00019f10: 7374 7970 6528 2269 6e74 2229 0d0a 2020  stype("int")..  
+00019f20: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00019f30: 2020 6967 6e6f 7265 5f76 616c 7565 7320    ignore_values 
+00019f40: 3d20 5b74 7261 636b 5f61 6e61 6c79 7369  = [track_analysi
+00019f50: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
+00019f60: 6e5f 696e 7465 6e73 6974 7922 5d2c 7472  n_intensity"],tr
+00019f70: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+00019f80: 745f 6b65 7973 5b22 746f 7461 6c5f 696e  t_keys["total_in
+00019f90: 7465 6e73 6974 7922 5d5d 0d0a 2020 2020  tensity"]]..    
+00019fa0: 2020 2020 666f 7220 286b 2c76 2920 696e      for (k,v) in
+00019fb0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+00019fc0: 7370 6f74 5f6b 6579 732e 6974 656d 7328  spot_keys.items(
+00019fd0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+00019fe0: 2020 2020 2020 6966 2064 6574 6563 7469        if detecti
+00019ff0: 6f6e 6368 616e 6e65 6c20 3d3d 2031 3a0d  onchannel == 1:.
+0001a000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a010: 2020 2020 2020 6966 206b 203d 3d20 226d        if k == "m
+0001a020: 6561 6e5f 696e 7465 6e73 6974 795f 6368  ean_intensity_ch
+0001a030: 3222 3a0d 0a20 2020 2020 2020 2020 2020  2":..           
+0001a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a050: 7661 6c75 6520 3d20 7472 6163 6b5f 616e  value = track_an
+0001a060: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001a070: 5b22 6d65 616e 5f69 6e74 656e 7369 7479  ["mean_intensity
+0001a080: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+0001a090: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0001a0a0: 6c6c 5661 6c75 6573 5b76 616c 7565 5d20  llValues[value] 
+0001a0b0: 3d20 7370 6f74 5f64 6174 6173 6574 5b76  = spot_dataset[v
+0001a0c0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+0001a0d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a0e0: 2020 2020 2020 2020 6966 206b 203d 3d20          if k == 
+0001a0f0: 2274 6f74 616c 5f69 6e74 656e 7369 7479  "total_intensity
+0001a100: 5f63 6832 223a 0d0a 2020 2020 2020 2020  _ch2":..        
+0001a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a120: 2020 2076 616c 7565 203d 2074 7261 636b     value = track
+0001a130: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001a140: 6579 735b 2274 6f74 616c 5f69 6e74 656e  eys["total_inten
+0001a150: 7369 7479 225d 0d0a 2020 2020 2020 2020  sity"]..        
+0001a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a170: 2020 2041 6c6c 5661 6c75 6573 5b76 616c     AllValues[val
+0001a180: 7565 5d20 3d20 7370 6f74 5f64 6174 6173  ue] = spot_datas
+0001a190: 6574 5b76 5d2e 6173 7479 7065 2822 666c  et[v].astype("fl
+0001a1a0: 6f61 7422 2920 2020 2020 2020 0d0a 0d0a  oat")       ....
+0001a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1c0: 6966 2076 206e 6f74 2069 6e20 6967 6e6f  if v not in igno
+0001a1d0: 7265 5f76 616c 7565 733a 0d0a 2020 2020  re_values:..    
+0001a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0001a200: 2020 2020 2020 2020 2020 2020 416c 6c56              AllV
+0001a210: 616c 7565 735b 765d 203d 2073 706f 745f  alues[v] = spot_
+0001a220: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
+0001a230: 6528 2266 6c6f 6174 2229 0d0a 2020 2020  e("float")..    
+0001a240: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0001a250: 0a0d 0a20 2020 2020 2020 2041 6c6c 5661  ...        AllVa
+0001a260: 6c75 6573 5b70 6f73 6978 5d20 3d20 726f  lues[posix] = ro
+0001a270: 756e 6428 4c6f 6361 7469 6f6e 582c 3329  und(LocationX,3)
+0001a280: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
+0001a290: 7565 735b 706f 7369 795d 203d 2072 6f75  ues[posiy] = rou
+0001a2a0: 6e64 284c 6f63 6174 696f 6e59 2c33 290d  nd(LocationY,3).
+0001a2b0: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
+0001a2c0: 6573 5b70 6f73 697a 5d20 3d20 726f 756e  es[posiz] = roun
+0001a2d0: 6428 4c6f 6361 7469 6f6e 5a2c 3329 0d0a  d(LocationZ,3)..
+0001a2e0: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+0001a2f0: 735b 6672 616d 655d 203d 2072 6f75 6e64  s[frame] = round
+0001a300: 284c 6f63 6174 696f 6e54 2c33 290d 0a20  (LocationT,3).. 
+0001a310: 2020 2020 2020 2041 7474 7269 6275 7465         Attribute
+0001a320: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
+0001a330: 2020 4174 7472 6962 7574 6569 6473 2e61    Attributeids.a
+0001a340: 7070 656e 6428 4174 7472 6962 7574 6542  ppend(AttributeB
+0001a350: 6f78 6e61 6d65 290d 0a20 2020 2020 2020  oxname)..       
+0001a360: 2066 6f72 2061 7474 7269 6275 7465 6e61   for attributena
+0001a370: 6d65 2069 6e20 416c 6c56 616c 7565 732e  me in AllValues.
+0001a380: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
+0001a390: 2020 2020 2020 2041 7474 7269 6275 7465         Attribute
+0001a3a0: 6964 732e 6170 7065 6e64 2861 7474 7269  ids.append(attri
+0001a3b0: 6275 7465 6e61 6d65 2920 2020 200d 0a20  butename)    .. 
+0001a3c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0001a3d0: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
+0001a3e0: 6574 7572 6e20 4174 7472 6962 7574 6569  eturn Attributei
+0001a3f0: 6473 2c20 416c 6c56 616c 7565 7320 2020  ds, AllValues   
+0001a400: 2020 0d0a 2020 2020 0d0a 6465 6620 6765    ..    ..def ge
+0001a410: 745f 7472 6163 6b5f 6461 7461 7365 7428  t_track_dataset(
+0001a420: 7472 6163 6b5f 6461 7461 7365 742c 2074  track_dataset, t
+0001a430: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001a440: 6f74 5f6b 6579 732c 2074 7261 636b 5f61  ot_keys, track_a
+0001a450: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+0001a460: 7973 2c20 5472 6163 6b41 7474 7269 6275  ys, TrackAttribu
+0001a470: 7465 426f 786e 616d 6529 3a0d 0a0d 0a20  teBoxname):.... 
+0001a480: 2020 2020 2020 2041 6c6c 5472 6163 6b56         AllTrackV
+0001a490: 616c 7565 7320 3d20 7b7d 0d0a 2020 2020  alues = {}..    
+0001a4a0: 2020 2020 7472 6163 6b5f 6964 203d 2074      track_id = t
+0001a4b0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001a4c0: 6f74 5f6b 6579 735b 2274 7261 636b 5f69  ot_keys["track_i
+0001a4d0: 6422 5d0d 0a20 2020 2020 2020 2054 6964  d"]..        Tid
+0001a4e0: 203d 2074 7261 636b 5f64 6174 6173 6574   = track_dataset
+0001a4f0: 5b74 7261 636b 5f69 645d 2e61 7374 7970  [track_id].astyp
+0001a500: 6528 2266 6c6f 6174 2229 0d0a 2020 2020  e("float")..    
+0001a510: 2020 200d 0a20 2020 2020 2020 2041 6c6c     ..        All
+0001a520: 5472 6163 6b56 616c 7565 735b 7472 6163  TrackValues[trac
+0001a530: 6b5f 6964 5d20 3d20 5469 640d 0a20 2020  k_id] = Tid..   
+0001a540: 2020 200d 0a20 2020 2020 2020 2066 6f72     ..        for
+0001a550: 2028 6b2c 2076 2920 696e 2074 7261 636b   (k, v) in track
+0001a560: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
+0001a570: 6b65 7973 2e69 7465 6d73 2829 3a0d 0a0d  keys.items():...
+0001a580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a590: 2078 203d 2074 7261 636b 5f64 6174 6173   x = track_datas
+0001a5a0: 6574 5b76 5d2e 6173 7479 7065 2822 666c  et[v].astype("fl
+0001a5b0: 6f61 7422 290d 0a20 2020 2020 2020 2020  oat")..         
+0001a5c0: 2020 2020 2020 206d 696e 7661 6c20 3d20         minval = 
+0001a5d0: 6d69 6e28 7829 0d0a 2020 2020 2020 2020  min(x)..        
+0001a5e0: 2020 2020 2020 2020 6d61 7876 616c 203d          maxval =
+0001a5f0: 206d 6178 2878 290d 0a0d 0a20 2020 2020   max(x)....     
+0001a600: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
+0001a610: 6e76 616c 203e 2030 2061 6e64 206d 6178  nval > 0 and max
+0001a620: 7661 6c20 3c3d 2031 3a0d 0a0d 0a20 2020  val <= 1:....   
+0001a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a640: 2078 203d 2078 202b 2031 0d0a 0d0a 2020   x = x + 1....  
+0001a650: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+0001a660: 6c54 7261 636b 5661 6c75 6573 5b6b 5d20  lTrackValues[k] 
+0001a670: 3d20 726f 756e 6428 782c 2033 290d 0a0d  = round(x, 3)...
+0001a680: 0a20 2020 2020 2020 2054 7261 636b 4174  .        TrackAt
+0001a690: 7472 6962 7574 6569 6473 203d 205b 5d0d  tributeids = [].
+0001a6a0: 0a20 2020 2020 2020 2054 7261 636b 4174  .        TrackAt
+0001a6b0: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
+0001a6c0: 6428 5472 6163 6b41 7474 7269 6275 7465  d(TrackAttribute
+0001a6d0: 426f 786e 616d 6529 0d0a 2020 2020 2020  Boxname)..      
+0001a6e0: 2020 666f 7220 6174 7472 6962 7574 656e    for attributen
+0001a6f0: 616d 6520 696e 2074 7261 636b 5f61 6e61  ame in track_ana
+0001a700: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
+0001a710: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+0001a720: 2020 2020 2020 5472 6163 6b41 7474 7269        TrackAttri
+0001a730: 6275 7465 6964 732e 6170 7065 6e64 2861  buteids.append(a
+0001a740: 7474 7269 6275 7465 6e61 6d65 2920 2020  ttributename)   
+0001a750: 200d 0a20 2020 200d 0a20 2020 2020 2020   ..    ..       
+0001a760: 2072 6574 7572 6e20 5472 6163 6b41 7474   return TrackAtt
+0001a770: 7269 6275 7465 6964 732c 2041 6c6c 5472  ributeids, AllTr
+0001a780: 6163 6b56 616c 7565 730d 0a20 2020 200d  ackValues..    .
+0001a790: 0a64 6566 2067 6574 5f65 6467 6573 5f64  .def get_edges_d
+0001a7a0: 6174 6173 6574 2865 6467 6573 5f64 6174  ataset(edges_dat
+0001a7b0: 6173 6574 2c20 6564 6765 735f 6461 7461  aset, edges_data
+0001a7c0: 7365 745f 696e 6465 782c 2074 7261 636b  set_index, track
+0001a7d0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001a7e0: 6579 732c 2074 7261 636b 5f61 6e61 6c79  eys, track_analy
+0001a7f0: 7369 735f 6564 6765 735f 6b65 7973 293a  sis_edges_keys):
+0001a800: 0d0a 0d0a 2020 2020 2020 2020 416c 6c45  ....        AllE
+0001a810: 6467 6573 5661 6c75 6573 203d 207b 7d0d  dgesValues = {}.
+0001a820: 0a20 2020 2020 2020 2074 7261 636b 5f69  .        track_i
+0001a830: 6420 3d20 7472 6163 6b5f 616e 616c 7973  d = track_analys
+0001a840: 6973 5f73 706f 745f 6b65 7973 5b22 7472  is_spot_keys["tr
+0001a850: 6163 6b5f 6964 225d 0d0a 2020 2020 2020  ack_id"]..      
+0001a860: 2020 5469 6420 3d20 6564 6765 735f 6461    Tid = edges_da
+0001a870: 7461 7365 745b 7472 6163 6b5f 6964 5d2e  taset[track_id].
+0001a880: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001a890: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
+0001a8a0: 203d 206e 702e 7768 6572 6528 5469 6420   = np.where(Tid 
+0001a8b0: 3d3d 2030 290d 0a20 2020 2020 2020 206d  == 0)..        m
+0001a8c0: 6178 7472 6163 6b5f 6964 203d 206d 6178  axtrack_id = max
+0001a8d0: 2854 6964 290d 0a20 2020 2020 2020 2063  (Tid)..        c
+0001a8e0: 6f6e 6469 7469 6f6e 5f69 6e64 6963 6573  ondition_indices
+0001a8f0: 203d 2065 6467 6573 5f64 6174 6173 6574   = edges_dataset
+0001a900: 5f69 6e64 6578 5b69 6e64 6963 6573 5d0d  _index[indices].
+0001a910: 0a20 2020 2020 2020 2054 6964 5b63 6f6e  .        Tid[con
+0001a920: 6469 7469 6f6e 5f69 6e64 6963 6573 5d20  dition_indices] 
+0001a930: 3d20 6d61 7874 7261 636b 5f69 6420 2b20  = maxtrack_id + 
+0001a940: 310d 0a20 2020 2020 2020 2041 6c6c 4564  1..        AllEd
+0001a950: 6765 7356 616c 7565 735b 7472 6163 6b5f  gesValues[track_
+0001a960: 6964 5d20 3d20 5469 640d 0a0d 0a20 2020  id] = Tid....   
+0001a970: 2020 2020 2066 6f72 206b 2069 6e20 7472       for k in tr
+0001a980: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
+0001a990: 6573 5f6b 6579 732e 7661 6c75 6573 2829  es_keys.values()
+0001a9a0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0001a9b0: 2069 6620 6b20 213d 2074 7261 636b 5f69   if k != track_i
+0001a9c0: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+0001a9d0: 2020 2020 7820 3d20 6564 6765 735f 6461      x = edges_da
+0001a9e0: 7461 7365 745b 6b5d 2e61 7374 7970 6528  taset[k].astype(
+0001a9f0: 2266 6c6f 6174 2229 0d0a 0d0a 2020 2020  "float")....    
+0001aa00: 2020 2020 2020 2020 2020 2020 416c 6c45              AllE
+0001aa10: 6467 6573 5661 6c75 6573 5b6b 5d20 3d20  dgesValues[k] = 
+0001aa20: 7820 2020 0d0a 2020 2020 2020 2020 200d  x   ..         .
+0001aa30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001aa40: 416c 6c45 6467 6573 5661 6c75 6573 2020  AllEdgesValues  
+0001aa50: 200d 0a20 2020 200d 0a20 2020 2020 2020   ..    ..       
+0001aa60: 0d0a 2020 2020 0d0a 6465 6620 7363 616c  ..    ..def scal
+0001aa70: 655f 7661 6c75 6528 782c 2073 6361 6c65  e_value(x, scale
+0001aa80: 203d 2032 3535 202a 2032 3535 293a 0d0a   = 255 * 255):..
+0001aa90: 0d0a 0d0a 2020 2020 2072 6574 7572 6e20  ....     return 
+0001aaa0: 7820 2a20 7363 616c 6520 2020 0d0a 2020  x * scale   ..  
+0001aab0: 2020 0d0a 0d0a 0d0a 6465 6620 7072 6f62    ......def prob
+0001aac0: 5f73 6967 6d6f 6964 2878 293a 0d0a 2020  _sigmoid(x):..  
+0001aad0: 2020 7265 7475 726e 2031 202d 206d 6174    return 1 - mat
+0001aae0: 682e 6578 7028 2d78 290d 0a0d 0a0d 0a64  h.exp(-x)......d
+0001aaf0: 6566 2061 6e67 756c 6172 5f63 6861 6e67  ef angular_chang
+0001ab00: 6528 7665 635f 302c 2076 6563 5f31 293a  e(vec_0, vec_1):
+0001ab10: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0001ab20: 2020 2020 7665 635f 3020 3d20 7665 635f      vec_0 = vec_
+0001ab30: 3020 2f20 6e70 2e6c 696e 616c 672e 6e6f  0 / np.linalg.no
+0001ab40: 726d 2876 6563 5f30 290d 0a20 2020 2020  rm(vec_0)..     
+0001ab50: 2020 2076 6563 5f31 203d 2076 6563 5f31     vec_1 = vec_1
+0001ab60: 202f 206e 702e 6c69 6e61 6c67 2e6e 6f72   / np.linalg.nor
+0001ab70: 6d28 7665 635f 3129 0d0a 2020 2020 2020  m(vec_1)..      
+0001ab80: 2020 616e 676c 6520 3d20 6e70 2e61 7263    angle = np.arc
+0001ab90: 636f 7328 6e70 2e63 6c69 7028 6e70 2e64  cos(np.clip(np.d
+0001aba0: 6f74 2876 6563 5f30 2c20 7665 635f 3129  ot(vec_0, vec_1)
+0001abb0: 2c20 2d31 2e30 2c20 312e 3029 290d 0a20  , -1.0, 1.0)).. 
+0001abc0: 2020 2020 2020 2061 6e67 6c65 203d 2061         angle = a
+0001abd0: 6e67 6c65 202a 2031 3830 202f 206e 702e  ngle * 180 / np.
+0001abe0: 7069 0d0a 2020 2020 2020 2020 7265 7475  pi..        retu
+0001abf0: 726e 2061 6e67 6c65 0d0a 2020 2020 200d  rn angle..     .
+0001ac00: 0a0d 0a64 6566 2065 7661 6c5f 626f 6f6c  ...def eval_bool
+0001ac10: 2876 616c 7565 293a 0d0a 2020 2020 2020  (value):..      
+0001ac20: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0001ac30: 2020 2020 2020 6966 2076 616c 7565 2020        if value  
+0001ac40: 3d3d 2027 5472 7565 273a 200d 0a20 2020  == 'True': ..   
+0001ac50: 2020 2020 2020 2020 2020 2020 2064 6976               div
+0001ac60: 5f6b 6579 203d 2054 7275 650d 0a20 2020  _key = True..   
+0001ac70: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0001ac80: 2020 2020 2020 2020 2020 2020 6469 765f              div_
+0001ac90: 6b65 7920 3d20 4661 6c73 6520 0d0a 0d0a  key = False ....
+0001aca0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+0001acb0: 6976 5f6b 6579 2020 2020 2020 2020 2020  iv_key          
+0001acc0: 2020 2020 2020 0d0a 0d0a 6465 6620 6368        ....def ch
+0001acd0: 6563 6b5f 616e 645f 7570 6461 7465 5f6d  eck_and_update_m
+0001ace0: 6173 6b28 6d61 736b 2c69 6d61 6765 293a  ask(mask,image):
+0001acf0: 0d0a 2020 2020 2020 200d 0a20 2020 2020  ..       ..     
+0001ad00: 2020 2069 6620 6c65 6e28 6d61 736b 2e73     if len(mask.s
+0001ad10: 6861 7065 2920 3c20 6c65 6e28 696d 6167  hape) < len(imag
+0001ad20: 652e 7368 6170 6529 3a0d 0a20 2020 2020  e.shape):..     
+0001ad30: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
+0001ad40: 736b 203d 206e 702e 7a65 726f 7328 0d0a  sk = np.zeros(..
+0001ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad60: 2020 2020 2020 2020 2020 2020 5b0d 0a20              [.. 
+0001ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001ad90: 6d61 6765 2e73 6861 7065 5b30 5d2c 0d0a  mage.shape[0],..
+0001ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001adc0: 696d 6167 652e 7368 6170 655b 315d 2c0d  image.shape[1],.
+0001add0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001adf0: 2069 6d61 6765 2e73 6861 7065 5b32 5d2c   image.shape[2],
+0001ae00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae20: 2020 696d 6167 652e 7368 6170 655b 335d    image.shape[3]
+0001ae30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001ae40: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0001ae50: 2c20 6474 7970 653d 2275 696e 7438 220d  , dtype="uint8".
+0001ae60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ae70: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+0001ae80: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0001ae90: 2072 616e 6765 2830 2c20 7570 6461 7465   range(0, update
+0001aea0: 5f6d 6173 6b2e 7368 6170 655b 305d 293a  _mask.shape[0]):
+0001aeb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001aec0: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+0001aed0: 2830 2c20 7570 6461 7465 5f6d 6173 6b2e  (0, update_mask.
+0001aee0: 7368 6170 655b 315d 293a 0d0a 0d0a 2020  shape[1]):....  
+0001aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af00: 2020 7570 6461 7465 5f6d 6173 6b5b 692c    update_mask[i,
+0001af10: 206a 2c20 3a2c 203a 5d20 3d20 6d61 736b   j, :, :] = mask
+0001af20: 5b69 2c20 3a2c 203a 5d0d 0a20 2020 2020  [i, :, :]..     
+0001af30: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0001af40: 2020 2020 2020 2020 2020 7570 6461 7465            update
+0001af50: 5f6d 6173 6b20 3d20 6d61 736b 0d0a 0d0a  _mask = mask....
+0001af60: 2020 2020 2020 2020 7265 7475 726e 2075          return u
+0001af70: 7064 6174 655f 6d61 736b 2020 2020 2020  pdate_mask      
+0001af80: 2020 0d0a 2020 2020 2020 200d 0a           ..       ..
```

### Comparing `napatrackmater-3.8.1/napatrackmater/Trackvector.py` & `napatrackmater-3.8.2/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/napatrackmater/__init__.py` & `napatrackmater-3.8.2/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/napatrackmater/clustering.py` & `napatrackmater-3.8.2/napatrackmater/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         output_largest_eigenvector = []
         output_largest_eigenvalue = []
         output_dimensions = []
         dataset = PointCloudDataset(clouds, scale_z=scale_z, scale_xy=scale_xy)
         dataloader = DataLoader(dataset, batch_size = batch_size)
         model.eval()
         print(f'Predicting {len(dataset)} clouds..., {len(centroids)} centroids...')
-        pretrainer = Trainer(accelerator=accelerator, devices=devices)
+        pretrainer = Trainer(accelerator=accelerator, devices=devices, inference_mode = True)
         outputs_list = pretrainer.predict(model=model, dataloaders=dataloader)
         output_cluster_centroid = output_cluster_centroid +  [tuple(centroid_input) for centroid_input in centroids]
         output_labels = output_labels + [int(float(label_input)) for label_input in labels]
         for outputs in outputs_list:
             output_cloud_eccentricity = output_cloud_eccentricity +  [tuple(get_eccentricity(cloud_input.detach().cpu().numpy()))[0] for cloud_input in outputs]
             output_largest_eigenvector = output_largest_eigenvector + [get_eccentricity(cloud_input.detach().cpu().numpy())[1] for cloud_input in outputs]
             output_largest_eigenvalue = output_largest_eigenvalue + [get_eccentricity(cloud_input.detach().cpu().numpy())[2] for cloud_input in outputs]
```

### Comparing `napatrackmater-3.8.1/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.8.2/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/napatrackmater/fate_mapping.py` & `napatrackmater-3.8.2/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/napatrackmater/pretrained.py` & `napatrackmater-3.8.2/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.8.2/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.1
+Version: 3.8.2
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.8.1/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.8.2/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.1/setup.py` & `napatrackmater-3.8.2/setup.py`

 * *Files identical despite different names*

