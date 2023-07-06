# Comparing `tmp/vios-1.0.6-py3-none-any.whl.zip` & `tmp/vios-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 33886 bytes, number of entries: 23
+Zip file size: 33887 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat      781 b- defN 23-Jun-26 13:01 vios/__init__.py
 -rw-rw-rw-  2.0 fat     6312 b- defN 23-Jul-04 14:13 vios/collection/__init__.py
 -rw-rw-rw-  2.0 fat     3515 b- defN 23-Jul-04 13:33 vios/collection/support.py
 -rw-rw-rw-  2.0 fat    11254 b- defN 23-Jun-19 15:11 vios/collection/tasks.py
 -rw-rw-rw-  2.0 fat    10198 b- defN 23-Jun-28 07:10 vios/collection/uapi.py
 -rw-rw-rw-  2.0 fat     4756 b- defN 23-Jun-19 15:11 vios/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat     2962 b- defN 23-Jun-19 15:11 vios/driver/__init__.py
@@ -13,13 +13,13 @@
 -rw-rw-rw-  2.0 fat      784 b- defN 23-Jun-30 06:18 vios/envelope/__init__.py
 -rw-rw-rw-  2.0 fat    13446 b- defN 23-Jul-06 02:54 vios/envelope/assembler.py
 -rw-rw-rw-  2.0 fat    10541 b- defN 23-Jun-26 11:28 vios/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1047 b- defN 23-Jun-19 15:11 vios/envelope/device.py
 -rw-rw-rw-  2.0 fat     1719 b- defN 23-Jun-26 11:28 vios/envelope/processor.py
 -rw-rw-rw-  2.0 fat     2980 b- defN 23-Jun-26 12:50 vios/envelope/rule.py
 -rw-rw-rw-  2.0 fat      522 b- defN 23-Jun-26 11:28 vios/tools/__init__.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-06 02:54 vios-1.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1000 b- defN 23-Jul-06 02:54 vios-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 02:54 vios-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-06 02:54 vios-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1857 b- defN 23-Jul-06 02:54 vios-1.0.6.dist-info/RECORD
-23 files, 89473 bytes uncompressed, 30906 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1000 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1857 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/RECORD
+23 files, 89473 bytes uncompressed, 30907 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: vios/envelope/rule.py
 Comment: 
 
 Filename: vios/tools/__init__.py
 Comment: 
 
-Filename: vios-1.0.6.dist-info/LICENSE
+Filename: vios-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: vios-1.0.6.dist-info/METADATA
+Filename: vios-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: vios-1.0.6.dist-info/WHEEL
+Filename: vios-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: vios-1.0.6.dist-info/top_level.txt
+Filename: vios-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-1.0.6.dist-info/RECORD
+Filename: vios-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vios-1.0.6.dist-info/LICENSE` & `vios-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-1.0.6.dist-info/METADATA` & `vios-1.0.7.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 1.0.6
+Version: 1.0.7
 Summary: runtime requirements for systemq
 Author-email: YL <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-1.0.6.dist-info/RECORD` & `vios-1.0.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 vios/envelope/__init__.py,sha256=97kXED9oaUd56J2OoVCTQpctkQZDcAZWxpEQakTxCRM,784
 vios/envelope/assembler.py,sha256=KE4Fcrid5UfBsbpOPz7eV2WJY1f7jXwVY0VtjwMvPBk,13446
 vios/envelope/calculator.py,sha256=eE7730YFzArrukuDh0dI0JabG2PiEz3eo3N4Czqgk88,10541
 vios/envelope/device.py,sha256=rQeLe_Y9MTwLZfJsSK9MhvZxdOnrtJNcOZriS6Rm1Io,1047
 vios/envelope/processor.py,sha256=4py3AwLurBTrhXXJCvdfHrMeKGzOFl-gICQTNjpoyQM,1719
 vios/envelope/rule.py,sha256=ANiUVCtozVP6B6m8En55VLqOHWdeMkuA7KqiAiFyAnQ,2980
 vios/tools/__init__.py,sha256=vq-1N9Zjm_ZYcD9_lwX9fKlcMT9Rx7Kd3BDRqmKhMT0,522
-vios-1.0.6.dist-info/LICENSE,sha256=N0ypn_97IUjlPVBH8az2Wt02D-9ROQafRq1D6tcqorE,1089
-vios-1.0.6.dist-info/METADATA,sha256=eVvyxS1pueldYAXk_2oqgPbsmS_PUdNh5fR5onA4QU4,1000
-vios-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vios-1.0.6.dist-info/top_level.txt,sha256=4DHqoaYuzp4X6-_w1r1lk0039QUzXe7OVi76KeUqjZM,5
-vios-1.0.6.dist-info/RECORD,,
+vios-1.0.7.dist-info/LICENSE,sha256=N0ypn_97IUjlPVBH8az2Wt02D-9ROQafRq1D6tcqorE,1089
+vios-1.0.7.dist-info/METADATA,sha256=aYJAj7l0t3xW48dCs3R0GzZ7NNsUBWfoQN_1zi4ATj8,1000
+vios-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vios-1.0.7.dist-info/top_level.txt,sha256=4DHqoaYuzp4X6-_w1r1lk0039QUzXe7OVi76KeUqjZM,5
+vios-1.0.7.dist-info/RECORD,,
```

