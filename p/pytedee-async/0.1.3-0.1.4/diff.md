# Comparing `tmp/pytedee_async-0.1.3.tar.gz` & `tmp/pytedee_async-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.1.3.tar", last modified: Mon Jul  3 13:20:52 2023, max compression
+gzip compressed data, was "pytedee_async-0.1.4.tar", last modified: Thu Jul  6 20:24:33 2023, max compression
```

## Comparing `pytedee_async-0.1.3.tar` & `pytedee_async-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/pytedee_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 13:20:52.000000 pytedee_async-0.1.3/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:20:52.154368 pytedee_async-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 13:20:38.000000 pytedee_async-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:24:33.083401 pytedee_async-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-06 20:24:33.083401 pytedee_async-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:24:33.083401 pytedee_async-0.1.4/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/pytedee_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/pytedee_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:24:33.083401 pytedee_async-0.1.4/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-06 20:24:33.000000 pytedee_async-0.1.4/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-06 20:24:33.000000 pytedee_async-0.1.4/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:24:33.000000 pytedee_async-0.1.4/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 20:24:33.000000 pytedee_async-0.1.4/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 20:24:33.000000 pytedee_async-0.1.4/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:24:33.083401 pytedee_async-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:24:19.000000 pytedee_async-0.1.4/setup.py
```

### Comparing `pytedee_async-0.1.3/LICENSE` & `pytedee_async-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.3/pytedee_async/Lock.py` & `pytedee_async-0.1.4/pytedee_async/Lock.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.3/pytedee_async/TedeeClient.py` & `pytedee_async-0.1.4/pytedee_async/TedeeClient.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,14 +72,42 @@
                         raise TedeeClientException("No lock found")
                 elif response.status == 401:
                     raise TedeeAuthException()
                 elif response.status == 429:
                     raise TedeeRateLimitException()
                 else:
                     raise TedeeClientException(f"Error during listing of devices. Status code {response.status}")
+                
+    async def sync(self) -> None:
+        '''Sync locks'''
+        _LOGGER.debug("Syncing locks...")
+        async with aiohttp.ClientSession(
+                headers=self._api_header, 
+                timeout=aiohttp.ClientTimeout(total=self._timeout)
+        ) as session:
+            async with session.get(API_URL_SYNC) as response:
+                if response.status == 200:
+                    r = await response.json()
+                    result = r["result"]
+
+                    for lock_json in result:            
+                        lock_id = lock_json["id"]
+
+                        lock = self.locks_dict[lock_id]
+
+                        lock.is_connected, lock.state, lock.battery_level, lock.is_charging, lock.state_change_result = self.parse_lock_properties(lock_json) 
+                        
+                        self._locks_dict[lock_id] = lock
+
+                elif response.status == 401:
+                    raise TedeeAuthException()
+                elif response.status == 429:
+                    raise TedeeRateLimitException()
+                else:
+                    raise TedeeClientException(f"Error during listing of devices. Status code {response.status}")
                     
 
     async def unlock(self, lock_id) -> None:
         '''Unlock method'''
         url = API_URL_LOCK + str(lock_id) + API_PATH_UNLOCK + "?mode=3"
         
         async with aiohttp.ClientSession(
@@ -87,17 +115,15 @@
                 timeout=aiohttp.ClientTimeout(total=self._timeout)
             ) as session:
             async with session.post(url) as response:
                 if response.status == 202:
                     self._locks_dict[lock_id].state = 4
                     _LOGGER.debug("unlock command successful, id: %d ", lock_id)
                     await asyncio.sleep(UNLOCK_DELAY)
-                    self._locks_dict[lock_id].state = 2
-
-                    await self.get_locks()
+                    self._locks_dict[lock_id].state = 2                   
 
                 elif response.status == 401:
                     raise TedeeAuthException()
                 elif response.status == 429:
                     raise TedeeRateLimitException()
                 else:
                     raise TedeeClientException(f"Error during unlocking of lock {lock_id}. Status code {response.status}")
@@ -113,15 +139,15 @@
             ) as session:
             async with session.post(url) as response:
                 if response.status == 202:
                     self._locks_dict[lock_id].state = 5
                     _LOGGER.debug(f"lock command successful, id: {lock_id}")
                     await asyncio.sleep(LOCK_DELAY)
                     self._locks_dict[lock_id].state = 6
-                    await self.get_locks()
+
                 elif response.status == 401:
                     raise TedeeAuthException()
                 elif response.status == 429:
                     raise TedeeRateLimitException()
                 else:
                     raise TedeeClientException(f"Error during locking of lock {lock_id}. Status code {response.status}")
 
@@ -139,15 +165,15 @@
             async with session.post(url) as response:
                 
                 if response.status == 202:
                     self._locks_dict[lock_id].state = 2
                     _LOGGER.debug(f"open command successful, id: {lock_id}")
 
                     await asyncio.sleep(self._locks_dict[lock_id].duration_pullspring + 1)
-                    await self.get_locks()
+
                 elif response.status == 401:
                     raise TedeeAuthException()
                 elif response.status == 429:
                     raise TedeeRateLimitException()
                 else: 
                     raise TedeeClientException(f"Error during unlatching of lock {lock_id}. Status code {response.status}")
                 
@@ -165,15 +191,15 @@
             async with session.post(url) as response:
                 
                 if response.status == 202:
                     self._locks_dict[lock_id].state = 7
                     _LOGGER.debug(f"open command successful, id: {lock_id}")
 
                     await asyncio.sleep(self._locks_dict[lock_id].duration_pullspring + 1)
-                    await self.get_locks()
+
                 elif response.status == 401:
                     raise TedeeAuthException()
                 elif response.status == 429:
                     raise TedeeRateLimitException()
                 else: 
                     raise TedeeClientException(f"Error during unlatching of lock {lock_id}. Status code {response.status}")
 
@@ -181,52 +207,52 @@
         lock = self._locks_dict[lock_id]
         return lock.state == 2
     
     def is_locked(self, lock_id) -> bool:
         lock = self._locks_dict[lock_id]
         return lock.state == 6
 
-    def parse_lock_properties(self, state: dict):
-        if state["isConnected"]:
-            connected = state["isConnected"]
+    def parse_lock_properties(self, json: dict):
+        if "isConnected" in json:
+            connected = json["isConnected"]
         else:
             connected = False
 
-        lock_properties = state["lockProperties"]
-
-        if lock_properties["state"]:
-            state = lock_properties["state"]
+        if "lockProperties" in json:
+            lock_properties = json["lockProperties"]
         else:
-            state = 9
+            lock_properties = None
 
-        if lock_properties["stateChangeResult"]:
-            state_change_result = lock_properties["stateChangeResult"]
-        else:
-            state_change_result = 0
-
-        if lock_properties["batteryLevel"]:
+        if lock_properties:
+            state = lock_properties["state"]
             battery_level = lock_properties["batteryLevel"]
-        else:
-            battery_level = 0
-
-        if lock_properties["isCharging"]:
             is_charging = lock_properties["isCharging"]
+            state_change_result = lock_properties["stateChangeResult"]
         else:
+            state = 9
+            battery_level = 0
             is_charging = False
+            state_change_result = 0
 
         return connected, state, battery_level, is_charging, state_change_result
     
     def parse_pull_spring_settings(self, settings: dict):
-        if settings["deviceSettings"]["pullSpringEnabled"]:
-            pullSpringEnabled = settings["deviceSettings"]["pullSpringEnabled"]
+
+        if "deviceSettings" in settings:
+            deviceSettings = settings["deviceSettings"]
+        else:
+            deviceSettings = {}
+
+        if "pullSpringEnabled" in deviceSettings:
+            pullSpringEnabled = deviceSettings["pullSpringEnabled"]
         else:
             pullSpringEnabled = False
 
-        if settings["deviceSettings"]["pullSpringDuration"]:  
-            pullSpringDuration = settings["deviceSettings"]["pullSpringDuration"]
+        if "pullSpringDuration" in deviceSettings:  
+            pullSpringDuration = deviceSettings["pullSpringDuration"]
         else:
             pullSpringDuration = 5
 
         return pullSpringEnabled, pullSpringDuration
     
 
     """ Legacy functions for backwards compability"""
```

### Comparing `pytedee_async-0.1.3/pytedee_async/helpers.py` & `pytedee_async-0.1.4/pytedee_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.3/setup.py` & `pytedee_async-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.1.3",
+    version="0.1.4",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
```

