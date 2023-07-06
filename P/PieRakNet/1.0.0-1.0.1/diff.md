# Comparing `tmp/PieRakNet-1.0.0.tar.gz` & `tmp/PieRakNet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PieRakNet-1.0.0.tar", last modified: Tue Jul  4 10:41:07 2023, max compression
+gzip compressed data, was "PieRakNet-1.0.1.tar", last modified: Thu Jul  6 10:53:37 2023, max compression
```

## Comparing `PieRakNet-1.0.0.tar` & `PieRakNet-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 10:41:07.339839 PieRakNet-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-06-29 08:26:14.000000 PieRakNet-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      985 2023-07-04 10:41:07.333850 PieRakNet-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 10:41:07.241103 PieRakNet-1.0.0/PieRakNet.egg-info/
--rw-rw-rw-   0        0        0      985 2023-07-04 10:41:06.000000 PieRakNet-1.0.0/PieRakNet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-04 10:41:06.000000 PieRakNet-1.0.0/PieRakNet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 10:41:06.000000 PieRakNet-1.0.0/PieRakNet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-04 10:41:06.000000 PieRakNet-1.0.0/PieRakNet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       75 2023-07-04 10:38:51.000000 PieRakNet-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 10:41:07.306255 PieRakNet-1.0.0/pieraknet/
--rw-rw-rw-   0        0        0      127 2023-07-03 09:12:34.000000 PieRakNet-1.0.0/pieraknet/__init__.py
--rw-rw-rw-   0        0        0     4833 2023-07-04 09:44:42.000000 PieRakNet-1.0.0/pieraknet/buffer.py
--rw-rw-rw-   0        0        0       29 2023-07-03 08:12:06.000000 PieRakNet-1.0.0/pieraknet/connection.py
--rw-rw-rw-   0        0        0      536 2023-07-03 09:03:19.000000 PieRakNet-1.0.0/pieraknet/protocol_info.py
--rw-rw-rw-   0        0        0     2358 2023-07-04 10:07:04.000000 PieRakNet-1.0.0/pieraknet/server.py
--rw-rw-rw-   0        0        0       42 2023-07-04 10:41:07.344825 PieRakNet-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-07-04 10:40:26.000000 PieRakNet-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:53:37.049191 PieRakNet-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-29 08:26:14.000000 PieRakNet-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      985 2023-07-06 10:53:37.047192 PieRakNet-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 10:53:36.836336 PieRakNet-1.0.1/PieRakNet.egg-info/
+-rw-rw-rw-   0        0        0      985 2023-07-06 10:53:35.000000 PieRakNet-1.0.1/PieRakNet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-06 10:53:35.000000 PieRakNet-1.0.1/PieRakNet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:53:35.000000 PieRakNet-1.0.1/PieRakNet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 10:53:35.000000 PieRakNet-1.0.1/PieRakNet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       75 2023-07-04 10:38:51.000000 PieRakNet-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 10:53:37.034465 PieRakNet-1.0.1/pieraknet/
+-rw-rw-rw-   0        0        0       89 2023-07-06 08:27:19.000000 PieRakNet-1.0.1/pieraknet/__init__.py
+-rw-rw-rw-   0        0        0     4988 2023-07-06 07:52:28.000000 PieRakNet-1.0.1/pieraknet/buffer.py
+-rw-rw-rw-   0        0        0     9947 2023-07-06 10:40:18.000000 PieRakNet-1.0.1/pieraknet/connection.py
+-rw-rw-rw-   0        0        0      608 2023-07-06 10:03:10.000000 PieRakNet-1.0.1/pieraknet/protocol_info.py
+-rw-rw-rw-   0        0        0     3869 2023-07-06 10:48:10.000000 PieRakNet-1.0.1/pieraknet/server.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 10:53:37.050189 PieRakNet-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-07-06 10:48:10.000000 PieRakNet-1.0.1/setup.py
```

### Comparing `PieRakNet-1.0.0/LICENSE` & `PieRakNet-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.0/PKG-INFO` & `PieRakNet-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.0
+Version: 1.0.1
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: nikitagavrilin005@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `PieRakNet-1.0.0/PieRakNet.egg-info/PKG-INFO` & `PieRakNet-1.0.1/PieRakNet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.0
+Version: 1.0.1
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: nikitagavrilin005@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `PieRakNet-1.0.0/pieraknet/buffer.py` & `PieRakNet-1.0.1/pieraknet/buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 
 
 class BuffError(Exception):
     pass
 
 
 class Buffer(BytesIO):
+    def feos(self):
+        if len(bytes(self.getvalue()).decode()[self.tell()]) == 0:
+            return True
+        else:
+            return False
 
     def read_packet_id(self):  # Read Packet ID
         return self.read_byte()
 
     def write_packet_id(self, data):
         self.write_byte(str(data))
```

### Comparing `PieRakNet-1.0.0/pieraknet/protocol_info.py` & `PieRakNet-1.0.1/pieraknet/protocol_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,9 +10,12 @@
     OPEN_CONNECTION_REPLY_2 = 0x08
     CONNECTION_REQUEST = 0x09
     CONNECTION_REQUEST_ACCEPTED = 0x10
     NEW_INCOMING_CONNECTION = 0x13
     DISCONNECT = 0x15
     INCOMPATIBLE_PROTOCOL_VERSION = 0x19
     FRAME_SET = 0x80
+    FRAME_SET_0 = 0x80
+    FRAME_SET_F = 0x8d
     NACK = 0xa0
     ACK = 0xc0
+    GAME_PACKET = 0xfe
```

### Comparing `PieRakNet-1.0.0/setup.py` & `PieRakNet-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='PieRakNet',
-    version='1.0.0',
+    version='1.0.1',
     author='lapismyt',
     author_email='nikitagavrilin005@gmail.com',
     description='RakNet implementation, written in Python. Created for PieMC.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/PieMC-Dev/PieRakNet',
     packages=find_packages(),
```

