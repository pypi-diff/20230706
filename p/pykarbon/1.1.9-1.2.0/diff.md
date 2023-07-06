# Comparing `tmp/pykarbon-1.1.9.tar.gz` & `tmp/pykarbon-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pykarbon-1.1.9.tar", last modified: Fri Oct 16 16:02:12 2020, max compression
+gzip compressed data, was "pykarbon-1.2.0.tar", last modified: Thu Jul  6 17:39:36 2023, max compression
```

## Comparing `pykarbon-1.1.9.tar` & `pykarbon-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2020-10-16 16:02:12.000000 pykarbon-1.1.9/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      913 2020-10-16 15:08:56.000000 pykarbon-1.1.9/setup.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3515 2020-03-27 19:11:55.000000 pykarbon-1.1.9/README.rst
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2020-10-16 16:02:12.000000 pykarbon-1.1.9/test/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3067 2020-10-16 14:50:40.000000 pykarbon-1.1.9/test/test_terminal.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      859 2020-03-09 17:06:03.000000 pykarbon-1.1.9/test/test_i2c.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2453 2020-10-16 14:40:25.000000 pykarbon-1.1.9/test/test_hardware.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5825 2020-10-16 14:40:25.000000 pykarbon-1.1.9/test/test_can.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2290 2020-10-16 14:40:25.000000 pykarbon-1.1.9/test/test_pykarbon.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1785 2020-03-09 16:18:51.000000 pykarbon-1.1.9/test/test_core.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       38 2020-10-16 16:02:12.000000 pykarbon-1.1.9/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2020-10-16 16:02:12.000000 pykarbon-1.1.9/pykarbon/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3788 2020-03-09 17:06:03.000000 pykarbon-1.1.9/pykarbon/i2c.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     8902 2020-03-09 16:18:51.000000 pykarbon-1.1.9/pykarbon/core.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5896 2020-03-09 16:18:51.000000 pykarbon-1.1.9/pykarbon/hardware.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    19746 2020-10-16 14:28:11.000000 pykarbon-1.1.9/pykarbon/can.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    23793 2020-10-16 14:28:11.000000 pykarbon-1.1.9/pykarbon/terminal.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       84 2020-03-09 16:18:51.000000 pykarbon-1.1.9/pykarbon/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5377 2020-03-09 16:18:51.000000 pykarbon-1.1.9/pykarbon/pykarbon.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5176 2020-10-16 16:02:12.000000 pykarbon-1.1.9/PKG-INFO
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2020-10-16 16:02:12.000000 pykarbon-1.1.9/scripts/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1724 2020-03-09 16:18:51.000000 pykarbon-1.1.9/scripts/update_karbon_firmware
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2020-10-16 16:02:12.000000 pykarbon-1.1.9/pykarbon.egg-info/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      460 2020-10-16 16:02:12.000000 pykarbon-1.1.9/pykarbon.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       14 2020-10-16 16:02:12.000000 pykarbon-1.1.9/pykarbon.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        9 2020-10-16 16:02:12.000000 pykarbon-1.1.9/pykarbon.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5176 2020-10-16 16:02:12.000000 pykarbon-1.1.9/pykarbon.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2020-10-16 16:02:12.000000 pykarbon-1.1.9/pykarbon.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:39:36.133320 pykarbon-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-06 17:39:18.000000 pykarbon-1.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     4299 2023-07-06 17:39:36.133320 pykarbon-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3515 2023-07-06 17:39:18.000000 pykarbon-1.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:39:36.133320 pykarbon-1.2.0/pykarbon/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-06 17:39:18.000000 pykarbon-1.2.0/pykarbon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19524 2023-07-06 17:39:18.000000 pykarbon-1.2.0/pykarbon/can.py
+-rw-r--r--   0 root         (0) root         (0)     8902 2023-07-06 17:39:18.000000 pykarbon-1.2.0/pykarbon/core.py
+-rw-r--r--   0 root         (0) root         (0)     5896 2023-07-06 17:39:18.000000 pykarbon-1.2.0/pykarbon/hardware.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-07-06 17:39:18.000000 pykarbon-1.2.0/pykarbon/i2c.py
+-rw-r--r--   0 root         (0) root         (0)     5377 2023-07-06 17:39:18.000000 pykarbon-1.2.0/pykarbon/pykarbon.py
+-rw-r--r--   0 root         (0) root         (0)    23739 2023-07-06 17:39:18.000000 pykarbon-1.2.0/pykarbon/terminal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:39:36.133320 pykarbon-1.2.0/pykarbon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4299 2023-07-06 17:39:36.000000 pykarbon-1.2.0/pykarbon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-06 17:39:36.000000 pykarbon-1.2.0/pykarbon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 17:39:36.000000 pykarbon-1.2.0/pykarbon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-06 17:39:36.000000 pykarbon-1.2.0/pykarbon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 17:39:36.000000 pykarbon-1.2.0/pykarbon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:39:36.133320 pykarbon-1.2.0/scripts/
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-07-06 17:39:18.000000 pykarbon-1.2.0/scripts/update_karbon_firmware
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 17:39:36.133320 pykarbon-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-06 17:39:18.000000 pykarbon-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:39:36.133320 pykarbon-1.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)     5825 2023-07-06 17:39:18.000000 pykarbon-1.2.0/test/test_can.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-07-06 17:39:18.000000 pykarbon-1.2.0/test/test_core.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-06 17:39:18.000000 pykarbon-1.2.0/test/test_hardware.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-06 17:39:18.000000 pykarbon-1.2.0/test/test_i2c.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-07-06 17:39:18.000000 pykarbon-1.2.0/test/test_pykarbon.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-07-06 17:39:18.000000 pykarbon-1.2.0/test/test_terminal.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pykarbon-1.1.9/setup.py` & `pykarbon-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 '''
 from setuptools import setup
 
 setup(
     name='pykarbon',
     url='https://github.com/onlogic/Pykarbon',
     author='OnLogic',
-    author_email='jacob.caughfield@onlogic.com',
+    author_email='firmwareengineeringteam@onlogic.com',
     packages=['pykarbon'],
-    install_requires=['pyserial==3.4'],
+    install_requires=['pyserial>=3.4'],
     scripts=['scripts/update_karbon_firmware'],
-    version='1.1.9',
+    version='1.2.0',
     license='BSD-2.0',
     description='Tools for Karbon hardware interfaces.',
     long_description=open('README.rst').read(),
     classifiers=[
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
     ]
 )
```

### Comparing `pykarbon-1.1.9/README.rst` & `pykarbon-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/test/test_terminal.py` & `pykarbon-1.2.0/test/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/test/test_i2c.py` & `pykarbon-1.2.0/test/test_i2c.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/test/test_hardware.py` & `pykarbon-1.2.0/test/test_hardware.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/test/test_can.py` & `pykarbon-1.2.0/test/test_can.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/test/test_pykarbon.py` & `pykarbon-1.2.0/test/test_pykarbon.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/test/test_core.py` & `pykarbon-1.2.0/test/test_core.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/pykarbon/i2c.py` & `pykarbon-1.2.0/pykarbon/i2c.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/pykarbon/core.py` & `pykarbon-1.2.0/pykarbon/core.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/pykarbon/hardware.py` & `pykarbon-1.2.0/pykarbon/hardware.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/pykarbon/can.py` & `pykarbon-1.2.0/pykarbon/can.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     Lets us autodetect the can bus baudrate, write data to the can bus, wait for some messages to
     be receive, and finally save those messages to can_messages.csv
 '''
 from time import sleep, time
 import threading
 import re
+import queue
 
 import pykarbon.hardware as pk
 
 # Tools --------------------------------------------------------------------------------------------
 
 
 def stringify(value):
@@ -91,40 +92,37 @@
         isopen: Bool to indicate if the interface is connected
         baudrate: Reports the discovered or set baudrate
         registry: Dict of registered DIO states and function responses
         bgmon: Thread object of the bus background monintor
     '''
     def __init__(self, baudrate='autobaud', timeout=.01, automon=True, reaction_poll_delay=.01):
         '''Discovers hardware port name.'''
-        self.interface = pk.Interface('can', timeout)
-
         self.poll_delay = reaction_poll_delay
         self.baudrate = None
-        self.pre_data = []
-        self.data = []
+        self.pre_data = queue.Queue()
+        self.data = queue.Queue()
         self.isopen = False
         self.bgmon = None
         self.registry = {}
 
+        self.interface = pk.Interface('can', timeout)
+
         if baudrate == 'autobaud':
             self.autobaud(None)
         elif isinstance(baudrate, int):
             self.autobaud(baudrate)
 
         if automon:
             self.open()
             self.bgmonitor()
         else:
             self.data = self.pre_data
 
     def __enter__(self):
-        if not self.isopen:
-            self.interface.__enter__()
-            self.isopen = True
-
+        self.open()
         return self
 
     def open(self):
         '''Claim the interface (only one application may open the serial port)'''
         if not self.isopen:
             self.interface.claim()
             self.isopen = True
@@ -136,15 +134,17 @@
 
         NOTE: Strips EoL characters.
 
         Args:
             line: Data that will be pushed onto the queue
         '''
 
-        self.data.append(line.strip('\n\r'))
+        while self.data.qsize() > 100:
+            self.data.get_nowait()
+        self.data.put(line.strip('\n\r'))
 
     def autobaud(self, baudrate: int) -> str:
         '''Autodetect the bus baudrate
 
         If the passed argument 'baudrate' is None, the baudrate will be autodetected,
         otherwise, the bus baudrate will be set to the passed value.
 
@@ -287,30 +287,27 @@
         Returns
             The data read from the port
         '''
         line = ""
         if self.isopen:
             line = self.interface.cread()[0]
             if line:
-                self.pre_data.append(line)
+                self.pre_data.put(line)
 
         return line
 
     def bgmonitor(self):
         '''Start monitoring the canbus in the background
 
         Uses python threading module to start the monitoring process.
 
         Returns:
             The 'thread' object of this background process
         '''
 
-        if not self.data:
-            self.data = []
-
         self.bgmon = threading.Thread(target=self.monitor)
         self.bgmon.start()
 
         threading.Thread(target=self.registry_service).start()
 
         return self.bgmon
 
@@ -338,24 +335,20 @@
     def registry_service(self):
         '''Check if receive line has a registered action.
 
         If the receive line does have an action, perform it, and then move the data
         into the main data queue. Otherwise, just move the data.
         '''
         while self.isopen:
-            # Allow CPU to have time
-            sleep(self.poll_delay)
-
-            try:
-                line = self.pre_data.pop(0)
-                if line:
-                    self.check_action(line)
-                    self.pushdata(line)
-            except IndexError:
-                continue
+            line = self.pre_data.get()
+            if line is None:
+                break
+            else:
+                self.check_action(line)
+                self.pushdata(line)
 
         return 0
 
     def check_action(self, line):
         '''Check is message has an action attached, and execute if found
 
         Args:
@@ -417,51 +410,48 @@
 
         Uses queue behavior, so data is returned with 'first in first out' logic
 
         Returns:
             String of the data read from the port. Returns empty string if the queue is empty
         '''
         try:
-            out = self.data.pop(0)
-        except IndexError:
+            out = self.data.get_nowait()
+        except queue.Empty:
             out = ""
 
         return out
 
     def close(self):
         '''Release the interface so that other session may interact with it
 
         Any existing background monitor session will also be closed. If this session re-opens the
         connection, background monitoring will need to be manually restarted with the 'bgmonitor'
         method.
         '''
+        if not self.isopen:
+            return
+
         self.isopen = False
 
+        # Wake up the registry service thread so it will exit
+        self.pre_data.put(None)
+
         try:
             if self.bgmon.isAlive():
                 sleep(.1)
         except AttributeError:
             sleep(.001)
 
         self.interface.release()
 
     def __exit__(self, etype, evalue, etraceback):
-        self.isopen = False
-
-        try:
-            if self.bgmon.isAlive():
-                sleep(.1)
-        except AttributeError:
-            sleep(.001)
-
-        self.interface.__exit__(etype, evalue, etraceback)
+        self.close()
 
     def __del__(self):
-        if self.isopen:
-            self.close()
+        self.close()
 
 
 class Reactions():
     '''A class for performing automated responses to certain can messages.
 
     If the action returns a dict of hex id and data, then the reaction will
     automatically respond with this id and data. If the dict has 'None' for
```

### Comparing `pykarbon-1.1.9/pykarbon/terminal.py` & `pykarbon-1.2.0/pykarbon/terminal.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     This snippet will update and print the microntrollers configuration information, and then set
     digital output zero high.
 '''
 from time import sleep, time
 import re
 import threading
+import queue
 
 import pykarbon.hardware as pk
 
 
 class Session():
     '''Attaches to terminal serial port and allows reading/writing from the port.
 
@@ -56,19 +57,21 @@
         isopen: Bool to indicate if the interface is connected
         info: Dictionary of information about the configuration of the mcu.
         registry: Dict of registered DIO states and function responses
         bgmon: Thread object of the bus background monintor
     '''
     def __init__(self, timeout=.01, automon=True):
         '''Discovers hardware port name. '''
+        self.pre_data = queue.Queue()
+        self.data = queue.Queue()
+        self.prev_line = "1111 0000"
+        self.isopen = False
+
         self.interface = pk.Interface('terminal', timeout)
 
-        self.pre_data = []
-        self.data = []
-        self.isopen = False
 
         self.info = {
             'version':
                 {
                     'value': None,
                     'desc': 'Firmware version number.'
                 },
@@ -145,18 +148,15 @@
         if automon:
             self.open()
             self.bgmonitor()
         else:
             self.data = self.pre_data
 
     def __enter__(self):
-        if not self.isopen:
-            self.interface.__enter__()
-            self.isopen = True
-
+        self.open()
         return self
 
     def open(self):
         '''Claim the interface (only one application may open the serial port)'''
         if not self.isopen:
             self.interface.claim()
             self.isopen = True
@@ -168,15 +168,17 @@
 
         NOTE: Does not push empty strings, and strips EoL characters.
 
         Args:
             line: Data that will be pushed onto the queue
         '''
 
-        self.data.append(line)
+        while self.data.qsize() > 100:
+            self.data.get_nowait()
+        self.data.put(line)
 
     def register(self, input_num, state, action, **kwargs):
         '''Automatically perform action upon receiving data_id
 
         Register an action that should be automatically performed when a certain digital input
         state is read. By default, this action will only be performed when the digital input
         first transitions to a state -- subsequent bus reads will be ignored:
@@ -225,15 +227,15 @@
                 auto_response: Automatically reply with returned message (Default: True)
 
         Returns:
             The 'Reaction' object that will be used in responses to this data_id
         '''
 
         reaction = Reactions(self.set_all_do, [input_num, state], action, **kwargs)
-        self.registry[input_num] = {state: reaction}
+        self.registry.setdefault(input_num, {}).update({state: reaction})
 
         return reaction
 
     def print_info(self):
         ''' Prints out mcu configuration information '''
         top_bot = "-"
         top_bot = top_bot.rjust(37, '-')
@@ -388,32 +390,29 @@
             The data read from the port
         '''
         line = ""
         if self.isopen:
             line = self.interface.cread()[0]
             dio_check = re.match(r'[0-1]{4} {0,1}[0-1]{4}', line)
             if dio_check:
-                self.pre_data.append(line[0:4] + ' ' + line[4:8])
+                self.pre_data.put(line[0:4] + ' ' + line[4:8])
             elif line:
                 self.parse_line(line)
 
         return line
 
     def bgmonitor(self):
         '''Start monitoring the terminal in the background
 
         Uses python threading module to start the monitoring process.
 
         Returns:
             The 'thread' object of this background process
         '''
 
-        if not self.data:
-            self.data = []
-
         self.bgmon = threading.Thread(target=self.monitor)
         self.bgmon.start()
 
         threading.Thread(target=self.registry_service).start()
 
         return self.bgmon
 
@@ -437,40 +436,42 @@
 
     def registry_service(self):
         '''Check if receive line has a registered action.
 
         If the receive line does have an action, perform it, and then move the data
         into the main data queue. Otherwise, just move the data.
         '''
+        prev_line = None
         while self.isopen:
-            try:
-                line = self.pre_data.pop()
-                if line:
-                    self.pushdata(line)
-                    self.check_action(line)
-            except IndexError:
-                continue
+            line = self.pre_data.get()
+            if line is None:
+                break
+            else:
+                self.pushdata(line)
+                self.check_action(line, prev_line)
+                prev_line = line
 
         return 0
 
-    def check_action(self, line):
+    def check_action(self, line, prev_line=None):
         '''Check is message has an action attached, and execute if found
 
         Args:
             line: Dio state formatted as '[0-1]{4} [0-1]{4}'
             prev_line: The previously known state of the bus
         '''
 
-        prev_state = self.get_previous_state(-2)
+        if prev_line is None:
+            prev_line = self.get_previous_state()
         state_map = {'1': 'high', '0': 'low'}
 
         # Check registry against current state of each digital input
         for input_num in self.registry:
             input_state = state_map[line[input_num]]
-            transition = state_map[prev_state[input_num]] != input_state
+            transition = state_map[prev_line[input_num]] != input_state
 
             action = self.registry[input_num].get(input_state)
 
             if not action:
                 continue
 
             if action.transition_only and not transition:
@@ -484,20 +485,15 @@
             else:
                 action.start(line)
 
         return
 
     def get_previous_state(self, index=-1):
         ''' Returns the previous state of the digital io '''
-        try:
-            prev_line = self.data[index]
-        except IndexError:
-            prev_line = '1111 0000'
-
-        return prev_line
+        return self.prev_line
 
     def storedata(self, filename: str, mode='a+'):
         '''Pops the entire queue and saves it to a csv.
 
         This method clears the entire queue: once you have called it, all previously received
         data will no longer be stored in the sessions 'data' attribute. Instead, this data will
         now reside in the specified .csv file.
@@ -532,51 +528,49 @@
 
         Uses queue behavior, so data is returned with 'first in first out' logic
 
         Returns:
             String of the data read from the port. Returns empty string if the queue is empty
         '''
         try:
-            out = self.data.pop(0)
-        except IndexError:
+            out = self.data.get_nowait(0)
+            self.prev_line = out
+        except queue.Empty:
             out = ""
 
         return out
 
     def close(self):
         '''Release the interface so that other session may interact with it
 
         Any existing background monitor session will also be closed. If this session re-opens the
         connection, background monitoring will need to be manually restarted with the 'bgmonitor'
         method.
         '''
+        if not self.isopen:
+            return
+
         self.isopen = False
 
+        # Wake up the registry service thread so it will exit
+        self.pre_data.put(None)
+
         try:
             if self.bgmon.is_alive():
                 sleep(.1)
         except AttributeError:
             sleep(.001)
 
         self.interface.release()
 
     def __exit__(self, etype, evalue, etraceback):
-        self.isopen = False
-
-        try:
-            if self.bgmon.is_alive():
-                sleep(.1)
-        except AttributeError:
-            sleep(.001)
-
-        self.interface.__exit__(etype, evalue, etraceback)
+        self.close()
 
     def __del__(self):
-        if self.isopen:
-            self.close()
+        self.close()
 
 
 class Reactions():
     '''A class for performing automated responses to certain dio transitions.
 
     If the action returns a list digital output states, then the reaction
     will set each of these states. If the action returns None, no digital
```

### Comparing `pykarbon-1.1.9/pykarbon/pykarbon.py` & `pykarbon-1.2.0/pykarbon/pykarbon.py`

 * *Files identical despite different names*

### Comparing `pykarbon-1.1.9/PKG-INFO` & `pykarbon-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,148 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pykarbon
-Version: 1.1.9
+Version: 1.2.0
 Summary: Tools for Karbon hardware interfaces.
 Home-page: https://github.com/onlogic/Pykarbon
 Author: OnLogic
-Author-email: jacob.caughfield@onlogic.com
+Author-email: firmwareengineeringteam@onlogic.com
 License: BSD-2.0
-Description: ===============
-        Pykarbon Module
-        ===============
-        For the full rundown, read `the rest of the docs <https://pykarbon.readthedocs.io/en/latest/>`_.
-        
-        -----------
-        What is it?
-        -----------
-        
-        The Pykarbon module provides a set of tools for interfacing with the hardware devices on
-        OnLogic's 'Karbon' series industrial PCs. These interfaces include the onboard CAN bus,
-        Digital IO, and a few other hardware devices.
-        
-        The goal of this package is to provide a simple, but powerful, base platform that will allow
-        users to quickly and easily integrate a Karbon into their own application.
-        
-        *The tools in this package are designed to work with specific hardware;
-        this will not work for more generalized projects*
-        
-        ----------------
-        How do I use it?
-        ----------------
-        
-        *You will need to install python 3 prior to following this guide.*
-        
-        Getting started with pykarbon takes only a few minutes:
-        
-        .. role:: bash(code)
-           :language: bash
-        
-        - Open up a terminal, and run :bash:`pip install pykarbon`
-        
-          + On some systems you may need to run as admin, or use the :bash:`--user` flag
-        
-        - Launch a python shell with :bash:`python`
-        
-          + Usually linux users do not have write access to serial ports; grant your user permanent access with :bash:`usermod -a -G dialout $USER` or use :bash:`sudo python`
-        
-        .. role:: python(code)
-           :language: python
-        
-        - Import pykarbon with :python:`import pykarbon.pykarbon as pk`
-        - And finally create a control object using :python:`dev = pk.Karbon()`
-        
-        If all went well, you should now be ready to control a variety of systems, but for now, let's just print out some
-        configuration information:
-        
-        - :python:`dev.show_info()`
-        
-        And close our session:
-        
-        - :python:`dev.close()`
-        
-        -------------------
-        What else can I do?
-        -------------------
-        
-        Pykarbon offers a number of tools for automating and using Karbon series hardware interfaces. These include:
-        
-        - CAN and DIO background data monitoring
-        - Exporting logged data to .csv
-        - Registering and making function calls based on these bus events:
-        
-          + CAN data IDs
-          + Digital Input Events
-          + DIO Bus States (Allows partial states)
-        
-        - Automated can message response to registered IDs
-        - Automated setting of Digital Output states
-        - Automatic CAN baudrate detection
-        - Updating user configuration information:
-        
-          + Ignition sense enable/disable
-          + Power timing configurations
-          + Low battery shutdown voltage
-          + Etc.
-        
-        - Firmware update
-        
-        Additonally, as Pykarbon's CAN and Terminal sessions must connect to device serial ports, functionality has been added
-        to allow running these sessions using a context manager:
-        
-        .. code-block:: python
-        
-            import pykarbon.pykarbon as pk
-            import pykarbon.can as pkc
-        
-            with pk.Karbon() as dev:
-                dev.show_info()
-        
-            with pkc.Session() as dev:
-                dev.write(0x123, 0x11223344)
-        
-        
-        -------------------------------
-        A Simple Example: Pykarbon.Core
-        -------------------------------
-        
-        .. code-block:: python
-        
-            import pykarbon.core as pkcore
-        
-            # Set up interfaces:
-            can = pkcore.Can()
-            term = pkcore.Terminal()
-        
-            # Claim the serial ports for use:
-            can.claim()
-            term.claim()
-        
-            # Configure the can baudrate, and view that config
-            term.command('set can-baudrate 800')
-        
-            print("\nRead User Configuration:")
-            term.print_command('config')
-        
-            # Write a message, and then listen for and print responses
-            can.send(0x123, 0x11223344)
-        
-            print("\nMonitoring CAN Bus, Press CTRL+C to Stop!")
-            can.sniff() # Will block until you exit with ctrl+c
-        
-            # Close the ports!
-            can.release()
-            term.release()
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+License-File: LICENSE.txt
+
+===============
+Pykarbon Module
+===============
+For the full rundown, read `the rest of the docs <https://pykarbon.readthedocs.io/en/latest/>`_.
+
+-----------
+What is it?
+-----------
+
+The Pykarbon module provides a set of tools for interfacing with the hardware devices on
+OnLogic's 'Karbon' series industrial PCs. These interfaces include the onboard CAN bus,
+Digital IO, and a few other hardware devices.
+
+The goal of this package is to provide a simple, but powerful, base platform that will allow
+users to quickly and easily integrate a Karbon into their own application.
+
+*The tools in this package are designed to work with specific hardware;
+this will not work for more generalized projects*
+
+----------------
+How do I use it?
+----------------
+
+*You will need to install python 3 prior to following this guide.*
+
+Getting started with pykarbon takes only a few minutes:
+
+.. role:: bash(code)
+   :language: bash
+
+- Open up a terminal, and run :bash:`pip install pykarbon`
+
+  + On some systems you may need to run as admin, or use the :bash:`--user` flag
+
+- Launch a python shell with :bash:`python`
+
+  + Usually linux users do not have write access to serial ports; grant your user permanent access with :bash:`usermod -a -G dialout $USER` or use :bash:`sudo python`
+
+.. role:: python(code)
+   :language: python
+
+- Import pykarbon with :python:`import pykarbon.pykarbon as pk`
+- And finally create a control object using :python:`dev = pk.Karbon()`
+
+If all went well, you should now be ready to control a variety of systems, but for now, let's just print out some
+configuration information:
+
+- :python:`dev.show_info()`
+
+And close our session:
+
+- :python:`dev.close()`
+
+-------------------
+What else can I do?
+-------------------
+
+Pykarbon offers a number of tools for automating and using Karbon series hardware interfaces. These include:
+
+- CAN and DIO background data monitoring
+- Exporting logged data to .csv
+- Registering and making function calls based on these bus events:
+
+  + CAN data IDs
+  + Digital Input Events
+  + DIO Bus States (Allows partial states)
+
+- Automated can message response to registered IDs
+- Automated setting of Digital Output states
+- Automatic CAN baudrate detection
+- Updating user configuration information:
+
+  + Ignition sense enable/disable
+  + Power timing configurations
+  + Low battery shutdown voltage
+  + Etc.
+
+- Firmware update
+
+Additonally, as Pykarbon's CAN and Terminal sessions must connect to device serial ports, functionality has been added
+to allow running these sessions using a context manager:
+
+.. code-block:: python
+
+    import pykarbon.pykarbon as pk
+    import pykarbon.can as pkc
+
+    with pk.Karbon() as dev:
+        dev.show_info()
+
+    with pkc.Session() as dev:
+        dev.write(0x123, 0x11223344)
+
+
+-------------------------------
+A Simple Example: Pykarbon.Core
+-------------------------------
+
+.. code-block:: python
+
+    import pykarbon.core as pkcore
+
+    # Set up interfaces:
+    can = pkcore.Can()
+    term = pkcore.Terminal()
+
+    # Claim the serial ports for use:
+    can.claim()
+    term.claim()
+
+    # Configure the can baudrate, and view that config
+    term.command('set can-baudrate 800')
+
+    print("\nRead User Configuration:")
+    term.print_command('config')
+
+    # Write a message, and then listen for and print responses
+    can.send(0x123, 0x11223344)
+
+    print("\nMonitoring CAN Bus, Press CTRL+C to Stop!")
+    can.sniff() # Will block until you exit with ctrl+c
+
+    # Close the ports!
+    can.release()
+    term.release()
+
+
```

### Comparing `pykarbon-1.1.9/scripts/update_karbon_firmware` & `pykarbon-1.2.0/scripts/update_karbon_firmware`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     except FileNotFoundError:
         rtval = 3
 
     return rtval
 
 
 def update_firmware(binary_file):
-    ''' Update the K300 firware with specified binary update file '''
+    ''' Update the K300 firmware with specified binary update file '''
 
     print("Starting update...")
 
     # Check file is OK
     file_error = check_file(binary_file)
     if file_error:
         return file_error
```

### Comparing `pykarbon-1.1.9/pykarbon.egg-info/PKG-INFO` & `pykarbon-1.2.0/pykarbon.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,148 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pykarbon
-Version: 1.1.9
+Version: 1.2.0
 Summary: Tools for Karbon hardware interfaces.
 Home-page: https://github.com/onlogic/Pykarbon
 Author: OnLogic
-Author-email: jacob.caughfield@onlogic.com
+Author-email: firmwareengineeringteam@onlogic.com
 License: BSD-2.0
-Description: ===============
-        Pykarbon Module
-        ===============
-        For the full rundown, read `the rest of the docs <https://pykarbon.readthedocs.io/en/latest/>`_.
-        
-        -----------
-        What is it?
-        -----------
-        
-        The Pykarbon module provides a set of tools for interfacing with the hardware devices on
-        OnLogic's 'Karbon' series industrial PCs. These interfaces include the onboard CAN bus,
-        Digital IO, and a few other hardware devices.
-        
-        The goal of this package is to provide a simple, but powerful, base platform that will allow
-        users to quickly and easily integrate a Karbon into their own application.
-        
-        *The tools in this package are designed to work with specific hardware;
-        this will not work for more generalized projects*
-        
-        ----------------
-        How do I use it?
-        ----------------
-        
-        *You will need to install python 3 prior to following this guide.*
-        
-        Getting started with pykarbon takes only a few minutes:
-        
-        .. role:: bash(code)
-           :language: bash
-        
-        - Open up a terminal, and run :bash:`pip install pykarbon`
-        
-          + On some systems you may need to run as admin, or use the :bash:`--user` flag
-        
-        - Launch a python shell with :bash:`python`
-        
-          + Usually linux users do not have write access to serial ports; grant your user permanent access with :bash:`usermod -a -G dialout $USER` or use :bash:`sudo python`
-        
-        .. role:: python(code)
-           :language: python
-        
-        - Import pykarbon with :python:`import pykarbon.pykarbon as pk`
-        - And finally create a control object using :python:`dev = pk.Karbon()`
-        
-        If all went well, you should now be ready to control a variety of systems, but for now, let's just print out some
-        configuration information:
-        
-        - :python:`dev.show_info()`
-        
-        And close our session:
-        
-        - :python:`dev.close()`
-        
-        -------------------
-        What else can I do?
-        -------------------
-        
-        Pykarbon offers a number of tools for automating and using Karbon series hardware interfaces. These include:
-        
-        - CAN and DIO background data monitoring
-        - Exporting logged data to .csv
-        - Registering and making function calls based on these bus events:
-        
-          + CAN data IDs
-          + Digital Input Events
-          + DIO Bus States (Allows partial states)
-        
-        - Automated can message response to registered IDs
-        - Automated setting of Digital Output states
-        - Automatic CAN baudrate detection
-        - Updating user configuration information:
-        
-          + Ignition sense enable/disable
-          + Power timing configurations
-          + Low battery shutdown voltage
-          + Etc.
-        
-        - Firmware update
-        
-        Additonally, as Pykarbon's CAN and Terminal sessions must connect to device serial ports, functionality has been added
-        to allow running these sessions using a context manager:
-        
-        .. code-block:: python
-        
-            import pykarbon.pykarbon as pk
-            import pykarbon.can as pkc
-        
-            with pk.Karbon() as dev:
-                dev.show_info()
-        
-            with pkc.Session() as dev:
-                dev.write(0x123, 0x11223344)
-        
-        
-        -------------------------------
-        A Simple Example: Pykarbon.Core
-        -------------------------------
-        
-        .. code-block:: python
-        
-            import pykarbon.core as pkcore
-        
-            # Set up interfaces:
-            can = pkcore.Can()
-            term = pkcore.Terminal()
-        
-            # Claim the serial ports for use:
-            can.claim()
-            term.claim()
-        
-            # Configure the can baudrate, and view that config
-            term.command('set can-baudrate 800')
-        
-            print("\nRead User Configuration:")
-            term.print_command('config')
-        
-            # Write a message, and then listen for and print responses
-            can.send(0x123, 0x11223344)
-        
-            print("\nMonitoring CAN Bus, Press CTRL+C to Stop!")
-            can.sniff() # Will block until you exit with ctrl+c
-        
-            # Close the ports!
-            can.release()
-            term.release()
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+License-File: LICENSE.txt
+
+===============
+Pykarbon Module
+===============
+For the full rundown, read `the rest of the docs <https://pykarbon.readthedocs.io/en/latest/>`_.
+
+-----------
+What is it?
+-----------
+
+The Pykarbon module provides a set of tools for interfacing with the hardware devices on
+OnLogic's 'Karbon' series industrial PCs. These interfaces include the onboard CAN bus,
+Digital IO, and a few other hardware devices.
+
+The goal of this package is to provide a simple, but powerful, base platform that will allow
+users to quickly and easily integrate a Karbon into their own application.
+
+*The tools in this package are designed to work with specific hardware;
+this will not work for more generalized projects*
+
+----------------
+How do I use it?
+----------------
+
+*You will need to install python 3 prior to following this guide.*
+
+Getting started with pykarbon takes only a few minutes:
+
+.. role:: bash(code)
+   :language: bash
+
+- Open up a terminal, and run :bash:`pip install pykarbon`
+
+  + On some systems you may need to run as admin, or use the :bash:`--user` flag
+
+- Launch a python shell with :bash:`python`
+
+  + Usually linux users do not have write access to serial ports; grant your user permanent access with :bash:`usermod -a -G dialout $USER` or use :bash:`sudo python`
+
+.. role:: python(code)
+   :language: python
+
+- Import pykarbon with :python:`import pykarbon.pykarbon as pk`
+- And finally create a control object using :python:`dev = pk.Karbon()`
+
+If all went well, you should now be ready to control a variety of systems, but for now, let's just print out some
+configuration information:
+
+- :python:`dev.show_info()`
+
+And close our session:
+
+- :python:`dev.close()`
+
+-------------------
+What else can I do?
+-------------------
+
+Pykarbon offers a number of tools for automating and using Karbon series hardware interfaces. These include:
+
+- CAN and DIO background data monitoring
+- Exporting logged data to .csv
+- Registering and making function calls based on these bus events:
+
+  + CAN data IDs
+  + Digital Input Events
+  + DIO Bus States (Allows partial states)
+
+- Automated can message response to registered IDs
+- Automated setting of Digital Output states
+- Automatic CAN baudrate detection
+- Updating user configuration information:
+
+  + Ignition sense enable/disable
+  + Power timing configurations
+  + Low battery shutdown voltage
+  + Etc.
+
+- Firmware update
+
+Additonally, as Pykarbon's CAN and Terminal sessions must connect to device serial ports, functionality has been added
+to allow running these sessions using a context manager:
+
+.. code-block:: python
+
+    import pykarbon.pykarbon as pk
+    import pykarbon.can as pkc
+
+    with pk.Karbon() as dev:
+        dev.show_info()
+
+    with pkc.Session() as dev:
+        dev.write(0x123, 0x11223344)
+
+
+-------------------------------
+A Simple Example: Pykarbon.Core
+-------------------------------
+
+.. code-block:: python
+
+    import pykarbon.core as pkcore
+
+    # Set up interfaces:
+    can = pkcore.Can()
+    term = pkcore.Terminal()
+
+    # Claim the serial ports for use:
+    can.claim()
+    term.claim()
+
+    # Configure the can baudrate, and view that config
+    term.command('set can-baudrate 800')
+
+    print("\nRead User Configuration:")
+    term.print_command('config')
+
+    # Write a message, and then listen for and print responses
+    can.send(0x123, 0x11223344)
+
+    print("\nMonitoring CAN Bus, Press CTRL+C to Stop!")
+    can.sniff() # Will block until you exit with ctrl+c
+
+    # Close the ports!
+    can.release()
+    term.release()
+
+
```

