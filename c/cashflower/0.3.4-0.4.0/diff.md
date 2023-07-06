# Comparing `tmp/cashflower-0.3.4.tar.gz` & `tmp/cashflower-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.3.4.tar", last modified: Thu Jun  1 15:50:57 2023, max compression
+gzip compressed data, was "cashflower-0.4.0.tar", last modified: Thu Jul  6 19:18:54 2023, max compression
```

## Comparing `cashflower-0.3.4.tar` & `cashflower-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-01 15:50:45.000000 cashflower-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 15:50:45.000000 cashflower-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-01 15:50:57.547887 cashflower-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-01 15:50:45.000000 cashflower-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/cashflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/model_tpl/model.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-01 15:50:45.000000 cashflower-0.3.4/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 15:50:57.000000 cashflower-0.3.4/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:50:57.547887 cashflower-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-01 15:50:45.000000 cashflower-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:50:57.547887 cashflower-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-06-01 15:50:45.000000 cashflower-0.3.4/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-01 15:50:45.000000 cashflower-0.3.4/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-01 15:50:45.000000 cashflower-0.3.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.567023 cashflower-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-06 19:18:44.000000 cashflower-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 19:18:44.000000 cashflower-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-06 19:18:54.567023 cashflower-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-06 19:18:44.000000 cashflower-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.563023 cashflower-0.4.0/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.567023 cashflower-0.4.0/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/model_tpl/model.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.567023 cashflower-0.4.0/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:18:54.567023 cashflower-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-06 19:18:44.000000 cashflower-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.567023 cashflower-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-06 19:18:44.000000 cashflower-0.4.0/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-06 19:18:44.000000 cashflower-0.4.0/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-06 19:18:44.000000 cashflower-0.4.0/tests/test_utils.py
```

### Comparing `cashflower-0.3.4/LICENSE` & `cashflower-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.3.4/PKG-INFO` & `cashflower-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.3.4
+Version: 0.4.0
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cashflower.svg)](https://pypi.org/project/cashflower/)
-[![codecov](https://codecov.io/gh/acturtle/cashflower/branch/main/graph/badge.svg?token=1VA8Q65RUW)](https://codecov.io/gh/acturtle/cashflower)
+[![pytest](https://github.com/acturtle/cashflower/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/acturtle/cashflower/actions/workflows/pytest.yml)
 [![Documentation Status](https://readthedocs.org/projects/cashflower/badge/)](https://cashflower.acturtle.com)
 
 # Info
 
 Cashflower is an open-source Python framework for actuarial cash flow models.
 
 # Prerequisities
@@ -52,29 +52,26 @@
 assumption["mortality"] = pd.read_csv("C:/my_data/mortality.csv", index_col="age")
 ```
 
 ## Model
 
 my_model/model.py
 ```python
-age = ModelVariable()
-death_prob = ModelVariable()
-
-@assign(age)
-def _age(t):
+@variable()
+def age(t):
     if t == 0:
         return int(main.get("AGE"))
     elif t % 12 == 0:
         return age(t-1) + 1
     else:
         return age(t-1)
 
 
-@assign(death_prob)
-def _death_prob(t):
+@variable()
+def death_prob(t):
     if age(t) == age(t-1):
         return death_prob(t-1) 
     elif age(t) <= 100:
         sex = main.get("SEX")
         yearly_rate = assumption["mortality"].loc[age(t)][sex]
         monthly_rate = (1 - (1 - yearly_rate)**(1/12))
         return monthly_rate
@@ -82,20 +79,14 @@
         return 1
 ```
 
 ## Calculate
 
 Run `run.py`
 
-# Quick start
-
-Watch how to create a cash flow model on a YouTube video: 
-
-[![YouTube screenshot](https://img.youtube.com/vi/xuZaymWsUzw/0.jpg)](https://www.youtube.com/watch?v=xuZaymWsUzw)
-
 # Contribution
 
 The cashflower package is open-source. Everyone can use it and contribute to its development.
 
 GitHub repository:
 
 [https://github.com/acturtle/cashflower](https://github.com/acturtle/cashflower)
```

### Comparing `cashflower-0.3.4/README.md` & `cashflower-0.4.0/cashflower.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+Metadata-Version: 2.1
+Name: cashflower
+Version: 0.4.0
+Summary: Framework for actuarial cash flow models
+Home-page: https://github.com/acturtle/cashflower
+Author: Zuzanna Chmielewska
+Project-URL: Source, https://github.com/acturtle/cashflower
+Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
+Project-URL: Documentation, https://cashflower.acturtle.com
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cashflower.svg)](https://pypi.org/project/cashflower/)
-[![codecov](https://codecov.io/gh/acturtle/cashflower/branch/main/graph/badge.svg?token=1VA8Q65RUW)](https://codecov.io/gh/acturtle/cashflower)
+[![pytest](https://github.com/acturtle/cashflower/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/acturtle/cashflower/actions/workflows/pytest.yml)
 [![Documentation Status](https://readthedocs.org/projects/cashflower/badge/)](https://cashflower.acturtle.com)
 
 # Info
 
 Cashflower is an open-source Python framework for actuarial cash flow models.
 
 # Prerequisities
@@ -39,29 +52,26 @@
 assumption["mortality"] = pd.read_csv("C:/my_data/mortality.csv", index_col="age")
 ```
 
 ## Model
 
 my_model/model.py
 ```python
-age = ModelVariable()
-death_prob = ModelVariable()
-
-@assign(age)
-def _age(t):
+@variable()
+def age(t):
     if t == 0:
         return int(main.get("AGE"))
     elif t % 12 == 0:
         return age(t-1) + 1
     else:
         return age(t-1)
 
 
-@assign(death_prob)
-def _death_prob(t):
+@variable()
+def death_prob(t):
     if age(t) == age(t-1):
         return death_prob(t-1) 
     elif age(t) <= 100:
         sex = main.get("SEX")
         yearly_rate = assumption["mortality"].loc[age(t)][sex]
         monthly_rate = (1 - (1 - yearly_rate)**(1/12))
         return monthly_rate
@@ -69,20 +79,14 @@
         return 1
 ```
 
 ## Calculate
 
 Run `run.py`
 
-# Quick start
-
-Watch how to create a cash flow model on a YouTube video: 
-
-[![YouTube screenshot](https://img.youtube.com/vi/xuZaymWsUzw/0.jpg)](https://www.youtube.com/watch?v=xuZaymWsUzw)
-
 # Contribution
 
 The cashflower package is open-source. Everyone can use it and contribute to its development.
 
 GitHub repository:
 
 [https://github.com/acturtle/cashflower](https://github.com/acturtle/cashflower)
```

### Comparing `cashflower-0.3.4/cashflower/start.py` & `cashflower-0.4.0/cashflower/start.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,23 @@
 import importlib
 import inspect
 import multiprocessing
 import os
 import pandas as pd
 import shutil
 
-from .cashflow import CashflowModelError, ModelVariable, ModelPointSet, Model, Constant, Runplan
+from .cashflow import Model, ModelPointSet, Runplan, Variable
+from .error import CashflowModelError
 from .utils import print_log, replace_in_file
 
 
 def create_model(model):
-    """Create a folder structure for a model.
-
+    """
+    Create a folder structure for a model.
     Copies the whole content of the model_tpl folder and changes templates to scripts.
-
-    Parameters
-    ----------
-    model : str
-        Name of the model to be added.
-
     """
     template_path = os.path.join(os.path.dirname(__file__), "model_tpl")
     current_path = os.getcwd()
 
     shutil.copytree(template_path, model)
 
     # Some scripts needs words replacements
@@ -41,32 +36,32 @@
 def load_settings(settings=None):
     """Add missing settings."""
     initial_settings = {
         "AGGREGATE": True,
         "MULTIPROCESSING": False,
         "OUTPUT_COLUMNS": [],
         "ID_COLUMN": "id",
+        "SAVE_DIAGNOSTIC": True,
         "SAVE_OUTPUT": True,
-        "SAVE_RUNTIME": False,
-        "T_CALCULATION_MAX": 1200,
-        "T_OUTPUT_MAX": 1200,
+        "T_MAX_CALCULATION": 720,
+        "T_MAX_OUTPUT": 720,
     }
 
     if settings is None:
         return initial_settings
 
     # Update with the user settings
     for key, value in settings.items():
         initial_settings[key] = value
 
     # Maximal output t can't exceed maximal calculation t
-    if initial_settings["T_CALCULATION_MAX"] < initial_settings["T_OUTPUT_MAX"]:
-        initial_settings["T_OUTPUT_MAX"] = initial_settings["T_CALCULATION_MAX"]
-        msg = "The T_CALCULATION_MAX setting is greater than the T_OUTPUT_MAX setting. " \
-              "T_OUTPUT_MAX has been set to T_CALCULATION_MAX."
+    if initial_settings["T_MAX_CALCULATION"] < initial_settings["T_MAX_OUTPUT"]:
+        initial_settings["T_MAX_OUTPUT"] = initial_settings["T_MAX_CALCULATION"]
+        msg = "The T_MAX_CALCULATION setting is greater than the T_MAX_OUTPUT setting. " \
+              "T_MAX_OUTPUT has been set to T_MAX_CALCULATION."
         print_log(msg)
 
     return initial_settings
 
 
 def get_runplan(input_members):
     """Get runplan object from input.py script."""
@@ -94,162 +89,142 @@
 
     if main is None:
         raise CashflowModelError("\nA model must have a model point set named 'main'.")
 
     return model_point_sets, main
 
 
-def get_variables(model_members, main, settings):
-    """Get model variables from input.py script."""
-    variable_members = [m for m in model_members if isinstance(m[1], ModelVariable)]
+def get_variables(model_members, settings):
+    """Get model variables from model.py script."""
+    variable_members = [m for m in model_members if isinstance(m[1], Variable)]
     variables = []
 
     for name, variable in variable_members:
         if name in ["t", "r"]:
-            msg = f"\nA model component can not be named '{name}' because it is a system variable. Please rename it."
+            msg = f"\nA variable can not be named '{name}' because it is a system variable. Please rename it."
             raise CashflowModelError(msg)
         variable.name = name
         variable.settings = settings
-        variable.initialize(main)
         variables.append(variable)
     return variables
 
 
-def get_constants(model_members, main):
-    """Get constants from input.py script."""
-    constant_members = [m for m in model_members if isinstance(m[1], Constant)]
-    constants = []
-    for name, constant in constant_members:
-        if name in ["t", "r"]:
-            msg = f"\nA model component can not be named '{name}' because it is a system variable. Please rename it."
-            raise CashflowModelError(msg)
-        constant.name = name
-        constant.initialize(main)
-        constants.append(constant)
-    return constants
-
-
 def prepare_model_input(model_name, settings, argv):
     """Get input for the cash flow model."""
     input_module = importlib.import_module(model_name + ".input")
     model_module = importlib.import_module(model_name + ".model")
 
     # input.py contains runplan and model point sets
     input_members = inspect.getmembers(input_module)
     runplan = get_runplan(input_members)
     model_point_sets, main = get_model_point_sets(input_members, settings)
 
-    # model.py contains model variables and constants
+    # model.py contains model variables
     model_members = inspect.getmembers(model_module)
-    variables = get_variables(model_members, main, settings)
-    constants = get_constants(model_members, main)
+    variables = get_variables(model_members, settings)
 
     # User can provide runplan version in CLI command
     if runplan is not None and len(argv) > 1:
         runplan.version = argv[1]
 
-    return runplan, model_point_sets, variables, constants
-
-
-def dict_to_csv(_dict, timestamp):
-    if not os.path.exists("output"):
-        os.makedirs("output")
-
-    for key in _dict:
-        filepath = f"output/{timestamp}_{key}.csv"
-        data = _dict.get(key)
-        data.to_csv(filepath, index=False)
-        print(f"{' ' * 10} {filepath}")
-
-    return None
-
-
-def df_to_csv(df, timestamp):
-    df.to_csv(f"output/{timestamp}_runtime.csv", index=False)
-    print(f"{' ' * 10} output/{timestamp}_runtime.csv")
-    return None
+    return runplan, model_point_sets, variables
 
 
 def start_single_core(model_name, settings, argv):
     """Create and run a cash flow model."""
-    runplan, model_point_sets, variables, constants = prepare_model_input(model_name, settings, argv)
+    runplan, model_point_sets, variables = prepare_model_input(model_name, settings, argv)
 
     # Run model on single core
-    model = Model(model_name, variables, constants, model_point_sets, settings)
+    model = Model(model_name, variables, model_point_sets, settings)
     model_output, runtime = model.run()
     return model_output, runtime
 
 
 def start_multiprocessing(part, cpu_count, model_name, settings, argv):
     """Run subset of the model points using multiprocessing."""
-    runplan, model_point_sets, variables, constants = prepare_model_input(model_name, settings, argv)
+    runplan, model_point_sets, variables = prepare_model_input(model_name, settings, argv)
 
     # Run model on multiple cores
-    model = Model(model_name, variables, constants, model_point_sets, settings, cpu_count)
-
+    model = Model(model_name, variables, model_point_sets, settings, cpu_count)
     output = model.run(part)
+
     if output is None:
         part_model_output, part_runtime = None, None
     else:
         part_model_output, part_runtime = output
     return part_model_output, part_runtime
 
 
 def merge_part_model_outputs(part_model_outputs, settings):
     """Merge outputs from multiprocessing and save to files."""
     # Nones are returned, when number of policies < number of cpus
     part_model_outputs = [pmo for pmo in part_model_outputs if pmo is not None]
-    first = part_model_outputs[0]
 
-    # Merge outputs into one
-    model_output = {}
-    for key in first.keys():
-        if settings["AGGREGATE"]:
-            model_output[key] = sum(pmo[key] for pmo in part_model_outputs)
-        else:
-            model_output[key] = pd.concat(pmo[key] for pmo in part_model_outputs)
+    # Merge or concatenate outputs into one
+    if settings["AGGREGATE"] is False:
+        model_output = pd.concat(part_model_outputs)
+    else:
+        model_output = functools.reduce(lambda x, y: x.add(y, fill_value=0), part_model_outputs)
+
     return model_output
 
 
-def merge_part_runtimes(part_runtimes):
-    total_runtimes = sum([pr["runtime"] for pr in part_runtimes])
-    first = part_runtimes[0]
+def merge_part_diagnostic(part_diagnostic):
+    # Nones are returned, when number of policies < number of cpus
+    part_diagnostic = [pd for pd in part_diagnostic if pd is not None]
+    total_runtimes = sum([pd["runtime"] for pd in part_diagnostic])
+    first = part_diagnostic[0]
     runtimes = pd.DataFrame({
-        "component": first["component"],
+        "variable": first["variable"],
+        "calc_order": first["calc_order"],
+        "cycle": first["cycle"],
+        "calc_direction": first["calc_direction"],
         "runtime": total_runtimes
     })
     return runtimes
 
 
 def start(model_name, settings, argv):
     timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
     settings = load_settings(settings)
+    output, diagnostic = None, None
 
     if settings["MULTIPROCESSING"]:
         cpu_count = multiprocessing.cpu_count()
         p = functools.partial(start_multiprocessing, cpu_count=cpu_count, model_name=model_name, settings=settings,
                               argv=argv)
         with multiprocessing.Pool(cpu_count) as pool:
             parts = pool.map(p, range(cpu_count))
+
+        # Merge model outputs
         part_model_outputs = [p[0] for p in parts]
         output = merge_part_model_outputs(part_model_outputs, settings)
+
+        # Merge runtimes
         if settings["SAVE_RUNTIME"]:
             part_runtimes = [p[1] for p in parts]
-            runtime = merge_part_runtimes(part_runtimes)
+            diagnostic = merge_part_diagnostic(part_runtimes)
     else:
-        output, runtime = start_single_core(model_name, settings, argv)
+        output, diagnostic = start_single_core(model_name, settings, argv)
 
     # Add time column
-    for key in output.keys():
-        values = [*range(settings["T_OUTPUT_MAX"]+1)] * int(output[key].shape[0] / (settings["T_OUTPUT_MAX"]+1))
-        output[key].insert(0, "t", values)
+    values = [*range(settings["T_MAX_OUTPUT"]+1)] * int(output.shape[0] / (settings["T_MAX_OUTPUT"]+1))
+    output.insert(0, "t", values)
+
+    # Save to csv files
+    if not os.path.exists("output"):
+        os.makedirs("output")
 
     if settings["SAVE_OUTPUT"]:
-        print_log("Saving results:")
-        dict_to_csv(output, timestamp)
+        print_log("Saving output:")
+        filepath = f"output/{timestamp}_output.csv"
+        output.to_csv(filepath, index=False)
+        print(f"{' ' * 10} {filepath}")
 
-    if settings["SAVE_RUNTIME"]:
-        print_log("Saving runtime:")
-        df_to_csv(runtime, timestamp)
+    if settings["SAVE_DIAGNOSTIC"]:
+        print_log("Saving diagnostic file:")
+        filepath = f"output/{timestamp}_diagnostic.csv"
+        diagnostic.to_csv(filepath, index=False)
+        print(f"{' ' * 10} {filepath}")
 
     print_log("Finished")
     return output
```

### Comparing `cashflower-0.3.4/cashflower.egg-info/PKG-INFO` & `cashflower-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-Metadata-Version: 2.1
-Name: cashflower
-Version: 0.3.4
-Summary: Framework for actuarial cash flow models
-Home-page: https://github.com/acturtle/cashflower
-Author: Zuzanna Chmielewska
-Project-URL: Source, https://github.com/acturtle/cashflower
-Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
-Project-URL: Documentation, https://cashflower.acturtle.com
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cashflower.svg)](https://pypi.org/project/cashflower/)
-[![codecov](https://codecov.io/gh/acturtle/cashflower/branch/main/graph/badge.svg?token=1VA8Q65RUW)](https://codecov.io/gh/acturtle/cashflower)
+[![pytest](https://github.com/acturtle/cashflower/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/acturtle/cashflower/actions/workflows/pytest.yml)
 [![Documentation Status](https://readthedocs.org/projects/cashflower/badge/)](https://cashflower.acturtle.com)
 
 # Info
 
 Cashflower is an open-source Python framework for actuarial cash flow models.
 
 # Prerequisities
@@ -52,29 +39,26 @@
 assumption["mortality"] = pd.read_csv("C:/my_data/mortality.csv", index_col="age")
 ```
 
 ## Model
 
 my_model/model.py
 ```python
-age = ModelVariable()
-death_prob = ModelVariable()
-
-@assign(age)
-def _age(t):
+@variable()
+def age(t):
     if t == 0:
         return int(main.get("AGE"))
     elif t % 12 == 0:
         return age(t-1) + 1
     else:
         return age(t-1)
 
 
-@assign(death_prob)
-def _death_prob(t):
+@variable()
+def death_prob(t):
     if age(t) == age(t-1):
         return death_prob(t-1) 
     elif age(t) <= 100:
         sex = main.get("SEX")
         yearly_rate = assumption["mortality"].loc[age(t)][sex]
         monthly_rate = (1 - (1 - yearly_rate)**(1/12))
         return monthly_rate
@@ -82,20 +66,14 @@
         return 1
 ```
 
 ## Calculate
 
 Run `run.py`
 
-# Quick start
-
-Watch how to create a cash flow model on a YouTube video: 
-
-[![YouTube screenshot](https://img.youtube.com/vi/xuZaymWsUzw/0.jpg)](https://www.youtube.com/watch?v=xuZaymWsUzw)
-
 # Contribution
 
 The cashflower package is open-source. Everyone can use it and contribute to its development.
 
 GitHub repository:
 
 [https://github.com/acturtle/cashflower](https://github.com/acturtle/cashflower)
```

### Comparing `cashflower-0.3.4/setup.py` & `cashflower-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 
 setup(
     author="Zuzanna Chmielewska",
     description="Framework for actuarial cash flow models",
     include_package_data=True,
     install_requires=[
         'pandas',
+        'networkx'
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="cashflower",
     packages=find_packages(include=["cashflower", "cashflower.*"]),
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.3.4",
+    version="0.4.0",
 )
```

