# Comparing `tmp/dl_myo-1.0.4.tar.gz` & `tmp/dl_myo-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_myo-1.0.4.tar", max compression
+gzip compressed data, was "dl_myo-1.0.5.tar", max compression
```

## Comparing `dl_myo-1.0.4.tar` & `dl_myo-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35123 2023-06-24 11:42:42.130414 dl_myo-1.0.4/LICENSE
--rw-r--r--   0        0        0     3837 2023-06-24 11:42:42.130414 dl_myo-1.0.4/README.md
--rw-r--r--   0        0        0      751 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/commands.py
--rw-r--r--   0        0        0      504 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/constants.py
--rw-r--r--   0        0        0    15170 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/core.py
--rw-r--r--   0        0        0     5805 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/profile.py
--rw-r--r--   0        0        0     8991 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/types.py
--rw-r--r--   0        0        0       22 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/version.py
--rw-r--r--   0        0        0     3210 2023-06-24 11:43:00.134503 dl_myo-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 dl_myo-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35123 2023-07-06 08:00:14.900174 dl_myo-1.0.5/LICENSE
+-rw-r--r--   0        0        0     4456 2023-07-06 08:00:14.900174 dl_myo-1.0.5/README.md
+-rw-r--r--   0        0        0      751 2023-07-06 08:00:14.900174 dl_myo-1.0.5/myo/__init__.py
+-rw-r--r--   0        0        0     3293 2023-07-06 08:00:14.900174 dl_myo-1.0.5/myo/commands.py
+-rw-r--r--   0        0        0      504 2023-07-06 08:00:14.900174 dl_myo-1.0.5/myo/constants.py
+-rw-r--r--   0        0        0    15170 2023-07-06 08:00:14.900174 dl_myo-1.0.5/myo/core.py
+-rw-r--r--   0        0        0     5805 2023-07-06 08:00:14.900174 dl_myo-1.0.5/myo/profile.py
+-rw-r--r--   0        0        0     8991 2023-07-06 08:00:14.900174 dl_myo-1.0.5/myo/types.py
+-rw-r--r--   0        0        0       22 2023-07-06 08:00:14.900174 dl_myo-1.0.5/myo/version.py
+-rw-r--r--   0        0        0     3262 2023-07-06 08:00:37.076539 dl_myo-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 dl_myo-1.0.5/PKG-INFO
```

### Comparing `dl_myo-1.0.4/LICENSE` & `dl_myo-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.4/README.md` & `dl_myo-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 See [`myo/profile.py`](https://github.com/iomz/dl-myo/blob/main/myo/profile.py) for more detail.
 
 <!-- vim-markdown-toc GFM -->
 
 - [Features](#features)
 - [Platform Support](#platform-support)
 - [Install](#install)
-- [Example](#example)
+- [Examples](#examples)
+  - [`sample_client.py`](#sample_clientpy)
+  - [influxdb](#influxdb)
   - [Try the example with Docker](#try-the-example-with-docker)
 - [Build with Poetry](#build-with-poetry)
 - [Credits](#credits)
 - [Author](#author)
 
 <!-- vim-markdown-toc -->
 
@@ -45,15 +47,17 @@
 
 ## Install
 
 ```bash
 pip install dl-myo
 ```
 
-## Example
+## Examples
+
+### `sample_client.py`
 
 The script scans a Myo device, connect to the device, prints the GATT profile from the device, collect EMG data for 5 seconds, and then disconnect.
 
 Any Myo Armband should have the service UUID `d5060001-a904-deb9-4748-2c7f4a124842`.
 
 ```bash
 python examples/sample_client.py
@@ -61,16 +65,37 @@
 
 Otherwise, you can also bind to a specific MAC address. For example,
 
 ```bash
 python examples/sample_client.py --mac D2:3B:85:94:32:8E
 ```
 
+### influxdb
+
+The `examples/influxdb/influx_client.py` emits datapoints to be stored in InfluxDB.
+The `docker-compose.yml` lanches the required database for this by default.
+
+```bash
+docker compose up -d influxdb
+```
+
+then
+
+```bash
+python examples/influxdb/influx_client.py
+```
+
+Make use of the dashboard config `examples/influxdb/myo.json`.
+
+<img width="80%" alt="influxdb" src="https://github.com/iomz/dl-myo/assets/26181/8c5d79f4-f5d8-4e9e-8cab-d5e959972d06">
+
 ### Try the example with Docker
 
+NOTE: The docker example currently doesn't work on macOS.
+
 ```bash
 docker compose pull
 docker compose run --rm dl-myo
 ```
 
 ## Build with Poetry
```

### Comparing `dl_myo-1.0.4/myo/__init__.py` & `dl_myo-1.0.5/myo/__init__.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.4/myo/commands.py` & `dl_myo-1.0.5/myo/commands.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.4/myo/core.py` & `dl_myo-1.0.5/myo/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 
 
 from .constants import (
     RGB_CYAN,
     RGB_PINK,
-    RGB_YELLOW,
+    RGB_ORANGE,
     RGB_GREEN,
 )
 from .commands import (
     Command,
     SetMode,
     Vibrate,
     DeepSleep,
@@ -344,15 +344,15 @@
         classifier_mode=ClassifierMode.DISABLED,
         emg_mode=EMGMode.SEND_FILT,
         imu_mode=IMUMode.NONE,
     ):
         """
         <> setup the myo device
         """
-        await self.led(RGB_YELLOW)
+        await self.led(RGB_ORANGE)
         logger.info(f"setting up the myo: {self.device.name}")
         battery = await self.m.battery_level(self._client)
         logger.info(f"remaining battery: {battery} %")
         # vibrate short *3
         await self.vibrate(VibrationType.SHORT)
         await self.vibrate(VibrationType.SHORT)
         await self.vibrate(VibrationType.SHORT)
```

### Comparing `dl_myo-1.0.4/myo/profile.py` & `dl_myo-1.0.5/myo/profile.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.4/myo/types.py` & `dl_myo-1.0.5/myo/types.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.4/pyproject.toml` & `dl_myo-1.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
   { name="Iori Mizutani", email="iomz@sazanka.io" },
 ]
 description = "Yet another MyoConnect alternative without dongles"
 readme = "README.md"
 classifiers = [
     "Environment :: Console",
     "Framework :: AsyncIO",
-    "Framework :: Hatch",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -92,24 +91,26 @@
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.poetry]
 name = "dl-myo"
-version = "1.0.4"
+version = "1.0.5"
 description = "Yet another MyoConnect alternative without dongles"
 authors = ["Iori Mizutani <iomz@sazanka.io>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "myo"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 bleak = "^0.20.2"
+influxdb-client = {extras = ["ciso"], version = "^1.36.1"}
+aiohttp = "^3.8.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.0"
```

