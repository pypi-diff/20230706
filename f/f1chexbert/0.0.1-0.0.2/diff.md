# Comparing `tmp/f1chexbert-0.0.1.tar.gz` & `tmp/f1chexbert-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f1chexbert-0.0.1.tar", last modified: Thu Jan 26 21:06:43 2023, max compression
+gzip compressed data, was "f1chexbert-0.0.2.tar", last modified: Thu Jul  6 20:19:59 2023, max compression
```

## Comparing `f1chexbert-0.0.1.tar` & `f1chexbert-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-01-26 21:06:43.617623 f1chexbert-0.0.1/
--rw-rw-r--   0 jb        (1000) jb        (1000)      321 2023-01-26 21:06:43.617623 f1chexbert-0.0.1/PKG-INFO
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-01-26 21:06:43.617623 f1chexbert-0.0.1/f1chexbert/
--rw-rw-r--   0 jb        (1000) jb        (1000)       35 2023-01-26 20:54:15.000000 f1chexbert-0.0.1/f1chexbert/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11950 2023-01-26 21:05:43.000000 f1chexbert-0.0.1/f1chexbert/f1chexbert.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-01-26 21:06:43.617623 f1chexbert-0.0.1/f1chexbert.egg-info/
--rw-rw-r--   0 jb        (1000) jb        (1000)      321 2023-01-26 21:06:43.000000 f1chexbert-0.0.1/f1chexbert.egg-info/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)      258 2023-01-26 21:06:43.000000 f1chexbert-0.0.1/f1chexbert.egg-info/SOURCES.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-01-26 21:06:43.000000 f1chexbert-0.0.1/f1chexbert.egg-info/dependency_links.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-01-26 21:06:43.000000 f1chexbert-0.0.1/f1chexbert.egg-info/not-zip-safe
--rw-rw-r--   0 jb        (1000) jb        (1000)       68 2023-01-26 21:06:43.000000 f1chexbert-0.0.1/f1chexbert.egg-info/requires.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       11 2023-01-26 21:06:43.000000 f1chexbert-0.0.1/f1chexbert.egg-info/top_level.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       38 2023-01-26 21:06:43.617623 f1chexbert-0.0.1/setup.cfg
--rw-rw-r--   0 jb        (1000) jb        (1000)      814 2023-01-26 21:06:12.000000 f1chexbert-0.0.1/setup.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 20:19:59.659757 f1chexbert-0.0.2/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4621 2023-07-06 20:19:59.659757 f1chexbert-0.0.2/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4222 2023-07-06 20:19:17.000000 f1chexbert-0.0.2/README.md
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 20:19:59.655757 f1chexbert-0.0.2/f1chexbert/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       35 2023-01-26 20:54:15.000000 f1chexbert-0.0.2/f1chexbert/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10465 2023-07-06 20:18:16.000000 f1chexbert-0.0.2/f1chexbert/f1chexbert.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 20:19:59.659757 f1chexbert-0.0.2/f1chexbert.egg-info/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4621 2023-07-06 20:19:58.000000 f1chexbert-0.0.2/f1chexbert.egg-info/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)      311 2023-07-06 20:19:59.000000 f1chexbert-0.0.2/f1chexbert.egg-info/SOURCES.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-07-06 20:19:58.000000 f1chexbert-0.0.2/f1chexbert.egg-info/dependency_links.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-07-06 20:19:58.000000 f1chexbert-0.0.2/f1chexbert.egg-info/not-zip-safe
+-rw-rw-r--   0 jb        (1000) jb        (1000)       68 2023-07-06 20:19:59.000000 f1chexbert-0.0.2/f1chexbert.egg-info/requires.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       17 2023-07-06 20:19:59.000000 f1chexbert-0.0.2/f1chexbert.egg-info/top_level.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       38 2023-07-06 20:19:59.659757 f1chexbert-0.0.2/setup.cfg
+-rw-rw-r--   0 jb        (1000) jb        (1000)      793 2023-07-06 20:15:33.000000 f1chexbert-0.0.2/setup.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 20:19:59.659757 f1chexbert-0.0.2/tests/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-07-06 20:12:13.000000 f1chexbert-0.0.2/tests/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4922 2023-07-06 20:14:34.000000 f1chexbert-0.0.2/tests/f1chexbert_test.py
```

### Comparing `f1chexbert-0.0.1/f1chexbert/f1chexbert.py` & `f1chexbert-0.0.2/f1chexbert/f1chexbert.py`

 * *Files 13% similar despite different names*

```diff
@@ -238,60 +238,7 @@
 
     def train(self, mode: bool = True):
         mode = False  # force False
         self.training = mode
         for module in self.children():
             module.train(mode)
         return self
-
-
-if __name__ == '__main__':
-    import json
-
-    f1chexbert = F1CheXbert(device="cuda")
-    accuracy, accuracy_not_averaged, class_report, class_report_5 = f1chexbert(
-        hyps=['No pleural effusion. Normal heart size.', 'Normal heart size.'],
-        refs=['No pleural effusions.', 'Enlarged heart.'])
-    print(accuracy)
-    print(accuracy_not_averaged)
-    print(json.dumps(class_report, indent=4))
-    # 0.5
-    # [1. 0.]
-    # {
-    # ...
-    #     "Cardiomegaly": {
-    #         "precision": 0.0,
-    #         "recall": 0.0,
-    #         "f1-score": 0.0,
-    #         "support": 1
-    # ....
-    #     "No Finding": {
-    #         "precision": 0.5,
-    #         "recall": 1.0,
-    #         "f1-score": 0.6666666666666666,
-    #         "support": 1
-    #     },
-    #     "micro avg": {
-    #         "precision": 0.5,
-    #         "recall": 0.5,
-    #         "f1-score": 0.5,
-    #         "support": 2
-    #     },
-    #     "macro avg": {
-    #         "precision": 0.03571428571428571,
-    #         "recall": 0.07142857142857142,
-    #         "f1-score": 0.047619047619047616,
-    #         "support": 2
-    #     },
-    #     "weighted avg": {
-    #         "precision": 0.25,
-    #         "recall": 0.5,
-    #         "f1-score": 0.3333333333333333,
-    #         "support": 2
-    #     },
-    #     "samples avg": {
-    #         "precision": 0.5,
-    #         "recall": 0.5,
-    #         "f1-score": 0.5,
-    #         "support": 2
-    #     }
-    # }
```

