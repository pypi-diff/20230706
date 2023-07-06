# Comparing `tmp/mlserver-xgboost-1.4.0.dev2.tar.gz` & `tmp/mlserver_xgboost-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-xgboost-1.4.0.dev2.tar", last modified: Thu May  4 09:30:37 2023, max compression
+gzip compressed data, was "mlserver_xgboost-1.4.0.dev3.tar", max compression
```

## Comparing `mlserver-xgboost-1.4.0.dev2.tar` & `mlserver_xgboost-1.4.0.dev3.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 09:30:36.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 09:30:37.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:36.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 09:30:36.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 09:30:36.000000 mlserver-xgboost-1.4.0.dev2/mlserver_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:37.289166 mlserver-xgboost-1.4.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-04 09:29:57.000000 mlserver-xgboost-1.4.0.dev2/setup.py
+-rw-r--r--   0        0        0    11354 2023-07-05 11:14:06.611541 mlserver_xgboost-1.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0     3432 2023-07-05 11:14:06.611541 mlserver_xgboost-1.4.0.dev3/README.md
+-rw-r--r--   0        0        0       62 2023-07-05 11:14:06.611541 mlserver_xgboost-1.4.0.dev3/mlserver_xgboost/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-05 11:14:06.611541 mlserver_xgboost-1.4.0.dev3/mlserver_xgboost/version.py
+-rw-r--r--   0        0        0     3146 2023-07-05 11:14:06.611541 mlserver_xgboost-1.4.0.dev3/mlserver_xgboost/xgboost.py
+-rw-r--r--   0        0        0      540 2023-07-05 11:14:06.611541 mlserver_xgboost-1.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 mlserver_xgboost-1.4.0.dev3/PKG-INFO
```

### Comparing `mlserver-xgboost-1.4.0.dev2/LICENSE` & `mlserver_xgboost-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-xgboost-1.4.0.dev2/mlserver_xgboost/xgboost.py` & `mlserver_xgboost-1.4.0.dev3/mlserver_xgboost/xgboost.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ResponseOutput,
 )
 
 PREDICT_OUTPUT = "predict"
 PREDICT_PROBA_OUTPUT = "predict_proba"
 VALID_OUTPUTS = [PREDICT_OUTPUT, PREDICT_PROBA_OUTPUT]
 
-WELLKNOWN_MODEL_FILENAMES = ["model.bst", "model.json"]
+WELLKNOWN_MODEL_FILENAMES = ["model.bst", "model.json", "model.ubj"]
 
 
 def _load_sklearn_interface(model_uri: str) -> XGBModel:
     try:
         regressor = xgb.XGBRegressor()
         regressor.load_model(model_uri)
         return regressor
```

