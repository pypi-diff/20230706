# Comparing `tmp/era_5g_client-0.2.0.tar.gz` & `tmp/era_5g_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_client-0.2.0.tar", last modified: Mon Mar 20 08:50:34 2023, max compression
+gzip compressed data, was "era_5g_client-0.3.0.tar", last modified: Thu Jul  6 12:58:31 2023, max compression
```

## Comparing `era_5g_client-0.2.0.tar` & `era_5g_client-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-20 08:50:34.852870 era_5g_client-0.2.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      420 2023-03-20 08:50:34.852870 era_5g_client-0.2.0/PKG-INFO
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      625 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/backend_shim.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-20 08:50:34.852870 era_5g_client-0.2.0/era_5g_client/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    11364 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/client.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     9387 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/client_base.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1719 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/data_sender_gstreamer.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2813 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/data_sender_gstreamer_from_file.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2904 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/data_sender_gstreamer_from_source.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      986 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/dataclasses.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      662 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/exceptions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2636 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/middleware_resource_checker.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client/py.typed
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-20 08:50:34.852870 era_5g_client-0.2.0/era_5g_client.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      420 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      609 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       78 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       14 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/era_5g_client.egg-info/top_level.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-03-20 08:50:34.852870 era_5g_client-0.2.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      944 2023-03-20 08:50:34.000000 era_5g_client-0.2.0/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.643878 era_5g_client-0.3.0/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      420 2023-07-06 12:58:31.643878 era_5g_client-0.3.0/PKG-INFO
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      749 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/backend_shim.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.639879 era_5g_client-0.3.0/era_5g_client/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    11907 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/client.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6599 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/client_base.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1759 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2813 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer_from_file.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2904 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer_from_source.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      986 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/dataclasses.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      662 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/exceptions.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2635 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/middleware_resource_checker.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client/py.typed
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 12:58:31.643878 era_5g_client-0.3.0/era_5g_client.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      420 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      609 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      127 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       14 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/era_5g_client.egg-info/top_level.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-06 12:58:31.643878 era_5g_client-0.3.0/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1015 2023-07-06 12:58:31.000000 era_5g_client-0.3.0/setup.py
```

### Comparing `era_5g_client-0.2.0/backend_shim.py` & `era_5g_client-0.3.0/backend_shim.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 # DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
 
 import os
 import setuptools.build_meta
 
 backend = setuptools.build_meta.__legacy__
 
-dist_dir = "dist"
+dist_dir = "dist/"
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `era_5g_client-0.2.0/era_5g_client/client.py` & `era_5g_client-0.3.0/era_5g_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from collections.abc import Callable
 from enum import Enum
 from typing import Dict, List, Optional, Tuple
 
 import numpy as np
 import requests
-from requests import HTTPError, Response
+from requests import HTTPError
 
 from era_5g_client.client_base import NetAppClientBase
 from era_5g_client.dataclasses import MiddlewareInfo, NetAppLocation
 from era_5g_client.exceptions import FailedToConnect, NetAppNotReady
 from era_5g_client.middleware_resource_checker import MiddlewareResourceChecker
 
 buffer: List[Tuple[np.ndarray, Optional[str]]] = []
@@ -36,32 +36,39 @@
     """
 
     def __init__(
         self,
         results_event: Callable,
         image_error_event: Optional[Callable] = None,
         json_error_event: Optional[Callable] = None,
+        control_cmd_event: Optional[Callable] = None,
+        control_cmd_error_event: Optional[Callable] = None,
     ) -> None:
         """Constructor.
 
         Args:
-            results_event (Callable): callback where results will arrive
+            results_event (Callable): Callback where results will arrive.
             image_error_event (Callable, optional): Callback which is emitted when server
                 failed to process the incoming image.
             json_error_event (Callable, optional): Callback which is emitted when server
                 failed to process the incoming json data.
+            control_cmd_event (Callable, optional): Callback for receiving data that are
+                sent as a result of performing a control command (e.g. NetApp state
+                obtained by get-state command).
+            control_cmd_error_event (Callable, optional): Callback which is emited when
+                server failed to process the incoming control command.
 
         Raises:
             FailedToConnect: When connection to the middleware could not be set or
                 login failed
             FailedToObtainPlan: When the plan was not successfully returned from
                 the middleware
         """
 
-        super().__init__(results_event, image_error_event, json_error_event)
+        super().__init__(results_event, image_error_event, json_error_event, control_cmd_event, control_cmd_error_event)
 
         self.host: Optional[str] = None
         self.action_plan_id: Optional[str] = None
         self.resource_checker: Optional[MiddlewareResourceChecker] = None
         self.middleware_info: Optional[MiddlewareInfo] = None
         self.token: Optional[str] = None
 
@@ -87,16 +94,14 @@
 
     def run_task(
         self,
         task_id: str,
         robot_id: str,
         resource_lock: bool,
         mode: Optional[RunTaskMode] = RunTaskMode.WAIT_AND_REGISTER,
-        gstreamer: Optional[bool] = False,
-        ws_data: Optional[bool] = False,
         args: Optional[Dict] = None,
     ) -> None:
         """Deploys the task with provided *task_id* using middleware and
         (optionally) waits until the netapp is ready and register with it.
 
         Args:
             task_id (str): The GUID of the task which should be deployed.
@@ -135,37 +140,38 @@
             self.resource_checker.start()
             if mode in [RunTaskMode.WAIT, RunTaskMode.WAIT_AND_REGISTER]:
                 self.wait_until_netapp_ready()
                 self.load_netapp_address()
                 if not self.netapp_location:
                     raise FailedToConnect("Failed to obtain NetApp URI or port")
                 if mode == RunTaskMode.WAIT_AND_REGISTER:
-                    self.register(self.netapp_location, gstreamer, ws_data, args)
+                    self.register(self.netapp_location, args)
         except (FailedToConnect, NetAppNotReady) as ex:
             self.delete_all_resources()
             logging.error(f"Failed to run task: {ex}")
             raise
 
     def register(
         self,
         netapp_location: NetAppLocation,
-        gstreamer: Optional[bool] = False,
-        ws_data: Optional[bool] = False,
         args: Optional[Dict] = None,
-    ) -> Response:
+    ) -> None:
         """Calls the /register endpoint of the NetApp interface and if the
         registration is successful, it sets up the WebSocket connection for
         results retrieval.
 
         Args:
             netapp_location (NetAppLocation): The URI and port of the NetApp interface.
             gstreamer (Optional[bool], optional):  Indicates if a GStreamer pipeline
                 should be initialized for image transport. Defaults to False.
             ws_data (Optional[bool], optional): Indicates if a separate websocket channel
                 for data transport should be set. Defaults to False.
+            use_control_cmds (Optional[bool], optional): Indicates if a websocket channel
+                for control commands should be used. Control commands are indended for
+                changing the internal state of a stateful NetApp. Defaults to False.
             args (Optional[Dict], optional): NetApp-specific arguments. Defaults to None.
 
         Raises:
             NetAppNotReady: Raised when register called before the NetApp is ready.
 
         Returns:
             Response: The response from the NetApp.
@@ -173,17 +179,15 @@
 
         if not self.resource_checker:
             raise NetAppNotReady("Not connected to the middleware.")
 
         if not self.resource_checker.is_ready():
             raise NetAppNotReady("Not ready.")
 
-        response = super().register(netapp_location, gstreamer, ws_data, args)
-
-        return response
+        super().register(netapp_location, args)
 
     def disconnect(self) -> None:
         """Calls the /unregister endpoint of the server and disconnects the
         WebSocket connection."""
         super().disconnect()
         if self.resource_checker is not None:
             self.resource_checker.stop()
```

### Comparing `era_5g_client-0.2.0/era_5g_client/data_sender_gstreamer.py` & `era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,21 +22,22 @@
         self.fps = fps
         self.threads = threads
         self.width = width
         self.height = height
 
         # default pipeline for sending h264 encoded stream
         # ultrafast and zero latency params for near real-time processing
-        gst_str_rtp = (
-            "appsrc ! videoconvert ! queue ! x264enc "
-            + "speed-preset=ultrafast  tune=zerolatency  byte-stream=true "
-            + f"threads={self.threads} key-int-max=15 intra-refresh=true ! h264parse ! "
-            + f"rtph264pay ! queue ! udpsink host={self.host} port={self.gstreamer_port}"
+        pipeline = (
+            "appsrc is-live=true ! videoconvert ! "
+            "x264enc speed-preset=ultrafast tune=zerolatency byte-stream=true "
+            f"threads={self.threads} key-int-max=15 intra-refresh=true ! h264parse ! "
+            f"rtph264pay ! udpsink host={self.host} port={self.gstreamer_port}"
         )
-        self.out = cv2.VideoWriter(gst_str_rtp, cv2.CAP_GSTREAMER, 0, fps, (width, height), True)
+        self.out = cv2.VideoWriter(pipeline, cv2.CAP_GSTREAMER, 0, fps, (width, height), True)
         # TODO: How to check valid VideoWriter?
         if not self.out.isOpened():
             raise Exception("Cannot open VideoWriter pipeline")
+        # self.out.set(cv2.VIDEOWRITER_PROP_QUALITY, 10)
 
     def send_image(self, frame: np.ndarray) -> None:
         self.out.write(frame)
         # TODO: How to check valid write?
```

### Comparing `era_5g_client-0.2.0/era_5g_client/data_sender_gstreamer_from_file.py` & `era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer_from_file.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.2.0/era_5g_client/data_sender_gstreamer_from_source.py` & `era_5g_client-0.3.0/era_5g_client/data_sender_gstreamer_from_source.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.2.0/era_5g_client/dataclasses.py` & `era_5g_client-0.3.0/era_5g_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.2.0/era_5g_client/exceptions.py` & `era_5g_client-0.3.0/era_5g_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.2.0/era_5g_client/middleware_resource_checker.py` & `era_5g_client-0.3.0/era_5g_client/middleware_resource_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
                 raise FailedToConnect("Invalid response.")
 
         except HTTPError as e:
             print(e.response.status_code)
             raise FailedToConnect("Could not get the resource status, revisit the log files for more details.")
 
     def wait_until_resource_ready(self, timeout: int = -1) -> None:
-
         while not self.stop_event.is_set():
             # if timeout < 0 and time.time() < timeout:
             #    raise TimeoutError
 
             if self.is_ready():
                 return
             time.sleep(0.1)
```

### Comparing `era_5g_client-0.2.0/era_5g_client.egg-info/SOURCES.txt` & `era_5g_client-0.3.0/era_5g_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.2.0/setup.py` & `era_5g_client-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,29 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
     ],
     'description': 'A client for 5G-ERA NetApps',
     'install_requires': (
-        'numpy~=1.24.2',
-        'opencv-python~=4.6.0.37',
-        'python-socketio~=5.7.2',
-        'requests~=2.28.2',
+        'era-5g-interface~=0.3.0',
+        'numpy~=1.24.4',
+        'opencv-python~=4.6.0.66',
+        'python-socketio~=5.8.0',
+        'requests~=2.31.0',
+        'types-requests==2.31.0.1',
     ),
     'license': 'LGPL',
     'name': 'era_5g_client',
     'namespace_packages': (
     ),
     'package_data': {
         'era_5g_client': (
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_client',
     ),
     'python_requires': '>=3.8,<3.11',
-    'version': '0.2.0',
+    'version': '0.3.0',
 })
```

