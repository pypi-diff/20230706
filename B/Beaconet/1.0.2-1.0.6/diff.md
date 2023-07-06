# Comparing `tmp/Beaconet-1.0.2-py3-none-any.whl.zip` & `tmp/Beaconet-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9370 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      106 b- defN 22-Sep-03 07:37 Beaconet/__init__.py
--rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-03 07:37 Beaconet/metrics/__init__.py
--rw-rw-rw-  2.0 fat     2810 b- defN 22-Sep-03 07:37 Beaconet/metrics/compute_LME.py
--rw-rw-rw-  2.0 fat     4745 b- defN 22-Sep-03 07:38 Beaconet/metrics/show.py
--rw-rw-rw-  2.0 fat       37 b- defN 22-Sep-02 10:23 Beaconet/model/__init__.py
--rw-rw-rw-  2.0 fat    10926 b- defN 22-Sep-03 08:23 Beaconet/model/model.py
--rw-rw-rw-  2.0 fat     1103 b- defN 22-Sep-03 08:42 Beaconet-1.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      707 b- defN 22-Sep-03 08:42 Beaconet-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-03 08:42 Beaconet-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Sep-03 08:42 Beaconet-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      879 b- defN 22-Sep-03 08:42 Beaconet-1.0.2.dist-info/RECORD
-11 files, 21506 bytes uncompressed, 7880 bytes compressed:  63.4%
+Zip file size: 9391 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      118 b- defN 23-Jul-06 07:25 Beaconet/__init__.py
+-rw-rw-rw-  2.0 fat      105 b- defN 23-Jul-06 07:25 Beaconet/metrics/__init__.py
+-rw-rw-rw-  2.0 fat     2810 b- defN 23-Jul-06 07:16 Beaconet/metrics/compute_PME.py
+-rw-rw-rw-  2.0 fat     4807 b- defN 23-Jul-06 07:29 Beaconet/metrics/show.py
+-rw-rw-rw-  2.0 fat       37 b- defN 23-Jul-06 07:03 Beaconet/model/__init__.py
+-rw-rw-rw-  2.0 fat    10770 b- defN 23-Jul-06 07:27 Beaconet/model/model.py
+-rw-rw-rw-  2.0 fat     1103 b- defN 23-Jul-06 08:26 Beaconet-1.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      645 b- defN 23-Jul-06 08:26 Beaconet-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 08:26 Beaconet-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-06 08:26 Beaconet-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      880 b- defN 23-Jul-06 08:26 Beaconet-1.0.6.dist-info/RECORD
+11 files, 21376 bytes uncompressed, 7901 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
 Filename: Beaconet/__init__.py
 Comment: 
 
 Filename: Beaconet/metrics/__init__.py
 Comment: 
 
-Filename: Beaconet/metrics/compute_LME.py
+Filename: Beaconet/metrics/compute_PME.py
 Comment: 
 
 Filename: Beaconet/metrics/show.py
 Comment: 
 
 Filename: Beaconet/model/__init__.py
 Comment: 
 
 Filename: Beaconet/model/model.py
 Comment: 
 
-Filename: Beaconet-1.0.2.dist-info/LICENSE
+Filename: Beaconet-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: Beaconet-1.0.2.dist-info/METADATA
+Filename: Beaconet-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: Beaconet-1.0.2.dist-info/WHEEL
+Filename: Beaconet-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: Beaconet-1.0.2.dist-info/top_level.txt
+Filename: Beaconet-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: Beaconet-1.0.2.dist-info/RECORD
+Filename: Beaconet-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Beaconet/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .model import Model,correction
-from .metrics import visualization,get_umap,get_lmd,visualization_lmd
+from .metrics import visualization,get_umap,get_pmd,visualization_pmd,get_cluster
```

## Beaconet/metrics/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .show import visualization,get_umap,visualization_lmd
-from .compute_LME import get_lmd
+from .show import visualization,get_umap,visualization_pmd, get_cluster
+from .compute_PME import get_pmd
```

## Beaconet/metrics/show.py

```diff
@@ -1,54 +1,53 @@
 # the necessary tools collections. some common functions is implemented here.
 from umap import UMAP
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn.decomposition import PCA
 import pandas as pd
 import seaborn as sns
+from sklearn.cluster import KMeans
 
 def _check_ndarray(emb):
     if(isinstance(emb,pd.DataFrame)):
         return emb.values
     elif(isinstance(emb,np.ndarray)):
         return emb
     else:
         raise RuntimeError(f"unknown type {type(emb)}")
 
-def visualization_lmd(emb, lmd, filename, s=1):
+def visualization_pmd(emb, pmd, filename, s=1):
     emb = _check_ndarray(emb)
-    index = pd.isna(lmd)
+    index = pd.isna(pmd)
     plt.figure()
     plt.scatter(emb[index, 0], emb[index, 1], s=s, c="red")
-    pts = plt.scatter(emb[~index, 0], emb[~index, 1], s=s, c=lmd[~index], cmap="Blues_r")
+    pts = plt.scatter(emb[~index, 0], emb[~index, 1], s=s, c=pmd[~index], cmap="Blues_r")
     plt.colorbar(pts)
 
     plt.xlabel("UMAP_1")
     plt.ylabel("UMAP_2")
-    plt.title(f"positive_rate: {lmd.notna().sum() / lmd.shape[0]:.4}")
+    plt.title(f"positive_rate: {pmd.notna().sum() / pmd.shape[0]:.4}")
     plt.tight_layout()
 
     if (filename is not None):
         plt.savefig(filename)
         plt.close()
     else:
         plt.show()
 
 
-def visualization(emb,batch_col="batch",bio_col="cell_type"):
+def visualization(emb,batch_col="batch",bio_col="cell_type",filename1="batch.png",filename2="bio.png"):
     ndarray_emb = emb[["UMAP_1", "UMAP_2"]].values
-    plot(ndarray_emb, groupby=emb["batch"].values, filename=f"batch.png",
+    plot(ndarray_emb, groupby=emb[batch_col].values, filename=filename1,
          dpi=500)
-    plot(ndarray_emb, groupby=emb["cell_type"].values,
-         filename=f"bio.png", dpi=500)
+    plot(ndarray_emb, groupby=emb[bio_col].values,
+         filename=filename2, dpi=500)
 
-def get_umap(df,meta,batch_col="batch",bio_col="cell_type"):
+def get_umap(df):
     _, emb, pc = umap(df, downsampling=None)
-    emb[batch_col] = pc[batch_col] = meta[batch_col]
-    emb[bio_col] = pc[bio_col] = meta[bio_col]
     return emb
 
 
 def umap(df,downsampling=None,n_pc=30,direct_select=False):
     """
     umap embedding that maps a high-dimensional data into 2-dimensional space.
     For the data that does not distinguish the information abundance in each dimension, it first maps the data to
@@ -141,7 +140,13 @@
 
     plt.tight_layout()
     if (filename is not None):
         plt.savefig(filename,dpi=dpi)
         plt.close()
     else:
         plt.show()
+
+def get_cluster(X,k):
+    if(X.shape[1]>30):
+        X=ump=get_umap(X)
+
+    return KMeans(n_clusters=k,n_init=100).fit_predict(X)
```

## Beaconet/model/model.py

```diff
@@ -204,18 +204,14 @@
 class Generator(nn.Module):
     def __init__(self,n_features,n_batches,d_model=512,eps=1e-8):
         super(Generator,self).__init__()
 
         self.fc=nn.Sequential(
             nn.Linear(n_features,d_model),
             nn.LeakyReLU(0.1),
-            # nn.Linear(d_model, d_model),
-            # nn.LeakyReLU(0.1),
-            # nn.Linear(d_model, d_model),
-            # nn.LeakyReLU(0.1),
             nn.Linear(d_model, d_model),
             nn.LeakyReLU(0.1),
             nn.Linear(d_model, n_features),
             nn.Tanh(),
         )
         self.bsn=BatchSpecificNorm(n_batches=n_batches,n_features=n_features,eps=eps)
         self.relu=nn.ReLU()
```

## Comparing `Beaconet/metrics/compute_LME.py` & `Beaconet/metrics/compute_PME.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import numpy as np
 import pandas as pd
 from tqdm import trange
 from sklearn.model_selection import ParameterGrid
 from sklearn.neighbors import kneighbors_graph
 from scipy.stats import entropy
 
-def get_lmd(df,batch_col="batch",bio_col="cell_type"):
-    LMD = compute_LME(X=df[["UMAP_1", "UMAP_2"]], meta=df[[batch_col, bio_col]], batch_label=batch_col,
+def get_pmd(df,batch_col="batch",bio_col="cell_type"):
+    LMD = compute_PME(X=df[["UMAP_1", "UMAP_2"]], meta=df[[batch_col, bio_col]], batch_label=batch_col,
                       bio_label=bio_col)
     positive_rate=LMD.notna().sum()/LMD.shape[0]
     return positive_rate,LMD
 
 def concat(x,sep="_"):
     return sep.join([str(e) for e in x])
 
 
-def compute_LME(X,meta,batch_label,bio_label,k=None):
+def compute_PME(X,meta,batch_label,bio_label,k=None):
     assert isinstance(X,pd.DataFrame)
 
     if(k is None):
         k=max(15,int(X.shape[0]*0.01))
 
     batch=meta[batch_label]
     bio=meta[bio_label]
```

## Comparing `Beaconet-1.0.2.dist-info/LICENSE` & `Beaconet-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Beaconet-1.0.2.dist-info/METADATA` & `Beaconet-1.0.6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Beaconet
-Version: 1.0.2
+Version: 1.0.6
 Summary: A reference-free method for integration of multiple batches of scRNA-seq data.
-Home-page: https://github.com/xuxiaohan
-Author: Xu Han, Gao Lin
+Home-page: https://github.com/xuxiaohan/Beaconet
+Author: Xu Han
 Author-email: hxu10670@gmail.com
 Maintainer: Xu Han
 Maintainer-email: hxu10670@gmail.com
 License: MIT Licence
 Keywords: scRNA-seq,single cell,batch effect,multiple sources,reference-free
 Platform: any
 License-File: LICENSE
@@ -17,9 +17,9 @@
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
 Requires-Dist: torch
 Requires-Dist: umap-learn
 Requires-Dist: scipy
 
-the misc-tools for experiment of machine learning and bioinformatics.
+UNKNOWN
```

## Comparing `Beaconet-1.0.2.dist-info/RECORD` & `Beaconet-1.0.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Beaconet/__init__.py,sha256=ang49Xa8uaC2KyGB3W8gZvMqKqZIk3wjI3qTkSmSi3Y,106
-Beaconet/metrics/__init__.py,sha256=zx_lKDFkjSr59jRIFmGeLz8b1tQTEjFYDjUytCSQnXo,92
-Beaconet/metrics/compute_LME.py,sha256=aotWEY8hxRWsQ6jD3HTbZia7Bwvg1mVoURXOT5KPuHo,2810
-Beaconet/metrics/show.py,sha256=Dc5TZ7vB3eHnVoB5LzGEAUlIMPYYb6Q9SRj-1Xhf0Jo,4745
+Beaconet/__init__.py,sha256=CTtZxasMY-qwAX87egAi9Oy8h5P6-a-L1mYg_foc98o,118
+Beaconet/metrics/__init__.py,sha256=3648K6bHGLM0-gK5-t_g4oMnsdGJF2dH3HwAOZj5NIM,105
+Beaconet/metrics/compute_PME.py,sha256=o-I_iyleCowrGcJZrgRYWTWPCH4_-NVJT1XJQ4qdEHs,2810
+Beaconet/metrics/show.py,sha256=Yz3an07DtVRaygUUcGaMkChIZQG-dwYZJOrTZ3FjKSQ,4807
 Beaconet/model/__init__.py,sha256=rTLMmku0RIsLT3muie9ySWnNiMlZgxV1muIt-V-Rb2Q,37
-Beaconet/model/model.py,sha256=enBTt_gzqJZ5-E8aCPXLfuFF6m4nZmghnIMPpEML59k,10926
-Beaconet-1.0.2.dist-info/LICENSE,sha256=N29C1dsYz9lRx6JUc18XhIPqTrtuJUfoxCTsDGr_65k,1103
-Beaconet-1.0.2.dist-info/METADATA,sha256=USSrTYwnYgugbpvZCMeo1pB63gbKuyyngOuxvxUK470,707
-Beaconet-1.0.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-Beaconet-1.0.2.dist-info/top_level.txt,sha256=wOpa2fsqRLjp-1xUGl1HV4qpPfO1U87GD291op-hFIE,9
-Beaconet-1.0.2.dist-info/RECORD,,
+Beaconet/model/model.py,sha256=xw0rX8d0dLSLVBVr1SiNOVrdpZBnCdksn94kLa5LO8s,10770
+Beaconet-1.0.6.dist-info/LICENSE,sha256=N29C1dsYz9lRx6JUc18XhIPqTrtuJUfoxCTsDGr_65k,1103
+Beaconet-1.0.6.dist-info/METADATA,sha256=2JsPigPKxb7uOz8eorcF-TU4L8YCKo2nc3q_ZZptack,645
+Beaconet-1.0.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+Beaconet-1.0.6.dist-info/top_level.txt,sha256=wOpa2fsqRLjp-1xUGl1HV4qpPfO1U87GD291op-hFIE,9
+Beaconet-1.0.6.dist-info/RECORD,,
```

