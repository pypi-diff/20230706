# Comparing `tmp/animl-1.0.4.tar.gz` & `tmp/animl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animl-1.0.4.tar", last modified: Wed Mar  8 20:52:56 2023, max compression
+gzip compressed data, was "animl-1.1.0.tar", last modified: Thu Jul  6 18:17:59 2023, max compression
```

## Comparing `animl-1.0.4.tar` & `animl-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-03-08 20:52:56.451678 animl-1.0.4/
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     1084 2023-03-07 19:37:47.000000 animl-1.0.4/LICENSE
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      788 2023-03-08 20:52:56.451678 animl-1.0.4/PKG-INFO
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      233 2023-03-07 19:37:47.000000 animl-1.0.4/README.md
--rw-rw-r--   0 kyra      (1000) kyra      (1000)       85 2022-08-25 18:50:16.000000 animl-1.0.4/pyproject.toml
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      680 2023-03-08 20:52:56.451678 animl-1.0.4/setup.cfg
-drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-03-08 20:52:56.447678 animl-1.0.4/src/
-drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-03-08 20:52:56.447678 animl-1.0.4/src/animl/
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     1533 2023-03-07 22:29:13.000000 animl-1.0.4/src/animl/FileManagement.py
--rwxrwxr-x   0 kyra      (1000) kyra      (1000)     2551 2023-03-07 22:24:51.000000 animl-1.0.4/src/animl/ImageCropGenerator.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     9479 2023-03-08 00:54:28.000000 animl-1.0.4/src/animl/TFDetector.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     4586 2023-03-08 00:33:08.000000 animl-1.0.4/src/animl/Workflow.py
--rwxrwxr-x   0 kyra      (1000) kyra      (1000)     6620 2023-03-07 22:19:28.000000 animl-1.0.4/src/animl/ZooniverseAPI.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)        0 2022-08-25 18:50:16.000000 animl-1.0.4/src/animl/__init__.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     2298 2023-03-07 21:42:13.000000 animl-1.0.4/src/animl/detectMD.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     2753 2023-03-07 22:26:53.000000 animl-1.0.4/src/animl/extractFrames.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)     1114 2023-03-07 21:26:09.000000 animl-1.0.4/src/animl/parseResults.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      671 2023-03-08 00:32:22.000000 animl-1.0.4/src/animl/splitData.py
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      674 2023-03-07 21:29:37.000000 animl-1.0.4/src/animl/symlink.py
-drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-03-08 20:52:56.451678 animl-1.0.4/src/animl.egg-info/
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      788 2023-03-08 20:52:56.000000 animl-1.0.4/src/animl.egg-info/PKG-INFO
--rw-rw-r--   0 kyra      (1000) kyra      (1000)      448 2023-03-08 20:52:56.000000 animl-1.0.4/src/animl.egg-info/SOURCES.txt
--rw-rw-r--   0 kyra      (1000) kyra      (1000)        1 2023-03-08 20:52:56.000000 animl-1.0.4/src/animl.egg-info/dependency_links.txt
--rw-rw-r--   0 kyra      (1000) kyra      (1000)        6 2023-03-08 20:52:56.000000 animl-1.0.4/src/animl.egg-info/top_level.txt
+drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-06 18:17:59.854955 animl-1.1.0/
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     1084 2023-03-07 19:37:47.000000 animl-1.1.0/LICENSE
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      788 2023-07-06 18:17:59.854955 animl-1.1.0/PKG-INFO
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      233 2023-03-07 19:37:47.000000 animl-1.1.0/README.md
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)       85 2022-08-25 18:50:16.000000 animl-1.1.0/pyproject.toml
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      680 2023-07-06 18:17:59.854955 animl-1.1.0/setup.cfg
+drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-06 18:17:59.854955 animl-1.1.0/src/
+drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-06 18:17:59.854955 animl-1.1.0/src/animl/
+-rwxrwxr-x   0 kyra      (1000) kyra      (1000)     6620 2023-03-07 22:19:28.000000 animl-1.1.0/src/animl/ZooniverseAPI.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        0 2022-08-25 18:50:16.000000 animl-1.1.0/src/animl/__init__.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     4586 2023-03-08 00:33:08.000000 animl-1.1.0/src/animl/__main__.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     6305 2023-06-08 19:05:39.000000 animl-1.1.0/src/animl/detectMD.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     4046 2023-06-12 22:35:23.000000 animl-1.1.0/src/animl/fileManagement.py
+-rwxrwxr-x   0 kyra      (1000) kyra      (1000)     2489 2023-06-13 21:36:40.000000 animl-1.1.0/src/animl/imageCropGenerator.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     9362 2023-06-12 18:16:13.000000 animl-1.1.0/src/animl/imageUtils.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)    15363 2023-06-06 20:15:23.000000 animl-1.1.0/src/animl/loadMD.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     2338 2023-06-13 23:24:58.000000 animl-1.1.0/src/animl/parseResults.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     1194 2023-06-13 21:35:58.000000 animl-1.1.0/src/animl/predictSpecies.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        0 2023-05-18 17:02:37.000000 animl-1.1.0/src/animl/setupDirectory.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     1112 2023-06-13 23:48:39.000000 animl-1.1.0/src/animl/splitData.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      693 2023-05-17 21:35:40.000000 animl-1.1.0/src/animl/symlink.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     2430 2023-05-17 22:35:04.000000 animl-1.1.0/src/animl/test.py
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)     4880 2023-06-08 18:04:13.000000 animl-1.1.0/src/animl/videoProcessing.py
+drwxrwxr-x   0 kyra      (1000) kyra      (1000)        0 2023-07-06 18:17:59.854955 animl-1.1.0/src/animl.egg-info/
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      788 2023-07-06 18:17:59.000000 animl-1.1.0/src/animl.egg-info/PKG-INFO
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)      544 2023-07-06 18:17:59.000000 animl-1.1.0/src/animl.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        1 2023-07-06 18:17:59.000000 animl-1.1.0/src/animl.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyra      (1000) kyra      (1000)        6 2023-07-06 18:17:59.000000 animl-1.1.0/src/animl.egg-info/top_level.txt
```

### Comparing `animl-1.0.4/LICENSE` & `animl-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `animl-1.0.4/PKG-INFO` & `animl-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animl
-Version: 1.0.4
+Version: 1.1.0
 Summary: Functions required to classify subjects within camera trap field data.
 Home-page: https://github.com/conservationtechlab/animl-py
 Author: Kyra Swanson
 Author-email: tswanson@sdzwa.org
 Project-URL: Bug Tracker, https://github.com/conservationtechlab/animl-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `animl-1.0.4/setup.cfg` & `animl-1.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = animl
-version = 1.0.4
+version = 1.1.0
 author = Kyra Swanson
 author_email = tswanson@sdzwa.org
 description = Functions required to classify subjects within camera trap field data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/conservationtechlab/animl-py
 project_urls =
```

### Comparing `animl-1.0.4/src/animl/ImageCropGenerator.py` & `animl-1.1.0/src/animl/imageCropGenerator.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,30 +22,31 @@
     pad_height = delta_height // 2
     padding = (pad_width, pad_height,
                delta_width - pad_width, delta_height - pad_height)
     return ImageOps.expand(img, padding)
 
 
 class GenerateCropsFromFile(Sequence):
-    def __init__(self, x, resize=299, buffer=2, batch_size=32, standardize=True):
+    def __init__(self, x, filecol = 'file', resize=299, buffer=0, batch=32, standardize=True):
         self.x = x
+        self.filecol = filecol
         self.resize = int(resize)
         self.buffer = buffer
-        self.batch_size = int(batch_size)
+        self.batch = int(batch)
         self.standardize = standardize
 
     def __len__(self):
-        return int(np.ceil(len(self.x.index) / float(self.batch_size)))
+        return int(np.ceil(len(self.x.index) / float(self.batch)))
 
     def __getitem__(self, idx):
         imgarray = []
-        for i in range(min(len(self.x.index), idx * self.batch_size),
-                       min(len(self.x.index), (idx + 1) * self.batch_size)):
+        for i in range(min(len(self.x.index), idx * self.batch),
+                       min(len(self.x.index), (idx + 1) * self.batch)):
             try:
-                file = self.x['file'].iloc[i]
+                file = self.x[self.filecol].iloc[i]
                 img = Image.open(file)
             except OSError:
                 continue
             width, height = img.size
 
             bbox1 = self.x['bbox1'].iloc[i]
             bbox2 = self.x['bbox2'].iloc[i]
@@ -59,13 +60,12 @@
 
             left = max(0, left - self.buffer)
             top = max(0, top - self.buffer)
             right = min(width, right + self.buffer)
             bottom = min(height, bottom + self.buffer)
 
             img = img.crop((left, top, right, bottom))
-            img = tf.image.resize(img, [456, 456])
-            img = Image.fromarray((img.numpy()).astype(np.uint8)).convert('RGB')
-            img = tf.convert_to_tensor(img, dtype=tf.float32)
+            img = img.resize((self.resize, self.resize))
+            img = tf.keras.utils.img_to_array(img)
             imgarray.append(img)
 
-        return np.asarray(imgarray)
+        return np.asarray(imgarray)
```

### Comparing `animl-1.0.4/src/animl/Workflow.py` & `animl-1.1.0/src/animl/__main__.py`

 * *Files identical despite different names*

### Comparing `animl-1.0.4/src/animl/ZooniverseAPI.py` & `animl-1.1.0/src/animl/ZooniverseAPI.py`

 * *Files identical despite different names*

### Comparing `animl-1.0.4/src/animl/symlink.py` & `animl-1.1.0/src/animl/symlink.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,7 +15,9 @@
                        linkdir + data.at[i, 'class'] + "/" + os.path.basename(data.at[i, 'file']))
         except Exception as e:
             print('File already exists. Exception: {}'.format(e))
             continue
             
             
 #def symlinkMD():
+
+#der symUnlink():
```

### Comparing `animl-1.0.4/src/animl.egg-info/PKG-INFO` & `animl-1.1.0/src/animl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animl
-Version: 1.0.4
+Version: 1.1.0
 Summary: Functions required to classify subjects within camera trap field data.
 Home-page: https://github.com/conservationtechlab/animl-py
 Author: Kyra Swanson
 Author-email: tswanson@sdzwa.org
 Project-URL: Bug Tracker, https://github.com/conservationtechlab/animl-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

