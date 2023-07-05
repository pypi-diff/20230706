# Comparing `tmp/MEGNetSparse-0.0.3.tar.gz` & `tmp/MEGNetSparse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGNetSparse-0.0.3.tar", last modified: Wed Jul  5 18:57:41 2023, max compression
+gzip compressed data, was "MEGNetSparse-0.0.4.tar", last modified: Wed Jul  5 23:02:50 2023, max compression
```

## Comparing `MEGNetSparse-0.0.3.tar` & `MEGNetSparse-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 18:57:41.796352 MEGNetSparse-0.0.3/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.3/.gitignore
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     1091 2023-07-05 16:12:03.000000 MEGNetSparse-0.0.3/LICENSE
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 18:57:41.107634 MEGNetSparse-0.0.3/MEGNetSparse/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      120 2023-07-03 18:52:42.000000 MEGNetSparse-0.0.3/MEGNetSparse/__init__.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5423 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.3/MEGNetSparse/dense2sparse.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3586 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.3/MEGNetSparse/eos.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5105 2023-06-03 16:16:46.000000 MEGNetSparse-0.0.3/MEGNetSparse/layers.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3015 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.3/MEGNetSparse/model.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     6891 2023-06-03 16:26:00.000000 MEGNetSparse-0.0.3/MEGNetSparse/struct2graph.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     7461 2023-06-28 00:30:39.000000 MEGNetSparse-0.0.3/MEGNetSparse/trainer.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      885 2023-06-18 16:37:50.000000 MEGNetSparse-0.0.3/MEGNetSparse/utils.py
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 18:57:41.357196 MEGNetSparse-0.0.3/MEGNetSparse.egg-info/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-05 18:57:40.000000 MEGNetSparse-0.0.3/MEGNetSparse.egg-info/PKG-INFO
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      612 2023-07-05 18:57:40.000000 MEGNetSparse-0.0.3/MEGNetSparse.egg-info/SOURCES.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        1 2023-07-05 18:57:40.000000 MEGNetSparse-0.0.3/MEGNetSparse.egg-info/dependency_links.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       27 2023-07-05 18:57:40.000000 MEGNetSparse-0.0.3/MEGNetSparse.egg-info/requires.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       13 2023-07-05 18:57:40.000000 MEGNetSparse-0.0.3/MEGNetSparse.egg-info/top_level.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-05 18:57:41.790340 MEGNetSparse-0.0.3/PKG-INFO
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2536 2023-07-05 16:00:57.000000 MEGNetSparse-0.0.3/README.md
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 18:57:41.675665 MEGNetSparse-0.0.3/examples/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       19 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.3/examples/.gitignore
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      812 2023-06-05 21:35:25.000000 MEGNetSparse-0.0.3/examples/MoS2.cif
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      814 2022-09-29 08:35:52.000000 MEGNetSparse-0.0.3/examples/WSe2.cif
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    13944 2022-04-12 22:15:21.000000 MEGNetSparse-0.0.3/examples/descriptors.csv
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    15149 2023-07-03 19:04:43.000000 MEGNetSparse-0.0.3/examples/example.ipynb
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       82 2023-06-05 21:35:26.000000 MEGNetSparse-0.0.3/examples/initial_structures.csv
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 18:57:41.752853 MEGNetSparse-0.0.3/examples/pilot/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)   148416 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.3/examples/pilot/data.pickle.gz
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    10925 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.3/examples/pilot/targets.csv.gz
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      437 2023-07-05 18:55:58.000000 MEGNetSparse-0.0.3/pyproject.toml
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 18:57:41.801583 MEGNetSparse-0.0.3/setup.cfg
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:51.332479 MEGNetSparse-0.0.4/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.4/.gitignore
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     1091 2023-07-05 16:12:03.000000 MEGNetSparse-0.0.4/LICENSE
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:50.894993 MEGNetSparse-0.0.4/MEGNetSparse/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      120 2023-07-03 18:52:42.000000 MEGNetSparse-0.0.4/MEGNetSparse/__init__.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5423 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.4/MEGNetSparse/dense2sparse.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3586 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.4/MEGNetSparse/eos.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5105 2023-06-03 16:16:46.000000 MEGNetSparse-0.0.4/MEGNetSparse/layers.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3015 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.4/MEGNetSparse/model.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     6891 2023-06-03 16:26:00.000000 MEGNetSparse-0.0.4/MEGNetSparse/struct2graph.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     7445 2023-07-05 23:01:46.000000 MEGNetSparse-0.0.4/MEGNetSparse/trainer.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      885 2023-06-18 16:37:50.000000 MEGNetSparse-0.0.4/MEGNetSparse/utils.py
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:51.035601 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/PKG-INFO
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      612 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        1 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       27 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/requires.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       13 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/top_level.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-05 23:02:51.332479 MEGNetSparse-0.0.4/PKG-INFO
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2536 2023-07-05 16:00:57.000000 MEGNetSparse-0.0.4/README.md
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:51.223103 MEGNetSparse-0.0.4/examples/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       19 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.4/examples/.gitignore
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      812 2023-06-05 21:35:25.000000 MEGNetSparse-0.0.4/examples/MoS2.cif
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      814 2022-09-29 08:35:52.000000 MEGNetSparse-0.0.4/examples/WSe2.cif
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    13944 2022-04-12 22:15:21.000000 MEGNetSparse-0.0.4/examples/descriptors.csv
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    15149 2023-07-03 19:04:43.000000 MEGNetSparse-0.0.4/examples/example.ipynb
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       82 2023-06-05 21:35:26.000000 MEGNetSparse-0.0.4/examples/initial_structures.csv
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:51.301227 MEGNetSparse-0.0.4/examples/pilot/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)   148416 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.4/examples/pilot/data.pickle.gz
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    10925 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.4/examples/pilot/targets.csv.gz
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      437 2023-07-05 23:02:37.000000 MEGNetSparse-0.0.4/pyproject.toml
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 23:02:51.332479 MEGNetSparse-0.0.4/setup.cfg
```

### Comparing `MEGNetSparse-0.0.3/LICENSE` & `MEGNetSparse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse/dense2sparse.py` & `MEGNetSparse-0.0.4/MEGNetSparse/dense2sparse.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse/eos.py` & `MEGNetSparse-0.0.4/MEGNetSparse/eos.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse/layers.py` & `MEGNetSparse-0.0.4/MEGNetSparse/layers.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse/model.py` & `MEGNetSparse-0.0.4/MEGNetSparse/model.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse/struct2graph.py` & `MEGNetSparse-0.0.4/MEGNetSparse/struct2graph.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse/trainer.py` & `MEGNetSparse-0.0.4/MEGNetSparse/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,19 +132,19 @@
                 F.l1_loss(
                     self.scaler.inverse_transform(preds),
                     batch.y,
                     reduction='sum'
                 ).to('cpu').data.numpy()
             )
 
-            train_mae = sum(maes) / len(self.train_structures)
-            self.scheduler.step(train_mae)
-            train_mse = np.mean(mses)
+        train_mae = sum(maes) / len(self.train_structures)
+        self.scheduler.step(train_mae)
+        train_mse = np.mean(mses)
 
-            return train_mae, train_mse
+        return train_mae, train_mse
 
     def evaluate_on_test(self, return_predictions=False):
         total = []
         results = []
         self.model.train(False)
         with torch.no_grad():
             for batch in self.testloader:
```

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse/utils.py` & `MEGNetSparse-0.0.4/MEGNetSparse/utils.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse.egg-info/PKG-INFO` & `MEGNetSparse-0.0.4/MEGNetSparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGNetSparse
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Romanov Ignat <romanov.ignat.p@gmail.com>
 Project-URL: Homepage, https://github.com/RomanovIgnat/MEGNet_pytorch_test
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MEGNetSparse
```

### Comparing `MEGNetSparse-0.0.3/MEGNetSparse.egg-info/SOURCES.txt` & `MEGNetSparse-0.0.4/MEGNetSparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/PKG-INFO` & `MEGNetSparse-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGNetSparse
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Romanov Ignat <romanov.ignat.p@gmail.com>
 Project-URL: Homepage, https://github.com/RomanovIgnat/MEGNet_pytorch_test
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MEGNetSparse
```

### Comparing `MEGNetSparse-0.0.3/README.md` & `MEGNetSparse-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/examples/MoS2.cif` & `MEGNetSparse-0.0.4/examples/MoS2.cif`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/examples/WSe2.cif` & `MEGNetSparse-0.0.4/examples/WSe2.cif`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/examples/descriptors.csv` & `MEGNetSparse-0.0.4/examples/descriptors.csv`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/examples/example.ipynb` & `MEGNetSparse-0.0.4/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/examples/pilot/data.pickle.gz` & `MEGNetSparse-0.0.4/examples/pilot/data.pickle.gz`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.3/examples/pilot/targets.csv.gz` & `MEGNetSparse-0.0.4/examples/pilot/targets.csv.gz`

 * *Files identical despite different names*

