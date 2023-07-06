# Comparing `tmp/petkitaio-0.1.5.tar.gz` & `tmp/petkitaio-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petkitaio-0.1.5.tar", last modified: Mon Jun 26 20:30:38 2023, max compression
+gzip compressed data, was "petkitaio-0.1.6.tar", last modified: Thu Jul  6 18:48:07 2023, max compression
```

## Comparing `petkitaio-0.1.5.tar` & `petkitaio-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-26 20:30:38.385862 petkitaio-0.1.5/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-06-26 20:28:52.000000 petkitaio-0.1.5/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     5891 2023-06-26 20:30:38.386092 petkitaio-0.1.5/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4300 2023-06-26 20:28:52.000000 petkitaio-0.1.5/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-26 20:30:38.383650 petkitaio-0.1.5/petkitaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1868 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    10226 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1392 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/model.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    41909 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/petkit_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-26 20:30:38.385582 petkitaio-0.1.5/petkitaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     5891 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/top_level.txt
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-06-26 20:30:38.386663 petkitaio-0.1.5/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-06-26 20:28:52.000000 petkitaio-0.1.5/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-06 18:48:07.393586 petkitaio-0.1.6/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-07-06 18:44:46.000000 petkitaio-0.1.6/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     6153 2023-07-06 18:48:07.393803 petkitaio-0.1.6/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4546 2023-07-06 18:44:46.000000 petkitaio-0.1.6/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-06 18:48:07.391261 petkitaio-0.1.6/petkitaio/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1904 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    10730 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/constants.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1392 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/model.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    43295 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/petkit_client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-06 18:48:07.393282 petkitaio-0.1.6/petkitaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     6153 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/top_level.txt
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-07-06 18:48:07.394341 petkitaio-0.1.6/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-07-06 18:44:46.000000 petkitaio-0.1.6/setup.py
```

### Comparing `petkitaio-0.1.5/LICENSE` & `petkitaio-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.5/PKG-INFO` & `petkitaio-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
 Description: # PetKitAIO
         
         Asynchronous Python library for PetKit's API.
         
-        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
+        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`.
         
         ## **Currently Supported Devices**:
         
         `Feeders`
+        - [Fresh Element](https://petkit.us/products/petkit-element-wi-fi-enabled-smart-pet-food-container-feeder)
         - [D3 (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
         - [D4 (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
         - [D4s (Fresh Element Gemini)](https://www.amazon.com/PETKIT-Automatic-Combination-Dispenser-Stainless/dp/B0BF56RTQH)
         - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
         
         `Litter Boxes`
         - [T3 (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
@@ -51,14 +52,15 @@
         from petkitaio import PetKitClient
         from aiohttp import ClientSession
         
         async def main():
             async with ClientSession() as session:
         
                 # Create a client using PetKit account email and password
+                # For PetKit Asia accounts, the client would be in the form of client = PetKitClient('email', 'password', session, True)
                 client = PetKitClient('email', 'password', session)
         
         
                 ###################################################################################
                 Examples within the examples section utilize the PetKitClient instance created above
                 ###################################################################################
```

### Comparing `petkitaio-0.1.5/README.md` & `petkitaio-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # PetKitAIO
 
 Asynchronous Python library for PetKit's API.
 
-This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
+This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`.
 
 ## **Currently Supported Devices**:
 
 `Feeders`
+- [Fresh Element](https://petkit.us/products/petkit-element-wi-fi-enabled-smart-pet-food-container-feeder)
 - [D3 (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
 - [D4 (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
 - [D4s (Fresh Element Gemini)](https://www.amazon.com/PETKIT-Automatic-Combination-Dispenser-Stainless/dp/B0BF56RTQH)
 - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
 
 `Litter Boxes`
 - [T3 (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
@@ -41,14 +42,15 @@
 from petkitaio import PetKitClient
 from aiohttp import ClientSession
 
 async def main():
     async with ClientSession() as session:
 
         # Create a client using PetKit account email and password
+        # For PetKit Asia accounts, the client would be in the form of client = PetKitClient('email', 'password', session, True)
         client = PetKitClient('email', 'password', session)
 
 
         ###################################################################################
         Examples within the examples section utilize the PetKitClient instance created above
         ###################################################################################
```

### Comparing `petkitaio-0.1.5/petkitaio/__init__.py` & `petkitaio-0.1.6/petkitaio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .constants import (
     AUTH_ERROR_CODES,
     BLE_HEADER,
     BLUETOOTH_ERRORS,
     CLIENT_DICT,
+    FeederCommand,
     FEEDER_LIST,
     FeederSetting,
     LB_CMD_TO_KEY,
     LB_CMD_TO_TYPE,
     LB_CMD_TO_VALUE,
     LitterBoxCommand,
     LitterBoxCommandKey,
@@ -37,13 +38,13 @@
     W5_SETTINGS_COMMANDS,
 )
 from .petkit_client import (PetKitClient, LOGGER,)
 from .exceptions import (AuthError, BluetoothError, PetKitError, ServerError)
 from .model import (Feeder, LitterBox, Pet, PetKitData, Purifier, W5Fountain, )
 from .str_enum import StrEnum
 
-__all__ = ['AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint',
+__all__ = ['AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint', 'FeederCommand',
            'FEEDER_LIST', 'FeederSetting', 'Header', 'LB_CMD_TO_KEY', 'LB_CMD_TO_TYPE', 'LB_CMD_TO_VALUE', 'LitterBox', 'LitterBoxCommand', 'LitterBoxCommandKey',
            'LitterBoxCommandType', 'LitterBoxSetting', 'LITTER_LIST', 'LOGGER', 'Pet', 'PetKitClient', 'PetKitData', 'PetKitError', 'PetSetting', 'Purifier',
            'PurifierCommand', 'PurifierCommandKey', 'PurifierCommandType', 'PUR_CMD_TO_KEY', 'PUR_CMD_TO_TYPE', 'PUR_CMD_TO_VALUE', 'PURIFIER_LIST', 'PurifierSetting', 'Region',
            'ServerError', 'SERVER_ERROR_CODES', 'StrEnum', 'TIMEOUT', 'WATER_FOUNTAIN_LIST', 'W5Command', 'W5_COMMAND_TO_CODE', 'W5_DND_COMMANDS', 'W5Fountain', 'W5_LIGHT_BRIGHTNESS',
            'W5_LIGHT_POWER', 'W5_MODE', 'W5_SETTINGS_COMMANDS',  ]
```

### Comparing `petkitaio-0.1.5/petkitaio/constants.py` & `petkitaio-0.1.6/petkitaio/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,19 @@
     CANCEL_FEED = '/cancelRealtimeFeed'
     CONTROL_DEVICE = '/controlDevice'
     CONTROL_WF = '/ble/controlDevice'
     DEVICE_DETAIL = '/device_detail'
     DEVICE_RECORD = '/getDeviceRecord'
     DEVICE_ROSTER = '/discovery/device_roster'
     FEEDER_DESICCANT_RESET = '/desiccantReset'
+    FRESH_ELEMENT_CALIBRATION = '/food_reset'
+    FRESH_ELEMENT_CANCEL_FEED = '/cancel_realtime_feed'
+    FRESH_ELEMENT_DESICCANT_RESET = '/feeder/desiccant_reset'
+    FRESH_ELEMENT_MANUAL_FEED = '/feeder/save_dailyfeed'
+    FRESH_ELEMENT_SETTING = '/feeder/update'
     LOGIN = '/user/login'
     MANUAL_FEED = '/saveDailyFeed'
     MAX_ODOR_RESET = '/deodorantReset'
     MINI_DESICCANT_RESET = '/feedermini/desiccant_reset'
     MINI_MANUAL_FEED = '/feedermini/save_dailyfeed'
     MINI_SETTING = '/feedermini/update'
     PET_PROPS = '/pet/updatepetprops'
@@ -40,14 +45,16 @@
 
 class FeederSetting(StrEnum):
 
     CHILD_LOCK = 'manualLock'
     DISPENSE_TONE = 'feedSound'
     DO_NOT_DISTURB = 'disturbMode'
     FEED_TONE = 'feedTone'
+    FRESH_ELEMENT_CHILD_LOCK = 'settings.manualLock'
+    FRESH_ELEMENT_INDICATOR_LIGHT = 'settings.lightMode'
     INDICATOR_LIGHT = 'lightMode'
     MIN_EAT_DURATION = 'shortest'
     MINI_CHILD_LOCK = 'settings.manualLock'
     MINI_INDICATOR_LIGHT = 'settings.lightMode'
     SELECTED_SOUND = 'selectedSound'
     SHORTAGE_ALARM = 'foodWarn'
     SOUND_ENABLE = 'soundEnable'
@@ -67,14 +74,19 @@
     CONTENT_TYPE = 'application/x-www-form-urlencoded'
     AGENT = 'PETKIT/8.28.0 (iPhone; iOS 15.1; Scale/3.00)'
     TZ = 'America/New_York'
     CLIENT = 'ios(15.1;iPhone14,3)'
     LOCALE = 'en_US'
 
 
+class FeederCommand(StrEnum):
+
+    START_CALIBRATION = 'Start calibration'
+    STOP_CALIBRATION = 'Stop calibration'
+
 class LitterBoxCommand(StrEnum):
 
     LIGHT_ON = 'light_on'
     ODOR_REMOVAL = 'start_odor'
     PAUSE_CLEAN = 'stop_clean'
     POWER = 'power'
     RESET_DEODOR = 'reset_deodorizer'
@@ -248,15 +260,15 @@
 }
 
 SERVER_ERROR_CODES = {
     1: 'PetKit servers are busy. Please try again later.',
 }
 
 BLE_HEADER = [-6, -4, -3]
-FEEDER_LIST = ['D3', 'D4', 'D4s', 'FeederMini']
+FEEDER_LIST = ['D3', 'D4', 'D4s', 'Feeder', 'FeederMini']
 LITTER_LIST = ['T3', 'T4']
 PURIFIER_LIST = ['K2']
 WATER_FOUNTAIN_LIST = ['W5']
 
 LB_CMD_TO_KEY = {
     LitterBoxCommand.LIGHT_ON: LitterBoxCommandKey.START,
     LitterBoxCommand.POWER: LitterBoxCommandKey.POWER,
```

### Comparing `petkitaio-0.1.5/petkitaio/exceptions.py` & `petkitaio-0.1.6/petkitaio/exceptions.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.5/petkitaio/model.py` & `petkitaio-0.1.6/petkitaio/model.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.5/petkitaio/petkit_client.py` & `petkitaio-0.1.6/petkitaio/petkit_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from petkitaio.constants import (
     AUTH_ERROR_CODES,
     BLE_HEADER,
     BLUETOOTH_ERRORS,
     CLIENT_DICT,
     Endpoint,
+    FeederCommand,
     FEEDER_LIST,
     FeederSetting,
     Header,
     LB_CMD_TO_KEY,
     LB_CMD_TO_TYPE,
     LB_CMD_TO_VALUE,
     LitterBoxCommand,
@@ -765,14 +766,16 @@
         """Dispense food manually.
         Mini Feeder allowed amount (in grams) is 5, 10, 15, 20, 25, 30, 35, 40, 45, 50.
         D4 (Element Solo) allowed amount is 10, 20, 30, 40, 50.
         """
 
         if feeder.type == 'feedermini':
             url = f'{self.base_url}{Endpoint.MINI_MANUAL_FEED}'
+        elif feeder.type == 'feeder':
+            url = f'{self.base_url}{Endpoint.FRESH_ELEMENT_MANUAL_FEED}'
         else:
             url = f'{self.base_url}/{feeder.type}{Endpoint.MANUAL_FEED}'
         header = await self.create_header()
         data = {
             'amount': amount,
             'day': str(datetime.now().date()).replace('-', ''),
             'deviceId': feeder.id,
@@ -805,14 +808,17 @@
             self.last_manual_feed_id[feeder.id] = response['result']['id']
 
     async def update_feeder_settings(self, feeder: Feeder, setting: FeederSetting, value: int) -> None:
         """Change the setting on a feeder."""
 
         if feeder.type == 'feedermini':
             url = f'{self.base_url}{Endpoint.MINI_SETTING}'
+        # Fresh Element Feeder
+        elif feeder.type == 'feeder':
+            url = f'{self.base_url}{Endpoint.FRESH_ELEMENT_SETTING}'
         # D3 and D4 Feeders
         else:
             url = f'{self.base_url}/{feeder.type}{Endpoint.UPDATE_SETTING}'
         header = await self.create_header()
         setting_dict = {
             setting: value
         }
@@ -863,15 +869,19 @@
             'kv': json.dumps(setting_dict)
         }
         await self._post(url, header, data)
 
     async def cancel_manual_feed(self, feeder: Feeder) -> None:
         """Cancel a manual feed that is currently in progress. Not available for mini feeders"""
 
-        url = f'{self.base_url}/{feeder.type}{Endpoint.CANCEL_FEED}'
+        # Fresh Element feeder
+        if feeder.type == 'feeder':
+            url = f'{self.base_url}/{feeder.type}{Endpoint.FRESH_ELEMENT_CANCEL_FEED}'
+        else:
+            url = f'{self.base_url}/{feeder.type}{Endpoint.CANCEL_FEED}'
         header = await self.create_header()
         if feeder.type == 'd4s':
             if feeder.last_manual_feed_id is None:
                 raise PetKitError('Unable to cancel manual feeding. No valid last manual feeding ID found.')
             else:
                 data = {
                     'day': str(datetime.now().date()).replace('-', ''),
@@ -889,14 +899,17 @@
         await self._post(url, header, data)
 
     async def reset_feeder_desiccant(self, feeder: Feeder) -> None:
         """Reset the desiccant of a single feeder."""
 
         if feeder.type == 'feedermini':
             url = f'{self.base_url}{Endpoint.MINI_DESICCANT_RESET}'
+        # Fresh Element Feeder
+        elif feeder.type == 'feeder':
+            url = f'{self.base_url}{Endpoint.FRESH_ELEMENT_DESICCANT_RESET}'
         else:
             url = f'{self.base_url}/{feeder.type}{Endpoint.FEEDER_DESICCANT_RESET}'
         header = await self.create_header()
         data = {
             'deviceId': feeder.id
         }
         await self._post(url, header, data)
@@ -926,7 +939,27 @@
             url = f'{self.base_url}/{feeder.type}{Endpoint.REPLENISHED_FOOD}'
             header = await self.create_header()
             data = {
                 'deviceId': feeder.id,
                 'noRemind': 3
             }
             await self._post(url, header, data)
+
+    async def fresh_element_calibration(self, feeder: Feeder, command: FeederCommand) -> None:
+        """Start/stop calibration command to Fresh Element feeder.
+        This needs to be done whenever batteries are added or removed.
+        """
+
+        if feeder.type != 'feeder':
+            raise PetKitError('Calibration is only used for Fresh Element feeders.')
+        else:
+            url = f'{self.base_url}/{feeder.type}{Endpoint.FRESH_ELEMENT_CALIBRATION}'
+            header = await self.create_header()
+            if command == FeederCommand.START_CALIBRATION:
+                value = 1
+            else:
+                value = 0
+            data = {
+                'action': value,
+                'deviceId': feeder.id
+            }
+            await self._post(url, header, data)
```

### Comparing `petkitaio-0.1.5/petkitaio/str_enum.py` & `petkitaio-0.1.6/petkitaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.5/petkitaio.egg-info/PKG-INFO` & `petkitaio-0.1.6/petkitaio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
 Description: # PetKitAIO
         
         Asynchronous Python library for PetKit's API.
         
-        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
+        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`.
         
         ## **Currently Supported Devices**:
         
         `Feeders`
+        - [Fresh Element](https://petkit.us/products/petkit-element-wi-fi-enabled-smart-pet-food-container-feeder)
         - [D3 (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
         - [D4 (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
         - [D4s (Fresh Element Gemini)](https://www.amazon.com/PETKIT-Automatic-Combination-Dispenser-Stainless/dp/B0BF56RTQH)
         - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
         
         `Litter Boxes`
         - [T3 (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
@@ -51,14 +52,15 @@
         from petkitaio import PetKitClient
         from aiohttp import ClientSession
         
         async def main():
             async with ClientSession() as session:
         
                 # Create a client using PetKit account email and password
+                # For PetKit Asia accounts, the client would be in the form of client = PetKitClient('email', 'password', session, True)
                 client = PetKitClient('email', 'password', session)
         
         
                 ###################################################################################
                 Examples within the examples section utilize the PetKitClient instance created above
                 ###################################################################################
```

### Comparing `petkitaio-0.1.5/setup.py` & `petkitaio-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petkitaio",
-    version="0.1.5",
+    version="0.1.6",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for PetKit's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/petkitaio',
     keywords='petkit, eversweet 3 pro, feeder mini, d4, petkit feeder, petkit water fountain, freshelement solo, pura x, pura max, pura air',
```

