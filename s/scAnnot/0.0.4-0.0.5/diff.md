# Comparing `tmp/scAnnot-0.0.4.tar.gz` & `tmp/scAnnot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scAnnot-0.0.4.tar", last modified: Fri May 26 03:27:20 2023, max compression
+gzip compressed data, was "scAnnot-0.0.5.tar", last modified: Thu Jul  6 02:20:39 2023, max compression
```

## Comparing `scAnnot-0.0.4.tar` & `scAnnot-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-26 03:27:20.000000 scAnnot-0.0.4/
--rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)    11337 2023-01-20 02:50:04.000000 scAnnot-0.0.4/LICENSE
--rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)      111 2023-01-20 02:50:04.000000 scAnnot-0.0.4/MANIFEST.in
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1666 2023-05-26 03:27:20.000000 scAnnot-0.0.4/PKG-INFO
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      890 2023-05-10 13:08:24.000000 scAnnot-0.0.4/README.md
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-26 03:27:19.000000 scAnnot-0.0.4/scAnnot/
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       22 2023-05-26 03:23:53.000000 scAnnot-0.0.4/scAnnot/__init__.py
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      369 2023-05-26 03:23:54.000000 scAnnot-0.0.4/scAnnot/_modidx.py
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     3148 2023-05-26 03:23:53.000000 scAnnot-0.0.4/scAnnot/core.py
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-26 03:27:20.000000 scAnnot-0.0.4/scAnnot.egg-info/
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1666 2023-05-26 03:26:56.000000 scAnnot-0.0.4/scAnnot.egg-info/PKG-INFO
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      324 2023-05-26 03:27:12.000000 scAnnot-0.0.4/scAnnot.egg-info/SOURCES.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-05-26 03:26:56.000000 scAnnot-0.0.4/scAnnot.egg-info/dependency_links.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       86 2023-05-26 03:26:57.000000 scAnnot-0.0.4/scAnnot.egg-info/entry_points.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-03-08 02:12:46.000000 scAnnot-0.0.4/scAnnot.egg-info/not-zip-safe
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       85 2023-05-26 03:26:57.000000 scAnnot-0.0.4/scAnnot.egg-info/requires.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        8 2023-05-26 03:26:58.000000 scAnnot-0.0.4/scAnnot.egg-info/top_level.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1000 2023-05-26 03:22:04.000000 scAnnot-0.0.4/settings.ini
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       38 2023-05-26 03:27:20.000000 scAnnot-0.0.4/setup.cfg
--rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)     2560 2023-01-20 02:50:04.000000 scAnnot-0.0.4/setup.py
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-07-06 02:20:39.000000 scAnnot-0.0.5/
+-rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)    11337 2023-01-20 02:50:04.000000 scAnnot-0.0.5/LICENSE
+-rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)      111 2023-01-20 02:50:04.000000 scAnnot-0.0.5/MANIFEST.in
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1666 2023-07-06 02:20:39.000000 scAnnot-0.0.5/PKG-INFO
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      890 2023-05-10 13:08:24.000000 scAnnot-0.0.5/README.md
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-07-06 02:20:39.000000 scAnnot-0.0.5/scAnnot/
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       22 2023-07-06 02:19:02.000000 scAnnot-0.0.5/scAnnot/__init__.py
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      369 2023-07-06 02:19:02.000000 scAnnot-0.0.5/scAnnot/_modidx.py
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     3899 2023-07-06 02:19:02.000000 scAnnot-0.0.5/scAnnot/core.py
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-07-06 02:20:39.000000 scAnnot-0.0.5/scAnnot.egg-info/
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1666 2023-07-06 02:20:35.000000 scAnnot-0.0.5/scAnnot.egg-info/PKG-INFO
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      324 2023-07-06 02:20:37.000000 scAnnot-0.0.5/scAnnot.egg-info/SOURCES.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-07-06 02:20:35.000000 scAnnot-0.0.5/scAnnot.egg-info/dependency_links.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       86 2023-07-06 02:20:36.000000 scAnnot-0.0.5/scAnnot.egg-info/entry_points.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-03-08 02:12:46.000000 scAnnot-0.0.5/scAnnot.egg-info/not-zip-safe
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       85 2023-07-06 02:20:36.000000 scAnnot-0.0.5/scAnnot.egg-info/requires.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        8 2023-07-06 02:20:36.000000 scAnnot-0.0.5/scAnnot.egg-info/top_level.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1000 2023-07-06 02:17:54.000000 scAnnot-0.0.5/settings.ini
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       38 2023-07-06 02:20:39.000000 scAnnot-0.0.5/setup.cfg
+-rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)     2560 2023-01-20 02:50:04.000000 scAnnot-0.0.5/setup.py
```

### Comparing `scAnnot-0.0.4/LICENSE` & `scAnnot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scAnnot-0.0.4/PKG-INFO` & `scAnnot-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scAnnot
-Version: 0.0.4
+Version: 0.0.5
 Summary: single cell annotation
 Home-page: https://github.com/changebio/scAnnot
 Author: Yin Huang
 Author-email: changebio@yeah.net
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `scAnnot-0.0.4/README.md` & `scAnnot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `scAnnot-0.0.4/scAnnot/core.py` & `scAnnot-0.0.5/scAnnot/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['scAnnot']
+__all__ = ['model_paths', 'scAnnot']
 
 # %% ../nbs/00_core.ipynb 4
 import numpy as np
 import scanpy as sc
 import scvi
 from fastcore.script import *
+from scipy import sparse
 import warnings
 
 # %% ../nbs/00_core.ipynb 13
 @call_parse
 def scAnnot(h5:str, #the input h5ad file, must have row counts in X or layers
             output:str = None, # The path of output file. 1. None->output AnnData object with predicted labels, 2. a path end with h5ad->write out the AnnData. 3. a path end with csv-> write out the table of predicted labels. 
-            model_path='/home/huang_yin/projA/scBERT/model/twostep_2layer_subgenes/scanvi_3_epoch_model/',
-            ref_path='/home/huang_yin/projA/scBERT/model/reference_genes.h5ad',
+            model:str='Adult', # Adult and Fetal models are included. select Adult or Fetal.
             show:bool=False, #show umap plot. may not work in command line
             latent:bool=False, #add scvi latent space to anndata
            ):
+    if model in ['Adult','Fetal']:
+        sup_model_path,sub_model_path,ref_path=model_paths[model]
+    else:
+        raise(f'This {model} has not been deployed yet')
     warnings.filterwarnings("ignore")
     ad=sc.read(h5)
    
     if 'counts' not in ad.layers.keys():
         ad.layers['counts']=ad.X
     arr=ad.layers['counts'].data
     if not np.array_equal(arr, np.round(arr)):
         raise ValueError("Not all counts are integers")
-    
+    #make X to csr sparse matrix
+    ad.layers['counts']=sparse.csr_matrix(ad.layers['counts'])
     #concatenate query and ref
     ref=sc.read(ref_path)
     ref_var_idx=ref.var.index
     ad=ad[:,ad.var.index.isin(ref_var_idx)]
     print(f'{ad.shape[1]} of genes are found in ref genes (total {ref.shape[1]}). The percentage is {ad.shape[1]/ref.shape[1]}')
     ad=ad.concatenate(ref,join='outer')[:-1] #remove ref cell
+    ad=ad[:,ref.var.index] #reorder var by ref var
     ad.var['inref']=ad.var.index.isin(ref_var_idx)
     if not ad.var.index.equals(ref.var.index):
         raise ValueError("The order of gene are not the same between query and reference")
     model=scvi.model.SCANVI.load_query_data(
             ad,
-            model_path,
+            sup_model_path,
             freeze_dropout = True,
             inplace_subset_query_vars = True,
         )
     
     ad.obs['predict_level1']=model.predict()
     
     if show:
@@ -51,15 +57,15 @@
         latent=sc.AnnData(model.get_latent_representation())
           
     ad.obs['predict_level2']='unknown'
     for i in ad.obs['predict_level1'].unique():
         sub_ad=ad[ad.obs.predict_level1==i]
         model=scvi.model.SCANVI.load_query_data(
             sub_ad,
-            f'/home/huang_yin/projA/scBERT/model/twostep_2layer_subgenes/v1_scanvi_subtype_{i}/',
+            sub_model_path+f'_{i}/',
             freeze_dropout = True,
             inplace_subset_query_vars = True,
         )
         ad.obs['predict_level2'][ad.obs.predict_level1==i]=model.predict()
     if show:
         latent.obs['predict_level1']=ad.obs['predict_level1'].tolist()
         latent.obs['predict_level2']=ad.obs['predict_level2'].tolist()
@@ -74,7 +80,17 @@
             ad.obs[['predict_level1','predict_level2']].to_csv(output)
             return
         if output.split('.')[-1] in ['h5ad','h5']:
             ad.write_h5ad(output)
             return
     return ad
 
+model_paths={
+'Adult':['/home/huang_yin/projA/scBERT/model/twostep_2layer_subgenes/scanvi_3_epoch_model/',
+         '/home/huang_yin/projA/scBERT/model/twostep_2layer_subgenes/v1_scanvi_subtype',
+         '/home/huang_yin/projA/scBERT/model/reference_genes.h5ad',
+        ],
+'Fetal':['/home/huang_yin/projA/scBERT/model/twostep_2layer_subgenes/fetal_scanvi_2_epoch_model/',
+         '/home/huang_yin/projA/scBERT/model/twostep_2layer_subgenes/fetal_scanvi_subtype',
+         '/home/huang_yin/projA/scBERT/model/fetal_reference_genes.h5ad',
+        ]
+}
```

### Comparing `scAnnot-0.0.4/scAnnot.egg-info/PKG-INFO` & `scAnnot-0.0.5/scAnnot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scAnnot
-Version: 0.0.4
+Version: 0.0.5
 Summary: single cell annotation
 Home-page: https://github.com/changebio/scAnnot
 Author: Yin Huang
 Author-email: changebio@yeah.net
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `scAnnot-0.0.4/settings.ini` & `scAnnot-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = scAnnot
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = scAnnot
 nbs_path = nbs
```

### Comparing `scAnnot-0.0.4/setup.py` & `scAnnot-0.0.5/setup.py`

 * *Files identical despite different names*

