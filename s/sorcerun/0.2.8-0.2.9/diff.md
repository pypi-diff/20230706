# Comparing `tmp/sorcerun-0.2.8.tar.gz` & `tmp/sorcerun-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.2.8.tar", last modified: Mon Jun 26 18:42:34 2023, max compression
+gzip compressed data, was "sorcerun-0.2.9.tar", last modified: Thu Jul  6 18:15:32 2023, max compression
```

## Comparing `sorcerun-0.2.8.tar` & `sorcerun-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:42:34.028813 sorcerun-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-26 18:42:20.000000 sorcerun-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 18:42:34.028813 sorcerun-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-26 18:42:20.000000 sorcerun-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:42:34.028813 sorcerun-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-26 18:42:20.000000 sorcerun-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:42:34.024813 sorcerun-0.2.8/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:42:34.028813 sorcerun-0.2.8/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:15:32.053241 sorcerun-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-06 18:15:20.000000 sorcerun-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-06 18:15:32.053241 sorcerun-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-06 18:15:20.000000 sorcerun-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:15:32.053241 sorcerun-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-06 18:15:20.000000 sorcerun-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:15:32.053241 sorcerun-0.2.9/sorcerun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:15:20.000000 sorcerun-0.2.9/sorcerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-06 18:15:20.000000 sorcerun-0.2.9/sorcerun/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-06 18:15:20.000000 sorcerun-0.2.9/sorcerun/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 18:15:20.000000 sorcerun-0.2.9/sorcerun/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-06 18:15:20.000000 sorcerun-0.2.9/sorcerun/incense_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-06 18:15:20.000000 sorcerun-0.2.9/sorcerun/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-06 18:15:20.000000 sorcerun-0.2.9/sorcerun/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:15:32.053241 sorcerun-0.2.9/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-06 18:15:32.000000 sorcerun-0.2.9/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-06 18:15:32.000000 sorcerun-0.2.9/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:15:32.000000 sorcerun-0.2.9/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 18:15:32.000000 sorcerun-0.2.9/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 18:15:32.000000 sorcerun-0.2.9/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 18:15:32.000000 sorcerun-0.2.9/sorcerun.egg-info/top_level.txt
```

### Comparing `sorcerun-0.2.8/LICENSE` & `sorcerun-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.8/PKG-INFO` & `sorcerun-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.8
+Version: 0.2.9
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.8/README.md` & `sorcerun-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.8/setup.py` & `sorcerun-0.2.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.2.8",
+    version="0.2.9",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred==0.8.4",
         "pymongo",
         "pyyaml",
         "scikit-learn",
+        "incense",
+        "xarray",
+        "tqdm",
     ],
     entry_points="""
         [console_scripts]
-        sorcerun=sorcerun_package.cli:sorcerun
+        sorcerun=sorcerun.cli:sorcerun
     """,
     long_description="Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.",
 )
```

### Comparing `sorcerun-0.2.8/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.2.9/sorcerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.8
+Version: 0.2.9
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.8/sorcerun_package/auth_mongodb_option.py` & `sorcerun-0.2.9/sorcerun/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.8/sorcerun_package/cli.py` & `sorcerun-0.2.9/sorcerun/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from sklearn.model_selection import ParameterGrid
 import os
 import subprocess
 import json, yaml
 from contextlib import ExitStack
 from .mongodb_utils import mongodb_server, init_mongodb
 from .sacred_utils import load_adapter_function, run_sacred_experiment
+from .incense_utils import squish_dict, unsquish_dict
 from .globals import AUTH_FILE
 
 
 @click.group()
 def sorcerun():
     pass
 
@@ -39,32 +40,34 @@
     # Load the adapter function from the provided Python file
     adapter_func = load_adapter_function(python_file)
 
     # Load the config from the provided YAML file
     with open(grid_config_file, "r") as file:
         config = yaml.safe_load(file)
 
+    config = squish_dict(config)
     for k, v in config.items():
         if type(v) != list:
             config[k] = [v]
 
     param_grid = ParameterGrid([config])
     total_num_params = len(param_grid)
     print(f"Parameter grid contains {total_num_params} combinations")
 
     # Run the Sacred experiment with the provided adapter function and config
     for i, param in enumerate(param_grid):
+        conf = unsquish_dict(param)
         print(
             "-" * 5
             + "GRID RUN INFO: "
             + f"Starting run {i+1}/{total_num_params}"
             + "-" * 5
         )
-        print(f"Config:\n{param}")
-        run_sacred_experiment(adapter_func, param, auth_path)
+        print(f"Config:\n{conf}")
+        run_sacred_experiment(adapter_func, conf, auth_path)
         print(
             "-" * 5
             + "GRID RUN INFO: "
             + f"Completed run {i+1}/{total_num_params}"
             + "-" * 5
         )
```

### Comparing `sorcerun-0.2.8/sorcerun_package/mongodb_utils.py` & `sorcerun-0.2.9/sorcerun/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.8/sorcerun_package/sacred_utils.py` & `sorcerun-0.2.9/sorcerun/sacred_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from sacred import Experiment
+import traceback
 from sacred.observers import MongoObserver
 import importlib
 import json
 from .globals import AUTH_FILE
 import sys
 import os
 
@@ -46,8 +47,11 @@
     ex.add_config(config)
 
     @ex.main
     def run_experiment(_config, _run):
         result = adapter_func(_config, _run)
         return result
 
-    ex.run()
+    try:
+        ex.run()
+    except:
+        traceback.print_exc()
```

