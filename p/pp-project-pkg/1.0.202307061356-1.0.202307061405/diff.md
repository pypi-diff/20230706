# Comparing `tmp/pp_project_pkg-1.0.202307061356-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307061405-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 15479 bytes, number of entries: 21
+Zip file size: 15483 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/__init__.py
--rw-rw-r--  2.0 unx     1611 b- defN 23-Jul-06 12:40 mlflow_pipelines/main.py
+-rw-rw-r--  2.0 unx     1628 b- defN 23-Jul-06 14:05 mlflow_pipelines/main.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx      902 b- defN 23-Jul-06 12:34 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5130 b- defN 23-Jul-04 17:08 pp_project_pkg/extra.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     7661 b- defN 23-Jul-06 11:28 pp_project_pkg/train_loop.py
 -rw-rw-r--  2.0 unx     7847 b- defN 23-Jul-04 16:17 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-06 13:56 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-06 14:05 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-04 16:21 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307061356.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-06 13:56 pp_project_pkg-1.0.202307061356.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 13:56 pp_project_pkg-1.0.202307061356.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-06 13:56 pp_project_pkg-1.0.202307061356.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1880 b- defN 23-Jul-06 13:56 pp_project_pkg-1.0.202307061356.dist-info/RECORD
-21 files, 42259 bytes uncompressed, 12331 bytes compressed:  70.8%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307061405.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-06 14:05 pp_project_pkg-1.0.202307061405.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 14:05 pp_project_pkg-1.0.202307061405.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-06 14:05 pp_project_pkg-1.0.202307061405.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1880 b- defN 23-Jul-06 14:05 pp_project_pkg-1.0.202307061405.dist-info/RECORD
+21 files, 42276 bytes uncompressed, 12335 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061356.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307061405.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061356.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307061405.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061356.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307061405.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061356.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307061405.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061356.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307061405.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_pipelines/main.py

```diff
@@ -2,15 +2,15 @@
 import os
 import wandb
 import hydra
 from omegaconf import DictConfig
 
 
 #@hydra.main(config_path='mlflow_pipelines',config_name='config.yaml')
-@hydra.main(config_name='config.yaml')
+@hydra.main(config_path='./',config_name='config.yaml')
 def go(config: DictConfig):
 
     os.environ["WANDB_PROJECT"] = config["main"]["project_name"]
     os.environ["WANDB_RUN_GROUP"] = config["main"]["experiment_name"]
 
     root_path = hydra.utils.get_original_cwd()
     print(config)
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('06')
-VERSION_HOUR = int('13')
-VERSION_MINUTE = int('56')
+VERSION_HOUR = int('14')
+VERSION_MINUTE = int('05')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307061356
-version_date = '2023/07/06 13:56'
+PATCH_VERSION = 202307061405
+version_date = '2023/07/06 14:05'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202307061356.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307061405.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202307061356.dist-info/RECORD` & `pp_project_pkg-1.0.202307061405.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 mlflow_pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mlflow_pipelines/main.py,sha256=FCkXAcFFc7XYPGr7Fy6MOXA4HOrJ8UNwBHQokJ7SeX8,1611
+mlflow_pipelines/main.py,sha256=CcIyIYyGxOcb-4VphZtl8qqvAq5QHLLz1RZFkQpwV8E,1628
 mlflow_pipelines/fetch_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/fetch_data/get_data.py,sha256=OCLNFSznnHCMcPy2_8SKbTr5J_LG4LoOK9XwypRSCg0,902
 mlflow_pipelines/train_model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/train_model/model_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/extra.py,sha256=RreiMggIbiIxM4St8jtlyoUpW7hTxhwyJZ1M_w2UNqc,5130
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/train_loop.py,sha256=w5h4JaroFvA_yYeU2VKe5K6XucSuE_vJs_kQYFzZKi8,7661
 pp_project_pkg/utils.py,sha256=4qIYSi8u7uO2HujXvkYnV4FQ8tyOUbH3Cri8N_aJsY4,7847
-pp_project_pkg/version.py,sha256=SZeg6pwFQOvj15QF5SILBOnyzTjBUc_80Ac3HF_zSbo,396
+pp_project_pkg/version.py,sha256=4_-TZLJnd4sXpiTpvVHWpw02Mb8c5OnVFYfgFLQB2Rk,396
 pp_project_pkg/wrangling.py,sha256=0l0_MMgUEyjNlwOmrYrEj7pNtvCT_LyZFXOiKSko3PM,5301
-pp_project_pkg-1.0.202307061356.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202307061356.dist-info/METADATA,sha256=RYM4g9-NiPBYL-Ryuj_4DGT1PwbcO7MUllFrCb2VkEE,191
-pp_project_pkg-1.0.202307061356.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202307061356.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202307061356.dist-info/RECORD,,
+pp_project_pkg-1.0.202307061405.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202307061405.dist-info/METADATA,sha256=Ze_Mo1WSSd0aAqGOdQOc8uPLAT6sfIYfUnNTw1jeSoo,191
+pp_project_pkg-1.0.202307061405.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202307061405.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202307061405.dist-info/RECORD,,
```

