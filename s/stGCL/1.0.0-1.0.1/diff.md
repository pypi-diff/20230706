# Comparing `tmp/stGCL-1.0.0.tar.gz` & `tmp/stGCL-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stGCL-1.0.0.tar", last modified: Wed Jul  5 16:30:21 2023, max compression
+gzip compressed data, was "stGCL-1.0.1.tar", last modified: Thu Jul  6 12:28:47 2023, max compression
```

## Comparing `stGCL-1.0.0.tar` & `stGCL-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-07-05 16:30:21.000000 stGCL-1.0.0/
--rw-rw-r--   0 dell      (1000) dell      (1000)     1070 2022-04-29 09:56:50.000000 stGCL-1.0.0/LICENSE
--rw-rw-r--   0 dell      (1000) dell      (1000)      225 2023-07-05 16:30:21.000000 stGCL-1.0.0/PKG-INFO
--rw-rw-r--   0 dell      (1000) dell      (1000)       19 2023-07-05 16:27:16.000000 stGCL-1.0.0/README.rst
--rw-rw-r--   0 dell      (1000) dell      (1000)       38 2023-07-05 16:30:21.000000 stGCL-1.0.0/setup.cfg
--rw-rw-r--   0 dell      (1000) dell      (1000)      911 2023-07-05 16:18:13.000000 stGCL-1.0.0/setup.py
-drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-07-05 16:30:21.000000 stGCL-1.0.0/stGCL/
--rw-rw-r--   0 dell      (1000) dell      (1000)      420 2023-07-05 15:54:39.000000 stGCL-1.0.0/stGCL/__init__.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     3860 2022-09-26 02:26:42.000000 stGCL-1.0.0/stGCL/advance_deep_graph_infomax.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     9664 2022-04-29 09:56:50.000000 stGCL-1.0.0/stGCL/gat_conv.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     7775 2023-07-05 15:47:11.000000 stGCL-1.0.0/stGCL/image_processing.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     1424 2022-05-03 02:42:21.000000 stGCL-1.0.0/stGCL/image_resnet50.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     1328 2022-09-27 08:37:17.000000 stGCL-1.0.0/stGCL/inits.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     1579 2023-07-03 15:20:44.000000 stGCL-1.0.0/stGCL/modules.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     7953 2023-07-05 14:15:51.000000 stGCL-1.0.0/stGCL/process.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     8328 2023-07-05 15:47:12.000000 stGCL-1.0.0/stGCL/stGCL_model.py
--rw-rw-r--   0 dell      (1000) dell      (1000)     4622 2023-07-05 15:47:12.000000 stGCL-1.0.0/stGCL/train_model.py
--rw-rw-r--   0 dell      (1000) dell      (1000)    16939 2023-07-04 16:53:28.000000 stGCL-1.0.0/stGCL/utils.py
--rw-rw-r--   0 dell      (1000) dell      (1000)    16271 2022-11-04 11:17:23.000000 stGCL-1.0.0/stGCL/vit_model.py
-drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-07-05 16:30:21.000000 stGCL-1.0.0/stGCL.egg-info/
--rw-rw-r--   0 dell      (1000) dell      (1000)      225 2023-07-05 16:30:21.000000 stGCL-1.0.0/stGCL.egg-info/PKG-INFO
--rw-rw-r--   0 dell      (1000) dell      (1000)      446 2023-07-05 16:30:21.000000 stGCL-1.0.0/stGCL.egg-info/SOURCES.txt
--rw-rw-r--   0 dell      (1000) dell      (1000)        1 2023-07-05 16:30:21.000000 stGCL-1.0.0/stGCL.egg-info/dependency_links.txt
--rw-rw-r--   0 dell      (1000) dell      (1000)        1 2023-07-05 16:08:00.000000 stGCL-1.0.0/stGCL.egg-info/not-zip-safe
--rw-rw-r--   0 dell      (1000) dell      (1000)        9 2023-07-05 16:30:21.000000 stGCL-1.0.0/stGCL.egg-info/requires.txt
--rw-rw-r--   0 dell      (1000) dell      (1000)        6 2023-07-05 16:30:21.000000 stGCL-1.0.0/stGCL.egg-info/top_level.txt
+drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-07-06 12:28:47.114914 stGCL-1.0.1/
+-rw-rw-r--   0 dell      (1000) dell      (1000)     1070 2022-04-29 09:56:50.000000 stGCL-1.0.1/LICENSE
+-rw-rw-r--   0 dell      (1000) dell      (1000)      225 2023-07-06 12:28:47.114914 stGCL-1.0.1/PKG-INFO
+-rw-rw-r--   0 dell      (1000) dell      (1000)       19 2023-07-05 16:27:16.000000 stGCL-1.0.1/README.rst
+-rw-rw-r--   0 dell      (1000) dell      (1000)       38 2023-07-06 12:28:47.114914 stGCL-1.0.1/setup.cfg
+-rw-rw-r--   0 dell      (1000) dell      (1000)      911 2023-07-06 12:20:32.000000 stGCL-1.0.1/setup.py
+drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-07-06 12:28:47.114914 stGCL-1.0.1/stGCL/
+-rw-rw-r--   0 dell      (1000) dell      (1000)      389 2023-07-06 12:09:12.000000 stGCL-1.0.1/stGCL/__init__.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     3860 2022-09-26 02:26:42.000000 stGCL-1.0.1/stGCL/advance_deep_graph_infomax.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     9664 2022-04-29 09:56:50.000000 stGCL-1.0.1/stGCL/gat_conv.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     7852 2023-07-06 12:15:05.000000 stGCL-1.0.1/stGCL/image_processing.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     1424 2022-05-03 02:42:21.000000 stGCL-1.0.1/stGCL/image_resnet50.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     1328 2022-09-27 08:37:17.000000 stGCL-1.0.1/stGCL/inits.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     1571 2023-07-06 12:04:32.000000 stGCL-1.0.1/stGCL/modules.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     7953 2023-07-05 14:15:51.000000 stGCL-1.0.1/stGCL/process.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     8328 2023-07-05 15:47:12.000000 stGCL-1.0.1/stGCL/stGCL_model.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)     4622 2023-07-05 15:47:12.000000 stGCL-1.0.1/stGCL/train_model.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)    16939 2023-07-04 16:53:28.000000 stGCL-1.0.1/stGCL/utils.py
+-rw-rw-r--   0 dell      (1000) dell      (1000)    16271 2022-11-04 11:17:23.000000 stGCL-1.0.1/stGCL/vit_model.py
+drwxrwxr-x   0 dell      (1000) dell      (1000)        0 2023-07-06 12:28:47.114914 stGCL-1.0.1/stGCL.egg-info/
+-rw-rw-r--   0 dell      (1000) dell      (1000)      225 2023-07-06 12:28:47.000000 stGCL-1.0.1/stGCL.egg-info/PKG-INFO
+-rw-rw-r--   0 dell      (1000) dell      (1000)      446 2023-07-06 12:28:47.000000 stGCL-1.0.1/stGCL.egg-info/SOURCES.txt
+-rw-rw-r--   0 dell      (1000) dell      (1000)        1 2023-07-06 12:28:47.000000 stGCL-1.0.1/stGCL.egg-info/dependency_links.txt
+-rw-rw-r--   0 dell      (1000) dell      (1000)        1 2023-07-05 16:08:00.000000 stGCL-1.0.1/stGCL.egg-info/not-zip-safe
+-rw-rw-r--   0 dell      (1000) dell      (1000)        9 2023-07-06 12:28:47.000000 stGCL-1.0.1/stGCL.egg-info/requires.txt
+-rw-rw-r--   0 dell      (1000) dell      (1000)        6 2023-07-06 12:28:47.000000 stGCL-1.0.1/stGCL.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stGCL-1.0.0/LICENSE` & `stGCL-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/setup.py` & `stGCL-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 __lib_name__ = "stGCL"
-__lib_version__ = "1.0.0"
+__lib_version__ = "1.0.1"
 __description__ = "Deciphering spatial domains from spatially resolved transcriptomics with adaptive graph attention auto-encoder"
 __author__ = "Daoliang Zhang"
 __author_email__ = "201720386@mail.edu.sdu.cn"
 __license__ = "MIT"
 __keywords__ = ["spatial transcriptomics", "Deep learning", "Graph attention auto-encoder"]
 __requires__ = ["requests",]
```

### Comparing `stGCL-1.0.0/stGCL/advance_deep_graph_infomax.py` & `stGCL-1.0.1/stGCL/advance_deep_graph_infomax.py`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/stGCL/gat_conv.py` & `stGCL-1.0.1/stGCL/gat_conv.py`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/stGCL/image_processing.py` & `stGCL-1.0.1/stGCL/image_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,17 @@
 	cudnn.deterministic = True
 	torch.backends.cudnn.deterministic = True
 	cudnn.benchmark = False
 
 	os.environ['PYTHONHASHSEED'] = str(seed)
 	os.environ['CUBLAS_WORKSPACE_CONFIG'] = ':4096:8'
 
-def image_representation(positionsdata,image_adress,image_file,label=None,score_adress="",pca_num=3000,k=7,
+def image_representation(positionsdata,image_adress,image_file,label=None,score_adress="",pca_num=None,k=7,
 						 scale_file=None, image_net="Vit",image_type="full",crop_size=256,batch_size_lw=128,
-						 ARI=True,patch_size=64,scale=1,load=True,border=0):
+						 ARI=False,patch_size=64,scale=1,load=False,border=0):
 	set_seed(seed=0)
 	if scale_file==None :
 		if image_type=="full":
 			scale=scale
 		else:
 			raise Exception('Please enter scale_file address')
 	else:
@@ -208,34 +208,43 @@
 		f_num=feature.size()[1]
 
 		feature_dim.append(feature.data.cpu().numpy())
 		barcode.append(image_code)
 
 	feature_dim = np.concatenate(feature_dim)
 	barcode = np.concatenate(barcode)
-	print("PCA dimensionality reduction")
-	pca = PCA(n_components=pca_num)
-	pca.fit(feature_dim)
-	pca_feature = pca.transform(feature_dim)
 	filder=score_adress
 	if not os.path.exists(filder):
 		os.makedirs(filder)
 
+	if PCA !=0:
+		print("PCA dimensionality reduction")
+		pca = PCA(n_components=pca_num)
+		pca.fit(feature_dim)
+		pca_feature = pca.transform(feature_dim)
+
+		save_fileName = '{}/{}_representation.csv'.format(filder, image_net)
+		data_frame = pd.DataFrame(data=feature_dim, index=barcode, columns=list(range(1, f_num + 1)))
+		data_frame = data_frame.sort_index(axis=0)
+		data_frame.to_csv(save_fileName)
+		print(save_fileName)
+
+
 	save_fileName = '{}/{}_pca_representation.csv'.format(filder,image_net)
 	pca_frame = pd.DataFrame(data=pca_feature , index=barcode, columns=list(range(1, pca_num+1)))
 	pca_frame = pca_frame.sort_index(axis=0)
 	pca_frame.to_csv(save_fileName)
 
-	save_fileName ='{}/{}_representation.csv'.format(filder,image_net)
-	data_frame = pd.DataFrame(data=feature_dim, index=barcode, columns=list(range(1, f_num + 1)))
-	data_frame =data_frame.sort_index(axis=0)
-	data_frame.to_csv(save_fileName)
-	print(save_fileName)
+
 
 	if (label is not None) & ARI:
 		print("Clustering image features using kmeans")
-		pca_kmeans = KMeans(n_clusters=k, n_init=20).fit(feature_dim)
+		if pca !=0:
+			pca_kmeans = KMeans(n_clusters=k, n_init=20).fit(feature_dim)
+			pcaARI = adjusted_rand_score(label, pca_kmeans.labels_)
+		else:
+			pcaARI=0
 		kmeans = KMeans(n_clusters=k, n_init=20).fit(feature_dim)
 		ARI = adjusted_rand_score(label, kmeans.labels_)
-		pcaARI = adjusted_rand_score(label, pca_kmeans.labels_)
+
 		print(ARI,pcaARI,k)
 	print("Complete the extraction of image representation")
```

### Comparing `stGCL-1.0.0/stGCL/image_resnet50.py` & `stGCL-1.0.1/stGCL/image_resnet50.py`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/stGCL/inits.py` & `stGCL-1.0.1/stGCL/inits.py`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/stGCL/modules.py` & `stGCL-1.0.1/stGCL/modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from sklearn.cluster import KMeans
 from torch import optim
 from tqdm import tqdm
 from torch.autograd import Variable
 from torch.nn.modules.module import Module
 from torchvision import models
-from image_package.vit_model import VisionTransformer
+from stGCL.vit_model import VisionTransformer
 
 class extract_model(Module):
 	def __init__(self,net,crop_size, patch_size):
 		super(extract_model, self).__init__()
 
 		if net == "resnet50":
 			# model = resnet50_model().cuda()
```

### Comparing `stGCL-1.0.0/stGCL/process.py` & `stGCL-1.0.1/stGCL/process.py`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/stGCL/stGCL_model.py` & `stGCL-1.0.1/stGCL/stGCL_model.py`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/stGCL/train_model.py` & `stGCL-1.0.1/stGCL/train_model.py`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/stGCL/utils.py` & `stGCL-1.0.1/stGCL/utils.py`

 * *Files identical despite different names*

### Comparing `stGCL-1.0.0/stGCL/vit_model.py` & `stGCL-1.0.1/stGCL/vit_model.py`

 * *Files identical despite different names*

