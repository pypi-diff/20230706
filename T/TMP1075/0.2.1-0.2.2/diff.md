# Comparing `tmp/TMP1075-0.2.1-py3-none-any.whl.zip` & `tmp/TMP1075-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2791 bytes, number of entries: 7
--rw-r--r--  2.0 unx      629 b- defN 22-Jul-19 01:24 TMP1075/__init__.py
+Zip file size: 2883 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-06 18:13 TMP1075/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-04 14:52 TMP1075/py.typed
--rw-r--r--  2.0 unx     1094 b- defN 22-Jul-19 01:35 TMP1075-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      644 b- defN 22-Jul-19 01:35 TMP1075-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-19 01:35 TMP1075-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Jul-19 01:35 TMP1075-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      529 b- defN 22-Jul-19 01:35 TMP1075-0.2.1.dist-info/RECORD
-7 files, 2996 bytes uncompressed, 1849 bytes compressed:  38.3%
+-rw-r--r--  2.0 unx     1094 b- defN 23-Jul-06 18:13 TMP1075-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      679 b- defN 23-Jul-06 18:13 TMP1075-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 18:13 TMP1075-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-06 18:13 TMP1075-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      529 b- defN 23-Jul-06 18:13 TMP1075-0.2.2.dist-info/RECORD
+7 files, 3213 bytes uncompressed, 1941 bytes compressed:  39.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: TMP1075/__init__.py
 Comment: 
 
 Filename: TMP1075/py.typed
 Comment: 
 
-Filename: TMP1075-0.2.1.dist-info/LICENSE
+Filename: TMP1075-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: TMP1075-0.2.1.dist-info/METADATA
+Filename: TMP1075-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: TMP1075-0.2.1.dist-info/WHEEL
+Filename: TMP1075-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: TMP1075-0.2.1.dist-info/top_level.txt
+Filename: TMP1075-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: TMP1075-0.2.1.dist-info/RECORD
+Filename: TMP1075-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TMP1075/__init__.py

```diff
@@ -1,23 +1,31 @@
-import busio
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import board
+import busio
 from adafruit_bus_device.i2c_device import I2CDevice
 
 
 class TMP1075:
     """
     Driver for the TI TMP1075 temperature sensor.
     See datasheet: http://www.ti.com/lit/ds/symlink/tmp1075.pdf
 
     """
+
     TEMP_REGISTER = bytearray([0x00])
     CONFIG_REGISTER = bytearray([0x01])
 
-
-    def __init__(self, address: int=0x4f):
+    def __init__(self, address: int = 0x4F):
         comm_port = busio.I2C(board.SCL, board.SDA)
         self.i2c = I2CDevice(comm_port, address)
 
     def get_temperature(self) -> float:
         b = bytearray(2)
         self.i2c.write_then_readinto(self.TEMP_REGISTER, b)
         return ((b[0] << 4) + (b[1] >> 4)) * 0.0625
+
+    @property
+    def temperature(self):
+        """alias for get_temperature"""
+        return self.get_temperature()
```

## Comparing `TMP1075-0.2.1.dist-info/LICENSE` & `TMP1075-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `TMP1075-0.2.1.dist-info/METADATA` & `TMP1075-0.2.2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMP1075
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python wrapper for interacting with the TMP1075
 Home-page: https://github.com/Pioreactor/TMP1075
 Author: Cam Davidson-Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -19,9 +19,11 @@
 
 ## Usage
 
 ```python
 from TMP1075 import TMP1075
 
 tmp = TMP1075()
-tmp.get_temperature()
+print(tmp.get_temperature())
+# or
+print(tmp.temperature)
 ```
```

