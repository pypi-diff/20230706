# Comparing `tmp/mvf-0.0.6.tar.gz` & `tmp/mvf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvf-0.0.6.tar", last modified: Tue Jul  4 12:12:54 2023, max compression
+gzip compressed data, was "mvf-0.0.7.tar", last modified: Thu Jul  6 10:34:45 2023, max compression
```

## Comparing `mvf-0.0.6.tar` & `mvf-0.0.7.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.717522 mvf-0.0.6/
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-04 12:12:51.000000 mvf-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3415 2023-07-04 12:12:54.717522 mvf-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2845 2023-07-04 12:12:51.000000 mvf-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.711523 mvf-0.0.6/mvf/
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.713523 mvf-0.0.6/mvf/cli/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.713523 mvf-0.0.6/mvf/dag/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/dag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11636 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/dag/builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.714522 mvf-0.0.6/mvf/integration/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.715523 mvf-0.0.6/mvf/integration/config/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/config/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/config/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/config/preprocess_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/config/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/config/validate.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/config/validate_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1993 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/mvf_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.716523 mvf-0.0.6/mvf/integration/process/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3378 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/process/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/process/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/process/preprocess_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3556 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/process/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/process/validate.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/integration/process/validate_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.717522 mvf-0.0.6/mvf/process/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/process/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4129 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/process/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/process/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/process/validate.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-04 12:12:51.000000 mvf-0.0.6/mvf/process/validate_model_r.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:12:54.712523 mvf-0.0.6/mvf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3415 2023-07-04 12:12:54.000000 mvf-0.0.6/mvf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-04 12:12:54.000000 mvf-0.0.6/mvf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 12:12:54.000000 mvf-0.0.6/mvf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-04 12:12:54.000000 mvf-0.0.6/mvf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-04 12:12:54.000000 mvf-0.0.6/mvf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-04 12:12:54.000000 mvf-0.0.6/mvf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 12:12:54.717522 mvf-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-07-04 12:12:51.000000 mvf-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.251580 mvf-0.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-06 10:34:41.000000 mvf-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-07-06 10:34:45.251580 mvf-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2023-07-06 10:34:41.000000 mvf-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.244580 mvf-0.0.7/mvf/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.246580 mvf-0.0.7/mvf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3850 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.246580 mvf-0.0.7/mvf/dag/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/dag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12435 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/dag/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.247580 mvf-0.0.7/mvf/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.248580 mvf-0.0.7/mvf/integration/config/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/config/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/config/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/config/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/config/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/config/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/config/validate_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1993 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/mvf_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.249580 mvf-0.0.7/mvf/integration/process/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/process/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/integration/process/validate_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.250580 mvf-0.0.7/mvf/process/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5044 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/process/performance_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4134 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4867 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/process/validate_model_r.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.251580 mvf-0.0.7/mvf/template/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-06 10:34:41.000000 mvf-0.0.7/mvf/template/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:45.245580 mvf-0.0.7/mvf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-07-06 10:34:45.000000 mvf-0.0.7/mvf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1135 2023-07-06 10:34:45.000000 mvf-0.0.7/mvf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:34:45.000000 mvf-0.0.7/mvf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-06 10:34:45.000000 mvf-0.0.7/mvf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-06 10:34:45.000000 mvf-0.0.7/mvf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-06 10:34:45.000000 mvf-0.0.7/mvf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 10:34:45.251580 mvf-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2023-07-06 10:34:41.000000 mvf-0.0.7/setup.py
```

### Comparing `mvf-0.0.6/LICENSE` & `mvf-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mvf-0.0.6/PKG-INFO` & `mvf-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
```

### Comparing `mvf-0.0.6/README.md` & `mvf-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mvf-0.0.6/mvf/dag/builder.py` & `mvf-0.0.7/mvf/dag/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import click
 import mvf.integration.config as on_render
 import mvf.integration.process as on_finish
 import mvf.process as process
 import os
 from pathlib import Path
 from ploomber import DAG
 from ploomber.products import File
@@ -10,15 +9,14 @@
 
 
 class DagBuilder:
     def __init__(self, config, output_dir='output') -> None:
         '''
         Assigns key parameters as attributes. Initialises the Ploomber DAG.
         '''
-        click.echo('Building project workflow...')
         self.config = config
         self.output_dir = output_dir
         # path to source code
         self.path_to_process = process.__path__[0]
         self.dag = DAG(
             # set dag name as basename of working dir
             name=os.path.basename(os.getcwd())
@@ -49,14 +47,15 @@
                 validate_model = self.__build_validate_model(name, lang)
                 # set upstream
                 fit_model >> validate_model
             # set upstream
             split_data >> fit_model
             split_data >> predict_model
             fit_model >> predict_model
+            fit_model >> validate
             predict_model >> validate
         # set upstream
         preprocess_data >> split_data
         split_data >> validate
 
 
     def __build_preprocess_data(self):
@@ -206,14 +205,21 @@
                     os.path.join(
                         self.output_dir,
                         'models',
                         task_name
                     ),
                 ),
             }
+        product['process_metadata'] = File(
+            os.path.join(
+                self.output_dir,
+                'metadata',
+                f'{task_name}.metadata'
+            )
+        )
         # define task
         fit_model = PythonCallable(
             source=source,
             product=product,
             dag=self.dag,
             name=task_name,
             params=params,
@@ -247,17 +253,24 @@
         predict_model = PythonCallable(
             source=source,
             product={
                 'predictions': File(
                     os.path.join(
                         self.output_dir,
                         'data',
-                        task_name + '.feather'
+                        f'{task_name}.feather'
                     ),
                 ),
+                'process_metadata': File(
+                    os.path.join(
+                        self.output_dir,
+                        'metadata',
+                        f'{task_name}.metadata'
+                    )
+                )
             },
             dag=self.dag,
             name=task_name,
             params=params
         )
         # hooks
         if lang == 'Python':
@@ -305,32 +318,39 @@
                 ),
             },
             dag=self.dag,
             name=task_name,
             params=params,
         )
         # hooks
-        validate_model.on_render = on_render.validate_model.validate_model
+        if lang == 'Python':
+            validate_model.on_render = on_render.validate_model.validate_model_py
+        else:
+            validate_model.on_render = on_render.validate_model.validate_model_r
         validate_model.on_finish = on_finish.validate_model.validate_model
         return validate_model
 
 
     def __build_validate(self):
         source_path = Path(
             os.path.join(
                 self.path_to_process,
                 'validate.py'
             )
         )
         # params
         params = {
             'split_type': self.config['data']['split'],
+            'models': [model['name'] for model in self.config['models']]
         }
         if self.config['data']['split'] == 'k_fold':
             params['n_folds'] = self.config['data']['n_folds']
+        if 'output' in self.config:
+            if 'quantile_intervals' in self.config['output']:
+                params['quantile_intervals'] = self.config['output']['quantile_intervals']
         # define task
         validate = NotebookRunner(
             source=source_path,
             product={
                 'nb': File(
                     os.path.join(
                         self.output_dir,
```

### Comparing `mvf-0.0.6/mvf/integration/config/fit_model.py` & `mvf-0.0.7/mvf/integration/config/fit_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,54 @@
-import rpy2.robjects as robjects
-from rpy2.robjects import pandas2ri
-import rpy2_r6.r6b as r6b
-
-
 def fit_model_params(product: dict, params: dict) -> None:
     # check params for fit_model tasks
     assert 'model_name' in params, 'The \'model_name\' parameter must be defined.'
     assert 'split_type' in params, 'The \'split_type\' parameter must be defined.'
     if params['split_type'] == 'train_test':
         assert 'model' in product, 'The \'model\' product must be defined.'
     elif params['split_type'] == 'k_fold':
         assert 'n_folds' in params, 'For a K fold split, the n_folds must be defined.'
         n_folds = params['n_folds']
         for i in range(1, n_folds+1):
             assert f'model_{i}' in product, f'The {i}-th model product must be defined.'
 
 
 def fit_model_r(product: dict, params: dict) -> None:
+    import rpy2.robjects as robjects
+    import rpy2_r6.r6b as r6b
+
     # check params
     fit_model_params(product, params)
     # check that the correct model class is available
     r = robjects.r
     try:
         r.source('models.R')
         model_class = r6b.R6DynamicClassGenerator(r[params["model_name"]])
         model = model_class.new()
-        # check the model class has a callable 'fit' method
-        assert hasattr(model, 'fit'), f'The class {params["model_name"]} must have a fit() method. The class does not currently have a fit attribute.'
-        assert callable(getattr(model, 'fit')), f'The class {params["model_name"]} must have a fit() method. The class\' fit attribute is not currently callable.'
+        check_model(model, params['model_name'])
     except rpy2.rinterface_lib.embedded.RRuntimeError:
         raise ModuleNotFoundError(f'If using a R based model for {params["model_name"]}, you must have a models.R file in your project directory.')
 
 
 def fit_model_py(product: dict, params: dict) -> None:
     # check params
     fit_model_params(product, params)
     # check that the correct model class is available
     try:
         import models
         assert hasattr(models, params['model_name']), f'models.py must contain a class called {params["model_name"]}.'
         model_class = getattr(models, params['model_name'])
-        # check the model class has a callable 'fit' method
-        assert hasattr(model_class, 'fit'), f'The class {params["model_name"]} must have a fit() method. The class does not currently have a fit attribute.'
-        assert callable(getattr(model_class, 'fit')), f'The class {params["model_name"]} must have a fit() method. The class\' fit attribute is not currently callable.'
+        check_model(model_class, params['model_name'])
     except ModuleNotFoundError:
         raise ModuleNotFoundError(f'If using a Python based model for {params["model_name"]}, you must have a models.py file in your project directory. The project directory is {os.getcwd()}')
     
 
-from ploomber.products import File
-
-if __name__ == '__main__':
-    product = {
-        'nb': File('/home/tom/projects/model-validation-framework/examples/project1/output/fit_model_2.ipynb'),
-        'nb_html': File('/home/tom/projects/model-validation-framework/examples/project1/output/fit_model_2.html'),
-        'model': File('/home/tom/projects/model-validation-framework/examples/project1/output/fit_model_2')
-    }
-    params = {
-      'model_name': 'r_pois_reg',
-      'split_type': 'train_test'
-    }
-    fit_model_r(product, params)
+def check_model(model_class, model_name):
+    '''
+    Checks the instantiated model class or generic model class has the necessary methods.
+    '''
+    # check the model class has a callable 'fit' method
+    assert hasattr(model_class, 'fit'), f'The class {model_name} must have a fit() method. The class does not currently have a fit attribute.'
+    assert callable(getattr(model_class, 'fit')), f'The class {model_name} must have a fit() method. The class\' fit attribute is not currently callable.'
+    # check the model class has a callable 'save' method
+    assert hasattr(model_class, 'save'), f'The class {model_name} must have a save() method. The class does not currently have a save attribute.'
+    assert callable(getattr(model_class, 'save')), f'The class {model_name} must have a save() method. The class\' save attribute is not currently callable.'
+
```

### Comparing `mvf-0.0.6/mvf/integration/config/predict_model.py` & `mvf-0.0.7/mvf/integration/config/predict_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import rpy2.robjects as robjects
-from rpy2.robjects import pandas2ri
-import rpy2_r6.r6b as r6b
-
-
 def predict_model_py(product, params):
     import models
     # get model class
     model_class = getattr(models, params['model_name'])
     # init model
     model = model_class()
     # run common checks
     predict_model_common(product, params, model)
     
 
 def predict_model_r(product, params):
+    import rpy2.robjects as robjects
+    import rpy2_r6.r6b as r6b
     # get model class
     r = robjects.r
     r.source('models.R')
     model_class = r6b.R6DynamicClassGenerator(r[params['model_name']])
     # init model
     model = model_class.new()
     # run common checks
@@ -28,7 +25,10 @@
     '''
     Method to run checks common to Python and R
     '''
     assert 'predictions' in product, 'The \'predictions\' product must be defined.'
     # check the model has a predict method
     assert hasattr(model, 'predict'), f'The model class defined for {params["model_name"]} must have a predict() method.'
     assert callable(getattr(model, 'predict')), f'The model saved at {params["model_name"]} must have a predict() method. The class\' predict attribute is not currently callable.'
+    # check the model has a load method
+    assert hasattr(model, 'load'), f'The model class defined for {params["model_name"]} must have a load() method.'
+    assert callable(getattr(model, 'load')), f'The model saved at {params["model_name"]} must have a load() method. The class\' load attribute is not currently callable.'
```

### Comparing `mvf-0.0.6/mvf/integration/config/split_data.py` & `mvf-0.0.7/mvf/integration/config/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.6/mvf/integration/mvf_config.py` & `mvf-0.0.7/mvf/integration/mvf_config.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.6/mvf/integration/process/fit_model.py` & `mvf-0.0.7/mvf/integration/process/fit_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.6/mvf/integration/process/predict_model.py` & `mvf-0.0.7/mvf/integration/process/predict_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.6/mvf/integration/process/split_data.py` & `mvf-0.0.7/mvf/integration/process/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.6/mvf/process/fit_model.py` & `mvf-0.0.7/mvf/process/fit_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # imports
 import feather
 import pandas
+from mvf.process.performance_utils import ProcessTimer
 
 
 def fit_py(product, upstream, model_name, split_type, n_folds=10):
+    # start process timer
+    timer = ProcessTimer(f'{model_name}_fit')
     # imports
     import models
 
     if split_type == 'train_test':
         fit_py_train_test(
             product,
             upstream,
@@ -18,14 +21,18 @@
         fit_py_k_fold(
             product,
             upstream,
             model_name,
             models,
             n_folds
         )
+    # end process timer
+    timer.end()
+    # save process metadata
+    timer.save(product['process_metadata'])
 
 
 def fit_py_train_test(product, upstream, model_name, models):
     # load data from upstream process
     X_train = feather.read_dataframe(upstream['split_data']['train_X_data'])
     y_train = feather.read_dataframe(upstream['split_data']['train_y_data'])
 
@@ -79,14 +86,16 @@
     model.fit(X_train, y_train)
 
     # save model for next process
     model.save(path)
 
 
 def fit_r(product, upstream, model_name, split_type, n_folds=10):
+    # start process timer
+    timer = ProcessTimer(f'{model_name}_fit')
     # imports
     import rpy2.robjects as robjects
     from rpy2.robjects import pandas2ri
 
     r = robjects.r
     r.source('models.R')
 
@@ -103,14 +112,18 @@
             product,
             upstream,
             model_name,
             r,
             pandas2ri,
             n_folds
         )
+    # end process timer
+    timer.end()
+    # save process metadata
+    timer.save(product['process_metadata'])
 
 
 def fit_r_train_test(product, upstream, model_name, r, pandas2ri):
     # load data from upstream process
     pandas2ri.activate()
     X_train = pandas2ri.py2rpy_pandasdataframe(
         feather.read_dataframe(
```

### Comparing `mvf-0.0.6/mvf/process/predict_model.py` & `mvf-0.0.7/mvf/process/predict_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # imports
 import feather
 import pandas
+from mvf.process.performance_utils import ProcessTimer
 
 
 def predict_model(upstream, product, lang, model_name, split_type, n_folds=10, quantile_intervals=None):
+    # start process timer
+    timer = ProcessTimer(f'{model_name}_predict')
     # format variable
     upstream = dict(upstream)
 
     # import model class
     if lang == 'Python':
         import models
     elif lang == 'R':
-        import rpy2.robjects.conversion as cv
         import rpy2.robjects as robjects
         from rpy2.robjects import pandas2ri
         import rpy2_r6.r6b as r6b
 
         r = robjects.r
         r['source']('models.R')
-        # def _none2null(none_obj):
-        #     return r('NULL')
-
-
-        # none_converter = cv.Converter("None converter")
-        # none_converter.py2rpy.register(type(None), _none2null)
 
     if split_type == 'train_test':
         # load test data
         X_test = feather.read_dataframe(upstream['split_data']['test_X_data'])
         del upstream['split_data']
 
         # load model
@@ -112,14 +108,18 @@
             # append fold predictions to predictions set
             predictions.append(preds)
         # save data for next process
         feather.write_dataframe(
             pandas.concat(predictions),
             product['predictions']
         )
+    # end process timer
+    timer.end()
+    # save process metadata
+    timer.save(product['process_metadata'])
         
 
 def load_python_model(models, model_name, path):
     model_class = getattr(models, model_name)
     model = model_class()
     model.load(path)
     return model
```

### Comparing `mvf-0.0.6/mvf/process/split_data.py` & `mvf-0.0.7/mvf/process/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.6/mvf/process/validate_model_r.py` & `mvf-0.0.7/mvf/process/validate_model_r.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # imports
-import feather
 import rpy2.robjects as robjects
-from rpy2.robjects import pandas2ri
 import rpy2_r6.r6b as r6b
 r = robjects.r
 r['source']('models.R')
 
 # + tags=["parameters"]
 upstream = None
 product = None
```

### Comparing `mvf-0.0.6/mvf.egg-info/PKG-INFO` & `mvf-0.0.7/mvf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
```

### Comparing `mvf-0.0.6/mvf.egg-info/SOURCES.txt` & `mvf-0.0.7/mvf.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,11 +27,14 @@
 mvf/integration/process/predict_model.py
 mvf/integration/process/preprocess_data.py
 mvf/integration/process/split_data.py
 mvf/integration/process/validate.py
 mvf/integration/process/validate_model.py
 mvf/process/__init__.py
 mvf/process/fit_model.py
+mvf/process/performance_utils.py
 mvf/process/predict_model.py
 mvf/process/split_data.py
 mvf/process/validate.py
-mvf/process/validate_model_r.py
+mvf/process/validate_model_r.py
+mvf/template/__init__.py
+mvf/template/config.py
```

### Comparing `mvf-0.0.6/setup.py` & `mvf-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,11 +59,11 @@
         'Framework :: Jupyter',
         'License :: Free For Educational Use',
         'Operating System :: Unix',
     ],
     python_requires='>=3.9',
     entry_points={
         'console_scripts': [
-            'mvf=mvf.cli.cli:cmd_router'
+            'mvf=mvf.cli.cli:mvf'
         ]
     },
 )
```

