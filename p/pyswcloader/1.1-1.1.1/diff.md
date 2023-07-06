# Comparing `tmp/pyswcloader-1.1-py2.py3-none-any.whl.zip` & `tmp/pyswcloader-1.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 59133 bytes, number of entries: 17
+Zip file size: 59161 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx      366 b- defN 23-Jul-01 08:37 pyswcloader/__init__.py
 -rw-rw-r--  2.0 unx     2385 b- defN 23-Mar-06 01:56 pyswcloader/brain.py
 -rw-rw-r--  2.0 unx     2657 b- defN 23-Jan-31 03:26 pyswcloader/cluster.py
 -rw-rw-r--  2.0 unx     2890 b- defN 23-Jun-30 07:10 pyswcloader/distance.py
 -rw-rw-r--  2.0 unx      605 b- defN 23-Jul-03 04:46 pyswcloader/io.py
 -rw-rw-r--  2.0 unx     8946 b- defN 23-Jun-30 04:41 pyswcloader/projection.py
 -rw-rw-r--  2.0 unx     3477 b- defN 23-Jun-30 04:46 pyswcloader/projection_batch.py
--rw-rw-r--  2.0 unx     7419 b- defN 23-Jul-01 08:37 pyswcloader/swc.py
+-rw-rw-r--  2.0 unx     7418 b- defN 23-Jul-06 07:22 pyswcloader/swc.py
 -rw-rw-r--  2.0 unx     3432 b- defN 23-Jan-31 08:00 pyswcloader/visualization.py
 -rw-rw-r--  2.0 unx    13691 b- defN 23-Jan-28 06:56 pyswcloader/database/acro_stl_dict.pkl
 -rw-rw-r--  2.0 unx   146754 b- defN 23-Feb-14 05:50 pyswcloader/database/allen_brain_tree.pkl
 -rwxr-xr-x  2.0 unx    13691 b- defN 23-Jan-28 06:54 pyswcloader/database/stl_acro_dict.pkl
--rw-rw-r--  2.0 unx     1062 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      750 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       81 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1410 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/RECORD
-17 files, 209726 bytes uncompressed, 56825 bytes compressed:  72.9%
+-rw-rw-r--  2.0 unx     1062 b- defN 23-Jul-06 07:24 pyswcloader-1.1.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      752 b- defN 23-Jul-06 07:24 pyswcloader-1.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-06 07:24 pyswcloader-1.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jul-06 07:24 pyswcloader-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1420 b- defN 23-Jul-06 07:24 pyswcloader-1.1.1.dist-info/RECORD
+17 files, 209737 bytes uncompressed, 56833 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: pyswcloader/database/allen_brain_tree.pkl
 Comment: 
 
 Filename: pyswcloader/database/stl_acro_dict.pkl
 Comment: 
 
-Filename: pyswcloader-1.1.dist-info/LICENSE.txt
+Filename: pyswcloader-1.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pyswcloader-1.1.dist-info/METADATA
+Filename: pyswcloader-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyswcloader-1.1.dist-info/WHEEL
+Filename: pyswcloader-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyswcloader-1.1.dist-info/top_level.txt
+Filename: pyswcloader-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyswcloader-1.1.dist-info/RECORD
+Filename: pyswcloader-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyswcloader/swc.py

```diff
@@ -174,32 +174,33 @@
 
 def read_neuron_path(data_path):
     path_list = glob.glob(os.path.join(data_path, '**/*.swc'), recursive=True)
     return path_list
 
 def plot_soma_distribution(data_path, **kwargs):
     path_list = read_neuron_path(data_path)
-    soma_info = pd.DataFrame()
+    soma_info = []
     for path in tqdm(path_list):
         data = read_swc(path)
-        # soma_info = soma_info.append(data.loc[1, 'x':'z'])
-        soma_info = pd.concat([soma_info, data.loc[1, 'x':'z']], axis=0)
+        soma_info.append(np.array(data.loc[1, ['x', 'y', 'z']]))
+    soma_info = pd.DataFrame(soma_info)
+    soma_info.columns = ['x', 'y', 'z']
     fig, _ = plt.subplots(nrows=3, sharex=False, sharey=False)
     cnt = 1
     for axis in ['x', 'y', 'z']:
         plt.subplot(310+cnt)
         sns.kdeplot(list(soma_info[axis]), **kwargs)
         plt.ylabel('')
         ax = plt.gca()
         if axis == 'x':
             ax.set_title('Anterior - Posterior')
         elif axis == 'y':
             ax.set_title('Dorsal - Ventral')
         else:
-            ax.set_title('Medial - Lateral')
+            ax.set_title('Lateral - Medial')
         cnt += 1
         ax.spines['top'].set_visible(False)
         ax.spines['right'].set_visible(False)
     plt.subplots_adjust(hspace=1)
     plt.subplots_adjust(wspace=0)
     return fig
```

## Comparing `pyswcloader-1.1.dist-info/LICENSE.txt` & `pyswcloader-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pyswcloader-1.1.dist-info/METADATA` & `pyswcloader-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswcloader
-Version: 1.1
+Version: 1.1.1
 Summary: analysis tool for neuron swc files
 Home-page: https://github.com/txgxxx/pyswcloader/
 Author: tsgao
 Author-email: gaots@ion.ac.cn
 License: MIT
 Keywords: swc
 License-File: LICENSE.txt
```

## Comparing `pyswcloader-1.1.dist-info/RECORD` & `pyswcloader-1.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 pyswcloader/__init__.py,sha256=Nz1BR_F2HPd3IFEDljR7hpJaaX6TaZC1QTa0g8YeBB8,366
 pyswcloader/brain.py,sha256=8dMkpBVJ5niYRbPMKQi31pprX9K2igLMY9dCaZMjzhE,2385
 pyswcloader/cluster.py,sha256=rtkrQfufpk2BaVohQ20-rmiZdd_I3WKLtQ7f4vpsJlo,2657
 pyswcloader/distance.py,sha256=-UFgLcB81xtY2ADVq72L6Ilgfid-kDGl1GCM9-JNoAw,2890
 pyswcloader/io.py,sha256=altOMmP1IXyMAbaUz1aINcyx23GzU8UYn_LG_5RlZrA,605
 pyswcloader/projection.py,sha256=gUEH5XYAMk9MEajz0PneYAVNwVjExLi8I5USdvt0CoA,8946
 pyswcloader/projection_batch.py,sha256=juqPKzl_HgcdKreBjzKBLJ9m6cr5LkzdUDRweVeIqs0,3477
-pyswcloader/swc.py,sha256=W71B-JCXnt_YCdvZEiREj-oA31vlFE0DUNEN8X7kHCI,7419
+pyswcloader/swc.py,sha256=okM_F26yk3MQ7G-jw8JikGrsWh6x41JUZWnbdl3X2q0,7418
 pyswcloader/visualization.py,sha256=HONADF3oio27vuYfqfPFQqmc_gUkOuc8wExW4SeQ-rs,3432
 pyswcloader/database/acro_stl_dict.pkl,sha256=7MMt4HK-IXAM-AGkmv2_gXaWw8DvYJXaoptZrqJk6d0,13691
 pyswcloader/database/allen_brain_tree.pkl,sha256=Hrw7rt-LmvDkvH7i20YXttzozEY12hbPiEvKn1plcnM,146754
 pyswcloader/database/stl_acro_dict.pkl,sha256=A9IJP2lZIO-P-hconjDS2R1WgKjHily9Gd8j9pYircA,13691
-pyswcloader-1.1.dist-info/LICENSE.txt,sha256=kD2oe1i9Gq8wK3bMbliBamRR_hKEKImWBzZISNov6os,1062
-pyswcloader-1.1.dist-info/METADATA,sha256=kqYBOct0bSzqh3hSnSFHt4ZCZDHiXwKtSCwN-GbPtII,750
-pyswcloader-1.1.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
-pyswcloader-1.1.dist-info/top_level.txt,sha256=E3iDEX_8GHBgmTqDgo7zwYTv2lagnVFAnorZBnOc6yc,81
-pyswcloader-1.1.dist-info/RECORD,,
+pyswcloader-1.1.1.dist-info/LICENSE.txt,sha256=kD2oe1i9Gq8wK3bMbliBamRR_hKEKImWBzZISNov6os,1062
+pyswcloader-1.1.1.dist-info/METADATA,sha256=cmougJv0AXhKLvIYmiG3uvkSoIrOh0n1h6utQ9Z3VEc,752
+pyswcloader-1.1.1.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
+pyswcloader-1.1.1.dist-info/top_level.txt,sha256=E3iDEX_8GHBgmTqDgo7zwYTv2lagnVFAnorZBnOc6yc,81
+pyswcloader-1.1.1.dist-info/RECORD,,
```

