# Comparing `tmp/pymycobot-3.1.3.tar.gz` & `tmp/pymycobot-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.1.3.tar", last modified: Tue Jun 27 03:25:27 2023, max compression
+gzip compressed data, was "pymycobot-3.1.5.tar", last modified: Thu Jul  6 03:10:49 2023, max compression
```

## Comparing `pymycobot-3.1.3.tar` & `pymycobot-3.1.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 03:25:27.086076 pymycobot-3.1.3/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.3/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0    59140 2023-06-27 03:25:27.085080 pymycobot-3.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 03:25:27.054361 pymycobot-3.1.3/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.3/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1554 2023-06-27 03:25:13.000000 pymycobot-3.1.3/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.3/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    12276 2023-06-15 06:45:38.000000 pymycobot-3.1.3/pymycobot/common.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.3/pymycobot/error.py
--rw-rw-rw-   0        0        0    33758 2023-06-15 06:42:33.000000 pymycobot-3.1.3/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.3/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.3/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.3/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     9080 2023-06-27 03:24:18.000000 pymycobot-3.1.3/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13314 2023-06-27 03:24:50.000000 pymycobot-3.1.3/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.3/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.3/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.3/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7566 2023-06-27 03:24:05.000000 pymycobot-3.1.3/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.3/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8548 2023-06-27 03:24:57.000000 pymycobot-3.1.3/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.3/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.3/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.3/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:25:27.083077 pymycobot-3.1.3/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    59140 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 03:25:26.000000 pymycobot-3.1.3/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 03:25:27.086076 pymycobot-3.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:10:49.008346 pymycobot-3.1.5/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.5/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    59799 2023-07-06 03:10:49.007334 pymycobot-3.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 03:10:48.970371 pymycobot-3.1.5/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.5/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1627 2023-07-06 02:42:11.000000 pymycobot-3.1.5/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.5/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    12339 2023-07-06 02:36:59.000000 pymycobot-3.1.5/pymycobot/common.py
+-rw-rw-rw-   0        0        0     9159 2023-07-05 06:05:50.000000 pymycobot-3.1.5/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.5/pymycobot/error.py
+-rw-rw-rw-   0        0        0    34521 2023-07-06 02:36:43.000000 pymycobot-3.1.5/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.5/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.5/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.5/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     9080 2023-06-27 03:24:18.000000 pymycobot-3.1.5/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13314 2023-06-27 03:24:50.000000 pymycobot-3.1.5/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.5/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.5/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.5/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     7725 2023-07-06 02:40:02.000000 pymycobot-3.1.5/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.5/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     8707 2023-07-06 02:41:09.000000 pymycobot-3.1.5/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.5/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19696 2023-06-27 03:25:03.000000 pymycobot-3.1.5/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.5/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:10:49.005329 pymycobot-3.1.5/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    59799 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 03:10:48.000000 pymycobot-3.1.5/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:10:49.009351 pymycobot-3.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.5/setup.py
```

### Comparing `pymycobot-3.1.3/LICENSE` & `pymycobot-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/PKG-INFO` & `pymycobot-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.3
+Version: 3.1.5
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
@@ -177,14 +177,16 @@
     - [set\_end\_type](#set_end_type)
     - [get\_end\_type](#get_end_type)
     - [get\_plan\_speed](#get_plan_speed)
     - [get\_plan\_acceleration](#get_plan_acceleration)
     - [set\_plan\_speed](#set_plan_speed)
     - [set\_plan\_acceleration](#set_plan_acceleration)
     - [set\_gservo\_round](#set_gservo_round)
+    - [get\_basic\_version](#get_basic_version)
+    - [set\_communicate\_mode](#set_communicate_mode)
     - [get\_servo\_speeds](#get_servo_speeds)
     - [get\_servo\_currents](#get_servo_currents)
     - [get\_servo\_voltages](#get_servo_voltages)
     - [get\_servo\_status](#get_servo_status)
     - [get\_servo\_temps](#get_servo_temps)
     - [init\_eletric\_gripper](#init_eletric_gripper)
     - [set\_eletric\_gripper](#set_eletric_gripper)
@@ -1185,18 +1187,46 @@
 
   - `acceleration` (`int`) 0 - 100.
   - `is_linear` (`int`): 0 / 1 (0 ->joint, 1 -> line)
 
 
 ### set_gservo_round
 
-- **Prototype**: `set_gservo_round()`
+- **Prototype**: `set_gservo_round(angle)`
 
 - **Description**: Drive the 9g steering gear clockwise for one revolution.
 
+- **Parameters**
+
+  - `angle` (`int`) 0 - 255.
+      0 : stop
+      255 : Keep turning
+      1 ~ 254: Based on 30° (1->30°, 2->60°)
+
+### get_basic_version
+
+- **Prototype**: `get_basic_version()`
+
+- **Description**: Get basic firmware version.
+
+- **Return**
+
+  - `version` (`float`)
+
+### set_communicate_mode
+
+- **Prototype**: `set_communicate_mode(mode)`
+
+- **Description**: Set basic communication mode.
+
+- **Parameters**
+
+  - `mode` (`int`) 0 -  Turn off transparent transmission. 1 - Open transparent transmission
+
+
 ### get_servo_speeds
 
 - **Prototype**: `get_servo_speeds()`
 
 - **Description**: Get joint velocity.
 
 - **Return**: `list` Speed of each joint.
```

### Comparing `pymycobot-3.1.3/README.md` & `pymycobot-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/Interface.py` & `pymycobot-3.1.5/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/__init__.py` & `pymycobot-3.1.5/pymycobot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from pymycobot.genre import Angle, Coord
 from pymycobot import utils
 from pymycobot.mybuddysocket import MyBuddySocket
 from pymycobot.ultraArm import ultraArm
 from pymycobot.mybuddybluetooth import MyBuddyBlueTooth
 from pymycobot.mypalletizersocket import MyPalletizerSocket
 from pymycobot.myarm import MyArm
+from pymycobot.elephantrobot import ElephantRobot
 
 __all__ = [
     "MyCobot",
     "MyCobotCommandGenerator",
     "Angle",
     "Coord",
     "utils",
@@ -30,23 +31,24 @@
     "MyBuddyCommandGenerator",
     "MyBuddy",
     "MyBuddySocket",
     "MyBuddyBlueTooth",
     "ultraArm",
     "MyPalletizerSocket",
     "MechArm",
-    "MyArm"
+    "MyArm",
+    "ElephantRobot"
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.1.3"
+__version__ = "3.1.5"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.1.3/pymycobot/bluet.py` & `pymycobot-3.1.5/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/common.py` & `pymycobot-3.1.5/pymycobot/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,16 @@
     # set WIFI
     SET_SSID_PWD = 0xB0
     GET_SSID_PWD = 0xB1
     SET_SERVER_PORT = 0xB2
 
     # Get the measured distance
     GET_TOF_DISTANCE = 0xC0
+    GET_BASIC_VERSION = 0xC1
+    SET_COMMUNICATE_MODE = 0xC2
 
     # Coordinate transformation
     SET_TOOL_REFERENCE = 0x81
     GET_TOOL_REFERENCE = 0x82
     SET_WORLD_REFERENCE = 0x83
     GET_WORLD_REFERENCE = 0x84
     SET_REFERENCE_FRAME = 0x85
```

### Comparing `pymycobot-3.1.3/pymycobot/error.py` & `pymycobot-3.1.5/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/generate.py` & `pymycobot-3.1.5/pymycobot/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,21 @@
         return self._mesg(ProtocolCode.IS_POWER_ON, has_reply=True)
 
     def release_all_servos(self):
         """Relax all joints"""
         return self._mesg(ProtocolCode.RELEASE_ALL_SERVOS)
 
     def is_controller_connected(self):
-        """Wether connected with Atom."""
+        """Wether connected with Atom.
+        
+        Return:
+            1 - succeed
+            0 - failed
+            -1 - error data
+        """
         return self._mesg(ProtocolCode.IS_CONTROLLER_CONNECTED, has_reply=True)
 
     def read_next_error(self):
         """Robot Error Detection
         
         Return:
             list len 7.
@@ -1021,10 +1027,30 @@
         """
         return self._mesg(ProtocolCode.GET_ERROR_INFO, has_reply = True)
     
     def clear_error_information(self):
         """Clear robot error message"""
         return self._mesg(ProtocolCode.CLEAR_ERROR_INFO, has_reply = True)
     
-    def set_gservo_round(self):
-        """Drive the 9g steering gear clockwise for one revolution"""
-        return self._mesg(ProtocolCode.SET_GSERVO_ROUND)
+    def set_gservo_round(self, angle):
+        """Drive the 9g steering gear clockwise for one revolution
+        
+        Args:
+            angle (int): 0 ~ 255
+                0 : stop
+                255 : Keep turning
+                1 ~ 254: Based on 30° (1->30°, 2->60°)
+        """
+        return self._mesg(ProtocolCode.SET_GSERVO_ROUND, angle)
+
+
+    def get_basic_version(self):
+        """Get basic firmware version"""
+        return self._mesg(ProtocolCode.GET_BASIC_VERSION, has_reply = True)
+    
+    def set_communicate_mode(self, mode):
+        """Set basic communication mode
+        
+        Args:
+            mode: 0 - Turn off transparent transmission，1 - Open transparent transmission
+        """
+        return self._mesg(ProtocolCode.SET_COMMUNICATE_MODE, mode)
```

### Comparing `pymycobot-3.1.3/pymycobot/log.py` & `pymycobot-3.1.5/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/myarm.py` & `pymycobot-3.1.5/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/mybuddy.py` & `pymycobot-3.1.5/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/mybuddybluetooth.py` & `pymycobot-3.1.5/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/mybuddyemoticon.py` & `pymycobot-3.1.5/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/mybuddysocket.py` & `pymycobot-3.1.5/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/mycobot.py` & `pymycobot-3.1.5/pymycobot/mycobot.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,14 +125,16 @@
                     return r
                 else:
                     return res
             elif genre in [ProtocolCode.GET_SERVO_VOLTAGES]:
                 return [self._int2coord(angle) for angle in res]
             elif genre in [ProtocolCode.GET_JOINT_MAX_ANGLE, ProtocolCode.GET_JOINT_MIN_ANGLE]:
                 return self._int2coord(res[0])
+            elif genre in [ProtocolCode.GET_BASIC_VERSION, ProtocolCode.SOFTWARE_VERSION]:
+                return self._int2coord(self._process_single(res))
             else:
                 return res
         return None
 
     def get_radians(self):
         """Get the radians of all joints
```

### Comparing `pymycobot-3.1.3/pymycobot/mycobotsocket.py` & `pymycobot-3.1.5/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/mypalletizer.py` & `pymycobot-3.1.5/pymycobot/mypalletizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,16 @@
                 else:
                     return res
             elif genre in [
                 ProtocolCode.GET_JOINT_MIN_ANGLE,
                 ProtocolCode.GET_JOINT_MAX_ANGLE,
             ]:
                 return self._int2angle(res[0]) if res else 0
+            elif genre in [ProtocolCode.GET_BASIC_VERSION, ProtocolCode.SOFTWARE_VERSION]:
+                return self._int2coord(self._process_single(res))
             else:
                 return res
         return None
 
     def get_radians(self):
         """Get all angle return a list
```

### Comparing `pymycobot-3.1.3/pymycobot/mypalletizersocket.py` & `pymycobot-3.1.5/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/ultraArm.py` & `pymycobot-3.1.5/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot/utils.py` & `pymycobot-3.1.5/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.3/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.1.5/pymycobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.3
+Version: 3.1.5
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
@@ -177,14 +177,16 @@
     - [set\_end\_type](#set_end_type)
     - [get\_end\_type](#get_end_type)
     - [get\_plan\_speed](#get_plan_speed)
     - [get\_plan\_acceleration](#get_plan_acceleration)
     - [set\_plan\_speed](#set_plan_speed)
     - [set\_plan\_acceleration](#set_plan_acceleration)
     - [set\_gservo\_round](#set_gservo_round)
+    - [get\_basic\_version](#get_basic_version)
+    - [set\_communicate\_mode](#set_communicate_mode)
     - [get\_servo\_speeds](#get_servo_speeds)
     - [get\_servo\_currents](#get_servo_currents)
     - [get\_servo\_voltages](#get_servo_voltages)
     - [get\_servo\_status](#get_servo_status)
     - [get\_servo\_temps](#get_servo_temps)
     - [init\_eletric\_gripper](#init_eletric_gripper)
     - [set\_eletric\_gripper](#set_eletric_gripper)
@@ -1185,18 +1187,46 @@
 
   - `acceleration` (`int`) 0 - 100.
   - `is_linear` (`int`): 0 / 1 (0 ->joint, 1 -> line)
 
 
 ### set_gservo_round
 
-- **Prototype**: `set_gservo_round()`
+- **Prototype**: `set_gservo_round(angle)`
 
 - **Description**: Drive the 9g steering gear clockwise for one revolution.
 
+- **Parameters**
+
+  - `angle` (`int`) 0 - 255.
+      0 : stop
+      255 : Keep turning
+      1 ~ 254: Based on 30° (1->30°, 2->60°)
+
+### get_basic_version
+
+- **Prototype**: `get_basic_version()`
+
+- **Description**: Get basic firmware version.
+
+- **Return**
+
+  - `version` (`float`)
+
+### set_communicate_mode
+
+- **Prototype**: `set_communicate_mode(mode)`
+
+- **Description**: Set basic communication mode.
+
+- **Parameters**
+
+  - `mode` (`int`) 0 -  Turn off transparent transmission. 1 - Open transparent transmission
+
+
 ### get_servo_speeds
 
 - **Prototype**: `get_servo_speeds()`
 
 - **Description**: Get joint velocity.
 
 - **Return**: `list` Speed of each joint.
```

### Comparing `pymycobot-3.1.3/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.1.5/pymycobot.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 requirements.txt
 setup.py
 pymycobot/Interface.py
 pymycobot/__init__.py
 pymycobot/bluet.py
 pymycobot/common.py
+pymycobot/elephantrobot.py
 pymycobot/error.py
 pymycobot/generate.py
 pymycobot/genre.py
 pymycobot/log.py
 pymycobot/mecharm.py
 pymycobot/myarm.py
 pymycobot/mybuddy.py
```

### Comparing `pymycobot-3.1.3/setup.py` & `pymycobot-3.1.5/setup.py`

 * *Files identical despite different names*

