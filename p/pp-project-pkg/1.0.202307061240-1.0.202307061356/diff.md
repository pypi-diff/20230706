# Comparing `tmp/pp_project_pkg-1.0.202307061240-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307061356-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -9,15 +9,15 @@
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5130 b- defN 23-Jul-04 17:08 pp_project_pkg/extra.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     7661 b- defN 23-Jul-06 11:28 pp_project_pkg/train_loop.py
 -rw-rw-r--  2.0 unx     7847 b- defN 23-Jul-04 16:17 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-06 12:40 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-06 13:56 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-04 16:21 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307061240.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-06 12:40 pp_project_pkg-1.0.202307061240.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 12:40 pp_project_pkg-1.0.202307061240.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-06 12:40 pp_project_pkg-1.0.202307061240.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1880 b- defN 23-Jul-06 12:40 pp_project_pkg-1.0.202307061240.dist-info/RECORD
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307061356.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-06 13:56 pp_project_pkg-1.0.202307061356.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 13:56 pp_project_pkg-1.0.202307061356.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-06 13:56 pp_project_pkg-1.0.202307061356.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1880 b- defN 23-Jul-06 13:56 pp_project_pkg-1.0.202307061356.dist-info/RECORD
 21 files, 42259 bytes uncompressed, 12331 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061240.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307061356.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061240.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307061356.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061240.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307061356.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061240.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307061356.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061240.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307061356.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('06')
-VERSION_HOUR = int('12')
-VERSION_MINUTE = int('40')
+VERSION_HOUR = int('13')
+VERSION_MINUTE = int('56')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307061240
-version_date = '2023/07/06 12:40'
+PATCH_VERSION = 202307061356
+version_date = '2023/07/06 13:56'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202307061240.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307061356.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202307061240.dist-info/RECORD` & `pp_project_pkg-1.0.202307061356.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/extra.py,sha256=RreiMggIbiIxM4St8jtlyoUpW7hTxhwyJZ1M_w2UNqc,5130
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/train_loop.py,sha256=w5h4JaroFvA_yYeU2VKe5K6XucSuE_vJs_kQYFzZKi8,7661
 pp_project_pkg/utils.py,sha256=4qIYSi8u7uO2HujXvkYnV4FQ8tyOUbH3Cri8N_aJsY4,7847
-pp_project_pkg/version.py,sha256=kQQfpX44gnMxGdYg9J0fhzeIsJvZLYw4SWKhRcg2JhM,396
+pp_project_pkg/version.py,sha256=SZeg6pwFQOvj15QF5SILBOnyzTjBUc_80Ac3HF_zSbo,396
 pp_project_pkg/wrangling.py,sha256=0l0_MMgUEyjNlwOmrYrEj7pNtvCT_LyZFXOiKSko3PM,5301
-pp_project_pkg-1.0.202307061240.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202307061240.dist-info/METADATA,sha256=nJ7TfSFdhmuaCFrDYEIy7QbsiDzCsijbhxBriV7CcJI,191
-pp_project_pkg-1.0.202307061240.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202307061240.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202307061240.dist-info/RECORD,,
+pp_project_pkg-1.0.202307061356.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202307061356.dist-info/METADATA,sha256=RYM4g9-NiPBYL-Ryuj_4DGT1PwbcO7MUllFrCb2VkEE,191
+pp_project_pkg-1.0.202307061356.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202307061356.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202307061356.dist-info/RECORD,,
```

