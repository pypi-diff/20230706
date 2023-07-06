# Comparing `tmp/baseten-0.6.6.tar.gz` & `tmp/baseten-0.6.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseten-0.6.6.tar", max compression
+gzip compressed data, was "baseten-0.6.6rc1.tar", max compression
```

## Comparing `baseten-0.6.6.tar` & `baseten-0.6.6rc1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     5041 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/__init__.py
--rw-r--r--   0        0        0    12867 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/baseten_deployed_model.py
--rw-r--r--   0        0        0     5539 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/cli.py
--rw-r--r--   0        0        0      541 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/client_commands/baseten_cli.py
--rw-r--r--   0        0        0     1143 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/client_commands/dataset_cli.py
--rw-r--r--   0        0        0     5953 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/client_commands/finetuning_cli.py
--rw-r--r--   0        0        0     1088 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/client_commands/models_cli.py
--rw-r--r--   0        0        0      927 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/client_commands/pretrained_cli.py
--rw-r--r--   0        0        0        0 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/__init__.py
--rw-r--r--   0        0        0    29519 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/api.py
--rw-r--r--   0        0        0     2512 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/core.py
--rw-r--r--   0        0        0     1475 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/error_handler.py
--rw-r--r--   0        0        0     6576 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/files.py
--rw-r--r--   0        0        0     4292 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/lib_support.py
--rw-r--r--   0        0        0    18701 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/model_deployer.py
--rw-r--r--   0        0        0     2288 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/settings.py
--rw-r--r--   0        0        0     1787 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/tar.py
--rw-r--r--   0        0        0      907 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/types.py
--rw-r--r--   0        0        0     3413 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/common/util.py
--rw-r--r--   0        0        0      207 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/models/__init__.py
--rw-r--r--   0        0        0     7086 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/models/flan_t5.py
--rw-r--r--   0        0        0      284 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/models/foundational_model.py
--rw-r--r--   0        0        0     5130 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/models/llama.py
--rw-r--r--   0        0        0    13478 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/models/stable_diffusion.py
--rw-r--r--   0        0        0     4878 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/models/util.py
--rw-r--r--   0        0        0     3481 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/models/whisper.py
--rw-r--r--   0        0        0      389 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/training/__init__.py
--rw-r--r--   0        0        0     2852 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/training/datasets.py
--rw-r--r--   0        0        0    33964 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/training/finetuning.py
--rw-r--r--   0        0        0     6681 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/training/logs.py
--rw-r--r--   0        0        0      479 2023-07-06 21:06:33.898496 baseten-0.6.6/baseten/training/utils.py
--rw-r--r--   0        0        0      763 2023-07-06 21:06:33.902496 baseten-0.6.6/pypi_readme.md
--rw-r--r--   0        0        0     1960 2023-07-06 21:06:33.902496 baseten-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 baseten-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     5041 2023-06-30 18:08:26.650019 baseten-0.6.6rc1/baseten/__init__.py
+-rw-r--r--   0        0        0    12867 2023-06-30 18:08:26.650164 baseten-0.6.6rc1/baseten/baseten_deployed_model.py
+-rw-r--r--   0        0        0     5539 2023-02-28 15:48:08.032836 baseten-0.6.6rc1/baseten/cli.py
+-rw-r--r--   0        0        0      541 2023-02-28 15:48:08.033195 baseten-0.6.6rc1/baseten/client_commands/baseten_cli.py
+-rw-r--r--   0        0        0     1143 2023-06-30 18:08:26.650269 baseten-0.6.6rc1/baseten/client_commands/dataset_cli.py
+-rw-r--r--   0        0        0     5953 2023-02-28 15:48:08.033504 baseten-0.6.6rc1/baseten/client_commands/finetuning_cli.py
+-rw-r--r--   0        0        0     1088 2023-02-28 15:48:08.033647 baseten-0.6.6rc1/baseten/client_commands/models_cli.py
+-rw-r--r--   0        0        0      927 2023-02-28 15:48:08.033791 baseten-0.6.6rc1/baseten/client_commands/pretrained_cli.py
+-rw-r--r--   0        0        0        0 2022-09-07 01:02:04.877401 baseten-0.6.6rc1/baseten/common/__init__.py
+-rw-r--r--   0        0        0    29519 2023-06-30 18:08:26.650430 baseten-0.6.6rc1/baseten/common/api.py
+-rw-r--r--   0        0        0     2512 2023-06-30 18:08:26.650556 baseten-0.6.6rc1/baseten/common/core.py
+-rw-r--r--   0        0        0     1475 2023-02-28 15:48:08.034880 baseten-0.6.6rc1/baseten/common/error_handler.py
+-rw-r--r--   0        0        0     6576 2023-06-30 18:08:26.650670 baseten-0.6.6rc1/baseten/common/files.py
+-rw-r--r--   0        0        0     4292 2023-02-28 15:48:08.035269 baseten-0.6.6rc1/baseten/common/lib_support.py
+-rw-r--r--   0        0        0    18701 2023-06-30 18:08:26.650827 baseten-0.6.6rc1/baseten/common/model_deployer.py
+-rw-r--r--   0        0        0     2288 2023-06-30 18:10:46.800516 baseten-0.6.6rc1/baseten/common/settings.py
+-rw-r--r--   0        0        0     1787 2023-06-30 18:08:26.651045 baseten-0.6.6rc1/baseten/common/tar.py
+-rw-r--r--   0        0        0      907 2023-02-28 15:48:08.035833 baseten-0.6.6rc1/baseten/common/types.py
+-rw-r--r--   0        0        0     3413 2023-06-30 18:08:26.651165 baseten-0.6.6rc1/baseten/common/util.py
+-rw-r--r--   0        0        0      207 2023-06-30 18:08:26.651869 baseten-0.6.6rc1/baseten/models/__init__.py
+-rw-r--r--   0        0        0     7086 2023-06-30 18:08:26.652036 baseten-0.6.6rc1/baseten/models/flan_t5.py
+-rw-r--r--   0        0        0      284 2023-06-30 18:08:26.652139 baseten-0.6.6rc1/baseten/models/foundational_model.py
+-rw-r--r--   0        0        0     5130 2023-06-30 18:08:26.652207 baseten-0.6.6rc1/baseten/models/llama.py
+-rw-r--r--   0        0        0    13478 2023-06-30 18:08:26.652347 baseten-0.6.6rc1/baseten/models/stable_diffusion.py
+-rw-r--r--   0        0        0     4878 2023-02-28 15:48:08.036730 baseten-0.6.6rc1/baseten/models/util.py
+-rw-r--r--   0        0        0     3481 2023-06-30 18:08:26.652468 baseten-0.6.6rc1/baseten/models/whisper.py
+-rw-r--r--   0        0        0      389 2023-06-30 18:08:26.652587 baseten-0.6.6rc1/baseten/training/__init__.py
+-rw-r--r--   0        0        0     2852 2023-06-30 18:08:26.652688 baseten-0.6.6rc1/baseten/training/datasets.py
+-rw-r--r--   0        0        0    33964 2023-06-30 18:08:26.652899 baseten-0.6.6rc1/baseten/training/finetuning.py
+-rw-r--r--   0        0        0     6681 2023-02-28 15:48:08.037504 baseten-0.6.6rc1/baseten/training/logs.py
+-rw-r--r--   0        0        0      479 2023-02-28 15:48:08.037598 baseten-0.6.6rc1/baseten/training/utils.py
+-rw-r--r--   0        0        0      763 2023-02-28 15:48:08.044032 baseten-0.6.6rc1/pypi_readme.md
+-rw-r--r--   0        0        0     1963 2023-06-30 18:12:14.385356 baseten-0.6.6rc1/pyproject.toml
+-rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 baseten-0.6.6rc1/setup.py
+-rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 baseten-0.6.6rc1/PKG-INFO
```

### Comparing `baseten-0.6.6/baseten/__init__.py` & `baseten-0.6.6rc1/baseten/__init__.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/baseten_deployed_model.py` & `baseten-0.6.6rc1/baseten/baseten_deployed_model.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/cli.py` & `baseten-0.6.6rc1/baseten/cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/client_commands/baseten_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/baseten_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/client_commands/dataset_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/dataset_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/client_commands/finetuning_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/finetuning_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/client_commands/models_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/models_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/client_commands/pretrained_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/pretrained_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/api.py` & `baseten-0.6.6rc1/baseten/common/api.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/core.py` & `baseten-0.6.6rc1/baseten/common/core.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/error_handler.py` & `baseten-0.6.6rc1/baseten/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/files.py` & `baseten-0.6.6rc1/baseten/common/files.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/lib_support.py` & `baseten-0.6.6rc1/baseten/common/lib_support.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/model_deployer.py` & `baseten-0.6.6rc1/baseten/common/model_deployer.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/settings.py` & `baseten-0.6.6rc1/baseten/common/settings.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/tar.py` & `baseten-0.6.6rc1/baseten/common/tar.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/types.py` & `baseten-0.6.6rc1/baseten/common/types.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/common/util.py` & `baseten-0.6.6rc1/baseten/common/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/models/flan_t5.py` & `baseten-0.6.6rc1/baseten/models/flan_t5.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/models/llama.py` & `baseten-0.6.6rc1/baseten/models/llama.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/models/stable_diffusion.py` & `baseten-0.6.6rc1/baseten/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/models/util.py` & `baseten-0.6.6rc1/baseten/models/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/models/whisper.py` & `baseten-0.6.6rc1/baseten/models/whisper.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/training/datasets.py` & `baseten-0.6.6rc1/baseten/training/datasets.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/training/finetuning.py` & `baseten-0.6.6rc1/baseten/training/finetuning.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/baseten/training/logs.py` & `baseten-0.6.6rc1/baseten/training/logs.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/pypi_readme.md` & `baseten-0.6.6rc1/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `baseten-0.6.6/pyproject.toml` & `baseten-0.6.6rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baseten"
-version = "0.6.6"
+version = "0.6.6rc1"
 description = "Deploy machine learning models to Baseten"
 readme = "pypi_readme.md"
 authors = [
     "Amir Haghighat <amir@baseten.co>",
     "Phil Howes <phil@baseten.co>",
     "Tuhin Srivastava <tuhin@baseten.co>",
 ]
```

### Comparing `baseten-0.6.6/PKG-INFO` & `baseten-0.6.6rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseten
-Version: 0.6.6
+Version: 0.6.6rc1
 Summary: Deploy machine learning models to Baseten
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Amir Haghighat
 Author-email: amir@baseten.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

