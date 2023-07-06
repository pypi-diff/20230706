# Comparing `tmp/titan-iris-0.8.9.tar.gz` & `tmp/titan-iris-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.8.9.tar", last modified: Mon Jun 26 18:31:49 2023, max compression
+gzip compressed data, was "titan-iris-0.9.0.tar", last modified: Thu Jul  6 11:20:31 2023, max compression
```

## Comparing `titan-iris-0.8.9.tar` & `titan-iris-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:31:49.272388 titan-iris-0.8.9/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 18:31:31.000000 titan-iris-0.8.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 18:31:31.000000 titan-iris-0.8.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 18:31:31.000000 titan-iris-0.8.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 18:31:49.272388 titan-iris-0.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 18:31:31.000000 titan-iris-0.8.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 18:31:31.000000 titan-iris-0.8.9/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 18:31:31.000000 titan-iris-0.8.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 18:31:31.000000 titan-iris-0.8.9/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 18:31:49.276388 titan-iris-0.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 18:31:31.000000 titan-iris-0.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:31:49.268387 titan-iris-0.8.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:31:49.272388 titan-iris-0.8.9/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:31:49.272388 titan-iris-0.8.9/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:31:49.272388 titan-iris-0.8.9/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-06-26 18:31:31.000000 titan-iris-0.8.9/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:31:49.272388 titan-iris-0.8.9/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 18:31:49.000000 titan-iris-0.8.9/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 18:31:49.000000 titan-iris-0.8.9/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:31:49.000000 titan-iris-0.8.9/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 18:31:49.000000 titan-iris-0.8.9/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 18:31:49.000000 titan-iris-0.8.9/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 18:31:49.000000 titan-iris-0.8.9/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:31:49.272388 titan-iris-0.8.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 18:31:31.000000 titan-iris-0.8.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 18:31:31.000000 titan-iris-0.8.9/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:20:31.243452 titan-iris-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-06 11:20:16.000000 titan-iris-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 11:20:16.000000 titan-iris-0.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 11:20:16.000000 titan-iris-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-06 11:20:31.243452 titan-iris-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-06 11:20:16.000000 titan-iris-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 11:20:16.000000 titan-iris-0.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-06 11:20:16.000000 titan-iris-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 11:20:16.000000 titan-iris-0.9.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 11:20:31.243452 titan-iris-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-06 11:20:16.000000 titan-iris-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:20:31.239452 titan-iris-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:20:31.243452 titan-iris-0.9.0/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:20:31.243452 titan-iris-0.9.0/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:20:31.243452 titan-iris-0.9.0/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18417 2023-07-06 11:20:16.000000 titan-iris-0.9.0/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:20:31.243452 titan-iris-0.9.0/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-06 11:20:31.000000 titan-iris-0.9.0/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-06 11:20:31.000000 titan-iris-0.9.0/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:20:31.000000 titan-iris-0.9.0/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 11:20:31.000000 titan-iris-0.9.0/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 11:20:31.000000 titan-iris-0.9.0/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 11:20:31.000000 titan-iris-0.9.0/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:20:31.243452 titan-iris-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-06 11:20:16.000000 titan-iris-0.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-06 11:20:16.000000 titan-iris-0.9.0/tests/test_sdk.py
```

### Comparing `titan-iris-0.8.9/.gitignore` & `titan-iris-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/Dockerfile` & `titan-iris-0.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/PKG-INFO` & `titan-iris-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.9
+Version: 0.9.0
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.9/README.md` & `titan-iris-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/setup.py` & `titan-iris-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/src/iris/config.yaml` & `titan-iris-0.9.0/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/src/iris/gradio/run.py` & `titan-iris-0.9.0/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/src/iris/main.py` & `titan-iris-0.9.0/src/iris/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,25 +351,21 @@
     if experiment_name != "":
         flags.update({"name": experiment_name})
     if task == "sequence_classification":
         # sequence of task specific flags
         # if the flag shouldn't be accepted, set error_message to the error string to print.
         # if it should be, and you want to warn, print, but don't set error_message
         error_message = False
+        if no_qlora:
+            print("no_qlora is disregarded for sequence classification tasks")
         if not num_labels and not len(label_names):
             error_message = (
                 "Please provide either the number of labels (--num-labels, -nl) or "
                 "a mapping between user labels and (integer) dataset labels."
             )
-        elif num_labels and len(label_names) != num_labels and len(label_names):
-            error_message = (
-                "The given label map has a different number of labels to " "that specified with --num-labels"
-            )
-        elif num_labels and len(label_names):
-            print("If providing label_names, num_labels does not need to be provided.")
         elif label_names:
             if not all(":" in x for x in label_names):
                 error_message = (
                     "Label names should be specified as a map from integers to labels, e.g. "
                     "'-ln 0:Positive -ln 1:Negative ...'"
                 )
             if error_message:
@@ -397,14 +393,15 @@
         if error_message:
             print(error_message)
             raise typer.Abort(error_message)
 
         else:
             # new: label_names
             flags.update({"num_labels": num_labels, "text_fields": text_fields})
+
     elif task == "question_answering":
         is_error = False
         # sequence of task specific flags
         # if the flag shouldn't be accepted, set is_error=True
         # if it should be, and you want to warn, print, but don't set is_error
         if num_labels is not None:
             print("num_labels is not necessary for question answering tasks")
@@ -412,14 +409,15 @@
             print("text_fields is not necessary for question answering tasks")
         if label_names is not None and len(label_names) > 0:
             print("label_names is not necessary for question_answering tasks")
         if is_error:
             raise typer.Abort()
         else:
             flags.update({"has_negative": has_negative})
+
     elif task == "glue":
         # sequence of task specific flags
         # if the flag shouldn't be accepted, set is_error=True
         # if it should be, and you want to warn, print, but don't set is_error
         is_error = False
         if num_labels is not None:
             print("num_labels is not necessary for glue tasks")
```

### Comparing `titan-iris-0.8.9/src/iris/sdk/auth_utils.py` & `titan-iris-0.9.0/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/src/iris/sdk/conf_manager.py` & `titan-iris-0.9.0/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/src/iris/sdk/exception.py` & `titan-iris-0.9.0/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/src/iris/sdk/iris_sdk.py` & `titan-iris-0.9.0/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/src/iris/sdk/safe_convert.py` & `titan-iris-0.9.0/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/src/iris/sdk/utils.py` & `titan-iris-0.9.0/src/iris/sdk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 logger = getLogger("iris.utils")
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                         Utils                                                        #
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 
-
-VALID_QLORA_MODELS = ["t5", "pythia", "opt", "gptj", "gptneo"]
+# rw = RefinedWed ==> Falcon
+VALID_QLORA_MODELS = ["t5", "pythia", "opt", "gptj", "gptneo", "falcon"]
 # ------------------------------  Helper Function for Iris Pull, Upload and Download   ------------------------------ #
 
 
 def make_targz(local_folder_path: str):
     """Create a tar.gz archive of the local folder - make this deterministic / exclude timestamp info from gz header.
 
     Args:
```

### Comparing `titan-iris-0.8.9/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.9.0/src/titan_iris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.9
+Version: 0.9.0
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.9/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.9.0/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/tests/test_cli.py` & `titan-iris-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.9/tests/test_sdk.py` & `titan-iris-0.9.0/tests/test_sdk.py`

 * *Files identical despite different names*

