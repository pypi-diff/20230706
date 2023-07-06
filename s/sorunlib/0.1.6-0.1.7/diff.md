# Comparing `tmp/sorunlib-0.1.6.tar.gz` & `tmp/sorunlib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorunlib-0.1.6.tar", last modified: Thu Jan 12 20:53:21 2023, max compression
+gzip compressed data, was "sorunlib-0.1.7.tar", last modified: Thu Jul  6 14:32:19 2023, max compression
```

## Comparing `sorunlib-0.1.6.tar` & `sorunlib-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:53:21.930644 sorunlib-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-12 20:53:08.000000 sorunlib-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-12 20:53:08.000000 sorunlib-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-01-12 20:53:21.930644 sorunlib-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-01-12 20:53:08.000000 sorunlib-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-12 20:53:21.930644 sorunlib-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-12 20:53:08.000000 sorunlib-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:53:21.926644 sorunlib-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:53:21.930644 sorunlib-0.1.6/src/sorunlib/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-12 20:53:08.000000 sorunlib-0.1.6/src/sorunlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-01-12 20:53:08.000000 sorunlib-0.1.6/src/sorunlib/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-12 20:53:21.930644 sorunlib-0.1.6/src/sorunlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-12 20:53:08.000000 sorunlib-0.1.6/src/sorunlib/acu.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-12 20:53:08.000000 sorunlib-0.1.6/src/sorunlib/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-01-12 20:53:08.000000 sorunlib-0.1.6/src/sorunlib/seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-01-12 20:53:08.000000 sorunlib-0.1.6/src/sorunlib/smurf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-01-12 20:53:08.000000 sorunlib-0.1.6/src/sorunlib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:53:21.930644 sorunlib-0.1.6/src/sorunlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-01-12 20:53:21.000000 sorunlib-0.1.6/src/sorunlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-12 20:53:21.000000 sorunlib-0.1.6/src/sorunlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 20:53:21.000000 sorunlib-0.1.6/src/sorunlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-12 20:53:21.000000 sorunlib-0.1.6/src/sorunlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-12 20:53:21.000000 sorunlib-0.1.6/src/sorunlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-01-12 20:53:08.000000 sorunlib-0.1.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:32:19.410709 sorunlib-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-06 14:32:01.000000 sorunlib-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 14:32:01.000000 sorunlib-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-06 14:32:19.410709 sorunlib-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-06 14:32:01.000000 sorunlib-0.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-06 14:32:19.410709 sorunlib-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-06 14:32:01.000000 sorunlib-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:32:19.402710 sorunlib-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:32:19.410709 sorunlib-0.1.7/src/sorunlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 14:32:01.000000 sorunlib-0.1.7/src/sorunlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-06 14:32:01.000000 sorunlib-0.1.7/src/sorunlib/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 14:32:19.410709 sorunlib-0.1.7/src/sorunlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 14:32:01.000000 sorunlib-0.1.7/src/sorunlib/acu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-06 14:32:01.000000 sorunlib-0.1.7/src/sorunlib/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-06 14:32:01.000000 sorunlib-0.1.7/src/sorunlib/seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-06 14:32:01.000000 sorunlib-0.1.7/src/sorunlib/smurf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-06 14:32:01.000000 sorunlib-0.1.7/src/sorunlib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:32:19.410709 sorunlib-0.1.7/src/sorunlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-06 14:32:19.000000 sorunlib-0.1.7/src/sorunlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-06 14:32:19.000000 sorunlib-0.1.7/src/sorunlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:32:19.000000 sorunlib-0.1.7/src/sorunlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-06 14:32:19.000000 sorunlib-0.1.7/src/sorunlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 14:32:19.000000 sorunlib-0.1.7/src/sorunlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:32:19.410709 sorunlib-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-06 14:32:01.000000 sorunlib-0.1.7/tests/test__internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-06 14:32:01.000000 sorunlib-0.1.7/tests/test_acu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-06 14:32:01.000000 sorunlib-0.1.7/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-06 14:32:01.000000 sorunlib-0.1.7/tests/test_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-06 14:32:01.000000 sorunlib-0.1.7/tests/test_smurf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-06 14:32:01.000000 sorunlib-0.1.7/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-07-06 14:32:01.000000 sorunlib-0.1.7/versioneer.py
```

### Comparing `sorunlib-0.1.6/LICENSE.txt` & `sorunlib-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.6/PKG-INFO` & `sorunlib-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorunlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: OCS Control Programs for running the observatory.
 Home-page: https://github.com/simonsobs/sorunlib
 Project-URL: Source Code, https://github.com/simonsobs/sorunlib
 Project-URL: Documentation, https://sorunlib.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/simonsobs/sorunlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sorunlib-0.1.6/README.rst` & `sorunlib-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.6/setup.py` & `sorunlib-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: BSD License",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Astronomy",
     ],
     python_requires=">=3.7",
     install_requires=[
-        'ocs==0.10.1',
+        'ocs==0.10.2',
     ],
     extras_require={
         "tests": ["pytest>=7.0.0", "pytest-cov>=3.0.0"],
-        "docs": ["sphinx==5.3.0", "sphinx_rtd_theme==1.1.1"],
+        "docs": ["sphinx>=5.3.0", "sphinx_rtd_theme>=1.1.1"],
     },
 )
```

### Comparing `sorunlib-0.1.6/src/sorunlib/__init__.py` & `sorunlib-0.1.7/src/sorunlib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import acu, seq, smurf
 
-from .commands import wait
+from .commands import wait_until
 from .util import create_clients
 
 CLIENTS = None
 
 
 def initialize(test_mode=False):
     """Initialize global clients list.
@@ -14,11 +14,11 @@
             are meant to stand in for real agents while testing, i.e.
             SmurfFileEmulators instead of PysmurfControllers.
     """
     global CLIENTS
     CLIENTS = create_clients(test_mode=test_mode)
 
 
-__all__ = ["acu", "seq", "smurf", "wait", "initialize"]
+__all__ = ["acu", "seq", "smurf", "wait_until", "initialize"]
 
 from . import _version
 __version__ = _version.get_versions()['version']
```

### Comparing `sorunlib-0.1.6/src/sorunlib/_internal.py` & `sorunlib-0.1.7/src/sorunlib/_internal.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.6/src/sorunlib/seq.py` & `sorunlib-0.1.7/src/sorunlib/seq.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 import sorunlib as run
 from sorunlib._internal import check_response
 
 
 OP_TIMEOUT = 60
 
 
-def scan(description, stop_time, width):
+def scan(description, stop_time, width, tag=None):
     """Run a constant elevation scan, collecting detector data.
 
     Args:
         description (str): Description of the field/object being scanned.
         stop_time (str): Time in ISO format to scan until, i.e.
             "2022-06-21T15:58:00"
         width (float): Scan width in azimuth. The scan will start at the
             current position and move in the positive azimuth direction.
+        tag (str, optional): Tag or comma-separated listed of tags to attach to
+            the operation. Passed through to the smurf stream command.
 
     """
     # Enable SMuRF streams
-    run.smurf.stream('on')
+    run.smurf.stream('on', tag=tag)
 
-    # Grab current telescope position
-    resp = run.CLIENTS['acu'].monitor.status()
-    az = resp.session['data']['Corrected Azimuth']
-    el = resp.session['data']['Corrected Elevation']
-
-    # Start telescope motion
-    resp = run.CLIENTS['acu'].generate_scan.start(az_endpoint1=az,
-                                                  az_endpoint2=az + width,
-                                                  az_speed=2,
-                                                  acc=2.0,
-                                                  el_endpoint1=el,
-                                                  el_endpoint2=el,
-                                                  el_speed=0)
-
-    # Wait until stop time
-    run.commands.wait(stop_time)
-
-    # Stop motion
-    run.CLIENTS['acu'].generate_scan.stop()
-    resp = run.CLIENTS['acu'].generate_scan.wait(timeout=OP_TIMEOUT)
-    check_response(resp)
+    try:
+        # Grab current telescope position
+        resp = run.CLIENTS['acu'].monitor.status()
+        az = resp.session['data']['StatusDetailed']['Corrected Azimuth']
+        el = resp.session['data']['StatusDetailed']['Corrected Elevation']
+
+        # Start telescope motion
+        resp = run.CLIENTS['acu'].generate_scan.start(az_endpoint1=az,
+                                                      az_endpoint2=az + width,
+                                                      az_speed=2,
+                                                      az_accel=2.0,
+                                                      el_endpoint1=el,
+                                                      el_endpoint2=el,
+                                                      el_speed=0)
+
+        if not resp.session:
+            raise Exception(f"Generate Scan failed to start:\n  {resp}")
+
+        # Wait until stop time
+        run.commands.wait_until(stop_time)
+    finally:
+        # Stop motion
+        run.CLIENTS['acu'].generate_scan.stop()
+        resp = run.CLIENTS['acu'].generate_scan.wait(timeout=OP_TIMEOUT)
+        check_response(resp)
 
-    # Stop SMuRF streams
-    run.smurf.stream('off')
+        # Stop SMuRF streams
+        run.smurf.stream('off')
```

### Comparing `sorunlib-0.1.6/src/sorunlib/util.py` & `sorunlib-0.1.7/src/sorunlib/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     cfg = _load_site_config(config)
 
     reg_client = OCSClient(cfg.hub.data['registry_address'])
     _, _, session = reg_client.main.status()
 
     instances = []
     for entry in session['data'].values():
+        if entry['expired']:
+            continue
+
         if entry['agent_class'] == agent_class:
             instance_id = entry['agent_address'].split('.')[-1]
             instances.append(instance_id)
 
     return instances
 
 
@@ -111,12 +114,13 @@
 
     acu_id = _find_active_instances('ACUAgent', config=config)
     smurf_ids = _find_active_instances(smurf_agent_class, config=config)
 
     if acu_id:
         acu_client = OCSClient(acu_id[0])
         clients['acu'] = acu_client
-    if smurf_ids:
-        smurf_clients = [OCSClient(x) for x in smurf_ids]
-        clients['smurf'] = smurf_clients
+
+    # Always create smurf client list, even if empty
+    smurf_clients = [OCSClient(x) for x in smurf_ids]
+    clients['smurf'] = smurf_clients
 
     return clients
```

### Comparing `sorunlib-0.1.6/src/sorunlib.egg-info/PKG-INFO` & `sorunlib-0.1.7/src/sorunlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorunlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: OCS Control Programs for running the observatory.
 Home-page: https://github.com/simonsobs/sorunlib
 Project-URL: Source Code, https://github.com/simonsobs/sorunlib
 Project-URL: Documentation, https://sorunlib.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/simonsobs/sorunlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sorunlib-0.1.6/versioneer.py` & `sorunlib-0.1.7/versioneer.py`

 * *Files identical despite different names*

