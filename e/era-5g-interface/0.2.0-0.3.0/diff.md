# Comparing `tmp/era_5g_interface-0.2.0.tar.gz` & `tmp/era_5g_interface-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_interface-0.2.0.tar", last modified: Mon Apr 24 11:45:28 2023, max compression
+gzip compressed data, was "era_5g_interface-0.3.0.tar", last modified: Thu Jul  6 09:18:53 2023, max compression
```

## Comparing `era_5g_interface-0.2.0.tar` & `era_5g_interface-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/PKG-INFO
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      625 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/backend_shim.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/era_5g_interface/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/py.typed
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1251 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/task_handler.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2837 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/task_handler_gstreamer.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      968 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/task_handler_gstreamer_internal_q.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1450 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/task_handler_internal_q.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/era_5g_interface.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      513 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       24 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       17 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/top_level.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      873 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.998852 era_5g_interface-0.3.0/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/PKG-INFO
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      749 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/backend_shim.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/era_5g_interface/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/__init__.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/era_5g_interface/dataclasses/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/dataclasses/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1285 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/dataclasses/control_command.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/py.typed
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1730 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/task_handler.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2837 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/task_handler_gstreamer.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      968 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/task_handler_gstreamer_internal_q.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2158 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/task_handler_internal_q.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/era_5g_interface/utils/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/utils/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5875 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface/utils/rate_timer.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-06 09:18:52.994852 era_5g_interface-0.3.0/era_5g_interface.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      674 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       17 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/era_5g_interface.egg-info/top_level.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-06 09:18:52.998852 era_5g_interface-0.3.0/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      972 2023-07-06 09:18:52.000000 era_5g_interface-0.3.0/setup.py
```

### Comparing `era_5g_interface-0.2.0/backend_shim.py` & `era_5g_interface-0.3.0/backend_shim.py`

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

### Comparing `era_5g_interface-0.2.0/era_5g_interface/task_handler.py` & `era_5g_interface-0.3.0/era_5g_interface/task_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import ABC, abstractmethod
 from threading import Event, Thread
 from typing import Optional
 
 import numpy as np
 
+from era_5g_interface.dataclasses.control_command import ControlCommand
+
 
 class TaskHandlerInitializationFailed(Exception):
     pass
 
 
 class TaskHandler(Thread, ABC):
     """Abstract class.
@@ -40,7 +42,23 @@
         Args:
             metadata (dict): Arbitrary dictionary with metadata related to the image.
                 The format is NetApp-specific.
             image (_type_): The image to be processed.
         """
 
         pass
+
+    @abstractmethod
+    def store_control_data(self, data: ControlCommand) -> None:
+        """This method is intended to pass control commands to the worker.
+
+        Args:
+            data (ControlCommand): ControlCommand with control data.
+        """
+
+        pass
+
+    @abstractmethod
+    def clear_storage(self) -> None:
+        """Clear storage used for communication with worker."""
+
+        pass
```

### Comparing `era_5g_interface-0.2.0/era_5g_interface/task_handler_gstreamer.py` & `era_5g_interface-0.3.0/era_5g_interface/task_handler_gstreamer.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.2.0/era_5g_interface/task_handler_gstreamer_internal_q.py` & `era_5g_interface-0.3.0/era_5g_interface/task_handler_gstreamer_internal_q.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.2.0/era_5g_interface/task_handler_internal_q.py` & `era_5g_interface-0.3.0/era_5g_interface/task_handler_internal_q.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from queue import Full, Queue
+from queue import Empty, Full, Queue
 
 import numpy as np
 
+from era_5g_interface.dataclasses.control_command import ControlCommand
 from era_5g_interface.task_handler import TaskHandler
 
 
 class TaskHandlerInternalQ(TaskHandler):
     """Task handler which takes care of passing the data to the python internal
     queue for future processing.
 
@@ -39,9 +40,32 @@
 
         try:
             self._q.put((metadata, image), block=False)
         except Full:
             pass
             # TODO: raise an exception
 
+    def store_control_data(self, data: ControlCommand) -> None:
+        """Pass control commands to the worker using internal queue.
+
+        Args:
+            data (ControlCommand): ControlCommand with control data.
+        """
+
+        try:
+            self._q.put((data), block=False)
+        except Full:
+            pass
+            # TODO: raise an exception
+
+    def clear_storage(self) -> None:
+        """Clear all items from internal queue."""
+
+        while not self._q.empty():
+            try:
+                self._q.get(block=False)
+            except Empty:
+                break
+            self._q.task_done()
+
     def run(self) -> None:
         pass
```

### Comparing `era_5g_interface-0.2.0/era_5g_interface.egg-info/SOURCES.txt` & `era_5g_interface-0.3.0/era_5g_interface.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,8 +8,12 @@
 era_5g_interface/task_handler_gstreamer_internal_q.py
 era_5g_interface/task_handler_internal_q.py
 era_5g_interface.egg-info/PKG-INFO
 era_5g_interface.egg-info/SOURCES.txt
 era_5g_interface.egg-info/dependency_links.txt
 era_5g_interface.egg-info/namespace_packages.txt
 era_5g_interface.egg-info/requires.txt
-era_5g_interface.egg-info/top_level.txt
+era_5g_interface.egg-info/top_level.txt
+era_5g_interface/dataclasses/__init__.py
+era_5g_interface/dataclasses/control_command.py
+era_5g_interface/utils/__init__.py
+era_5g_interface/utils/rate_timer.py
```

### Comparing `era_5g_interface-0.2.0/setup.py` & `era_5g_interface-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,27 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
     ],
     'description': 'An interface for 5G-ERA NetApps',
     'install_requires': (
-        'opencv-python~=4.6.0.37',
+        'numpy~=1.24.4',
+        'opencv-python~=4.6.0.66',
     ),
     'license': 'LGPL',
     'name': 'era_5g_interface',
     'namespace_packages': (
     ),
     'package_data': {
         'era_5g_interface': (
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_interface',
+        'era_5g_interface.dataclasses',
+        'era_5g_interface.utils',
     ),
     'python_requires': '>=3.8,<3.11',
-    'version': '0.2.0',
+    'version': '0.3.0',
 })
```

