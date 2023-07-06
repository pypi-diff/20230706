# Comparing `tmp/lmcloud-0.3.4.tar.gz` & `tmp/lmcloud-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.3.4.tar", last modified: Sun May 14 11:56:33 2023, max compression
+gzip compressed data, was "lmcloud-0.3.5.tar", last modified: Thu Jul  6 10:51:41 2023, max compression
```

## Comparing `lmcloud-0.3.4.tar` & `lmcloud-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:56:33.603080 lmcloud-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-14 11:56:20.000000 lmcloud-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-14 11:56:33.603080 lmcloud-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-14 11:56:20.000000 lmcloud-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:56:33.603080 lmcloud-0.3.4/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 11:56:20.000000 lmcloud-0.3.4/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-14 11:56:20.000000 lmcloud-0.3.4/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-14 11:56:20.000000 lmcloud-0.3.4/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-14 11:56:20.000000 lmcloud-0.3.4/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-14 11:56:20.000000 lmcloud-0.3.4/lmcloud/lmbluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-05-14 11:56:20.000000 lmcloud-0.3.4/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-14 11:56:20.000000 lmcloud-0.3.4/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:56:33.603080 lmcloud-0.3.4/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-14 11:56:33.000000 lmcloud-0.3.4/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-14 11:56:33.000000 lmcloud-0.3.4/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:56:33.000000 lmcloud-0.3.4/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-14 11:56:33.000000 lmcloud-0.3.4/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 11:56:33.000000 lmcloud-0.3.4/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 11:56:33.603080 lmcloud-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-14 11:56:20.000000 lmcloud-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:51:41.232125 lmcloud-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-06 10:51:27.000000 lmcloud-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-06 10:51:41.232125 lmcloud-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-06 10:51:27.000000 lmcloud-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:51:41.232125 lmcloud-0.3.5/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/lmbluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22263 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-06 10:51:27.000000 lmcloud-0.3.5/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:51:41.232125 lmcloud-0.3.5/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 10:51:41.000000 lmcloud-0.3.5/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:51:41.232125 lmcloud-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-06 10:51:27.000000 lmcloud-0.3.5/setup.py
```

### Comparing `lmcloud-0.3.4/LICENSE` & `lmcloud-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.4/PKG-INFO` & `lmcloud-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.4/README.md` & `lmcloud-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.4/lmcloud/helpers.py` & `lmcloud-0.3.5/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.4/lmcloud/lmbluetooth.py` & `lmcloud-0.3.5/lmcloud/lmbluetooth.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.4/lmcloud/lmcloud.py` & `lmcloud-0.3.5/lmcloud/lmcloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     @property
     def config(self):
         """ 
         Return the config with capitalized keys to be consistent across local/remote APIs 
         """
 
-        return {k.upper():v for k,v in self._config.items()}
+        return self._config
     
     @property
     def status(self):
         return self._status
     
     @property
     def statistics(self):
@@ -56,29 +56,24 @@
         Build object which holds status for lamarzocco Home Assistant Integration
         """
 
         return {
             "power": True if self.config[MACHINE_MODE] == "BrewingMode" else False,
             "enable_prebrewing": True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "Enabled" else False,
             "enable_preinfusion": True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "TypeB" else False,
-            "steam_boiler_enable": next(item for item in self.config[BOILERS] if item["id"] == STEAM_BOILER_NAME)["isEnabled"],
+            "steam_boiler_enable": self._config_steamboiler["isEnabled"],
             "global_auto": self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"],
-            "coffee_temp": self.status[COFFEE_TEMP],
-            "coffee_set_temp": self.config[BOILER_TARGET_TEMP][COFFEE_BOILER_NAME],
-            "steam_temp": self.status[STEAM_TEMP],
-            "steam_set_temp": self.config[BOILER_TARGET_TEMP][STEAM_BOILER_NAME],
-            "water_reservoir_contact": self.status[TANK_LEVEL],
+            "coffee_temp": self._config_coffeeboiler[CURRENT],
+            "coffee_set_temp": self._config_coffeeboiler[TARGET],
+            "steam_temp": self._config_steamboiler[CURRENT],
+            "steam_set_temp": self._config_steamboiler[TARGET],
+            "water_reservoir_contact": self.config[TANK_STATUS],
             "plumbin_enable": self.config[PLUMBED_IN],
             "drinks_k1":        self.statistics[0]["count"],
-            "drinks_k2":        self.statistics[1]["count"],
-            "drinks_k3":        self.statistics[2]["count"],
-            "drinks_k4":        self.statistics[3]["count"],
-            "continuous":       self.statistics[4]["count"],
-            "total_flushing":   self.statistics[5]["count"],
-            "active_brew": self.status[ACTIVE_BREW] if self._use_websocket else False
+            "total_flushing":   self.statistics[1]["count"]
         }
 
 
     '''
     *******************************************
     ***  Getters for current machine state ****
     *******************************************
@@ -87,21 +82,19 @@
     # will return current machine mode (Brewing/StandBy)
     async def get_machine_mode(self):
         await self.update_local_machine_status()
         return self.config[MACHINE_MODE]
 
     async def get_coffee_boiler_enabled(self):
         await self.update_local_machine_status()
-        coffee_boiler = next(item for item in self.config[BOILERS] if item["id"] == COFFEE_BOILER_NAME)
-        return coffee_boiler["isEnabled"]
+        return self._config_coffeeboiler["isEnabled"]
 
     async def get_steam_boiler_enabled(self):
         await self.update_local_machine_status()
-        coffee_boiler = next(item for item in self.config[BOILERS] if item["id"] == STEAM_BOILER_NAME)
-        return coffee_boiler["isEnabled"]
+        return self._config_steamboiler["isEnabled"]
 
     async def get_coffee_temp(self):
         await self.update_local_machine_status()
         return self.config[BOILER_TARGET_TEMP][COFFEE_BOILER_NAME]
 
     async def get_steam_temp(self):
         await self.update_local_machine_status()
@@ -128,14 +121,16 @@
 
     def __init__(self):
         _logger.setLevel(logging.DEBUG)
         self._lm_local_api      = None
         self._lm_bluetooth      = None
         self. _config           = {}
         self. _status           = {}
+        self. _config_steamboiler  = {}
+        self. _config_coffeeboiler = {}
         self. _statistics       = {}
         self._use_websocket     = False
 
 
     @classmethod
     async def create(cls, credentials):
         '''
@@ -240,61 +235,41 @@
             # wait at least 10 seconds between config updates to not flood the remote API
             if (datetime.now() - self._last_config_update).total_seconds() < POLLING_DELAY_S or force_update:
                 return
         self._config = await self.get_config()
         self._last_config_update = datetime.now()
 
 
-    async def get_status(self):
-        '''
-        Get status from cloud
-        '''
-
-        url = f"{self._gw_url_with_serial}/status"
-        try:
-            status = await self._rest_api_call(url=url, verb="GET")
-            return status
-        except Exception as e:
-            _logger.error(f"Could not get config from cloud. Full error: {e}")
-            return self._status
-        
-    async def _update_status_obj(self, force_update=False):
-        if self._status:
-            # wait at least 10 seconds between config updates to not flood the remote API
-            if (datetime.now() - self._last_status_update).total_seconds() < POLLING_DELAY_S or force_update:
-                return
-        self._status = await self.get_status()
-        self._last_status_update = datetime.now() 
-
-
     async def update_local_machine_status(self, in_init=False):
         '''
         update config object
         '''
 
         if self._lm_local_api:
             try:
-                conf = await self._lm_local_api.local_get_config()
-                self._config = {k.upper():v for k,v in conf.items()}
+                self._config = await self._lm_local_api.local_get_config()
             except Exception as e:
                 _logger.warn(f"Could not connect to local API although initialized. Full error: {e}")
                 await self._update_config_obj()
 
             if self._lm_local_api._timestamp_last_websocket_msg == None or (datetime.now() - self._lm_local_api._timestamp_last_websocket_msg).total_seconds() > 30: 
                 if self._use_websocket and not in_init: # during init we don't want to log this warning
                     _logger.warn("Could not get local machine status. Falling back to cloud status.")
-                await self._update_status_obj()
+
                 self._status[ACTIVE_BREW] = False
             else:
                 # Get local status from WebSockets
                 _logger.info("Using local status")
                 self._status = self._lm_local_api._status # reference to the same object tp get websocket updates
         else:
             await self._update_config_obj()     
-            await self._update_status_obj()
+
+        self._config_coffeeboiler = next(item for item in self.config[BOILERS] if item["id"] == COFFEE_BOILER_NAME)
+        self._config_steamboiler  = next(item for item in self.config[BOILERS] if item["id"] == STEAM_BOILER_NAME)
+
 
         await self._update_statistics_obj()
 
 
     async def get_statistics(self):
         '''
         Get statistics
@@ -375,34 +350,35 @@
     
 
     async def get_firmware(self):
         '''
         Get Firmware details
         '''
 
-        url = f"{self._gw_url_with_serial}/firmwarev2/"
+        url = f"{self._gw_url_with_serial}/firmware/"
         return await self._rest_api_call(url=url, verb="GET")
 
    
     async def set_power(self, enabled: bool):
         '''
         Turn power of machine on or off
         '''
 
         if self._lm_bluetooth:
             bt_ok = await self._send_bluetooth_command(self._lm_bluetooth.set_power, enabled)
             response = "Ok"
 
+        mode = "BrewingMode" if enabled else "StandBy"
+
         if not self._lm_bluetooth or not bt_ok:
-            power_status = "ON" if enabled else "STANDBY"
-            data = {"status": power_status}
+            data = {"status": mode}
             url = f"{self._gw_url_with_serial}/status"
             response = await self._rest_api_call(url=url, verb="POST", data=data)
 
-        self._config[MACHINE_MODE] = "BrewingMode" if enabled else "StandBy"
+        self._config[MACHINE_MODE] = mode
         return response
 
 
     async def set_steam(self, steam_state:bool):
         '''
         Turn Steamboiler on or off
         '''
@@ -531,15 +507,15 @@
         else:
             if prebrewOnTime % 100 != 0 or prebrewOffTime % 100 != 0:
                 msg = "Prebrew times must be multiple of 100"
                 _logger.debug(msg)
                 raise ValueError(msg)
             url = f"{self._gw_url_with_serial}/setting-preinfusion"
             data = {
-                "button": "Continuous",
+                "button": "DoseA",
                 "group": "Group1",
                 "holdTimeMs": prebrewOffTime,
                 "wetTimeMs": prebrewOnTime
             }
             response = await self._rest_api_call(url=url, verb="POST", data=data)
 
             self._config[PRE_INFUSION_SETTINGS]["Group1"][0]["preWetTime"] = prebrewOnTime % 1000
```

### Comparing `lmcloud-0.3.4/lmcloud/lmlocalapi.py` & `lmcloud-0.3.5/lmcloud/lmlocalapi.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,26 +20,14 @@
         return self._local_port
     
     @property
     def local_ip(self):
         return self._local_ip
     
     @property
-    def coffee_temp(self):
-        return self._status[COFFEE_TEMP]
-    
-    @property
-    def steam_temp(self):
-        return self._status[STEAM_TEMP]
-    
-    @property
-    def water_reservoir_contact(self):
-        return self._status[TANK_LEVEL]
-    
-    @property
     def active_brew(self):
         return self._status[ACTIVE_BREW]
     
     @property
     def active_brew_duration(self):
         return self._status[ACTIVE_BREW_DURATION]
 
@@ -49,17 +37,15 @@
         self._local_bearer = local_bearer
 
         # init local variables
         self._full_config = None
         self._timestamp_last_websocket_msg = None
 
         self._status = {}
-        self._status[COFFEE_TEMP] = 0
-        self._status[STEAM_TEMP] = 0
-        self._status[TANK_LEVEL] = True
+
         self._status[ACTIVE_BREW] = False
         self._status[ACTIVE_BREW_DURATION] = 0
 
 
     '''
     Get current config of machine from local API
     '''
@@ -90,23 +76,23 @@
                 await asyncio.sleep(20)
                 continue
 
     async def handle_websocket_message(self, message):
         try:
             self._timestamp_last_websocket_msg = datetime.now()
             message = json.loads(message)
-            if type(message) is dict:
-                if message["name"] == "SteamBoilerUpdateTemperature":
-                    self._status[STEAM_TEMP] = message["value"]
-                elif message["name"] == "CoffeeBoiler1UpdateTemperature":
-                    self._status[COFFEE_TEMP] = message["value"]
-                elif message["name"] == "MachineConfiguration":
-                    self._full_config = message["value"]
-                    self._status[TANK_LEVEL] = message["value"]
-            elif type(message) is list:
+            # if type(message) is dict:
+            #     if message["name"] == "SteamBoilerUpdateTemperature":
+            #         self._status[STEAM_TEMP] = message["value"]
+            #     elif message["name"] == "CoffeeBoiler1UpdateTemperature":
+            #         self._status[COFFEE_TEMP] = message["value"]
+            #     elif message["name"] == "MachineConfiguration":
+            #         self._full_config = message["value"]
+            #         self._status[TANK_LEVEL] = message["value"]
+            if type(message) is list:
                 if message[0]["name"] == "BrewingUpdateGroup1Time":
                     self._status[ACTIVE_BREW_DURATION] = message[0]["value"]
                 elif message[0]["name"] in ["BrewingStartedGroup1StopType", "BrewingStartedGroup1DoseIndex"]:
                     # started active brew
                     self._status[ACTIVE_BREW] = True
                 elif message[0]["name"] in ["BrewingSnapshotGroup1", "FlushStoppedGroup1DoseIndex", "FlushStoppedGroup1Time"]:
                     # stopped active brew
```

### Comparing `lmcloud-0.3.4/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.3.5/lmcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.4/setup.py` & `lmcloud-0.3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.3.4",
+    version="0.3.5",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

