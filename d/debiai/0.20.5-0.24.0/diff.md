# Comparing `tmp/debiai-0.20.5.tar.gz` & `tmp/debiai-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debiai-0.20.5.tar", last modified: Fri Feb 10 14:35:18 2023, max compression
+gzip compressed data, was "debiai-0.24.0.tar", last modified: Thu Jul  6 15:19:47 2023, max compression
```

## Comparing `debiai-0.20.5.tar` & `debiai-0.24.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:35:18.428446 debiai-0.20.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-02-10 14:35:12.000000 debiai-0.20.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-02-10 14:35:18.428446 debiai-0.20.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-02-10 14:35:12.000000 debiai-0.20.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:35:18.428446 debiai-0.20.5/debiai/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:35:18.428446 debiai-0.20.5/debiai/debiai_services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai_services/df_to_dict_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai_services/np_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/debiai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-02-10 14:35:12.000000 debiai-0.20.5/debiai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:35:18.428446 debiai-0.20.5/debiai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-02-10 14:35:18.000000 debiai-0.20.5/debiai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-10 14:35:18.000000 debiai-0.20.5/debiai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:35:18.000000 debiai-0.20.5/debiai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-10 14:35:18.000000 debiai-0.20.5/debiai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-10 14:35:18.000000 debiai-0.20.5/debiai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 14:35:18.428446 debiai-0.20.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-10 14:35:12.000000 debiai-0.20.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:35:18.428446 debiai-0.20.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 14:35:12.000000 debiai-0.20.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-10 14:35:12.000000 debiai-0.20.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-02-10 14:35:12.000000 debiai-0.20.5/tests/test_project_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-02-10 14:35:12.000000 debiai-0.20.5/tests/test_projects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.874458 debiai-0.24.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-06 15:19:42.000000 debiai-0.24.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-06 15:19:47.870458 debiai-0.24.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-06 15:19:42.000000 debiai-0.24.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.870458 debiai-0.24.0/debiai/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21746 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.870458 debiai-0.24.0/debiai/debiai_services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_services/df_to_dict_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_services/np_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/debiai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-06 15:19:42.000000 debiai-0.24.0/debiai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.870458 debiai-0.24.0/debiai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 15:19:47.000000 debiai-0.24.0/debiai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 15:19:47.874458 debiai-0.24.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-06 15:19:42.000000 debiai-0.24.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:47.870458 debiai-0.24.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:19:42.000000 debiai-0.24.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-06 15:19:42.000000 debiai-0.24.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-06 15:19:42.000000 debiai-0.24.0/tests/test_project_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-06 15:19:42.000000 debiai-0.24.0/tests/test_projects.py
```

### Comparing `debiai-0.20.5/LICENSE` & `debiai-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/PKG-INFO` & `debiai-0.24.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debiai
-Version: 0.20.5
+Version: 0.24.0
 Summary: DebiAI python module
 Home-page: https://github.com/debiai/py-debiai
 Author: IRT-SystemX
 Author-email: debiai@irt-systemx.fr
 License: Apache 2.0
 Keywords: DebiAI,Data vis,AI,Bias
 Classifier: Programming Language :: Python :: 3
@@ -20,31 +20,31 @@
 ![Build](https://github.com/debiai/py-debiai/actions/workflows/python-publish.yml/badge.svg)
 ![Test](https://github.com/debiai/py-debiai/actions/workflows/python-test.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/badge/debiai)](https://pepy.tech/project/debiai)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 The DebiAI Python module is an interface with [DebiAI](https://debiai.irt-systemx.fr), you can use directly it in your Python project workflow to provide DebiAI with data.
 
-## Documentation
+## Web documentation
 [DebiAI Python module](https://debiai.irt-systemx.fr/dataInsertion/pythonModule)
 
 ## Features :
 - Basic:
   - Project creation
   - Project data insertion
   - Model metadata and model results insertion
 - Advanced:
   - Selection made with the dashboard samples recovery
   - tf.dataset creation from the project selections (beta)
 
-## Requierements:
+## Requirements:
 * [A running DebiAI instance](https://debiai.irt-systemx.fr/debiai/gettingStarted/installation/)
 * Numpy
 * Pandas
-* Eventualy Tensorflow
+* Eventually Tensorflow
 
 ## Installation
 
 ### With Pypi
 ```bash
 pip install --upgrade debiai
 ```
@@ -63,15 +63,15 @@
 from debiai import debiai
 import pandas as pd
 import numpy as np
 
 DEBIAI_URL = "http://localhost:3000/"
 DEBIAI_PROJECT_NAME = "Hello DebiAI"
 
-# Initialisation
+# Initialization
 my_debiai = debiai.Debiai(DEBIAI_URL)
 
 # Creating a project
 debiai_project = my_debiai.create_project(DEBIAI_PROJECT_NAME)
 
 # Creating the project block structure
 block_structure = [
@@ -84,14 +84,17 @@
         ],
         "groundTruth": [
             {"name": "My groundtruth 1", "type": "number"}
         ]
     }
 ]
 
+# Each columns belongs to a category, but you can algo group with a optional "group" key
+# The columns with the same group will be grouped in the dashboard
+
 debiai_project.set_blockstructure(block_structure)
 
 
 # ======== Adding the project samples ========
 # Adding samples with a dataframe
 samples_df = pd.DataFrame({
     "Image ID":         ["image-1", "image-2", "image-3"],
@@ -135,15 +138,15 @@
     "Model result": [5, 7, 19],
     "Model confidence": [0.22, 0.8, 0.9],
     "Model error": ["yes", "no", "no"],
 })
 
 debiai_model_2.add_results_df(results_df)
 
-# The model results are ready to be analysed with the Debiai dashboard
+# The model results are ready to be analyzed with the Debiai dashboard
 ```
 <img src="./images/quickstart_results.png">
 
 ## Limitations
 - Nan or empty values are not supported at the moment.
 - `/`, `.`, `:`, `?`, `*`, `\`, and `|`, are not supported in the project name and in the data/blocks ids.
```

### Comparing `debiai-0.20.5/README.md` & `debiai-0.24.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 ![Build](https://github.com/debiai/py-debiai/actions/workflows/python-publish.yml/badge.svg)
 ![Test](https://github.com/debiai/py-debiai/actions/workflows/python-test.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/badge/debiai)](https://pepy.tech/project/debiai)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 The DebiAI Python module is an interface with [DebiAI](https://debiai.irt-systemx.fr), you can use directly it in your Python project workflow to provide DebiAI with data.
 
-## Documentation
+## Web documentation
 [DebiAI Python module](https://debiai.irt-systemx.fr/dataInsertion/pythonModule)
 
 ## Features :
 - Basic:
   - Project creation
   - Project data insertion
   - Model metadata and model results insertion
 - Advanced:
   - Selection made with the dashboard samples recovery
   - tf.dataset creation from the project selections (beta)
 
-## Requierements:
+## Requirements:
 * [A running DebiAI instance](https://debiai.irt-systemx.fr/debiai/gettingStarted/installation/)
 * Numpy
 * Pandas
-* Eventualy Tensorflow
+* Eventually Tensorflow
 
 ## Installation
 
 ### With Pypi
 ```bash
 pip install --upgrade debiai
 ```
@@ -47,15 +47,15 @@
 from debiai import debiai
 import pandas as pd
 import numpy as np
 
 DEBIAI_URL = "http://localhost:3000/"
 DEBIAI_PROJECT_NAME = "Hello DebiAI"
 
-# Initialisation
+# Initialization
 my_debiai = debiai.Debiai(DEBIAI_URL)
 
 # Creating a project
 debiai_project = my_debiai.create_project(DEBIAI_PROJECT_NAME)
 
 # Creating the project block structure
 block_structure = [
@@ -68,14 +68,17 @@
         ],
         "groundTruth": [
             {"name": "My groundtruth 1", "type": "number"}
         ]
     }
 ]
 
+# Each columns belongs to a category, but you can algo group with a optional "group" key
+# The columns with the same group will be grouped in the dashboard
+
 debiai_project.set_blockstructure(block_structure)
 
 
 # ======== Adding the project samples ========
 # Adding samples with a dataframe
 samples_df = pd.DataFrame({
     "Image ID":         ["image-1", "image-2", "image-3"],
@@ -119,15 +122,15 @@
     "Model result": [5, 7, 19],
     "Model confidence": [0.22, 0.8, 0.9],
     "Model error": ["yes", "no", "no"],
 })
 
 debiai_model_2.add_results_df(results_df)
 
-# The model results are ready to be analysed with the Debiai dashboard
+# The model results are ready to be analyzed with the Debiai dashboard
 ```
 <img src="./images/quickstart_results.png">
 
 ## Limitations
 - Nan or empty values are not supported at the moment.
 - `/`, `.`, `:`, `?`, `*`, `\`, and `|`, are not supported in the project name and in the data/blocks ids.
```

### Comparing `debiai-0.20.5/debiai/config.py` & `debiai-0.24.0/debiai/config.py`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/debiai/debiai.py` & `debiai-0.24.0/debiai/debiai.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,18 +15,27 @@
 
 
 class Debiai:
     """
     Each Debiai object represent a Debiai server instance
     """
 
-    debiai_url = None
+    debiai_url = ""
 
     def __init__(self, debiai_url: str):
         self.debiai_url = debiai_url
+
+        # Check if the url is valid
+        if self.debiai_url is None or self.debiai_url == "":
+            raise ValueError("Backend url cannot be empty")
+
+        # Remove trailing slash
+        if self.debiai_url[-1] == "/":
+            self.debiai_url = self.debiai_url[:-1]
+
         utils.check_back(debiai_url)
 
     def get_projects(self) -> List[Debiai_project]:
         """
         Return the server existing projects
         """
         projects = []
```

### Comparing `debiai-0.20.5/debiai/debiai_model.py` & `debiai-0.24.0/debiai/debiai_model.py`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/debiai/debiai_project.py` & `debiai-0.24.0/debiai/debiai_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,109 +83,113 @@
                 + str(self.name)
                 + " DEBIAI project block_structure hasn't been set yet"
             )
 
     def set_blockstructure(self, block_structure: List[dict]) -> bool:
         """
         Add a block structure to the project
-        This step is requiered before uploading data
+        This step is required before uploading data
         Throw error if the block structure is already created
 
         block_structure syntax:
 
         [
             {
                 "name": str
                 "contexts": [
                     {
                         "name": str,
                         "type": 'text', 'number', 'boolean',
-                        "default"?: str, number
+                        "default"?: str, number,
+                        "group"?: str
                     },
                     ...
                 ],
                 "inputs": [
                     {
                         "name": str,
                         "type": 'text', 'number', 'boolean',
                         "default"?: str, number
+                        "group"?: str
                     },
                     ...
                 ],
                 "groundtruth": [
                     {
                         "name": str,
                         "type": 'text', 'number', 'boolean',
                         "default"?: str, number
+                        "group"?: str
                     },
                     ...
                 ],
                 "results": [
                     {
                         "name": str,
                         "type": 'text', 'number', 'boolean',
                         "default"?: str, number
+                        "group"?: str
                     },
                     ...
                 ]
             },
             ...
         ]
 
         The last block will be considered the sample block, and will mark the end of the tree
-        At least one block is requiered
+        At least one block is required
 
         """
 
         # Check if blocklevel structure is already created
         proj_info = self.project_infos()
         if proj_info["blockLevelInfo"] != []:
             raise ValueError("Cannot set the blocklevel structure - already created")
 
         # Check that there is at least one block
         if not len(block_structure):
-            raise ValueError("At least a block is requiered in the block structure")
+            raise ValueError("At least a block is required in the block structure")
 
         # Check that all the properties are correct
         for i, block in enumerate(block_structure):
             if "name" not in block:
-                raise ValueError("The 'name' is requiered in the block n°" + (i + 1))
+                raise ValueError("The 'name' is required in the block n°" + str(i + 1))
 
             for type_ in block:
                 if type_ not in DEBIAI_TYPES and type_ != "name":
                     print(
                         "Warning : unknown block type '"
                         + type_
                         + "'. Use those block types : "
                         + str(DEBIAI_TYPES)
                     )
 
             for debiai_type in DEBIAI_TYPES:
                 if debiai_type in block:
-                    for collumn in block[debiai_type]:
-                        if "name" not in collumn:
+                    for column in block[debiai_type]:
+                        if "name" not in column:
                             raise ValueError(
-                                "The name of the column is requiered in the '"
+                                "The name of the column is required in the '"
                                 + debiai_type
                                 + "' in the block '"
                                 + block["name"]
                                 + "'"
                             )
-                        if "type" not in collumn:
+                        if "type" not in column:
                             raise ValueError(
-                                "The type of the column is requiered in the '"
+                                "The type of the column is required in the '"
                                 + debiai_type
                                 + "' in the block '"
                                 + block["name"]
                                 + "'"
                             )
-                        if collumn["type"] not in ["text", "number", "boolean"]:
+                        if column["type"] not in ["text", "number", "boolean"]:
                             raise ValueError(
                                 "Unknown type of the column '"
-                                + collumn["name"]
+                                + column["name"]
                                 + "' in the block '"
                                 + block["name"]
                                 + "'. Use : ['text', 'number', 'boolean']"
                             )
 
         # Set the block_structure
         utils.add_blocklevel(self.debiai_url, self.id, block_structure)
@@ -214,17 +218,17 @@
         if self.expected_results is not None:
             raise ValueError("The project expected results have been already set")
 
         expResults = []
 
         for column in expected_results:
             if "name" not in column:
-                raise ValueError("The attribute 'name' is requiered in each column")
+                raise ValueError("The attribute 'name' is required in each column")
             if "type" not in column:
-                raise ValueError("The attribute 'type' is requiered in each column")
+                raise ValueError("The attribute 'type' is required in each column")
 
             col = [c for c in expResults if c["name"] == column["name"]]
             if len(col) > 0:
                 raise ValueError("Each result name need to be unique")
 
             newRes = {"name": column["name"], "type": column["type"]}
 
@@ -239,23 +243,23 @@
 
     def add_expected_result(self, column: dict) -> List[dict]:
         if self.expected_results is None:
             raise ValueError("The project does not have an expected results to update")
 
         if "name" not in column:
             raise ValueError(
-                "The attribute 'name' is requiered in the new result column"
+                "The attribute 'name' is required in the new result column"
             )
         if "type" not in column:
             raise ValueError(
-                "The attribute 'type' is requiered in the new result column"
+                "The attribute 'type' is required in the new result column"
             )
         if "default" not in column:
             raise ValueError(
-                "The attribute 'default' is requiered in the new result column"
+                "The attribute 'default' is required in the new result column"
             )
 
         # TODO check default type same as col type
 
         col = [c for c in self.expected_results if c["name"] == column["name"]]
         if len(col) > 0:
             raise ValueError("'" + column["name"] + "' is already expected as a result")
@@ -292,16 +296,16 @@
                                 =======block_1=======   ======block_2======   ========samples=========
                                 context_a, context_b,   context_c, input_d,   input_e, GDT_f, result_g
 
         The numpy array first row should containt the folowing labels in any order:
                                 block_1, context_a, context_b, block_2, context_c, input_d, samples, input_e, GDT_f
         note that the result_g is not asked.
 
-        If one the the requiered labels are missing, the samples wont be uploaded.
-        Any labels that are not requiered will be ignored
+        If one the the required labels are missing, the samples wont be uploaded.
+        Any labels that are not required will be ignored
         The folowing rows, if the types are correct, will be added to the database.
         """
 
         self.get_block_structure()  # Check that the block_structure has been set
 
         # Check that the array is correct and create a column index map
         indexMap = check_np_array(self.block_structure, samples)
@@ -336,16 +340,16 @@
                                 =======block_1=======   ======block_2======   ========samples=========
                                 context_a, context_b,   context_c, input_d,   input_e, GDT_f, result_g
 
         The dataframe columns should containt the folowing labels in any order:
                                 block_1, context_a, context_b, block_2, context_c, input_d, samples, input_e, GDT_f
         note that the result_g is not asked.
 
-        If one the the requiered labels are missing, the samples wont be uploaded.
-        Any labels that aren't requiered will be ignored
+        If one the the required labels are missing, the samples wont be uploaded.
+        Any labels that aren't required will be ignored
         """
         self.get_block_structure()  # Check that the block_structure has been set
 
         SAMPLE_CHUNK_SIZE = 5000  # Nuber of sample that will be added in one chunk
         SAMPLE_TO_UPLOAD = df.shape[0]
         p_bar = utils.progress_bar("Adding samples", SAMPLE_TO_UPLOAD)
 
@@ -378,26 +382,26 @@
             if name == model_name:
                 return Debiai_model(self, id, name)
         return None
 
     def create_model(self, name: str, metadata: dict = {}) -> Debiai_model:
         #  check parameters
         if not name:
-            raise ValueError("Can't create the model: The model name is requiered")
+            raise ValueError("Can't create the model: The model name is required")
 
         # Call the backend
         if utils.post_model(self.debiai_url, self.id, name, metadata):
             return Debiai_model(self, name, name)
         else:
             return False
 
     def delete_model(self, model_name: str) -> bool:
         #  check parameters
         if not model_name:
-            raise ValueError("Can't delete the model: The model name is requiered")
+            raise ValueError("Can't delete the model: The model name is required")
         # Find the model ID
         model = self.get_model(model_name)
         if not model:
             raise ValueError("The model '" + model_name + "' does not exist")
 
         # Call the backend
         utils.delete_model(self.debiai_url, self.id, model.id)
```

### Comparing `debiai-0.20.5/debiai/debiai_selection.py` & `debiai-0.24.0/debiai/debiai_selection.py`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/debiai/debiai_services/df_to_dict_tree.py` & `debiai-0.24.0/debiai/debiai_services/df_to_dict_tree.py`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/debiai/debiai_services/np_to_dict.py` & `debiai-0.24.0/debiai/debiai_services/np_to_dict.py`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/debiai/debiai_tag.py` & `debiai-0.24.0/debiai/debiai_tag.py`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/debiai/debiai_utils.py` & `debiai-0.24.0/debiai/debiai_utils.py`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/debiai.egg-info/PKG-INFO` & `debiai-0.24.0/debiai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debiai
-Version: 0.20.5
+Version: 0.24.0
 Summary: DebiAI python module
 Home-page: https://github.com/debiai/py-debiai
 Author: IRT-SystemX
 Author-email: debiai@irt-systemx.fr
 License: Apache 2.0
 Keywords: DebiAI,Data vis,AI,Bias
 Classifier: Programming Language :: Python :: 3
@@ -20,31 +20,31 @@
 ![Build](https://github.com/debiai/py-debiai/actions/workflows/python-publish.yml/badge.svg)
 ![Test](https://github.com/debiai/py-debiai/actions/workflows/python-test.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/badge/debiai)](https://pepy.tech/project/debiai)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 The DebiAI Python module is an interface with [DebiAI](https://debiai.irt-systemx.fr), you can use directly it in your Python project workflow to provide DebiAI with data.
 
-## Documentation
+## Web documentation
 [DebiAI Python module](https://debiai.irt-systemx.fr/dataInsertion/pythonModule)
 
 ## Features :
 - Basic:
   - Project creation
   - Project data insertion
   - Model metadata and model results insertion
 - Advanced:
   - Selection made with the dashboard samples recovery
   - tf.dataset creation from the project selections (beta)
 
-## Requierements:
+## Requirements:
 * [A running DebiAI instance](https://debiai.irt-systemx.fr/debiai/gettingStarted/installation/)
 * Numpy
 * Pandas
-* Eventualy Tensorflow
+* Eventually Tensorflow
 
 ## Installation
 
 ### With Pypi
 ```bash
 pip install --upgrade debiai
 ```
@@ -63,15 +63,15 @@
 from debiai import debiai
 import pandas as pd
 import numpy as np
 
 DEBIAI_URL = "http://localhost:3000/"
 DEBIAI_PROJECT_NAME = "Hello DebiAI"
 
-# Initialisation
+# Initialization
 my_debiai = debiai.Debiai(DEBIAI_URL)
 
 # Creating a project
 debiai_project = my_debiai.create_project(DEBIAI_PROJECT_NAME)
 
 # Creating the project block structure
 block_structure = [
@@ -84,14 +84,17 @@
         ],
         "groundTruth": [
             {"name": "My groundtruth 1", "type": "number"}
         ]
     }
 ]
 
+# Each columns belongs to a category, but you can algo group with a optional "group" key
+# The columns with the same group will be grouped in the dashboard
+
 debiai_project.set_blockstructure(block_structure)
 
 
 # ======== Adding the project samples ========
 # Adding samples with a dataframe
 samples_df = pd.DataFrame({
     "Image ID":         ["image-1", "image-2", "image-3"],
@@ -135,15 +138,15 @@
     "Model result": [5, 7, 19],
     "Model confidence": [0.22, 0.8, 0.9],
     "Model error": ["yes", "no", "no"],
 })
 
 debiai_model_2.add_results_df(results_df)
 
-# The model results are ready to be analysed with the Debiai dashboard
+# The model results are ready to be analyzed with the Debiai dashboard
 ```
 <img src="./images/quickstart_results.png">
 
 ## Limitations
 - Nan or empty values are not supported at the moment.
 - `/`, `.`, `:`, `?`, `*`, `\`, and `|`, are not supported in the project name and in the data/blocks ids.
```

### Comparing `debiai-0.20.5/debiai.egg-info/SOURCES.txt` & `debiai-0.24.0/debiai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debiai-0.20.5/setup.py` & `debiai-0.24.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="debiai",
-    version="0.20.5",
+    version="0.24.0",
     author="IRT-SystemX",
     author_email="debiai@irt-systemx.fr",
     description="DebiAI python module",
     license="Apache 2.0",
     keywords="DebiAI, Data vis, AI, Bias",
     url="https://github.com/debiai/py-debiai",
     long_description=open("README.md").read(),
```

### Comparing `debiai-0.20.5/tests/test_project_samples.py` & `debiai-0.24.0/tests/test_project_samples.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 PROJECT_NAME = "test_samples"
 
 block_structure = [
     {
         "name": "Image ID",
         "contexts": [
             {"name": "My context 1", "type": "text"},
-            {"name": "My context 2", "type": "number"},
+            {"name": "My context 2", "type": "number", "group": "My group 1"},
         ],
         "groundTruth": [{"name": "My groundtruth 1", "type": "number"}],
     }
 ]
 
 
 expected_results = [
```

### Comparing `debiai-0.20.5/tests/test_projects.py` & `debiai-0.24.0/tests/test_projects.py`

 * *Files identical despite different names*

