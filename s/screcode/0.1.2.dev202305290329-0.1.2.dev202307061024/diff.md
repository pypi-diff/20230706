# Comparing `tmp/screcode-0.1.2.dev202305290329-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202307061024-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 119319 bytes, number of entries: 6
+Zip file size: 119372 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    61723 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202305290329.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202305290329.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202305290329.dist-info/RECORD
-6 files, 212554 bytes uncompressed, 118415 bytes compressed:  44.3%
+-rw-r--r--  2.0 unx    61947 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202307061024.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202307061024.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202307061024.dist-info/RECORD
+6 files, 212778 bytes uncompressed, 118468 bytes compressed:  44.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202305290329.dist-info/METADATA
+Filename: screcode-0.1.2.dev202307061024.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202305290329.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202307061024.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202305290329.dist-info/RECORD
+Filename: screcode-0.1.2.dev202307061024.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -16,15 +16,15 @@
 class RECODE():
 	def __init__(
 		self,
 		fast_algorithm = True,
 		fast_algorithm_ell_ub = 1000,
 		seq_target = 'RNA',
 		version = 1,
-		stat_learning = False,
+		stat_learning = "Auto",
 		stat_learning_rate = 0.2,
 		stat_learning_seed = 0,
 		decimals = 5,
 		RECODE_key = 'RECODE',
 		anndata_key = 'layers',
 		verbose = True,
 		):
@@ -316,14 +316,18 @@
 		"""
 		start_time = datetime.datetime.now()
 		if self.verbose:
 			if self.seq_target in ['RNA','ATAC','Hi-C']:
 				print('start RECODE for sc%s-seq data' % self.seq_target)
 			if self.seq_target in ['Multiome']:
 				print('start RECODE for %s data' % self.seq_target)
+		
+		if type(self.stat_learning) != bool:
+			self.stat_learning = False if X.shape[0] < 10000 else True
+
 		if self.stat_learning:
 			if X.shape[0] < 10000:
 				self.logger.warning("Warning: The stat_learning option is for data with a large number of cells (>20000). \n"
 				"No use of the stat_learning option is recommended to keep the accuracy.")
 			np.random.seed(self.stat_learning_seed)
 			X_mat = self._check_datatype(X)
 			cell_stat = np.random.choice(X_mat.shape[0],int(self.stat_learning_rate*X.shape[0]),replace=False)					
@@ -337,14 +341,16 @@
 		end_time = datetime.datetime.now()
 		elapsed_time = end_time - start_time
 		hours, remainder = divmod(elapsed_time.seconds, 3600)
 		minutes, seconds = divmod(remainder, 60)
 		milliseconds = int(elapsed_time.microseconds / 1000)
 		self.elapsed_time =  f"{hours}h {minutes}m {seconds}s"
 		self.log_['Elapsed time'] = f"{hours}h {minutes}m {seconds}s {milliseconds:03}ms"
+		self.log_['stat_learning'] = self.stat_learning
+		self.log_['#test_data'] = int(self.stat_learning_rate*X.shape[0])
 		if self.verbose:
 			print('end RECODE for sc%s-seq' % self.seq_target)
 			print('log:',self.log_)
 		return X_RECODE
 	
 	def transform_integration(
 			self,
```

## Comparing `screcode-0.1.2.dev202305290329.dist-info/METADATA` & `screcode-0.1.2.dev202307061024.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202305290329
+Version: 0.1.2.dev202307061024
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

