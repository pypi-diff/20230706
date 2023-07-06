# Comparing `tmp/dtn7zero-0.0.6.tar.gz` & `tmp/dtn7zero-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\dtn7zero\dist\.tmp-xjrmxvmo\dtn7zero-0.0.6.tar", last modified: Wed May  3 14:39:49 2023, max compression
+gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\dtn7zero\dist\.tmp-akzhq7gz\dtn7zero-0.0.7.tar", last modified: Thu Jul  6 13:00:37 2023, max compression
```

## Comparing `dtn7zero-0.0.6.tar` & `dtn7zero-0.0.7.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/
--rw-rw-rw-   0        0        0    35184 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    10080 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     9755 2023-04-28 23:14:49.000000 dtn7zero-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero/
--rw-rw-rw-   0        0        0      261 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/__init__.py
--rw-rw-rw-   0        0        0     9731 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/api.py
--rw-rw-rw-   0        0        0    21246 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/bundle_protocol_agent.py
--rw-rw-rw-   0        0        0     1506 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/
--rw-rw-rw-   0        0        0      615 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/__init__.py
--rw-rw-rw-   0        0        0     3282 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
--rw-rw-rw-   0        0        0    13077 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/mtcp.py
--rw-rw-rw-   0        0        0     2435 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/data.py
--rw-rw-rw-   0        0        0     7598 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/endpoints.py
--rw-rw-rw-   0        0        0    13482 2023-05-03 14:33:51.000000 dtn7zero-0.0.6/dtn7zero/ipnd.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero/routers/
--rw-rw-rw-   0        0        0     3128 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/routers/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/routers/simple_epidemic_router.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero/storage/
--rw-rw-rw-   0        0        0     1402 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/storage/__init__.py
--rw-rw-rw-   0        0        0     2941 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/storage/simple_in_memory_storage.py
--rw-rw-rw-   0        0        0     4715 2023-05-03 14:30:38.000000 dtn7zero-0.0.6/dtn7zero/utility.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/
--rw-rw-rw-   0        0        0    10080 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      654 2023-05-03 13:35:28.000000 dtn7zero-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/test/
--rw-rw-rw-   0        0        0      956 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-api-background.py
--rw-rw-rw-   0        0        0      694 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-api-ping.py
--rw-rw-rw-   0        0        0      563 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-api-pong.py
--rw-rw-rw-   0        0        0      899 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-api-synchronous.py
--rw-rw-rw-   0        0        0     1944 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-protocol-agent-receiver.py
--rw-rw-rw-   0        0        0     2095 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-protocol-agent-sender.py
--rw-rw-rw-   0        0        0     1443 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-protocol-agent.py
--rw-rw-rw-   0        0        0     1711 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-serialization.py
--rw-rw-rw-   0        0        0    15498 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-size.py
--rw-rw-rw-   0        0        0     1688 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-dtn7rs-rest-cla.py
--rw-rw-rw-   0        0        0     1236 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-ipnd.py
--rw-rw-rw-   0        0        0     2028 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-mtcp-intermediate.py
--rw-rw-rw-   0        0        0     2260 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-mtcp-receiver.py
--rw-rw-rw-   0        0        0     2563 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-mtcp-sender.py
--rw-rw-rw-   0        0        0     5282 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-py-dtn7-functionality.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:00:37.000000 dtn7zero-0.0.7/
+-rw-rw-rw-   0        0        0    35184 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0    10795 2023-07-06 13:00:37.000000 dtn7zero-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10470 2023-07-06 11:54:34.000000 dtn7zero-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero/
+-rw-rw-rw-   0        0        0      261 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/dtn7zero/__init__.py
+-rw-rw-rw-   0        0        0     9886 2023-07-03 16:30:35.000000 dtn7zero-0.0.7/dtn7zero/api.py
+-rw-rw-rw-   0        0        0    21220 2023-07-03 15:37:31.000000 dtn7zero-0.0.7/dtn7zero/bundle_protocol_agent.py
+-rw-rw-rw-   0        0        0     2673 2023-07-03 16:28:59.000000 dtn7zero-0.0.7/dtn7zero/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/
+-rw-rw-rw-   0        0        0      939 2023-06-21 11:49:23.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/__init__.py
+-rw-rw-rw-   0        0        0     3311 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
+-rw-rw-rw-   0        0        0     2124 2023-06-21 12:09:12.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/espnow_cla.py
+-rw-rw-rw-   0        0        0    12993 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/mtcp.py
+-rw-rw-rw-   0        0        0     2435 2023-07-06 12:35:47.000000 dtn7zero-0.0.7/dtn7zero/data.py
+-rw-rw-rw-   0        0        0     7620 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/endpoints.py
+-rw-rw-rw-   0        0        0    14821 2023-07-06 12:35:49.000000 dtn7zero-0.0.7/dtn7zero/ipnd.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero/routers/
+-rw-rw-rw-   0        0        0     3133 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/routers/__init__.py
+-rw-rw-rw-   0        0        0     5115 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/routers/simple_epidemic_router.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero/storage/
+-rw-rw-rw-   0        0        0     1402 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/dtn7zero/storage/__init__.py
+-rw-rw-rw-   0        0        0     2910 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/storage/simple_in_memory_storage.py
+-rw-rw-rw-   0        0        0     4769 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/dtn7zero/utility.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/
+-rw-rw-rw-   0        0        0    10795 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 13:00:36.000000 dtn7zero-0.0.7/dtn7zero.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      654 2023-07-06 11:59:17.000000 dtn7zero-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:00:37.000000 dtn7zero-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 13:00:37.000000 dtn7zero-0.0.7/test/
+-rw-rw-rw-   0        0        0      960 2023-07-03 16:32:09.000000 dtn7zero-0.0.7/test/test-api-background.py
+-rw-rw-rw-   0        0        0      698 2023-07-03 16:32:30.000000 dtn7zero-0.0.7/test/test-api-ping.py
+-rw-rw-rw-   0        0        0      567 2023-07-03 16:32:43.000000 dtn7zero-0.0.7/test/test-api-pong.py
+-rw-rw-rw-   0        0        0      903 2023-07-03 16:32:56.000000 dtn7zero-0.0.7/test/test-api-synchronous.py
+-rw-rw-rw-   0        0        0     1940 2023-07-03 16:33:17.000000 dtn7zero-0.0.7/test/test-bundle-protocol-agent-receiver.py
+-rw-rw-rw-   0        0        0     2091 2023-07-03 16:33:34.000000 dtn7zero-0.0.7/test/test-bundle-protocol-agent-sender.py
+-rw-rw-rw-   0        0        0     1454 2023-06-23 13:58:42.000000 dtn7zero-0.0.7/test/test-bundle-protocol-agent.py
+-rw-rw-rw-   0        0        0     1711 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/test/test-bundle-serialization.py
+-rw-rw-rw-   0        0        0    15498 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/test/test-bundle-size.py
+-rw-rw-rw-   0        0        0     1745 2023-07-03 16:34:44.000000 dtn7zero-0.0.7/test/test-dtn7rs-rest-cla.py
+-rw-rw-rw-   0        0        0     2049 2023-07-05 14:49:44.000000 dtn7zero-0.0.7/test/test-espnow-receiver.py
+-rw-rw-rw-   0        0        0     2348 2023-07-05 14:49:40.000000 dtn7zero-0.0.7/test/test-espnow-sender.py
+-rw-rw-rw-   0        0        0     1236 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/test/test-ipnd.py
+-rw-rw-rw-   0        0        0     2114 2023-07-05 13:52:56.000000 dtn7zero-0.0.7/test/test-mtcp-intermediate.py
+-rw-rw-rw-   0        0        0     2315 2023-07-03 16:37:33.000000 dtn7zero-0.0.7/test/test-mtcp-receiver.py
+-rw-rw-rw-   0        0        0     2618 2023-07-03 16:37:33.000000 dtn7zero-0.0.7/test/test-mtcp-sender.py
+-rw-rw-rw-   0        0        0     5282 2023-04-28 22:29:12.000000 dtn7zero-0.0.7/test/test-py-dtn7-functionality.py
```

### Comparing `dtn7zero-0.0.6/LICENSE` & `dtn7zero-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.6/PKG-INFO` & `dtn7zero-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,24 @@
-Metadata-Version: 2.1
-Name: dtn7zero
-Version: 0.0.6
-Author-email: Lukas Holst <lh700@proton.me>
-License: AGPL-3.0
-Project-URL: Homepage, https://github.com/dtn7/dtn7zero
-Project-URL: Repository, https://github.com/dtn7/dtn7zero
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dtn7zero
 This is a DTN7 [RFC9171](https://datatracker.ietf.org/doc/html/rfc9171) compliant python implementation (work-in-progress) with a [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
 
 The current features are:
 - a full bundle protocol agent (without fragment, CRC, and status-report generation support -> todo)
 - a minimal TCP convergence layer
 - a [dtn7-rs](https://github.com/dtn7/dtn7-rs) convergence layer, using the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md) interface
-- automatic local-network node-discovery via ipnd module
+- automatic local-network node-discovery via IPND module
 - a standalone 'external' endpoint (which connects to a [dtn7-rs](https://github.com/dtn7/dtn7-rs) via the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md)) interface
 - a simplified [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API to easily get started
 - full MicroPython support (tested on an ESP32-GENERIC)
+- experimental ESPNOW cla (details can be found in the source code: *dtn7zero/convergence_layer_adapters/espnow_cla.py*)
 - (currently uses epidemic routing and in-memory storage managing)
 - (with extendability for new convergence layer adapters, routing algorithms, and storage managers)
 
 ## Getting Started
+
 To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux):
 ```shell
 $ pip install --upgrade dtn7zero
 ```
 The most simple example on what you can do:
 ```python
 import time
@@ -40,66 +31,71 @@
 
 node_endpoint.send(b'hello world', "dtn://node1/")
 
 time.sleep(1)
 ```
 Further examples for the 'simple' API can be found under `./examples` in the GitHub repository.
 
-For a deeper dive into the underlying concepts and the fully fletched dtn implementation, take a look at the 
-`dtn7zero.api` module implementation and the tests under `./tests`.
+For a deeper dive into the underlying concepts and the full-fledged dtn implementation, take a look at the 
+`dtn7zero.api` module implementation and the tests under `./test`.
 
 ## MicroPython Installation Guide
+Installation has been successfully tested on Windows and Linux (x86_64 and arm64). The required
+[mpy-cross](https://pypi.org/project/mpy-cross/) has been shown to have installation issues on Mac M1s
+under Mac OS X and may have to be built and installed manually.
+
 This whole project was tested on an ESP32 (GENERIC) and this installation guide is tailored for the ESP32.
 If you plan to use another microcontroller you might need to do adjustments 
 (most certainly the MicroPython installation, and the MPY_MARCH in esp-deployment.py).
 
 Important note for linux: it may be that mpremote assumes another USB device with higher priority than the ESP32.
 In that case all mpremote commands (especially inside esp-deployment.py) will fail as no communication is possible.
 Check all USB devices mpremote considers in priority order with `mpremote devs`.
 
 ### First Time MicroPython Installation For ESP32 (GENERIC)
 1. download the newest [firmware](https://micropython.org/download/esp32/)
 2. install the esp flash tool: `pip install esptool`
 3. connect your ESP32 via USB and start a terminal at the location of the downloaded firmware
-4. start the following command (with the correct USB port), then hold **boot** until it starts erasing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 erase_flash`
-5. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
+4. start the following command (with the correct USB port): \
+`esptool --chip esp32 --port /dev/ttyUSB0 erase_flash` (you may have to invoke esptool with `esptool.py --chip ...` here and subsequently, you may also have hold **boot** to enter the bootloader on the ESP32)
+5. start the following command (with the correct USB port and firmware name): \
+`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin` (you may have hold **boot** again to enter the bootloader on the ESP32)
 6. done, you may now connect to it via: `mpremote` (installation via pip: `pip install mpremote`)
 
 ### Update To New MicroPython Version
 1. download the newest [firmware](https://micropython.org/download/esp32/)
-2. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
+2. start the following command (with the correct USB port and firmware name): \
+`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin` (you may have hold **boot** to enter the bootloader on the ESP32)
 3. done
 
 ### First Time dtn7zero Deployment
 1. make sure you check out the repository and the submodules (especially py-dtn7)
 2. install the mpremote tool: `pip install mpremote`
-3. install the mpy-cross compiler tool: `pip install mpy-cross`
+3. install the mpy-cross compiler tool: `pip install mpy-cross` (this may not work on Mac M1s under Mac OS X) 
 4. populate wlan.json with an appropriate hostname and at least one ssid -> password mapping
 5. check your connection to the ESP32 with: `mpremote`
 6. copy wlan.json to your ESP32: `mpremote fs cp wlan.json :wlan.json`
 7. copy boot.py to your ESP32: `mpremote fs cp boot.py :boot.py`
 8. deploy the dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
-9. done
+9. install required packages: `mpremote mip install urequests` and `mpremote mip install datetime`
+10. done
 
 ### Continuous dtn7zero Deployment
 1. check your connection to the ESP32 with: `mpremote`
 2. deploy the changes of dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
 3. done
 
 ### First dtn7zero Functionality Check On MicroPython
 1. you may check that wlan is connecting correctly (connect via `mpremote` and press **enable** for a soft reset)
 2. you may also check that you can import dtn7zero (connect via `mpremote` and `import dtn7zero`)
 3. you can also check that everything works (run the test script `mpremote run examples/local_ping_echo.py`)
 
 ### Additional MicroPython Tips & Tricks
 The mpremote tool is normally interrupted by using `ctrl+c`. A special case is the REPL (simply call `mpremote`), which
-can be exited by using `ctrl+~` (tested on windows).
+can be exited by using `ctrl+~` (tested on Windows) or `ctrl+]` (Linux).
 
 If you start a script on MicroPython (`mpremote run ...`) and disconnect the console (`mpremote` -> `ctrl+c`) then the script 
 keeps running.
 
 If you must access the REPL via mpremote, but a script is blocking, then call `mpremote` and press EN (enable) on the 
 ESP32 for a soft-reset. Press `ctrl+c` a few times to interrupt the `boot.py` or `main.py` script execution. The session
 state is stored, so any subsequent `mpremote` call will start at REPL as long as no power disconnect is performed.
@@ -107,17 +103,17 @@
 You can deploy a script as `main.py` on MicroPython to be run every time the microcontroller gets power. \
 You can also remove the script. MicroPython will only execute the script if it is present.
 ```shell
 $ mpremote fs cp examples/remote_echo_callback.py :main.py
 $ mpremote fs rm :main.py
 ```
 
-Regarding `boot.py`, it is used for user-specific setup code and this framework uses a generic boot script that adjusts
+Regarding `boot.py`: it is used for user-specific setup code and this framework uses a generic boot script that adjusts
 the ESP32's frequency and connects to a Wi-Fi network (blocking until success). MicroPython will create a dummy `boot.py`
-if none is present. MicroPython will not create a dummy `main.py` is none is present. MicroPython will first execute
+if none is present. MicroPython will not create a dummy `main.py` if none is present. MicroPython will first execute
 the `boot.py` and then the `main.py` if it is present.
 
 
 ## Development Information
 
 ### Development Mode
 You can install this project locally to directly reflect code changes in your environment.
```

### Comparing `dtn7zero-0.0.6/README.md` & `dtn7zero-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,35 @@
+Metadata-Version: 2.1
+Name: dtn7zero
+Version: 0.0.7
+Author-email: Lukas Holst <lh700@proton.me>
+License: AGPL-3.0
+Project-URL: Homepage, https://github.com/dtn7/dtn7zero
+Project-URL: Repository, https://github.com/dtn7/dtn7zero
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dtn7zero
 This is a DTN7 [RFC9171](https://datatracker.ietf.org/doc/html/rfc9171) compliant python implementation (work-in-progress) with a [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
 
 The current features are:
 - a full bundle protocol agent (without fragment, CRC, and status-report generation support -> todo)
 - a minimal TCP convergence layer
 - a [dtn7-rs](https://github.com/dtn7/dtn7-rs) convergence layer, using the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md) interface
-- automatic local-network node-discovery via ipnd module
+- automatic local-network node-discovery via IPND module
 - a standalone 'external' endpoint (which connects to a [dtn7-rs](https://github.com/dtn7/dtn7-rs) via the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md)) interface
 - a simplified [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API to easily get started
 - full MicroPython support (tested on an ESP32-GENERIC)
+- experimental ESPNOW cla (details can be found in the source code: *dtn7zero/convergence_layer_adapters/espnow_cla.py*)
 - (currently uses epidemic routing and in-memory storage managing)
 - (with extendability for new convergence layer adapters, routing algorithms, and storage managers)
 
 ## Getting Started
+
 To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux):
 ```shell
 $ pip install --upgrade dtn7zero
 ```
 The most simple example on what you can do:
 ```python
 import time
@@ -29,66 +42,71 @@
 
 node_endpoint.send(b'hello world', "dtn://node1/")
 
 time.sleep(1)
 ```
 Further examples for the 'simple' API can be found under `./examples` in the GitHub repository.
 
-For a deeper dive into the underlying concepts and the fully fletched dtn implementation, take a look at the 
-`dtn7zero.api` module implementation and the tests under `./tests`.
+For a deeper dive into the underlying concepts and the full-fledged dtn implementation, take a look at the 
+`dtn7zero.api` module implementation and the tests under `./test`.
 
 ## MicroPython Installation Guide
+Installation has been successfully tested on Windows and Linux (x86_64 and arm64). The required
+[mpy-cross](https://pypi.org/project/mpy-cross/) has been shown to have installation issues on Mac M1s
+under Mac OS X and may have to be built and installed manually.
+
 This whole project was tested on an ESP32 (GENERIC) and this installation guide is tailored for the ESP32.
 If you plan to use another microcontroller you might need to do adjustments 
 (most certainly the MicroPython installation, and the MPY_MARCH in esp-deployment.py).
 
 Important note for linux: it may be that mpremote assumes another USB device with higher priority than the ESP32.
 In that case all mpremote commands (especially inside esp-deployment.py) will fail as no communication is possible.
 Check all USB devices mpremote considers in priority order with `mpremote devs`.
 
 ### First Time MicroPython Installation For ESP32 (GENERIC)
 1. download the newest [firmware](https://micropython.org/download/esp32/)
 2. install the esp flash tool: `pip install esptool`
 3. connect your ESP32 via USB and start a terminal at the location of the downloaded firmware
-4. start the following command (with the correct USB port), then hold **boot** until it starts erasing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 erase_flash`
-5. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
+4. start the following command (with the correct USB port): \
+`esptool --chip esp32 --port /dev/ttyUSB0 erase_flash` (you may have to invoke esptool with `esptool.py --chip ...` here and subsequently, you may also have hold **boot** to enter the bootloader on the ESP32)
+5. start the following command (with the correct USB port and firmware name): \
+`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin` (you may have hold **boot** again to enter the bootloader on the ESP32)
 6. done, you may now connect to it via: `mpremote` (installation via pip: `pip install mpremote`)
 
 ### Update To New MicroPython Version
 1. download the newest [firmware](https://micropython.org/download/esp32/)
-2. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
+2. start the following command (with the correct USB port and firmware name): \
+`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin` (you may have hold **boot** to enter the bootloader on the ESP32)
 3. done
 
 ### First Time dtn7zero Deployment
 1. make sure you check out the repository and the submodules (especially py-dtn7)
 2. install the mpremote tool: `pip install mpremote`
-3. install the mpy-cross compiler tool: `pip install mpy-cross`
+3. install the mpy-cross compiler tool: `pip install mpy-cross` (this may not work on Mac M1s under Mac OS X) 
 4. populate wlan.json with an appropriate hostname and at least one ssid -> password mapping
 5. check your connection to the ESP32 with: `mpremote`
 6. copy wlan.json to your ESP32: `mpremote fs cp wlan.json :wlan.json`
 7. copy boot.py to your ESP32: `mpremote fs cp boot.py :boot.py`
 8. deploy the dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
-9. done
+9. install required packages: `mpremote mip install urequests` and `mpremote mip install datetime`
+10. done
 
 ### Continuous dtn7zero Deployment
 1. check your connection to the ESP32 with: `mpremote`
 2. deploy the changes of dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
 3. done
 
 ### First dtn7zero Functionality Check On MicroPython
 1. you may check that wlan is connecting correctly (connect via `mpremote` and press **enable** for a soft reset)
 2. you may also check that you can import dtn7zero (connect via `mpremote` and `import dtn7zero`)
 3. you can also check that everything works (run the test script `mpremote run examples/local_ping_echo.py`)
 
 ### Additional MicroPython Tips & Tricks
 The mpremote tool is normally interrupted by using `ctrl+c`. A special case is the REPL (simply call `mpremote`), which
-can be exited by using `ctrl+~` (tested on windows).
+can be exited by using `ctrl+~` (tested on Windows) or `ctrl+]` (Linux).
 
 If you start a script on MicroPython (`mpremote run ...`) and disconnect the console (`mpremote` -> `ctrl+c`) then the script 
 keeps running.
 
 If you must access the REPL via mpremote, but a script is blocking, then call `mpremote` and press EN (enable) on the 
 ESP32 for a soft-reset. Press `ctrl+c` a few times to interrupt the `boot.py` or `main.py` script execution. The session
 state is stored, so any subsequent `mpremote` call will start at REPL as long as no power disconnect is performed.
@@ -96,17 +114,17 @@
 You can deploy a script as `main.py` on MicroPython to be run every time the microcontroller gets power. \
 You can also remove the script. MicroPython will only execute the script if it is present.
 ```shell
 $ mpremote fs cp examples/remote_echo_callback.py :main.py
 $ mpremote fs rm :main.py
 ```
 
-Regarding `boot.py`, it is used for user-specific setup code and this framework uses a generic boot script that adjusts
+Regarding `boot.py`: it is used for user-specific setup code and this framework uses a generic boot script that adjusts
 the ESP32's frequency and connects to a Wi-Fi network (blocking until success). MicroPython will create a dummy `boot.py`
-if none is present. MicroPython will not create a dummy `main.py` is none is present. MicroPython will first execute
+if none is present. MicroPython will not create a dummy `main.py` if none is present. MicroPython will first execute
 the `boot.py` and then the `main.py` if it is present.
 
 
 ## Development Information
 
 ### Development Mode
 You can install this project locally to directly reflect code changes in your environment.
```

### Comparing `dtn7zero-0.0.6/dtn7zero/api.py` & `dtn7zero-0.0.7/dtn7zero/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Provides a simple NDN (named data network) interface on top of DTN7.
 """
 import time
 
 from typing import Optional, List, Tuple, Callable
 
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP, RUNNING_MICROPYTHON
+from dtn7zero.configuration import CONFIGURATION, RUNNING_MICROPYTHON
 from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
 from dtn7zero.data import Node
 from dtn7zero.endpoints import LocalEndpoint, LocalGroupEndpoint
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
 from py_dtn7.bundle import Bundle, PrimaryBlock
@@ -104,16 +104,16 @@
     """
     global BPA
 
     if BPA is not None:
         raise Exception('setup(node_id) was called twice!')
 
     storage = SimpleInMemoryStorage()
-    router = SimpleEpidemicRouter({IPND_IDENTIFIER_MTCP: MTcpCLA()}, storage)
-    BPA = BundleProtocolAgent(full_node_uri, storage, router, use_ipnd=True)
+    router = SimpleEpidemicRouter({CONFIGURATION.IPND.IDENTIFIER_MTCP: MTcpCLA()}, storage)
+    BPA = BundleProtocolAgent(full_node_uri, storage, router)
 
     # node specific endpoint works like a normal endpoint (only receives exactly matched bundles), but for the node itself
     endpoint = SimpleEndpoint('', node_receive_callback)
     BPA.register_endpoint(endpoint._endpoint)
 
     return endpoint
 
@@ -193,15 +193,15 @@
 
     if BPA is None:
         raise Exception('setup(node_id was not called!')
 
     BPA.update()
 
 
-def run_forever(loop_callback=None, loop_callback_interval_milliseconds=1000, _sleep_time_seconds=0):
+def run_forever(loop_callback=None, loop_callback_interval_milliseconds=1000, sleep_time_milliseconds=10):
     """ update loop to run the bundle protocol agent until KeyboardInterrupt
 
     custom_logic_callback can be used for application specific logic after the bundle protocol agent was started
 
     custom_logic_callback signature:
 
     callback() -> None:
@@ -218,20 +218,23 @@
         while True:
             BPA.update()
 
             if loop_callback is not None and is_timestamp_older_than_timeout(last_callback_execution, loop_callback_interval_milliseconds):
                 last_callback_execution = get_current_clock_millis()
                 loop_callback()
 
-            time.sleep(_sleep_time_seconds)
+            if RUNNING_MICROPYTHON:
+                time.sleep_ms(sleep_time_milliseconds)
+            else:
+                time.sleep(sleep_time_milliseconds / 1000.0)
     except KeyboardInterrupt:
         pass
 
 
-def start_background_update_thread(_sleep_time_seconds=0):
+def start_background_update_thread(sleep_time_milliseconds=10):
     """ (experimental) background update thread
 
     On MicroPython the limited RAM can lead to crashes (most prominently a maximum-recursion-depth RuntimeError).
     The _thread.stack_size(...) can be adjusted for compensation if needed and possible.
     """
     global BPA
     global BPA_THREAD
@@ -244,18 +247,18 @@
 
     if RUNNING_MICROPYTHON:
         _thread.stack_size(11500)  # experimental setting: 7000 does not run, 8000 does run, 11500 picked for leeway
 
         def update_runner():
             while True:
                 BPA.update()
-                time.sleep(_sleep_time_seconds)
+                time.sleep_ms(sleep_time_milliseconds)
 
         BPA_THREAD = _thread.start_new_thread(update_runner, ())
     else:
         def self_stopping_update_runner():
             while threading.main_thread().is_alive():
                 BPA.update()
-                time.sleep(_sleep_time_seconds)
+                time.sleep(sleep_time_milliseconds / 1000.0)
 
         BPA_THREAD = threading.Thread(target=self_stopping_update_runner)
         BPA_THREAD.start()
```

### Comparing `dtn7zero-0.0.6/dtn7zero/bundle_protocol_agent.py` & `dtn7zero-0.0.7/dtn7zero/bundle_protocol_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from datetime import datetime, timezone, timedelta
 from typing import Dict, List
 
 from dtn7zero.data import BundleInformation, BundleStatusReportReasonCodes
-from dtn7zero.constants import SEND_STATUS_REPORTS_ENABLED, RUNNING_MICROPYTHON
+from dtn7zero.configuration import CONFIGURATION, RUNNING_MICROPYTHON
 from dtn7zero.endpoints import LocalEndpoint, LocalGroupEndpoint, _LocalEndpoint
 from dtn7zero.ipnd import IPND
 from dtn7zero.routers import Router
 from dtn7zero.storage import Storage
 from dtn7zero.utility import debug, is_correct_node_uri, is_correct_endpoint_uri, is_correct_group_uri
 from py_dtn7.bundle import PrimaryBlock
 
 if RUNNING_MICROPYTHON:
     from wlan import connect, isconnected
 
 
 class BundleProtocolAgent:
 
-    def __init__(self, full_node_uri: str, storage: Storage, router: Router, use_ipnd=True):
+    def __init__(self, full_node_uri: str, storage: Storage, router: Router):
         """ The main RFC 9171 compliant bpa component.
 
         full_node_uri examples:
             dtn addressing scheme -> "dtn://node1/", "dtn://cool-node/"  # '/' at the end is mandatory
             ipn addressing scheme -> "ipn://12", "ipn://24.25"  # will be joined with the endpoints via '.'
         """
         assert is_correct_node_uri(full_node_uri)
@@ -30,31 +30,28 @@
         self.router = router
         self.local_registered_endpoints: Dict[str, List[_LocalEndpoint]] = {}
 
         self.local_bundle_dispatch_queue: List[BundleInformation] = []  # this pipeline-stage is needed to prevent infinite-recursion if two local endpoints answer each other on every reception-callback
         self.storage_retry_generator = None
         self.router_poll_generator = None
 
-        self.use_ipnd = use_ipnd
-        if self.use_ipnd:
-            # on micropython we need to handle wireless connections manually
-            if RUNNING_MICROPYTHON and not isconnected():
-                connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
+        # on micropython we need to handle wireless connections manually
+        if RUNNING_MICROPYTHON and not isconnected():
+            connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
 
-            scheme_encoded, node_encoded = PrimaryBlock.from_full_uri(full_node_uri)
-            self.ipnd = IPND(scheme_encoded, node_encoded, storage)
+        scheme_encoded, node_encoded = PrimaryBlock.from_full_uri(full_node_uri)
+        self.ipnd = IPND(scheme_encoded, node_encoded, storage)
 
     def update(self):
         # on micropython we need to handle wireless connections manually
         if RUNNING_MICROPYTHON and not isconnected():
             connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
 
         # update discovery
-        if self.use_ipnd:
-            self.ipnd.update()
+        self.ipnd.update()
 
         # process stored/delayed bundle
         if self.storage_retry_generator is None:
             self.storage_retry_generator = self.storage.get_bundles_to_retry()
 
         try:
             self.bundle_dispatching(next(self.storage_retry_generator))
@@ -186,15 +183,15 @@
         * If the block processing control flags in that block neither indicate that the bundle must be deleted nor 
         indicate that the block must be discarded, then processing continues with the next extension block that the 
         BPA cannot process, if any; otherwise, processing proceeds from Step 5. […]
         """
         for block in bundle.other_blocks[:]:
             flags = block.block_processing_control_flags
 
-            if flags.report_status_if_block_cant_be_processed and SEND_STATUS_REPORTS_ENABLED:
+            if flags.report_status_if_block_cant_be_processed and CONFIGURATION.SEND_STATUS_REPORTS_ENABLED:
                 # todo: generate a status report
                 pass
 
             if flags.delete_bundle_if_block_cant_be_processed:
                 self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.BLOCK_UNSUPPORTED)
                 return
             elif flags.discard_block_if_block_cant_be_processed:
@@ -285,15 +282,16 @@
             """ RFC 9171, 5.4.1 Forwarding Contraindicated
             […] Step 1: The BPA MUST determine whether or not to declare failure in forwarding the bundle. 
             Note: This decision is likely to be influenced by the reason for which forwarding is contraindicated. […]
             """
             no_failure_codes = (
                 BundleStatusReportReasonCodes.NO_KNOWN_ROUTE_TO_DESTINATION_FROM_HERE,
                 BundleStatusReportReasonCodes.NO_TIMELY_CONTACT_WITH_NEXT_NODE_ON_ROUTE,
-                BundleStatusReportReasonCodes.TRAFFIC_PARED
+                BundleStatusReportReasonCodes.TRAFFIC_PARED,
+                BundleStatusReportReasonCodes.FORWARDED_OVER_UNIDIRECTIONAL_LINK
             )
 
             if reason in no_failure_codes:
                 """ RFC 9171, 5.4.1 Forwarding Contraindicated
                 […] when -- at some future time -- the forwarding of this bundle ceases to be contraindicated, 
                 processing proceeds from Step 4 of Section 5.4. […]
                 """
@@ -357,15 +355,15 @@
     def bundle_deletion(self, bundle_information: BundleInformation, reason: int):
         """ RFC 9171, 5.10 Bundle Deletion
         […] Step 1: If the "request reporting of bundle deletion" flag in the bundle's status report request field is
         set to 1 and if status reporting is enabled, then a bundle deletion status report citing the reason for
         deletion SHOULD be generated, destined for the bundle's report-to endpoint ID. […]
         """
         flags = bundle_information.bundle.primary_block.bundle_processing_control_flags
-        if flags.status_of_report_deletion_is_requested and SEND_STATUS_REPORTS_ENABLED:
+        if flags.status_of_report_deletion_is_requested and CONFIGURATION.SEND_STATUS_REPORTS_ENABLED:
             # todo: generate a status report
             pass
 
         """ RFC 9171, 5.10 Bundle Deletion
         […] Step 2: All of the bundle's retention constraints MUST be removed.
         """
         bundle_information.retention_constraint = None
```

### Comparing `dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/__init__.py` & `dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from abc import ABC
 from typing import Optional, List, Tuple
 
 from dtn7zero.data import Node
 from py_dtn7 import Bundle
 
 
-class CLA(ABC):
+class PullBasedCLA(ABC):
 
-    def poll(self, bundle_id: str = None, node: Node = None) -> Tuple[Optional[Bundle], Optional[str]]:
+    def poll(self, bundle_id: str, node: Node) -> Tuple[Optional[Bundle], Optional[str]]:
         raise NotImplementedError('do not instantiate CLA class directly')
 
     def poll_ids(self, node: Node) -> Optional[List[str]]:
         raise NotImplementedError('do not instantiate CLA class directly')
 
     def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
         raise NotImplementedError('do not instantiate CLA class directly')
+
+
+class PushBasedCLA(ABC):
+    def poll(self) -> Tuple[Optional[Bundle], Optional[str]]:
+        raise NotImplementedError('do not instantiate CLA class directly')
+
+    def send_to(self, node: Optional[Node], serialized_bundle: bytes) -> bool:
+        raise NotImplementedError('do not instantiate CLA class directly')
+
```

### Comparing `dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py` & `dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from typing import Dict, List, Optional, Tuple
 
-from dtn7zero.convergence_layer_adapters import CLA
+from dtn7zero.convergence_layer_adapters import PullBasedCLA
 from dtn7zero.data import Node
 from dtn7zero.utility import debug, warning
 
 try:
     import requests
 except ImportError:
     import urequests as requests
 
 from py_dtn7 import DTNRESTClient, Bundle
 
-from dtn7zero.constants import IPND_IDENTIFIER_REST
+from dtn7zero.configuration import CONFIGURATION
 
 
-class Dtn7RsRestCLA(CLA):
+class Dtn7RsRestCLA(PullBasedCLA):
 
     def __init__(self):
         self.connections: Dict[Node, DTNRESTClient] = {}
 
     def add_connection(self, node: Node):
         http_address = 'http://{}'.format(node.address)
-        port = node.clas[IPND_IDENTIFIER_REST]
+        port = node.clas[CONFIGURATION.IPND.IDENTIFIER_REST]
         try:
             # we assume if there is a dtn7rs-like HTTP-API present, then we can proceed
             dtn7rs_rest_client = DTNRESTClient(host=http_address, port=port)
         except OSError as e:  # urequests only uses default exceptions
             warning('could not add node: {}:{} error: {}'.format(http_address, port, e))
             return
 
         self.connections[node] = dtn7rs_rest_client
         node.eid = (1, self.connections[node].node_id)  # todo: remove hardcoded dtn uri scheme assignment
         debug('added new rest cla connection: {} {}'.format(node.eid, http_address))
 
-    def poll(self, bundle_id: str = None, node: Node = None) -> Tuple[Optional[Bundle], Optional[str]]:
+    def poll(self, bundle_id: str, node: Node) -> Tuple[Optional[Bundle], Optional[str]]:
         if bundle_id is None or node is None:
             return None, None
 
         if node not in self.connections:
             return None, None
 
         try:
@@ -59,15 +59,15 @@
         try:
             return self.connections[node].bundles
         except (OSError, ValueError):  # urequests only uses default exceptions
             del self.connections[node]
         return None
 
     def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
-        if IPND_IDENTIFIER_REST not in node.clas:
+        if CONFIGURATION.IPND.IDENTIFIER_REST not in node.clas:
             return False
 
         if node not in self.connections:
             # try to establish a new node connection, todo: what to do on repeated failures (slowing the framework down)?
             self.add_connection(node)
 
         try:
```

### Comparing `dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/mtcp.py` & `dtn7zero-0.0.7/dtn7zero/convergence_layer_adapters/mtcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import socket
 import struct
-from typing import Optional, Dict, List, Tuple
+from typing import Optional, Dict, Tuple
 
 try:
     from cbor2 import dumps
 except ImportError:
     from cbor import dumps
 
-from dtn7zero.constants import PORT_MTCP, MTCP_MAX_CONNECTIONS_STATE_WAITING, SOCKET_RECEIVE_BUFFER_SIZE, \
-    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE, MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE, \
-    MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND, RUNNING_MICROPYTHON, IPND_IDENTIFIER_MTCP
-from dtn7zero.convergence_layer_adapters import CLA
+from dtn7zero.configuration import CONFIGURATION, RUNNING_MICROPYTHON
+from dtn7zero.convergence_layer_adapters import PushBasedCLA
 from dtn7zero.data import Node
 from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout, debug, warning
 from py_dtn7 import Bundle
 
 
 TYPE_BYTES = 0x40
 
@@ -56,15 +54,15 @@
 
 
 def _receive_exactly_n_bytes(connection, num_bytes):
     result = b''
 
     while True:
         try:
-            buf = connection.recv(min(num_bytes, SOCKET_RECEIVE_BUFFER_SIZE))
+            buf = connection.recv(min(num_bytes, CONFIGURATION.SOCKET_RECEIVE_BUFFER_SIZE))
         # if a non-blocking read fails we have read everything there is to read at the moment
         # ,but we need to read exactly n bytes
         except OSError:
             pass
         else:
             # on 0 bytes received the socket connection is closed
             # the desired num_bytes could not be received in total -> incomplete data -> discard
@@ -137,15 +135,15 @@
     try:
         client_socket.connect((address, port))
     except OSError:
         # this will raise an exception on non-blocking sockets
         pass
 
     deadlock_check = get_current_clock_millis()
-    while len(message) > 0 and not is_timestamp_older_than_timeout(deadlock_check, MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND):
+    while len(message) > 0 and not is_timestamp_older_than_timeout(deadlock_check, CONFIGURATION.MTCP.TIMEOUT_MILLISECONDS_STALLED_SEND):
         try:
             bytes_sent = client_socket.send(message)
         # Windows behaviour??? If other end is forcibly closed it raises an ConnectionResetError -> OSError
         except OSError:
             # We ignore all OSErrors.
             # The correct way would be to check the errno for "busy" (MicroPython -> 11, CPython+Windows -> 10035)
             # but, because it is implementation dependent, and we do not expect the receiver to immediately close the
@@ -164,27 +162,27 @@
     if len(message) > 0:
         client_socket.close()
         raise RemoteStalledConnectionException()
 
     client_socket.close()
 
 
-class MTcpCLA(CLA):
+class MTcpCLA(PushBasedCLA):
 
     def __init__(self):
         # a standard ipv4 stream socket
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         # allow immediate rebind to a floating socket (last app crashed or otherwise non fully closed server socket)
         self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         # bind to all interfaces available
-        self.socket.bind(('0.0.0.0', PORT_MTCP))
+        self.socket.bind(('0.0.0.0', CONFIGURATION.PORT.MTCP))
         # We will accept a maximum of x connect requests into our connect queue before we are busy
         # A connection gets out of this queue on socket creation
-        self.socket.listen(MTCP_MAX_CONNECTIONS_STATE_WAITING)
+        self.socket.listen(CONFIGURATION.MTCP.MAX_CONNECTIONS_STATE_WAITING)
         # change to non-blocking mode
         # MicroPython supports only one thread/process, and therefore we need to implement everything synchronous
         self.socket.settimeout(0)
 
         self.open_receive_connections: Dict[str, (socket.socket, int)] = {}
         self.gracefully_shutdown_connections: Dict[str, socket.socket] = {}
 
@@ -229,15 +227,15 @@
                 connection.close()
                 del self.open_receive_connections[address_tuple]
             else:
                 if serialized_bundle is not None:
                     from_node_address = address_tuple[0]
                     self.open_receive_connections[address_tuple] = (connection, get_current_clock_millis())
                     break
-                elif is_timestamp_older_than_timeout(last_received, MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE):
+                elif is_timestamp_older_than_timeout(last_received, CONFIGURATION.MTCP.TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE):
                     if not RUNNING_MICROPYTHON:
                         debug('gracefully closing incoming mtcp connection {} due to inactivity timeout'.format(address_tuple))
                         connection.shutdown(socket.SHUT_WR)
                         self.gracefully_shutdown_connections[address_tuple] = connection
                     else:
                         debug('forcefully closing incoming mtcp connection {} due to inactivity timeout (no shutdown support on micropython)'.format(address_tuple))
                         connection.close()
@@ -263,15 +261,15 @@
                 if serialized_bundle is not None:
                     from_node_address = address_tuple[0]
                     break
 
         return serialized_bundle, from_node_address
 
     def _check_for_new_connections(self):
-        if len(self.open_receive_connections) < MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE:
+        if len(self.open_receive_connections) < CONFIGURATION.MTCP.MAX_CONNECTIONS_STATE_OPEN_RECEIVE:
             try:
                 client_socket, address_tuple = self.socket.accept()
             except OSError:
                 # no new connect request waiting
                 pass
             else:
                 # change to non-blocking mode to be able to poll without blocking
@@ -280,22 +278,22 @@
                 # we allow multiple connections from one IP address, because if we accept the connection, the whole bundle
                 #  could be already transmitted before we can close the connection from our checks
                 #  -> would lead to false positive on the sender side
                 # next best thing: limit number of open-receive-connections
                 # print('new mtcp receive connection opened from address {}'.format(address_tuple))
                 self.open_receive_connections[address_tuple] = (client_socket, get_current_clock_millis())
 
-    def poll_ids(self, node: Node) -> Optional[List[str]]:
-        return None  # we cannot poll ids, and None signals that
+    def send_to(self, node: Optional[Node], serialized_bundle: bytes) -> bool:
+        if node is None:
+            raise Exception('cannot send bundle to unspecified node with mtcp cla')
 
-    def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
         message = dumps(serialized_bundle)
 
-        if IPND_IDENTIFIER_MTCP in node.clas:
+        if CONFIGURATION.IPND.IDENTIFIER_MTCP in node.clas:
             try:
-                port = node.clas[IPND_IDENTIFIER_MTCP]
+                port = node.clas[CONFIGURATION.IPND.IDENTIFIER_MTCP]
                 _send_message(node.address, port, message)
             except (RemoteClosedConnectionException, RemoteStalledConnectionException):
-                del node.clas[IPND_IDENTIFIER_MTCP]  # the node can re-announce it, but currently we cannot connect
+                del node.clas[CONFIGURATION.IPND.IDENTIFIER_MTCP]  # the node can re-announce it, but currently we cannot connect
                 return False
             return True
         return False
```

### Comparing `dtn7zero-0.0.6/dtn7zero/data.py` & `dtn7zero-0.0.7/dtn7zero/data.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.6/dtn7zero/endpoints.py` & `dtn7zero-0.0.7/dtn7zero/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable
 
-from dtn7zero.constants import RUNNING_MICROPYTHON, PORT_REST
+from dtn7zero.configuration import RUNNING_MICROPYTHON, CONFIGURATION
 from dtn7zero.data import BundleInformation
 from dtn7zero.utility import debug
 from py_dtn7 import Bundle, DTNRESTClient, to_dtn_timestamp
 from py_dtn7.bundle import BundleProcessingControlFlags, PrimaryBlock, HopCountBlock, PayloadBlock, BundleAgeBlock, \
     NONE_ENDPOINT_SPECIFIC_PART_NAME, URI_SCHEME_DTN_NAME
 
 
@@ -155,15 +155,15 @@
         """
         This is a relic of a time when we could not generate bundles on our own.
 
         It is functional and encapsulated, meaning it requires no other dtn7zero dependencies to operate.
         """
         self.endpoint_identifier = endpoint_identifier
 
-        self.dtn_rest_client: DTNRESTClient = DTNRESTClient('http://{}'.format(dtn7rs_ip), PORT_REST)
+        self.dtn_rest_client: DTNRESTClient = DTNRESTClient('http://{}'.format(dtn7rs_ip), CONFIGURATION.PORT.REST)
 
         self.dtn_rest_client.register(self.endpoint_identifier)
 
     def __del__(self):
         self.dtn_rest_client.unregister(self.endpoint_identifier)
 
     @property
```

### Comparing `dtn7zero-0.0.6/dtn7zero/ipnd.py` & `dtn7zero-0.0.7/dtn7zero/ipnd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import socket
 from typing import Tuple, Optional, List, Dict
 
-from dtn7zero.constants import RUNNING_MICROPYTHON, IPND_IDENTIFIER_MTCP, PORT_MTCP, PORT_IPND, IPND_SEND_INTERVAL_MILLISECONDS, IPND_BEACON_MAX_SIZE
+from dtn7zero.configuration import RUNNING_MICROPYTHON, CONFIGURATION
 from dtn7zero.data import Node
 from dtn7zero.storage import Storage
-from dtn7zero.utility import is_timestamp_older_than_timeout, get_current_clock_millis, debug, warning, \
-    build_broadcast_ipv4_address
+from dtn7zero.utility import is_timestamp_older_than_timeout, get_current_clock_millis, debug, warning, build_broadcast_ipv4_address
 from py_dtn7.bundle import Flags
 
 if RUNNING_MICROPYTHON:
     import wlan
 else:
     import netifaces
 
@@ -168,49 +167,63 @@
         return self.beacon_sequence_number == old_beacon_sequence_number
 
 
 class IPND:
 
     """
     for now, we only support broadcast on all interfaces and IPv4 only.
-    todo: extend functionality to filter network interfaces and support IPv6
+    todo: extend functionality to support IPv6
     todo: extend functionality to delete nodes after a beacon timeout
     """
     def __init__(self, eid_scheme: int, eid_specific_part: str, storage: Storage):
         self.storage = storage
 
         # todo: check dynamically for new networks -> also test with changing networks
         if RUNNING_MICROPYTHON:
             self.broadcast_addresses, self.own_addresses = IPND.get_micropython_ipv4_broadcast_addresses()
         else:
             self.broadcast_addresses, self.own_addresses = IPND.get_cpython_ipv4_broadcast_addresses()
 
+        debug("IPND SETUP: own addresses in use: {}".format(self.own_addresses))
+        debug("IPND SETUP: broadcast addresses in use: {}".format(self.broadcast_addresses))
+
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 
         if not RUNNING_MICROPYTHON:
             self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.settimeout(0)
 
-        self.sock.bind(('', 3003))
+        # todo: is there a valid case in enabling IPND dynamically? If so, this case needs to be handled
+        if CONFIGURATION.IPND.ENABLED:
+            self._was_enabled_once = True
+            self.sock.bind(('', 3003))
+        else:
+            self._was_enabled_once = False
 
         # self.own_beacon = create_minimal_output_beacon(eid_scheme, eid_specific_part)
         self.own_beacon = Beacon.from_objects(
             beacon_sequence_number=0,
             eid_scheme=eid_scheme,
             eid_specific_part=eid_specific_part,
-            service_block=([(IPND_IDENTIFIER_MTCP, PORT_MTCP)], {})  # todo: extend for all and active clas'
+            service_block=([(CONFIGURATION.IPND.IDENTIFIER_MTCP, CONFIGURATION.PORT.MTCP)], {})  # todo: extend for all and active clas'
         )
 
         self.last_beacon_broadcast = 0
 
     def update(self):
+        if not CONFIGURATION.IPND.ENABLED:
+            return
+        elif not self._was_enabled_once:
+            self._was_enabled_once = True
+            self.sock.bind(('', 3003))
+
         try:
             # todo: for now it seems one full datagram is returned here, as long as the datagram is smaller than bytes-trying-to-receive
-            raw_data, (address, port) = self.sock.recvfrom(IPND_BEACON_MAX_SIZE)
+            raw_data, (address, port) = self.sock.recvfrom(CONFIGURATION.IPND.BEACON_MAX_SIZE)
         except OSError:
             pass
         except MemoryError:
             warning('MEMORY ERROR DURING BEACON RECEIVE, PASS')
         else:
             try:
                 # eid_scheme, eid_specific_part, clas, services = extract_beacon_information_from(raw_data)
@@ -218,22 +231,22 @@
             except Exception as e:
                 warning('could not decode beacon. error: {}'.format(e))
             else:
                 if address not in self.own_addresses:
                     existing_node = self.storage.get_node(address)
 
                     if existing_node is None:
-                        debug('received beacon from new node: {}, size: {}'.format(address, len(raw_data)))
+                        debug('received beacon from new node: {}, {}'.format(address, beacon))
 
                         new_node = Node(address, (beacon.eid_scheme, beacon.eid_specific_part), dict(beacon.service_block[0]), beacon.beacon_sequence_number)
                         self.storage.add_node(new_node)
 
                         sequence_number_matches = False
                     else:
-                        debug('received beacon from known node: {}, size: {}'.format(address, len(raw_data)))
+                        debug('received beacon from known node: {}, {}'.format(address, beacon))
                         # existing_node.merge_new_info(eid_scheme, eid_specific_part, dict(clas))
                         existing_node.merge_new_info(beacon.eid_scheme, beacon.eid_specific_part, dict(beacon.service_block[0]))
 
                         sequence_number_matches = existing_node.advance_sequence_number(beacon.beacon_sequence_number)
 
                     if not sequence_number_matches:
                         # send back a uni-cast beacon to a previously unknown node for faster knowledge spread
@@ -242,44 +255,56 @@
                         # dtn7zero specific detail: we add unicast information to the beacon, so there is no second unicast beacon sent back to us
 
                         if not (42 in beacon.service_block[1] and beacon.service_block[1][42] == b'unicast'):
                             self.own_beacon.service_block[1][42] = b'unicast'
                             self.send_own_beacon_to(address)
                             del self.own_beacon.service_block[1][42]
 
-        if is_timestamp_older_than_timeout(self.last_beacon_broadcast, IPND_SEND_INTERVAL_MILLISECONDS):
+        if is_timestamp_older_than_timeout(self.last_beacon_broadcast, CONFIGURATION.IPND.SEND_INTERVAL_MILLISECONDS):
+            # Increase before sending because it might happen that a unicast-reply with that number was already sent
+            self.own_beacon.increment_beacon_sequence_number_by_one()
             for address in self.broadcast_addresses:
                 self.send_own_beacon_to(address)
-            # minimal_output_beacon_increase_counter_by_one(self.own_beacon)
-            self.own_beacon.increment_beacon_sequence_number_by_one()
             self.last_beacon_broadcast = get_current_clock_millis()
 
     def send_own_beacon_to(self, address: str):
         message = self.own_beacon.to_cbor()
 
         while len(message) > 0:
-            sent_bytes = self.sock.sendto(message, (address, PORT_IPND))
+            sent_bytes = self.sock.sendto(message, (address, CONFIGURATION.PORT.IPND))
             message = message[sent_bytes:]
 
     @staticmethod
     def get_micropython_ipv4_broadcast_addresses() -> (list, list):
+        if CONFIGURATION.IPND.INTERFACE_WHITELIST:
+            raise Exception("IPND interface whitelist is not supported on Micropython, list: {}".format(CONFIGURATION.IPND.INTERFACE_WHITELIST))
+
         address, subnet, _, _ = wlan.ifconfig()
 
         if address == '0.0.0.0':
             warning('wlan is not connected, cannot form broadcast address')
             return []
 
         return [build_broadcast_ipv4_address(address, subnet)], [address]
 
     @staticmethod
     def get_cpython_ipv4_broadcast_addresses() -> (list, list):
         broadcast_addresses = []
         own_addresses = []
 
+        # check that all interface names in the whitelist are valid
+        for interface in CONFIGURATION.IPND.INTERFACE_WHITELIST:
+            if interface not in netifaces.interfaces():
+                raise Exception("IPND INTERFACE_WHITELIST contains non-existent interface: {}".format(interface))
+
         for interface in netifaces.interfaces():
+            # no whitelist -> all enabled; whitelist -> skip interfaces that are not in the list
+            if CONFIGURATION.IPND.INTERFACE_WHITELIST and interface not in CONFIGURATION.IPND.INTERFACE_WHITELIST:
+                continue
+
             interface_information = netifaces.ifaddresses(interface).get(netifaces.AF_INET, [])
 
             for address_information in interface_information:
                 address = address_information['addr']
                 netmask = address_information['netmask']
 
                 # in case 'peer' exists => on linux 'lo' interface there is no 'broadcast', only 'peer', but 'netmask' exists
```

### Comparing `dtn7zero-0.0.6/dtn7zero/routers/__init__.py` & `dtn7zero-0.0.7/dtn7zero/routers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 from abc import ABC
 from typing import Iterable
 
-from dtn7zero.constants import ATTACH_PREVIOUS_NODE_BLOCK
+from dtn7zero.configuration import CONFIGURATION
 from dtn7zero.data import BundleInformation
 from py_dtn7 import Bundle
 from py_dtn7.bundle import PreviousNodeBlock, BlockProcessingControlFlags
 
 
 class Router(ABC):
 
@@ -30,15 +30,15 @@
 
         # copy bundle to not alter the storage instance
         bundle = Bundle.from_cbor(bundle_information.bundle.to_cbor())
 
         if bundle.previous_node_block:
             bundle.remove_block(bundle.previous_node_block)
 
-        if ATTACH_PREVIOUS_NODE_BLOCK:
+        if CONFIGURATION.ATTACH_PREVIOUS_NODE_BLOCK:
             flags = BlockProcessingControlFlags(0)
             flags.set_flag(4)  # discard block if block cant be processed
 
             previous_node_block = PreviousNodeBlock.from_objects(full_node_uri, flags)
 
             bundle.insert_canonical_block(previous_node_block)
```

### Comparing `dtn7zero-0.0.6/dtn7zero/storage/__init__.py` & `dtn7zero-0.0.7/dtn7zero/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.6/dtn7zero/storage/simple_in_memory_storage.py` & `dtn7zero-0.0.7/dtn7zero/storage/simple_in_memory_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Tuple, List, Optional, Iterable
 
-from dtn7zero.constants import SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES, SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS
+from dtn7zero.configuration import CONFIGURATION
 from dtn7zero.data import BundleInformation, Node
 from dtn7zero.storage import Storage
 from dtn7zero.utility import get_oldest_bundle, get_oldest_bundle_id
 
 
 class SimpleInMemoryStorage(Storage):
 
@@ -28,31 +28,31 @@
     def was_seen(self, bundle_id: str) -> bool:
         return bundle_id in self.bundle_ids
 
     def store_seen(self, bundle_id: str, node_address):
         if node_address is None and self.bundle_ids.get(bundle_id, None) is not None:
             return  # we do not want to overwrite a valid node with None from an unknown source
 
-        if len(self.bundle_ids) >= SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS:
+        if len(self.bundle_ids) >= CONFIGURATION.SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS:
             del self.bundle_ids[get_oldest_bundle_id(self.bundle_ids)]
         self.bundle_ids[bundle_id] = node_address
 
     def remove_bundle(self, bundle_id: str) -> bool:
         return self.bundles.pop(bundle_id, False)  # if the bundle exists it is 'truthy'
 
     def delay_bundle(self, bundle_information: BundleInformation) -> Tuple[bool, List[BundleInformation]]:
         removed_bundles = []
 
         if bundle_information.bundle.bundle_id in self.bundles:
             return True, removed_bundles
 
-        if len(self.bundles) >= SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
+        if len(self.bundles) >= CONFIGURATION.SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
             self.garbage_collect()
 
-        if len(self.bundles) >= SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
+        if len(self.bundles) >= CONFIGURATION.SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
             oldest_bundle = self.bundles.pop(get_oldest_bundle(self.bundles.values()).bundle.bundle_id)
             removed_bundles.append(oldest_bundle)
 
         self.store_seen(bundle_information.bundle.bundle_id, None)
 
         self.bundles[bundle_information.bundle.bundle_id] = bundle_information
```

### Comparing `dtn7zero-0.0.6/dtn7zero/utility.py` & `dtn7zero-0.0.7/dtn7zero/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 import re
 from typing import Iterable
 
-from dtn7zero.constants import DEBUG, WARNING
+from dtn7zero.configuration import CONFIGURATION
 
 NODE_URI_REGEX = re.compile(r'(^dtn://[^~/]+/$)|(^ipn://\d+(\.\d+)*$)')
 ENDPOINT_URI_REGEX = re.compile(r'(^dtn://none$)|(^dtn://[^~/]+/([^~/]+/)*[^~/]+$)|(^ipn://\d+(\.\d+)+$)')
 GROUP_URI_REGEX = re.compile(r'^dtn://[^~/]+/([^~]+/)*~[^/]+$')
 
 
 def get_oldest_bundle_id(bundle_ids: Iterable[str]):
@@ -67,20 +67,20 @@
 
 
 def is_timestamp_older_than_timeout(clock_timestamp_millis: int, timeout_millis: int):
     return time.time_ns() // 1000000 - clock_timestamp_millis >= timeout_millis
 
 
 def debug(*args):
-    if DEBUG:
+    if CONFIGURATION.DEBUG:
         print(*args)
 
 
 def warning(*args):
-    if WARNING:
+    if CONFIGURATION.WARNING or CONFIGURATION.DEBUG:
         print(*args)
 
 
 def is_correct_node_uri(node_uri: str) -> bool:
     """ match description:
     dtn -> starts with "dtn://", then one or more characters (except "~" or "/"), ends with "/"
     ipn -> starts with "ipn://", then one or more digits, then zero or more "." + one or more digits
```

### Comparing `dtn7zero-0.0.6/dtn7zero.egg-info/PKG-INFO` & `dtn7zero-0.0.7/dtn7zero.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtn7zero
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Lukas Holst <lh700@proton.me>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/dtn7/dtn7zero
 Project-URL: Repository, https://github.com/dtn7/dtn7zero
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,22 +12,24 @@
 # dtn7zero
 This is a DTN7 [RFC9171](https://datatracker.ietf.org/doc/html/rfc9171) compliant python implementation (work-in-progress) with a [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
 
 The current features are:
 - a full bundle protocol agent (without fragment, CRC, and status-report generation support -> todo)
 - a minimal TCP convergence layer
 - a [dtn7-rs](https://github.com/dtn7/dtn7-rs) convergence layer, using the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md) interface
-- automatic local-network node-discovery via ipnd module
+- automatic local-network node-discovery via IPND module
 - a standalone 'external' endpoint (which connects to a [dtn7-rs](https://github.com/dtn7/dtn7-rs) via the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md)) interface
 - a simplified [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API to easily get started
 - full MicroPython support (tested on an ESP32-GENERIC)
+- experimental ESPNOW cla (details can be found in the source code: *dtn7zero/convergence_layer_adapters/espnow_cla.py*)
 - (currently uses epidemic routing and in-memory storage managing)
 - (with extendability for new convergence layer adapters, routing algorithms, and storage managers)
 
 ## Getting Started
+
 To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux):
 ```shell
 $ pip install --upgrade dtn7zero
 ```
 The most simple example on what you can do:
 ```python
 import time
@@ -40,66 +42,71 @@
 
 node_endpoint.send(b'hello world', "dtn://node1/")
 
 time.sleep(1)
 ```
 Further examples for the 'simple' API can be found under `./examples` in the GitHub repository.
 
-For a deeper dive into the underlying concepts and the fully fletched dtn implementation, take a look at the 
-`dtn7zero.api` module implementation and the tests under `./tests`.
+For a deeper dive into the underlying concepts and the full-fledged dtn implementation, take a look at the 
+`dtn7zero.api` module implementation and the tests under `./test`.
 
 ## MicroPython Installation Guide
+Installation has been successfully tested on Windows and Linux (x86_64 and arm64). The required
+[mpy-cross](https://pypi.org/project/mpy-cross/) has been shown to have installation issues on Mac M1s
+under Mac OS X and may have to be built and installed manually.
+
 This whole project was tested on an ESP32 (GENERIC) and this installation guide is tailored for the ESP32.
 If you plan to use another microcontroller you might need to do adjustments 
 (most certainly the MicroPython installation, and the MPY_MARCH in esp-deployment.py).
 
 Important note for linux: it may be that mpremote assumes another USB device with higher priority than the ESP32.
 In that case all mpremote commands (especially inside esp-deployment.py) will fail as no communication is possible.
 Check all USB devices mpremote considers in priority order with `mpremote devs`.
 
 ### First Time MicroPython Installation For ESP32 (GENERIC)
 1. download the newest [firmware](https://micropython.org/download/esp32/)
 2. install the esp flash tool: `pip install esptool`
 3. connect your ESP32 via USB and start a terminal at the location of the downloaded firmware
-4. start the following command (with the correct USB port), then hold **boot** until it starts erasing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 erase_flash`
-5. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
+4. start the following command (with the correct USB port): \
+`esptool --chip esp32 --port /dev/ttyUSB0 erase_flash` (you may have to invoke esptool with `esptool.py --chip ...` here and subsequently, you may also have hold **boot** to enter the bootloader on the ESP32)
+5. start the following command (with the correct USB port and firmware name): \
+`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin` (you may have hold **boot** again to enter the bootloader on the ESP32)
 6. done, you may now connect to it via: `mpremote` (installation via pip: `pip install mpremote`)
 
 ### Update To New MicroPython Version
 1. download the newest [firmware](https://micropython.org/download/esp32/)
-2. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
+2. start the following command (with the correct USB port and firmware name): \
+`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin` (you may have hold **boot** to enter the bootloader on the ESP32)
 3. done
 
 ### First Time dtn7zero Deployment
 1. make sure you check out the repository and the submodules (especially py-dtn7)
 2. install the mpremote tool: `pip install mpremote`
-3. install the mpy-cross compiler tool: `pip install mpy-cross`
+3. install the mpy-cross compiler tool: `pip install mpy-cross` (this may not work on Mac M1s under Mac OS X) 
 4. populate wlan.json with an appropriate hostname and at least one ssid -> password mapping
 5. check your connection to the ESP32 with: `mpremote`
 6. copy wlan.json to your ESP32: `mpremote fs cp wlan.json :wlan.json`
 7. copy boot.py to your ESP32: `mpremote fs cp boot.py :boot.py`
 8. deploy the dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
-9. done
+9. install required packages: `mpremote mip install urequests` and `mpremote mip install datetime`
+10. done
 
 ### Continuous dtn7zero Deployment
 1. check your connection to the ESP32 with: `mpremote`
 2. deploy the changes of dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
 3. done
 
 ### First dtn7zero Functionality Check On MicroPython
 1. you may check that wlan is connecting correctly (connect via `mpremote` and press **enable** for a soft reset)
 2. you may also check that you can import dtn7zero (connect via `mpremote` and `import dtn7zero`)
 3. you can also check that everything works (run the test script `mpremote run examples/local_ping_echo.py`)
 
 ### Additional MicroPython Tips & Tricks
 The mpremote tool is normally interrupted by using `ctrl+c`. A special case is the REPL (simply call `mpremote`), which
-can be exited by using `ctrl+~` (tested on windows).
+can be exited by using `ctrl+~` (tested on Windows) or `ctrl+]` (Linux).
 
 If you start a script on MicroPython (`mpremote run ...`) and disconnect the console (`mpremote` -> `ctrl+c`) then the script 
 keeps running.
 
 If you must access the REPL via mpremote, but a script is blocking, then call `mpremote` and press EN (enable) on the 
 ESP32 for a soft-reset. Press `ctrl+c` a few times to interrupt the `boot.py` or `main.py` script execution. The session
 state is stored, so any subsequent `mpremote` call will start at REPL as long as no power disconnect is performed.
@@ -107,17 +114,17 @@
 You can deploy a script as `main.py` on MicroPython to be run every time the microcontroller gets power. \
 You can also remove the script. MicroPython will only execute the script if it is present.
 ```shell
 $ mpremote fs cp examples/remote_echo_callback.py :main.py
 $ mpremote fs rm :main.py
 ```
 
-Regarding `boot.py`, it is used for user-specific setup code and this framework uses a generic boot script that adjusts
+Regarding `boot.py`: it is used for user-specific setup code and this framework uses a generic boot script that adjusts
 the ESP32's frequency and connects to a Wi-Fi network (blocking until success). MicroPython will create a dummy `boot.py`
-if none is present. MicroPython will not create a dummy `main.py` is none is present. MicroPython will first execute
+if none is present. MicroPython will not create a dummy `main.py` if none is present. MicroPython will first execute
 the `boot.py` and then the `main.py` if it is present.
 
 
 ## Development Information
 
 ### Development Mode
 You can install this project locally to directly reflect code changes in your environment.
```

### Comparing `dtn7zero-0.0.6/dtn7zero.egg-info/SOURCES.txt` & `dtn7zero-0.0.7/dtn7zero.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 dtn7zero/__init__.py
 dtn7zero/api.py
 dtn7zero/bundle_protocol_agent.py
-dtn7zero/constants.py
+dtn7zero/configuration.py
 dtn7zero/data.py
 dtn7zero/endpoints.py
 dtn7zero/ipnd.py
 dtn7zero/utility.py
 dtn7zero.egg-info/PKG-INFO
 dtn7zero.egg-info/SOURCES.txt
 dtn7zero.egg-info/dependency_links.txt
 dtn7zero.egg-info/requires.txt
 dtn7zero.egg-info/top_level.txt
 dtn7zero/convergence_layer_adapters/__init__.py
 dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
+dtn7zero/convergence_layer_adapters/espnow_cla.py
 dtn7zero/convergence_layer_adapters/mtcp.py
 dtn7zero/routers/__init__.py
 dtn7zero/routers/simple_epidemic_router.py
 dtn7zero/storage/__init__.py
 dtn7zero/storage/simple_in_memory_storage.py
 test/test-api-background.py
 test/test-api-ping.py
@@ -27,12 +28,14 @@
 test/test-api-synchronous.py
 test/test-bundle-protocol-agent-receiver.py
 test/test-bundle-protocol-agent-sender.py
 test/test-bundle-protocol-agent.py
 test/test-bundle-serialization.py
 test/test-bundle-size.py
 test/test-dtn7rs-rest-cla.py
+test/test-espnow-receiver.py
+test/test-espnow-sender.py
 test/test-ipnd.py
 test/test-mtcp-intermediate.py
 test/test-mtcp-receiver.py
 test/test-mtcp-sender.py
 test/test-py-dtn7-functionality.py
```

### Comparing `dtn7zero-0.0.6/pyproject.toml` & `dtn7zero-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtn7zero"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     {name = "Lukas Holst", email = "lh700@proton.me"},
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "AGPL-3.0"}
```

### Comparing `dtn7zero-0.0.6/test/test-api-background.py` & `dtn7zero-0.0.7/test/test-api-background.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dtn7zero import setup, register, start_background_update_thread
 from py_dtn7.bundle import PrimaryBlock
 
 
 setup("dtn://node1/")
 
-start_background_update_thread(_sleep_time_seconds=0.1)
+start_background_update_thread(sleep_time_milliseconds=100)
 
 
 def ping_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
     print("received pong: {}".format(payload))
 
 
 ping = register("ping", ping_callback)
```

### Comparing `dtn7zero-0.0.6/test/test-api-ping.py` & `dtn7zero-0.0.7/test/test-api-ping.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dtn7zero import setup, register, start_background_update_thread
 from py_dtn7.bundle import PrimaryBlock
 
 
 setup("dtn://node1/")
 
-start_background_update_thread(_sleep_time_seconds=0.1)
+start_background_update_thread(sleep_time_milliseconds=100)
 
 
 def ping_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
     print("received pong: {}".format(payload))
 
 
 ping = register("ping", ping_callback)
```

### Comparing `dtn7zero-0.0.6/test/test-api-pong.py` & `dtn7zero-0.0.7/test/test-api-pong.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dtn7zero import setup, register, start_background_update_thread
 from py_dtn7.bundle import PrimaryBlock
 
 
 setup("dtn://node2/")
 
-start_background_update_thread(_sleep_time_seconds=0.1)
+start_background_update_thread(sleep_time_milliseconds=100)
 
 
 def pong_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
     print("sending back pong {}".format(payload))
     pong.send(payload, full_source_uri)
```

### Comparing `dtn7zero-0.0.6/test/test-api-synchronous.py` & `dtn7zero-0.0.7/test/test-api-synchronous.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     global counter
     payload = str(counter).encode()
     print("sending ping: {}".format(payload))
     ping.send(payload, "dtn://node1/pong")
     counter += 1
 
 
-run_forever(main_loop, loop_callback_interval_milliseconds=2000, _sleep_time_seconds=0.1)
+run_forever(main_loop, loop_callback_interval_milliseconds=2000, sleep_time_milliseconds=100)
```

### Comparing `dtn7zero-0.0.6/test/test-bundle-protocol-agent-receiver.py` & `dtn7zero-0.0.7/test/test-bundle-protocol-agent-receiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 # import gc
 # print("init free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
 from dtn7zero.endpoints import LocalEndpoint
 from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP
+from dtn7zero.configuration import CONFIGURATION
 # from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
 from py_dtn7 import Bundle
 # print("after import free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
 # gc.collect()
 # print("after import garbage collect free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
 
 
 def callback(bundle: Bundle):
     print('bundle reached receiver endpoint: {}'.format(bundle.payload_block.data))
 
 
 storage = SimpleInMemoryStorage()
 
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+clas = {CONFIGURATION.IPND.IDENTIFIER_MTCP: MTcpCLA()}
 router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://nodeRECEIVE/', storage, router, use_ipnd=True)
+bpa = BundleProtocolAgent('dtn://nodeRECEIVE/', storage, router)
 
 receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
 
 bpa.register_endpoint(receiver_endpoint)
 
 # last_garbage_collect = get_current_clock_millis()
 try:
```

### Comparing `dtn7zero-0.0.6/test/test-bundle-protocol-agent-sender.py` & `dtn7zero-0.0.7/test/test-bundle-protocol-agent-sender.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 # import gc
 # print("init free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
 from dtn7zero.endpoints import LocalEndpoint
 from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP
+from dtn7zero.configuration import CONFIGURATION
 from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
 # print("after import free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
 # gc.collect()
 # print("after import garbage collect free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
 storage = SimpleInMemoryStorage()
 
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+clas = {CONFIGURATION.IPND.IDENTIFIER_MTCP: MTcpCLA()}
 router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://nodeSEND/', storage, router, use_ipnd=True)
+bpa = BundleProtocolAgent('dtn://nodeSEND/', storage, router)
 
 sender_endpoint = LocalEndpoint('sender')
 
 
 bpa.register_endpoint(sender_endpoint)
 
 # print("next free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
```

### Comparing `dtn7zero-0.0.6/test/test-bundle-protocol-agent.py` & `dtn7zero-0.0.7/test/test-bundle-protocol-agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 To be run either on CPython or MicroPython.
 
 Registers two local endpoints and sends from one to the other.
 """
 import time
 
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP
+from dtn7zero.configuration import CONFIGURATION
 from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
 from dtn7zero.endpoints import LocalEndpoint
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
 from py_dtn7 import Bundle
 
 
 def callback(bundle: Bundle):
     print('bundle reached receiver endpoint: {}'.format(bundle))
 
 
 storage = SimpleInMemoryStorage()
 
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+clas = {CONFIGURATION.IPND.IDENTIFIER_MTCP: MTcpCLA()}
 
 router = SimpleEpidemicRouter(clas, storage)
 bpa = BundleProtocolAgent('dtn://node2/', storage, router)
 
 sender_endpoint = LocalEndpoint('sender')
 receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
```

### Comparing `dtn7zero-0.0.6/test/test-bundle-serialization.py` & `dtn7zero-0.0.7/test/test-bundle-serialization.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.6/test/test-bundle-size.py` & `dtn7zero-0.0.7/test/test-bundle-size.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.6/test/test-dtn7rs-rest-cla.py` & `dtn7zero-0.0.7/test/test-dtn7rs-rest-cla.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,30 +6,34 @@
 
 Note on MicroPython:
 The current configuration of maximum in-memory stored bundles collides with the memory intensive urequests library.
 It therefore will likely crash after a few exchanged bundles.
 This is an open end topic to investigate.
 """
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.constants import IPND_IDENTIFIER_REST, PORT_REST
+from dtn7zero.configuration import CONFIGURATION
 from dtn7zero.convergence_layer_adapters.dtn7rs_rest import Dtn7RsRestCLA
 from dtn7zero.data import Node
 from dtn7zero.endpoints import LocalEndpoint
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
 
-dtn7rs = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_REST: PORT_REST})
+
+CONFIGURATION.IPND.ENABLED = False
+
+
+dtn7rs = Node('192.168.2.163', (1, '//node1/'), {CONFIGURATION.IPND.IDENTIFIER_REST: CONFIGURATION.PORT.REST}, 0)
 
 storage = SimpleInMemoryStorage()
 storage.add_node(dtn7rs)
 
-clas = {IPND_IDENTIFIER_REST: Dtn7RsRestCLA()}
+clas = {CONFIGURATION.IPND.IDENTIFIER_REST: Dtn7RsRestCLA()}
 router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://node2/', storage, router, use_ipnd=False)
+bpa = BundleProtocolAgent('dtn://node2/', storage, router)
 
 endpoint = LocalEndpoint('hello')
 bpa.register_endpoint(endpoint)
 
 last_send = get_current_clock_millis()
 try:
     while True:
```

### Comparing `dtn7zero-0.0.6/test/test-ipnd.py` & `dtn7zero-0.0.7/test/test-ipnd.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.6/test/test-mtcp-intermediate.py` & `dtn7zero-0.0.7/test/test-mtcp-intermediate.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 --> PLEASE CHECK AND SET THE CORRECT IP ADDRESSES
 --> THIS TEST WAS DESIGNED FOR SENDER AND RECEIVER TO BE RUN ON AN ESP32
 --> THE INTERMEDIATE NODE SHOULD BE RUNNING ON A COMPUTER
 --> THE INTERMEDIATE NODE CAN BE REPLACED BY THE dtn7rs
 
 start-command for the dtn7rs intermediate node:
-dtnd -n node1 -r epidemic -C mtcp -e incoming -s mtcp://192.168.2.182:16162/ESP32-6 -s mtcp://192.168.2.162:16162/ESP32-4
+dtnd -n node1 -r epidemic -C mtcp -e incoming -s mtcp://192.168.2.146:16162/ESP32-6 -s mtcp://192.168.2.177:16162/ESP32-4
 
 
 additional notes on the ESP32 sender:
 
 As only one ESP32 can be accessed to start a script on one computer, it may be useful to set the sender-script as main-script on one ESP32:
 mpremote fs cp test/test-mtcp-sender.py :main.py
 
@@ -23,26 +23,29 @@
 mpremote fs rm :main.py
 """
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
 from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
 from dtn7zero.data import Node
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP, PORT_MTCP
+from dtn7zero.configuration import CONFIGURATION
 
 
-esp32_4 = Node('192.168.2.162', (1, '//ESP32-4/'), {IPND_IDENTIFIER_MTCP: PORT_MTCP})
-esp32_6 = Node('192.168.2.182', (1, '//ESP32-6/'), {IPND_IDENTIFIER_MTCP: PORT_MTCP})
+CONFIGURATION.IPND.ENABLED = False
+
+
+esp32_4 = Node('192.168.2.146', (1, '//ESP32-4/'), {CONFIGURATION.IPND.IDENTIFIER_MTCP: CONFIGURATION.PORT.MTCP}, 0)
+esp32_6 = Node('192.168.2.177', (1, '//ESP32-6/'), {CONFIGURATION.IPND.IDENTIFIER_MTCP: CONFIGURATION.PORT.MTCP}, 0)
 
 storage = SimpleInMemoryStorage()
 storage.add_node(esp32_4)
 storage.add_node(esp32_6)
 
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+clas = {CONFIGURATION.IPND.IDENTIFIER_MTCP: MTcpCLA()}
 router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://node1/', storage, router, use_ipnd=False)
+bpa = BundleProtocolAgent('dtn://node1/', storage, router)
 
 try:
     while True:
         bpa.update()
 except KeyboardInterrupt:
     pass
```

### Comparing `dtn7zero-0.0.6/test/test-mtcp-receiver.py` & `dtn7zero-0.0.7/test/test-mtcp-receiver.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,26 +24,29 @@
 """
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
 from dtn7zero.endpoints import LocalEndpoint
 from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
 from dtn7zero.data import Node
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP, PORT_MTCP
+from dtn7zero.configuration import CONFIGURATION
 from py_dtn7 import Bundle
 
 
-dtn7rs_node = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_MTCP: PORT_MTCP})
+CONFIGURATION.IPND.ENABLED = False
+
+
+dtn7rs_node = Node('192.168.2.163', (1, '//node1/'), {CONFIGURATION.IPND.IDENTIFIER_MTCP: CONFIGURATION.PORT.MTCP}, 0)
 
 storage = SimpleInMemoryStorage()
 storage.add_node(dtn7rs_node)
 
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+clas = {CONFIGURATION.IPND.IDENTIFIER_MTCP: MTcpCLA()}
 router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://ESP32-4/', storage, router, use_ipnd=False)
+bpa = BundleProtocolAgent('dtn://ESP32-4/', storage, router)
 
 
 def callback(bundle: Bundle):
     print('received: {}'.format(bundle.payload_block.data))
 
 
 receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
```

### Comparing `dtn7zero-0.0.6/test/test-mtcp-sender.py` & `dtn7zero-0.0.7/test/test-mtcp-sender.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,26 +24,29 @@
 """
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
 from dtn7zero.endpoints import LocalEndpoint
 from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
 from dtn7zero.data import Node
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP, PORT_MTCP
+from dtn7zero.configuration import CONFIGURATION
 from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
 
 
-dtn7rs_node = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_MTCP: PORT_MTCP})
+CONFIGURATION.IPND.ENABLED = False
+
+
+dtn7rs_node = Node('192.168.2.163', (1, '//node1/'), {CONFIGURATION.IPND.IDENTIFIER_MTCP: CONFIGURATION.PORT.MTCP}, 0)
 
 storage = SimpleInMemoryStorage()
 storage.add_node(dtn7rs_node)
 
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+clas = {CONFIGURATION.IPND.IDENTIFIER_MTCP: MTcpCLA()}
 router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://ESP32-6/', storage, router, use_ipnd=False)
+bpa = BundleProtocolAgent('dtn://ESP32-6/', storage, router)
 
 sender_endpoint = LocalEndpoint('sender')
 
 
 bpa.register_endpoint(sender_endpoint)
 
 message_str = 'hello_world {}'
```

### Comparing `dtn7zero-0.0.6/test/test-py-dtn7-functionality.py` & `dtn7zero-0.0.7/test/test-py-dtn7-functionality.py`

 * *Files identical despite different names*

