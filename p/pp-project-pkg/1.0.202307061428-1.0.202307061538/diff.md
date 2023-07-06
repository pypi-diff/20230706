# Comparing `tmp/pp_project_pkg-1.0.202307061428-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307061538-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -9,15 +9,15 @@
 -rw-rw-r--  2.0 unx      669 b- defN 23-Jul-06 14:21 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5130 b- defN 23-Jul-04 17:08 pp_project_pkg/extra.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     7661 b- defN 23-Jul-06 11:28 pp_project_pkg/train_loop.py
 -rw-rw-r--  2.0 unx     7847 b- defN 23-Jul-04 16:17 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-06 14:28 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-06 15:38 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-04 16:21 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307061428.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-06 15:37 pp_project_pkg-1.0.202307061428.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 15:37 pp_project_pkg-1.0.202307061428.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-06 15:37 pp_project_pkg-1.0.202307061428.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1883 b- defN 23-Jul-06 15:37 pp_project_pkg-1.0.202307061428.dist-info/RECORD
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307061538.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-06 15:38 pp_project_pkg-1.0.202307061538.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 15:38 pp_project_pkg-1.0.202307061538.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-06 15:38 pp_project_pkg-1.0.202307061538.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1883 b- defN 23-Jul-06 15:38 pp_project_pkg-1.0.202307061538.dist-info/RECORD
 21 files, 44198 bytes uncompressed, 13022 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061428.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307061538.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061428.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307061538.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061428.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307061538.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061428.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307061538.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307061428.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307061538.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('06')
-VERSION_HOUR = int('14')
-VERSION_MINUTE = int('28')
+VERSION_HOUR = int('15')
+VERSION_MINUTE = int('38')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307061428
-version_date = '2023/07/06 14:28'
+PATCH_VERSION = 202307061538
+version_date = '2023/07/06 15:38'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202307061428.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307061538.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

