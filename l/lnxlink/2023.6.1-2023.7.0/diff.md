# Comparing `tmp/lnxlink-2023.6.1.tar.gz` & `tmp/lnxlink-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnxlink-2023.6.1.tar", last modified: Mon Jun 12 15:59:09 2023, max compression
+gzip compressed data, was "lnxlink-2023.7.0.tar", last modified: Thu Jul  6 16:31:52 2023, max compression
```

## Comparing `lnxlink-2023.6.1.tar` & `lnxlink-2023.7.0.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:59:09.008688 lnxlink-2023.6.1/lnxlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14770 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/lnxlink/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/amd_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/boot_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/camera_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/microphone_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/notify.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/nvidia_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/required_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/screen_onoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/send_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/suspend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/sys_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/webcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/xdg_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/lnxlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 15:59:09.000000 lnxlink-2023.6.1/lnxlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:31:52.752973 lnxlink-2023.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 16:31:52.752973 lnxlink-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:31:52.748973 lnxlink-2023.7.0/lnxlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15363 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:31:52.752973 lnxlink-2023.7.0/lnxlink/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/boot_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/camera_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/microphone_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/required_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/screen_onoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/sys_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/modules/xdg_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/lnxlink/system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:31:52.748973 lnxlink-2023.7.0/lnxlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 16:31:52.000000 lnxlink-2023.7.0/lnxlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-06 16:31:52.000000 lnxlink-2023.7.0/lnxlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:31:52.000000 lnxlink-2023.7.0/lnxlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-06 16:31:52.000000 lnxlink-2023.7.0/lnxlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-06 16:31:52.000000 lnxlink-2023.7.0/lnxlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 16:31:52.000000 lnxlink-2023.7.0/lnxlink.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-07-06 16:31:39.000000 lnxlink-2023.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-06 16:31:52.752973 lnxlink-2023.7.0/setup.cfg
```

### Comparing `lnxlink-2023.6.1/LICENSE.md` & `lnxlink-2023.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/__main__.py` & `lnxlink-2023.7.0/lnxlink/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,27 @@
 version = importlib.metadata.version(__package__ or __name__)
 
 
 class LNXlink():
 
     def __init__(self, config_path):
         print(f"LNXlink {version} started: {platform.python_version()}")
+        self.kill = False
 
         # Read configuration from yaml file
         self.pref_topic = 'lnxlink'
         self.config = self.read_config(config_path)
 
         # Run each addon included in the modules folder
         self.Addons = {}
-        for service, addon in modules.parse_modules(self.config['modules']).items():
+        conf_modules = self.config.get('modules', None)
+        conf_exclude = self.config.get('exclude', [])
+        conf_exclude = [] if conf_exclude is None else conf_exclude
+        loaded_modules = modules.parse_modules(conf_modules, conf_exclude)
+        for service, addon in loaded_modules.items():
             try:
                 tmp_addon = addon(self)
                 self.Addons[addon.service] = tmp_addon
             except Exception as e:
                 print(f"Error with addon {addon.service}, please remove it from your config")
                 traceback.print_exc()
 
@@ -85,16 +90,17 @@
                     traceback.print_exc()
 
     def monitor_run_thread(self):
         '''Runs method to get sensor information every prespecified interval'''
         self.monitor_run()
 
         interval = self.config.get('update_interval', 1)
-        self.monitor = threading.Timer(interval, self.monitor_run_thread)
-        self.monitor.start()
+        if not self.kill:
+            self.monitor = threading.Timer(interval, self.monitor_run_thread)
+            self.monitor.start()
 
     def setup_mqtt(self):
         '''Creates the mqtt object'''
         self.client = mqtt.Client()
         self.client.on_connect = self.on_connect
         self.client.on_message = self.on_message
 
@@ -127,42 +133,52 @@
                 f"{self.pref_topic}/lwt",
                 payload=self.config['mqtt']['lwt']['connectMsg'],
                 qos=self.config['mqtt']['lwt']['qos'],
                 retain=self.config['mqtt']['lwt']['retain']
             )
         if self.config['mqtt']['discovery']['enabled']:
             self.setup_discovery()
+        if self.kill:
+            self.kill = False
+            self.monitor_run_thread()
 
     def disconnect(self, *args):
         '''Reports to MQTT server that the service has stopped'''
         print("Disconnected from MQTT.")
         if self.config['mqtt']['lwt']['enabled']:
             self.client.publish(
                 f"{self.pref_topic}/lwt",
                 payload=self.config['mqtt']['lwt']['disconnectMsg'],
                 qos=self.config['mqtt']['lwt']['qos'],
                 retain=self.config['mqtt']['lwt']['retain']
             )
+        self.kill = True
         try:
             self.monitor.cancel()
         except Exception as e:
             pass
         self.client.disconnect()
 
     def temp_connection_callback(self, status):
         '''Report the connection status to MQTT server'''
+        self.kill = True
         if self.config['mqtt']['lwt']['enabled']:
             if status:
+                print("Power Down detected.")
                 self.client.publish(
                     f"{self.pref_topic}/lwt",
                     payload=self.config['mqtt']['lwt']['disconnectMsg'],
                     qos=self.config['mqtt']['lwt']['qos'],
                     retain=self.config['mqtt']['lwt']['retain']
                 )
             else:
+                print("Power Up detected.")
+                if self.kill:
+                    self.kill = False
+                    self.monitor_run_thread()
                 self.client.publish(
                     f"{self.pref_topic}/lwt",
                     payload=self.config['mqtt']['lwt']['connectMsg'],
                     qos=self.config['mqtt']['lwt']['qos'],
                     retain=self.config['mqtt']['lwt']['retain']
                 )
 
@@ -329,15 +345,14 @@
         required=True)
     args = parser.parse_args()
 
     config_file = os.path.abspath(args.config)
     config.setup_config(config_file)
     config.setup_systemd(config_file)
     lnxlink = LNXlink(config_file)
-    lnxlink.monitor_run_thread()
 
     # Monitor for system changes (Shutdown/Suspend/Sleep)
     monitor_suspend = MonitorSuspend(lnxlink.temp_connection_callback)
     monitor_suspend.start()
     monitor_gracefulkiller = GracefulKiller(lnxlink.temp_connection_callback)
     while not monitor_gracefulkiller.kill_now:
         time.sleep(0.2)
```

### Comparing `lnxlink-2023.6.1/lnxlink/config.py` & `lnxlink-2023.7.0/lnxlink/config.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/consts.py` & `lnxlink-2023.7.0/lnxlink/consts.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/__init__.py` & `lnxlink-2023.7.0/lnxlink/modules/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 import time
 import traceback
 import glob
 import os
 import sys
 
 
-def autoload_modules():
+def autoload_modules(auto_exclude):
     modules = []
     modules_path = f"{os.path.dirname(__file__)}/*.py"
     for module_path in glob.glob(modules_path):
         module = os.path.basename(module_path)
         if '__' not in module and '.py' in module:
-            modules.append(module.replace('.py', ''))
+            module = module.replace('.py', '')
+            if module not in auto_exclude:
+                modules.append(module)
 
     return modules
 
 
-def parse_modules(list_modules=None):
+def parse_modules(list_modules=None, auto_exclude=[]):
     if list_modules is None:
-        list_modules = autoload_modules()
+        list_modules = autoload_modules(auto_exclude)
     modules = {}
     for module_name in list_modules:
         retries = 10
         while retries >= 0:
             try:
                 if '.py' in module_name:
                     module_path = os.path.dirname(module_name)
```

### Comparing `lnxlink-2023.6.1/lnxlink/modules/battery.py` & `lnxlink-2023.7.0/lnxlink/modules/battery.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/boot_select.py` & `lnxlink-2023.7.0/lnxlink/modules/boot_select.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/brightness.py` & `lnxlink-2023.7.0/lnxlink/modules/brightness.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class Addon():
 
     def __init__(self, lnxlink=None):
         self.name = 'Brightness'
 
     def getControlInfo(self):
         displays = self._get_displays()
-        avg_brightness = sum(displays.values()) / len(displays.values())
+        avg_brightness = sum(displays.values()) / max(1, len(displays.values()))
 
         info = {"status": avg_brightness}
         for display, brightness in displays.items():
             display = display.replace("-", "_")
             info[display] = brightness
         return info
```

### Comparing `lnxlink-2023.6.1/lnxlink/modules/camera_used.py` & `lnxlink-2023.7.0/lnxlink/modules/camera_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/disk_usage.py` & `lnxlink-2023.7.0/lnxlink/modules/disk_usage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 import psutil
 
 
 class Addon():
 
     def __init__(self, lnxlink):
         self.name = 'Disk Usage'
-        self.sensor_type = 'sensor'
-        self.icon = 'mdi:harddisk'
 
-    def getInfo(self) -> dict:
-        disks = {"status": False}
+    def exposedControls(self):
+        discovery_info = {}
         for disk in psutil.disk_partitions():
             if disk.fstype == 'squashfs':
                 continue
-            disks[disk.device] = {}
+            if 'docker/overlay' in disk.mountpoint:
+                continue
+            device = disk.device.replace('/', '_').strip('_')
+            discovery_info[f"Disk {device}"] = {
+                "type": "sensor",
+                "icon": "mdi:harddisk",
+                "unit": "%",
+                "state_class": "measurement",
+                "value_template": f"{{{{ value_json.{device}.percent }}}}",
+                "enabled": True,
+            }
+        return discovery_info
+
+    def getControlInfo(self):
+        disks = {}
+        for disk in psutil.disk_partitions():
+            if disk.fstype == 'squashfs':
+                continue
+            if 'docker/overlay' in disk.mountpoint:
+                continue
+            device = disk.device.replace('/', '_').strip('_')
+            disks[device] = {}
             disk_stats = psutil.disk_usage(disk.mountpoint)
-            disks[disk.device]["total"] = self._bytetomb(disk_stats.total)
-            disks[disk.device]["used"] = self._bytetomb(disk_stats.used)
-            disks[disk.device]["free"] = self._bytetomb(disk_stats.free)
-            disks[disk.device]["percent"] = disk_stats.percent
-            if disk_stats.percent > 80:
-                disks["status"] = True
+            disks[device]["total"] = self._bytetomb(disk_stats.total)
+            disks[device]["used"] = self._bytetomb(disk_stats.used)
+            disks[device]["free"] = self._bytetomb(disk_stats.free)
+            disks[device]["percent"] = disk_stats.percent
         return disks
 
     def _bytetomb(self, byte):
         return round(byte / 1024 / 1024, 1)
```

### Comparing `lnxlink-2023.6.1/lnxlink/modules/keep_alive.py` & `lnxlink-2023.7.0/lnxlink/modules/keep_alive.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/media.py` & `lnxlink-2023.7.0/lnxlink/modules/media.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/memory.py` & `lnxlink-2023.7.0/lnxlink/modules/memory.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/microphone_used.py` & `lnxlink-2023.7.0/lnxlink/modules/microphone_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/network.py` & `lnxlink-2023.7.0/lnxlink/modules/network.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/notify.py` & `lnxlink-2023.7.0/lnxlink/modules/notify.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/screen_onoff.py` & `lnxlink-2023.7.0/lnxlink/modules/screen_onoff.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/screenshot.py` & `lnxlink-2023.7.0/lnxlink/modules/screenshot.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/sys_updates.py` & `lnxlink-2023.7.0/lnxlink/modules/sys_updates.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/update.py` & `lnxlink-2023.7.0/lnxlink/modules/update.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/modules/webcam.py` & `lnxlink-2023.7.0/lnxlink/modules/webcam.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink/system_monitor.py` & `lnxlink-2023.7.0/lnxlink/system_monitor.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.1/lnxlink.egg-info/SOURCES.txt` & `lnxlink-2023.7.0/lnxlink.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 lnxlink.egg-info/PKG-INFO
 lnxlink.egg-info/SOURCES.txt
 lnxlink.egg-info/dependency_links.txt
 lnxlink.egg-info/entry_points.txt
 lnxlink.egg-info/requires.txt
 lnxlink.egg-info/top_level.txt
 lnxlink/modules/__init__.py
-lnxlink/modules/amd_gpu.py
 lnxlink/modules/bash.py
 lnxlink/modules/battery.py
 lnxlink/modules/boot_select.py
 lnxlink/modules/brightness.py
 lnxlink/modules/camera_used.py
 lnxlink/modules/cpu.py
 lnxlink/modules/disk_usage.py
+lnxlink/modules/gpu.py
 lnxlink/modules/idle.py
 lnxlink/modules/keep_alive.py
 lnxlink/modules/media.py
 lnxlink/modules/memory.py
 lnxlink/modules/microphone_used.py
 lnxlink/modules/network.py
 lnxlink/modules/notify.py
-lnxlink/modules/nvidia_gpu.py
 lnxlink/modules/required_restart.py
 lnxlink/modules/restart.py
 lnxlink/modules/screen_onoff.py
 lnxlink/modules/screenshot.py
 lnxlink/modules/send_keys.py
 lnxlink/modules/shutdown.py
 lnxlink/modules/suspend.py
```

### Comparing `lnxlink-2023.6.1/pyproject.toml` & `lnxlink-2023.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name              = "lnxlink"
-version           = "2023.6.1"
+version           = "2023.7.0"
 description       = "Internet Of Things (IOT) integration with Linux using MQTT"
 readme            = "README.md"
 keywords          = ["lnxlink"]
 requires-python   = ">=3.7.0"
 authors     = [
     {name="bkbilly", email="bkbilly@hotmail.com"}
 ]
@@ -28,15 +28,17 @@
     "pgi>=0.0.11.2",
     "pyOpenSSL>=22.1.0",
     "requests>=2.28.1",
     "jc>=1.23.0",
     "dbus-idle>=2023.3.2",
     "opencv-python>=4.7.0.68",
     "mss>=7.0.1",
-    "pyamdgpuinfo>=2.1.4"
+    "pyamdgpuinfo>=2.1.4",
+    "nvsmi>=0.4.2",
+    "distro>=1.7.0"
 ]
 
 
 [project.urls]
 "Source Code" = "https://github.com/bkbilly/lnxlink"
 "Home Page"   = "https://bkbilly.github.io/lnxlink"
```

