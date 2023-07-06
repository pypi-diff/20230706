# Comparing `tmp/AidlabSDK-1.3.26.tar.gz` & `tmp/AidlabSDK-1.3.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AidlabSDK-1.3.26.tar", last modified: Tue Aug  9 12:13:03 2022, max compression
+gzip compressed data, was "dist/AidlabSDK-1.3.27.tar", last modified: Thu Jul  6 13:07:41 2023, max compression
```

## Comparing `AidlabSDK-1.3.26.tar` & `AidlabSDK-1.3.27.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 szymongesicki   (501) staff       (20)        0 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/
-drwxr-xr-x   0 szymongesicki   (501) staff       (20)        0 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/Aidlab/
--rwxr-xr-x   0 szymongesicki   (501) staff       (20)     9109 2022-08-09 09:33:23.000000 AidlabSDK-1.3.26/Aidlab/Aidlab.py
--rw-r--r--   0 szymongesicki   (501) staff       (20)     1834 2022-07-14 18:41:53.000000 AidlabSDK-1.3.26/Aidlab/AidlabCharacteristicsUUID.py
--rw-r--r--   0 szymongesicki   (501) staff       (20)     3411 2022-07-14 18:41:53.000000 AidlabSDK-1.3.26/Aidlab/AidlabNotificationHandler.py
--rwxr-xr-x   0 szymongesicki   (501) staff       (20)    10543 2022-08-09 09:32:59.000000 AidlabSDK-1.3.26/Aidlab/AidlabPeripheral.py
--rwxr-xr-x   0 szymongesicki   (501) staff       (20)    23763 2022-08-09 09:32:55.000000 AidlabSDK-1.3.26/Aidlab/AidlabSDK.py
--rwxr-xr-x   0 szymongesicki   (501) staff       (20)      652 2022-07-14 18:41:53.000000 AidlabSDK-1.3.26/Aidlab/IAidlab.py
--rwxr-xr-x   0 szymongesicki   (501) staff       (20)      427 2022-08-09 09:46:01.000000 AidlabSDK-1.3.26/Aidlab/Signal.py
--rw-r--r--   0 szymongesicki   (501) staff       (20)       32 2022-07-14 18:41:53.000000 AidlabSDK-1.3.26/Aidlab/__init__.py
--rw-rw-r--   0 szymongesicki   (501) staff       (20)   212480 2022-07-14 17:11:36.000000 AidlabSDK-1.3.26/Aidlab/aidlabsdk.dll
--rwxr-xr-x   0 szymongesicki   (501) staff       (20)   838184 2022-07-14 18:41:53.000000 AidlabSDK-1.3.26/Aidlab/aidlabsdk.dylib
--rw-r--r--   0 szymongesicki   (501) staff       (20)   934536 2022-07-14 18:41:53.000000 AidlabSDK-1.3.26/Aidlab/aidlabsdk.so
-drwxr-xr-x   0 szymongesicki   (501) staff       (20)        0 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/AidlabSDK.egg-info/
--rw-r--r--   0 szymongesicki   (501) staff       (20)     1593 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/AidlabSDK.egg-info/PKG-INFO
--rw-r--r--   0 szymongesicki   (501) staff       (20)      448 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/AidlabSDK.egg-info/SOURCES.txt
--rw-r--r--   0 szymongesicki   (501) staff       (20)        1 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/AidlabSDK.egg-info/dependency_links.txt
--rw-r--r--   0 szymongesicki   (501) staff       (20)       24 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/AidlabSDK.egg-info/requires.txt
--rw-r--r--   0 szymongesicki   (501) staff       (20)        7 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/AidlabSDK.egg-info/top_level.txt
--rw-r--r--   0 szymongesicki   (501) staff       (20)       87 2022-07-14 18:41:53.000000 AidlabSDK-1.3.26/MANIFEST.in
--rw-r--r--   0 szymongesicki   (501) staff       (20)     1593 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/PKG-INFO
--rw-r--r--   0 szymongesicki   (501) staff       (20)      165 2022-07-14 18:41:53.000000 AidlabSDK-1.3.26/README.md
--rw-r--r--   0 szymongesicki   (501) staff       (20)       38 2022-08-09 12:13:03.000000 AidlabSDK-1.3.26/setup.cfg
--rw-r--r--   0 szymongesicki   (501) staff       (20)      786 2022-08-09 12:12:45.000000 AidlabSDK-1.3.26/setup.py
+drwxr-xr-x   0 szymongesicki   (501) staff       (20)        0 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/
+drwxr-xr-x   0 szymongesicki   (501) staff       (20)        0 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/Aidlab/
+-rwxr-xr-x   0 szymongesicki   (501) staff       (20)     9211 2023-02-06 11:15:49.000000 AidlabSDK-1.3.27/Aidlab/Aidlab.py
+-rw-r--r--   0 szymongesicki   (501) staff       (20)     1934 2023-02-06 11:15:49.000000 AidlabSDK-1.3.27/Aidlab/AidlabCharacteristicsUUID.py
+-rw-r--r--   0 szymongesicki   (501) staff       (20)     3411 2023-05-26 16:19:40.000000 AidlabSDK-1.3.27/Aidlab/AidlabNotificationHandler.py
+-rwxr-xr-x   0 szymongesicki   (501) staff       (20)    11239 2023-02-06 11:15:49.000000 AidlabSDK-1.3.27/Aidlab/AidlabPeripheral.py
+-rwxr-xr-x   0 szymongesicki   (501) staff       (20)    24012 2023-02-06 11:15:49.000000 AidlabSDK-1.3.27/Aidlab/AidlabSDK.py
+-rwxr-xr-x   0 szymongesicki   (501) staff       (20)      725 2023-02-06 11:15:49.000000 AidlabSDK-1.3.27/Aidlab/IAidlab.py
+-rwxr-xr-x   0 szymongesicki   (501) staff       (20)      427 2022-12-19 11:35:18.000000 AidlabSDK-1.3.27/Aidlab/Signal.py
+-rw-r--r--   0 szymongesicki   (501) staff       (20)       32 2022-07-14 18:41:53.000000 AidlabSDK-1.3.27/Aidlab/__init__.py
+-rw-r--r--   0 szymongesicki   (501) staff       (20)   212480 2022-12-19 11:35:18.000000 AidlabSDK-1.3.27/Aidlab/aidlabsdk.dll
+-rwxr-xr-x   0 szymongesicki   (501) staff       (20)   838184 2022-12-19 11:35:18.000000 AidlabSDK-1.3.27/Aidlab/aidlabsdk.dylib
+-rw-r--r--   0 szymongesicki   (501) staff       (20)   934536 2022-12-19 11:35:18.000000 AidlabSDK-1.3.27/Aidlab/aidlabsdk.so
+drwxr-xr-x   0 szymongesicki   (501) staff       (20)        0 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/AidlabSDK.egg-info/
+-rw-r--r--   0 szymongesicki   (501) staff       (20)     1593 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/AidlabSDK.egg-info/PKG-INFO
+-rw-r--r--   0 szymongesicki   (501) staff       (20)      448 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/AidlabSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 szymongesicki   (501) staff       (20)        1 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/AidlabSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 szymongesicki   (501) staff       (20)       24 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/AidlabSDK.egg-info/requires.txt
+-rw-r--r--   0 szymongesicki   (501) staff       (20)        7 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/AidlabSDK.egg-info/top_level.txt
+-rw-r--r--   0 szymongesicki   (501) staff       (20)       87 2022-07-14 18:41:53.000000 AidlabSDK-1.3.27/MANIFEST.in
+-rw-r--r--   0 szymongesicki   (501) staff       (20)     1593 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/PKG-INFO
+-rw-r--r--   0 szymongesicki   (501) staff       (20)      165 2022-07-14 18:41:53.000000 AidlabSDK-1.3.27/README.md
+-rw-r--r--   0 szymongesicki   (501) staff       (20)       38 2023-07-06 13:07:41.000000 AidlabSDK-1.3.27/setup.cfg
+-rw-r--r--   0 szymongesicki   (501) staff       (20)      786 2023-07-06 13:07:20.000000 AidlabSDK-1.3.27/setup.py
```

### Comparing `AidlabSDK-1.3.26/Aidlab/Aidlab.py` & `AidlabSDK-1.3.27/Aidlab/Aidlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
     def destroy(self, aidlab_address):
         self.aidlab_sdk[aidlab_address].destroy()
 
     def connect(self, real_time_signal, sync_signal=[], aidlabsMAC=None):
         self.aidlab_peripheral.run(real_time_signal, sync_signal, aidlabsMAC)
 
+    def disconnect(self, aidlab_address):
+        self.aidlab_peripheral.disconnect(aidlab_address)
+	
     def did_connect_aidlab(self, aidlab_address):
         self.aidlab_sdk[aidlab_address].did_connect_aidlab()
 
     def did_disconnect_aidlab(self, aidlab_address):
         self.aidlab_sdk[aidlab_address].did_disconnect_aidlab()
 
     def did_receive_raw_temperature(self, data, aidlab_address):
```

### Comparing `AidlabSDK-1.3.26/Aidlab/AidlabCharacteristicsUUID.py` & `AidlabSDK-1.3.27/Aidlab/AidlabCharacteristicsUUID.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,13 +25,13 @@
         self.respirationUUID =        {"uuid": "48366e80-cf3a-11e1-9ab4-0002a5d5c51b", "handle": 19}
         self.activityUUID =           {"uuid": "61366e80-cf3a-11e1-9ab4-0002a5d5c51b", "handle": 49}
         self.stepsUUID =              {"uuid": "62366e80-cf3a-11e1-9ab4-0002a5d5c51b", "handle": 52}
         self.soundVolumeUUID =        {"uuid": "52366e80-cf3a-11e1-9ab4-0002a5d5c51b", "handle": 31}
         self.cmdUUID =                {"uuid": "51366e80-cf3a-11e1-9ab4-0002a5d5c51b", "handle": 13}
         self.heartRateUUID =          {"uuid": "00002a37-0000-1000-8000-00805f9b34fb", "handle": 45}
         self.healthThermometerUUID =  {"uuid": "00002a1c-0000-1000-8000-00805f9b34fb", "handle": 63}
-
+        self.currentTimeUUID =        {"uuid": "00002a2b-0000-1000-8000-00805f9b34fb", "handle": 46}
```

### Comparing `AidlabSDK-1.3.26/Aidlab/AidlabNotificationHandler.py` & `AidlabSDK-1.3.27/Aidlab/AidlabNotificationHandler.py`

 * *Files identical despite different names*

### Comparing `AidlabSDK-1.3.26/Aidlab/AidlabPeripheral.py` & `AidlabSDK-1.3.27/Aidlab/AidlabPeripheral.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 from Aidlab.Signal import Signal
 from bleak import BleakClient, discover, BleakError
 import asyncio
 from multiprocessing import Process
 import sys
 import logging
 from packaging import version
+from time import time
 
 logging.getLogger("bleak").setLevel(logging.ERROR)
 logger = logging.getLogger(__name__)
 
 class AidlabPeripheral():
     connected_aidlab = []
 
     def __init__(self, aidlab_delegate):
         self.aidlab_delegate = aidlab_delegate
         self.queue_to_send = []
         self.max_cmd_length = 20
+        self.should_disconnect = dict()
 
     async def scan_for_aidlab(self):
         devices = await discover()
         # Container for Aidlab's MAC addresses (these were found during the scan process)
         aidlabMACs = []
 
         for dev in devices:
@@ -122,34 +124,44 @@
             for characteristic in self.converter_to_uuids(real_time_signal, aidlab_address):
                 try:
                     await client.start_notify(characteristic, aidlabNotificationHandler.handle_notification)
                 except BleakError as e:
                     logger.debug(str(e) + " (this might be due to compatibility with older aidlabs)")
                     pass
 
+            await self.set_aidlab_time(client, time())
+
             if version.parse("3.6.0") < version.parse(firmware_revision):
                 logger.debug("Version later than 3.6 start collect data")
                 await self.start_collect_data(client, aidlab_address, real_time_signal, sync_signal)
             else:
                 logger.debug("Version older than 3.6")
 
             while True:
                 await asyncio.sleep(command_send_delay_sec)
                 await self.send_command_if_needed(client)
+                
+
+                if self.should_disconnect.get(aidlab_address, False):
+                    self.should_disconnect.pop(aidlab_address, None)
+                    await client.disconnect()
+
                 if not client.is_connected:
                     self.aidlab_delegate.did_disconnect_aidlab(aidlab_address)
                     self.aidlab_delegate.destroy(aidlab_address)
                     self.connected_aidlab.remove(aidlab_address)
                     break
 
         except Exception as e:
             logging.info("Exception " + str(e))
             if aidlab_address in self.connected_aidlab: self.connected_aidlab.remove(aidlab_address)
 
-
+    def disconnect(self, aidlab_address):
+        self.should_disconnect[aidlab_address] = True
+    
     def start_synchronization(self, address):
         self.queue_to_send.append({"address": address, "command": "sync start"})
 
     def stop_synchronization(self, address):
         self.queue_to_send.append({"address": address, "command": "sync stop"})
     
     def send(self, address, command):
@@ -170,14 +182,19 @@
     async def send_to_aidlab(self, client, message, size):
         logger.debug("will send msg" + str(message) + " len " + str(size))
         for i in range(round(int(size/self.max_cmd_length) + (size%self.max_cmd_length > 0))):
             message_byte = bytearray(message[i*self.max_cmd_length:(i+1)*self.max_cmd_length])
             logger.debug("sending bytes\n" + str(message_byte))
             await client.write_gatt_char(self.aidlabCharacteristicsUUID.cmdUUID["uuid"], message_byte, True)
 
+    async def set_aidlab_time(self, client, timestamp):
+        timestamp = int(timestamp)
+        message = [b for b in timestamp.to_bytes(4, "little")]
+        await client.write_gatt_char(self.aidlabCharacteristicsUUID.currentTimeUUID["uuid"], bytearray(message), True)
+
     def signal_list_to_int_list(self, signals):
         int_list = []
         for signal in signals:
             int_list.append(signal.value)
         return int_list
 
     async def start_collect_data(self, client, aidlab_address, real_time_signal, sync_signal):
```

### Comparing `AidlabSDK-1.3.26/Aidlab/AidlabSDK.py` & `AidlabSDK-1.3.27/Aidlab/AidlabSDK.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,18 @@
         self.aidlab.address = aidlab_address
 
         # loading  aidlabsdk lib
         full_path = os.path.realpath(__file__)
         cwd, filename = os.path.split(full_path)
 
         if 'linux' in sys.platform:
-            self.lib = cdll.LoadLibrary(cwd+"/aidlabsdk.so")
+            if os.uname()[4][:3] == 'arm':
+            	self.lib = cdll.LoadLibrary(cwd+"/aidlabsdk_raspberry.so") # arm(raspberry pi) version
+            else:
+            	self.lib = cdll.LoadLibrary(cwd+"/aidlabsdk.so")
         elif 'win32' in sys.platform:
             self.lib = cdll.LoadLibrary(cwd+"/aidlabsdk.dll")
         elif 'darwin' in sys.platform:
             self.lib = cdll.LoadLibrary(cwd+"/aidlabsdk.dylib")
         else:
             raise RuntimeError("Unsupported operating system: {}".format(sys.platform))
 
@@ -178,14 +181,17 @@
         self.delegate.start_synchronization(address)        
 
     def stop_synchronization(self, address):
         self.delegate.stop_synchronization(address)
     
     def send(self, address, command):
         self.delegate.send(address, command)
+        
+    def disconnect(self, address):
+        self.delegate.disconnect(address)
 
     def destroy(self):
         self.lib.destroy(self.aidlab_sdk_ptr)
 
     def did_connect_aidlab(self):
         self.delegate.did_connect(self.aidlab)
 
@@ -462,8 +468,8 @@
         self.delegate.did_receive_past_signal_quality(self.aidlab, timestamp, value)
 
     def sync_state_did_change(self, context, sync_state):
         sync_state = self.Sync_state.get(sync_state, "empty")
         self.delegate.sync_state_did_change(self.aidlab, sync_state)
 
     def did_receive_unsynchronized_size(self, context, unsynchronized_size, sync_bytes_per_second):
-        self.delegate.did_receive_unsynchronized_size(self.aidlab, unsynchronized_size, sync_bytes_per_second)
+        self.delegate.did_receive_unsynchronized_size(self.aidlab, unsynchronized_size, sync_bytes_per_second)
```

### Comparing `AidlabSDK-1.3.26/Aidlab/IAidlab.py` & `AidlabSDK-1.3.27/Aidlab/IAidlab.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,10 +23,11 @@
 
     def stop_synchronization(self):
         self.delegate.stop_synchronization(self.address)
     
     def send(self, command):
         self.delegate.send(self.address, command)
 
-
+    def disconnect(self):
+        self.delegate.disconnect(self.address)
+    
     
-
```

### Comparing `AidlabSDK-1.3.26/Aidlab/aidlabsdk.dll` & `AidlabSDK-1.3.27/Aidlab/aidlabsdk.dll`

 * *Files identical despite different names*

### Comparing `AidlabSDK-1.3.26/Aidlab/aidlabsdk.dylib` & `AidlabSDK-1.3.27/Aidlab/aidlabsdk.dylib`

 * *Files identical despite different names*

### Comparing `AidlabSDK-1.3.26/Aidlab/aidlabsdk.so` & `AidlabSDK-1.3.27/Aidlab/aidlabsdk.so`

 * *Files identical despite different names*

### Comparing `AidlabSDK-1.3.26/AidlabSDK.egg-info/PKG-INFO` & `AidlabSDK-1.3.27/AidlabSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AidlabSDK
-Version: 1.3.26
+Version: 1.3.27
 Summary: SDK tools to integrate Aidlab into your projects.
 Home-page: https://www.aidlab.com
 Author: Aidlab
 Author-email: contact@aidlab.com
 License: MIT License
 Copyright (c) 2016-2020 Aidlab
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AidlabSDK-1.3.26/PKG-INFO` & `AidlabSDK-1.3.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AidlabSDK
-Version: 1.3.26
+Version: 1.3.27
 Summary: SDK tools to integrate Aidlab into your projects.
 Home-page: https://www.aidlab.com
 Author: Aidlab
 Author-email: contact@aidlab.com
 License: MIT License
 Copyright (c) 2016-2020 Aidlab
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AidlabSDK-1.3.26/setup.py` & `AidlabSDK-1.3.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
    long_description = fh.read()
 
 with open("LICENSE.md", "r") as fh:
    license = fh.read()
 
 setup_args = dict(
     name='AidlabSDK',
-    version='1.3.26',
+    version='1.3.27',
     description='SDK tools to integrate Aidlab into your projects.',
     long_description_content_type="text/markdown",
     long_description=long_description,
     license=license,
     packages=find_packages(),
     install_requires=['bleak==0.14.3', 'packaging'],
     author='Aidlab',
```

