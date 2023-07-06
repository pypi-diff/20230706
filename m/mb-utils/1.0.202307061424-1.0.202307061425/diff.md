# Comparing `tmp/mb_utils-1.0.202307061424-py3-none-any.whl.zip` & `tmp/mb_utils-1.0.202307061425-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 7946 bytes, number of entries: 14
+Zip file size: 7950 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx      311 b- defN 23-Jun-06 15:13 mb_utils/src/__init__.py
 -rw-rw-r--  2.0 unx     3330 b- defN 23-May-30 16:38 mb_utils/src/deprecated.py
 -rw-rw-r--  2.0 unx     1318 b- defN 23-May-30 16:38 mb_utils/src/extra.py
 -rw-rw-r--  2.0 unx     1813 b- defN 23-May-30 16:38 mb_utils/src/logging.py
 -rw-rw-r--  2.0 unx      664 b- defN 23-May-30 16:38 mb_utils/src/path_checker.py
 -rw-rw-r--  2.0 unx     1306 b- defN 23-May-30 16:38 mb_utils/src/retry_decorator.py
--rw-rw-r--  2.0 unx     3817 b- defN 23-Jun-27 15:44 mb_utils/src/s3.py
+-rw-rw-r--  2.0 unx     3817 b- defN 23-Jul-06 14:25 mb_utils/src/s3.py
 -rw-rw-r--  2.0 unx      777 b- defN 23-May-30 16:38 mb_utils/src/terminal.py
 -rw-rw-r--  2.0 unx     1821 b- defN 23-May-30 16:38 mb_utils/src/verify_image.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-06 14:24 mb_utils/src/version.py
--rw-rw-r--  2.0 unx      272 b- defN 23-Jul-06 14:24 mb_utils-1.0.202307061424.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 14:24 mb_utils-1.0.202307061424.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-06 14:24 mb_utils-1.0.202307061424.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1156 b- defN 23-Jul-06 14:24 mb_utils-1.0.202307061424.dist-info/RECORD
-14 files, 17082 bytes uncompressed, 6016 bytes compressed:  64.8%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-06 14:25 mb_utils/src/version.py
+-rw-rw-r--  2.0 unx      272 b- defN 23-Jul-06 14:25 mb_utils-1.0.202307061425.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 14:25 mb_utils-1.0.202307061425.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-06 14:25 mb_utils-1.0.202307061425.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1156 b- defN 23-Jul-06 14:25 mb_utils-1.0.202307061425.dist-info/RECORD
+14 files, 17082 bytes uncompressed, 6020 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: mb_utils/src/verify_image.py
 Comment: 
 
 Filename: mb_utils/src/version.py
 Comment: 
 
-Filename: mb_utils-1.0.202307061424.dist-info/METADATA
+Filename: mb_utils-1.0.202307061425.dist-info/METADATA
 Comment: 
 
-Filename: mb_utils-1.0.202307061424.dist-info/WHEEL
+Filename: mb_utils-1.0.202307061425.dist-info/WHEEL
 Comment: 
 
-Filename: mb_utils-1.0.202307061424.dist-info/top_level.txt
+Filename: mb_utils-1.0.202307061425.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_utils-1.0.202307061424.dist-info/RECORD
+Filename: mb_utils-1.0.202307061425.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_utils/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('06')
 VERSION_HOUR = int('14')
-VERSION_MINUTE = int('24')
+VERSION_MINUTE = int('25')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307061424
-version_date = '2023/07/06 14:24'
+PATCH_VERSION = 202307061425
+version_date = '2023/07/06 14:25'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_utils-1.0.202307061424.dist-info/RECORD` & `mb_utils-1.0.202307061425.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 mb_utils/src/extra.py,sha256=NP5JlU0oktw7j2cn_-W3rAMzjMYDKwzBeiSjpg-Evh4,1318
 mb_utils/src/logging.py,sha256=bwkKDej4pI1WzNKrQs9rTRx73z-EyZkB7UCPsYHnbs0,1813
 mb_utils/src/path_checker.py,sha256=MrE3P2hkDjOIWyZJ-Lh1X3wODKRnJk_nfVgKW0nQEMU,664
 mb_utils/src/retry_decorator.py,sha256=1lotNMXwALWFgb0ikrK9B-flOOMj9tTlOQgYCb-ejwY,1306
 mb_utils/src/s3.py,sha256=A7uQx45z7z6f5emz0AoahpOwklsWWspc0TOxSRYtSpA,3817
 mb_utils/src/terminal.py,sha256=_1l8K9CwAFYx4UgfkwOWfgeZ2bZu4s-71gnyxWJc2xA,777
 mb_utils/src/verify_image.py,sha256=L_XAlYBsdAhTkMSVcMpgwS0Ea8I9r-ZjoChjL0GHT38,1821
-mb_utils/src/version.py,sha256=EL0X0CziYbCLhgsTBF7mIlGpP1vbcw1eZYrE8xHC454,396
-mb_utils-1.0.202307061424.dist-info/METADATA,sha256=REeTmAk94FvjmGXmHatS5cL0XDNp8IGPEApcL9iVeI0,272
-mb_utils-1.0.202307061424.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mb_utils-1.0.202307061424.dist-info/top_level.txt,sha256=xeK1qEZ7uoXfZyNlYlurb_F_T8trKUaTU_Fm_UpKhyg,9
-mb_utils-1.0.202307061424.dist-info/RECORD,,
+mb_utils/src/version.py,sha256=unR-qShxqERhStiTzmcam5XBsgfRVwUg-jFhE96a63M,396
+mb_utils-1.0.202307061425.dist-info/METADATA,sha256=JpL30HN4lvi9Tx88pH6lKitzWF79bwHRLIxqQZ_yFps,272
+mb_utils-1.0.202307061425.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mb_utils-1.0.202307061425.dist-info/top_level.txt,sha256=xeK1qEZ7uoXfZyNlYlurb_F_T8trKUaTU_Fm_UpKhyg,9
+mb_utils-1.0.202307061425.dist-info/RECORD,,
```

