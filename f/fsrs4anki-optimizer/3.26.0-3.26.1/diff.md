# Comparing `tmp/fsrs4anki_optimizer-3.26.0.tar.gz` & `tmp/fsrs4anki_optimizer-3.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.26.0.tar", last modified: Tue Jul  4 08:37:11 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.26.1.tar", last modified: Thu Jul  6 02:15:28 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.26.0.tar` & `fsrs4anki_optimizer-3.26.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:37:11.672903 fsrs4anki_optimizer-3.26.0/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 08:37:11.668903 fsrs4anki_optimizer-3.26.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:37:11.668903 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45606 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:37:11.668903 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 08:37:11.000000 fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:37:11.672903 fsrs4anki_optimizer-3.26.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 08:36:54.000000 fsrs4anki_optimizer-3.26.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 02:15:28.000000 fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 02:15:28.098245 fsrs4anki_optimizer-3.26.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 02:15:17.000000 fsrs4anki_optimizer-3.26.1/setup.py
```

### Comparing `fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.26.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.26.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,17 +308,18 @@
         with torch.no_grad():
             line_tensor = lineToTensor(list(zip([t_history], [r_history]))[0]).unsqueeze(1)
             output_t = self.model(line_tensor)
             return output_t[-1][0]
 
     def batch_predict(self, dataset):
         fast_dataset = RevlogDataset(dataset)
-        outputs, _ = self.model(fast_dataset.x_train.transpose(0, 1))
-        stabilities, difficulties = outputs[fast_dataset.seq_len-1, torch.arange(len(fast_dataset))].transpose(0, 1)
-        return stabilities.tolist(), difficulties.tolist()
+        with torch.no_grad():
+            outputs, _ = self.model(fast_dataset.x_train.transpose(0, 1))
+            stabilities, difficulties = outputs[fast_dataset.seq_len-1, torch.arange(len(fast_dataset))].transpose(0, 1)
+            return stabilities.tolist(), difficulties.tolist()
 
 """Used to store all the results from FSRS related functions"""
 class Optimizer:
     def __init__(self) -> None:
         tqdm.pandas()
 
     @staticmethod
```

