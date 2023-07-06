# Comparing `tmp/viam_sdk-0.4.3-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/viam_sdk-0.4.3rc1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9842164 bytes, number of entries: 371
+Zip file size: 9842194 bytes, number of entries: 371
 -rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx     1411 b- defN 80-Jan-01 00:00 viam/__init__.py
 -rw-r--r--  2.0 unx     1531 b- defN 80-Jan-01 00:00 viam/app/client.py
 -rw-r--r--  2.0 unx    12643 b- defN 80-Jan-01 00:00 viam/app/data/client.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 viam/components/__init__.py
 -rw-r--r--  2.0 unx     1125 b- defN 80-Jan-01 00:00 viam/components/arm/__init__.py
 -rw-r--r--  2.0 unx     3454 b- defN 80-Jan-01 00:00 viam/components/arm/arm.py
@@ -362,12 +362,12 @@
 -rw-r--r--  2.0 unx     1633 b- defN 80-Jan-01 00:00 viam/services/slam/slam.py
 -rw-r--r--  2.0 unx      426 b- defN 80-Jan-01 00:00 viam/services/vision/__init__.py
 -rw-r--r--  2.0 unx     5176 b- defN 80-Jan-01 00:00 viam/services/vision/client.py
 -rw-r--r--  2.0 unx     5076 b- defN 80-Jan-01 00:00 viam/services/vision/service.py
 -rw-r--r--  2.0 unx     4996 b- defN 80-Jan-01 00:00 viam/services/vision/vision.py
 -rw-r--r--  2.0 unx     5286 b- defN 80-Jan-01 00:00 viam/sessions_client.py
 -rw-r--r--  2.0 unx     7927 b- defN 80-Jan-01 00:00 viam/utils.py
--rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.4.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     8730 b- defN 80-Jan-01 00:00 viam_sdk-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.4.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx    34218 b- defN 16-Jan-01 00:00 viam_sdk-0.4.3.dist-info/RECORD
-371 files, 30137829 bytes uncompressed, 9787070 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.4.3rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8733 b- defN 80-Jan-01 00:00 viam_sdk-0.4.3rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.4.3rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    34230 b- defN 16-Jan-01 00:00 viam_sdk-0.4.3rc1.dist-info/RECORD
+371 files, 30137844 bytes uncompressed, 9787076 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1095,20 +1095,20 @@
 
 Filename: viam/sessions_client.py
 Comment: 
 
 Filename: viam/utils.py
 Comment: 
 
-Filename: viam_sdk-0.4.3.dist-info/LICENSE
+Filename: viam_sdk-0.4.3rc1.dist-info/LICENSE
 Comment: 
 
-Filename: viam_sdk-0.4.3.dist-info/METADATA
+Filename: viam_sdk-0.4.3rc1.dist-info/METADATA
 Comment: 
 
-Filename: viam_sdk-0.4.3.dist-info/WHEEL
+Filename: viam_sdk-0.4.3rc1.dist-info/WHEEL
 Comment: 
 
-Filename: viam_sdk-0.4.3.dist-info/RECORD
+Filename: viam_sdk-0.4.3rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `viam_sdk-0.4.3.dist-info/LICENSE` & `viam_sdk-0.4.3rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `viam_sdk-0.4.3.dist-info/METADATA` & `viam_sdk-0.4.3rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viam-sdk
-Version: 0.4.3
+Version: 0.4.3rc1
 Summary: Viam Robotics Python SDK
 License: Apache-2.0
 Author: Naveed
 Author-email: naveed@viam.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `viam_sdk-0.4.3.dist-info/RECORD` & `viam_sdk-0.4.3rc1.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -361,11 +361,11 @@
 viam/services/slam/slam.py,sha256=872OV9JvSEvwWRBDiX-P8Zs87fNBp-5mbMx4ruot-gY,1633
 viam/services/vision/__init__.py,sha256=8DPwRKggv0cMb3Z4R5-pAHvbAIIMBfNYWUktuh58gyE,426
 viam/services/vision/client.py,sha256=EHiVW1R2JgS_DzyenmJzcIhQdtiegeUUBy2lYBpKemg,5176
 viam/services/vision/service.py,sha256=ae0zUVBi-QiNYoxfT7KurCUvdy0umdUdFVqMLprF_3c,5076
 viam/services/vision/vision.py,sha256=MFeEWjiS2Dp7ttqL3lmHTznxmGpoVEkIgYbWTuiZPPg,4996
 viam/sessions_client.py,sha256=Et7ipPP89RJ6PGjfwfstunDfZzGEmkrfDeldzBZ-Zso,5286
 viam/utils.py,sha256=gGoMOLkeJSerDIH2nPDydTfL7-p2AWqZCMU4jQEp0go,7927
-viam_sdk-0.4.3.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
-viam_sdk-0.4.3.dist-info/METADATA,sha256=6x7N47bgH8eg_YoE2Yo8sc3NKXb2VTp-IhkqlInye7Q,8730
-viam_sdk-0.4.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-viam_sdk-0.4.3.dist-info/RECORD,,
+viam_sdk-0.4.3rc1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
+viam_sdk-0.4.3rc1.dist-info/METADATA,sha256=obtLw_OwDTyqnPTbXxAui49cDfCJU15nzukgGFdjOFI,8733
+viam_sdk-0.4.3rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+viam_sdk-0.4.3rc1.dist-info/RECORD,,
```

