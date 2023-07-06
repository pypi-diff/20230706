# Comparing `tmp/fc-server-0.6.0.tar.gz` & `tmp/fc-server-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-server-0.6.0.tar", last modified: Wed Jul  5 06:32:29 2023, max compression
+gzip compressed data, was "dist/fc-server-0.6.1.tar", last modified: Thu Jul  6 05:55:12 2023, max compression
```

## Comparing `fc-server-0.6.0.tar` & `fc-server-0.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-03-29 08:28:44.000000 fc-server-0.6.0/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-05 06:32:29.000000 fc-server-0.6.0/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2022-08-17 06:53:34.000000 fc-server-0.6.0/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_common/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-05 06:30:26.000000 fc-server-0.6.0/fc_common/VERSION
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_common/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_common/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_common/etcd.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-05 06:29:52.000000 fc-server-0.6.0/fc_common/logger.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_common/version.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-03-07 07:55:27.000000 fc-server-0.6.0/fc_server/__init__.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/config/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      530 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/config/sample_cfg.yaml
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       82 2022-03-07 07:55:27.000000 fc-server-0.6.0/fc_server/config/sample_lavacli.yaml
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/core/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      935 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     6466 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/api_svr.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     4037 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    12182 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/coordinator.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1990 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/decorators.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      623 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_server/core/plugin.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/management/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-03-07 07:55:27.000000 fc-server-0.6.0/fc_server/management/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2498 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_server/management/cmd_online_lava_devices.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      212 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_server/management/common.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/plugins/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-07-06 05:36:14.000000 fc-server-0.6.0/fc_server/plugins/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     8138 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/plugins/labgrid.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    17708 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/plugins/lava.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/plugins/utils/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-08-17 06:53:34.000000 fc-server-0.6.0/fc_server/plugins/utils/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2819 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/plugins/utils/labgrid.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     5264 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/plugins/utils/lava.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1113 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/server.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      993 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      157 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/requires.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server_daemon/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server_daemon/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1960 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server_daemon/server_daemon.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-05 06:32:29.000000 fc-server-0.6.0/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3859 2023-07-05 06:29:52.000000 fc-server-0.6.0/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-06 05:53:39.000000 fc-server-0.6.1/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 05:55:12.000000 fc-server-0.6.1/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-06 05:53:39.000000 fc-server-0.6.1/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_common/version.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/__init__.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server/config/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      530 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/config/sample_cfg.yaml
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       82 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/config/sample_lavacli.yaml
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server/core/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      935 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/core/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     6461 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/core/api_svr.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3967 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/core/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    12182 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/core/coordinator.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1990 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/core/decorators.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      623 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/core/plugin.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server/management/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/management/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2498 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/management/cmd_online_lava_devices.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      212 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/management/common.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server/plugins/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/plugins/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     8138 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/plugins/labgrid.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    17708 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/plugins/lava.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server/plugins/utils/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/plugins/utils/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2819 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/plugins/utils/labgrid.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     5264 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/plugins/utils/lava.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1113 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server/server.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      993 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      157 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:12.000000 fc-server-0.6.1/fc_server_daemon/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server_daemon/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2185 2023-07-06 05:53:39.000000 fc-server-0.6.1/fc_server_daemon/server_daemon.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-06 05:55:12.000000 fc-server-0.6.1/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-06 05:53:39.000000 fc-server-0.6.1/setup.py
```

### Comparing `fc-server-0.6.0/LICENSE` & `fc-server-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/PKG-INFO` & `fc-server-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-server
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-server-0.6.0/README.rst` & `fc-server-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_common/config.py` & `fc-server-0.6.1/fc_common/config.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_common/etcd.py` & `fc-server-0.6.1/fc_common/etcd.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_common/logger.py` & `fc-server-0.6.1/fc_common/logger.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_common/version.py` & `fc-server-0.6.1/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/config/sample_cfg.yaml` & `fc-server-0.6.1/fc_server/config/sample_cfg.yaml`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/core/__init__.py` & `fc-server-0.6.1/fc_server/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/core/api_svr.py` & `fc-server-0.6.1/fc_server/core/api_svr.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,12 +171,12 @@
         app.add_routes([web.get("/booking", self.booking)])
         app.add_routes([web.get("/resource", self.resource_status)])
         app.add_routes([web.get("/resource/{res}", self.resource_status)])
 
         app_runner = web.AppRunner(app)
         await app_runner.setup()
 
-        api_interface = svr_args["ip"]
+        api_interface = "0.0.0.0"
         api_port = svr_args["port"]
         loop = asyncio.get_event_loop()
         await loop.create_server(app_runner.server, api_interface, api_port)
         self.logger.info("Api Server ready at http://%s:%d.", api_interface, api_port)
```

### Comparing `fc-server-0.6.0/fc_server/core/config.py` & `fc-server-0.6.1/fc_server/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,16 +86,14 @@
         if "port" not in Config.api_server:
             Config.logger.error("port for api_server is mandatory")
             sys.exit(1)
         if "ip" not in Config.api_server:
             if cluster and Config.cluster["enable"]:
                 Config.logger.error("ip for api_server in cluster mode is mandatory")
                 sys.exit(1)
-            else:
-                Config.api_server["ip"] = "0.0.0.0"
 
         default_framework_strategies = [
             framework
             for framework in Config.registered_frameworks
             if Config.frameworks_config[framework].get("default", False)
         ]
         default_framework_number = len(default_framework_strategies)
```

### Comparing `fc-server-0.6.0/fc_server/core/coordinator.py` & `fc-server-0.6.1/fc_server/core/coordinator.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/core/decorators.py` & `fc-server-0.6.1/fc_server/core/decorators.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/core/plugin.py` & `fc-server-0.6.1/fc_server/core/plugin.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/management/cmd_online_lava_devices.py` & `fc-server-0.6.1/fc_server/management/cmd_online_lava_devices.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/plugins/labgrid.py` & `fc-server-0.6.1/fc_server/plugins/labgrid.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/plugins/lava.py` & `fc-server-0.6.1/fc_server/plugins/lava.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/plugins/utils/labgrid.py` & `fc-server-0.6.1/fc_server/plugins/utils/labgrid.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/plugins/utils/lava.py` & `fc-server-0.6.1/fc_server/plugins/utils/lava.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server/server.py` & `fc-server-0.6.1/fc_server/server.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server.egg-info/PKG-INFO` & `fc-server-0.6.1/fc_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-server
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-server-0.6.0/fc_server.egg-info/SOURCES.txt` & `fc-server-0.6.1/fc_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/fc_server_daemon/server_daemon.py` & `fc-server-0.6.1/fc_server_daemon/server_daemon.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 # Copyright 2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import logging
 import multiprocessing
+import os
 import signal
 import time
 
 import prctl
 
 from fc_common.etcd import Etcd
 from fc_common.logger import Logger
 
 
 class ServerDaemon:
     def __init__(self, daemon_paras):
         self.daemon_paras = daemon_paras
+        self.server_daemon = None
         self.logger = logging.getLogger("fc_server_daemon")
 
     def __action(self):
         prctl.set_pdeathsig(signal.SIGHUP)  # pylint: disable=no-member
 
         Logger.init("fc_server_daemon", "fc_server_daemon.log", log_type="file_only")
 
@@ -57,10 +59,16 @@
                         time.sleep(ttl / 4)
                         lock.refresh()
             except Exception as lock_exec:  # pylint: disable=broad-except
                 self.logger.debug(lock_exec)
 
             time.sleep(30)
 
+    def handler(self, *_):
+        if self.server_daemon:
+            os.kill(self.server_daemon.pid, signal.SIGINT)
+
     def run(self):
-        server_daemon = multiprocessing.Process(target=self.__action, daemon=True)
-        server_daemon.start()
+        self.server_daemon = multiprocessing.Process(target=self.__action, daemon=True)
+        self.server_daemon.start()
+
+        signal.signal(signal.SIGTERM, self.handler)
```

### Comparing `fc-server-0.6.0/setup.cfg` & `fc-server-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.0/setup.py` & `fc-server-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         },
         install_requires=[
             "prettytable>=2.2.1",
             "labgrid==23.0.1",
             "python-daemon",
             "etcd3-fc",
             "tenacity",
+            "aiohttp",
             "protobuf==3.20.3",
         ],
     )
 elif PKG == "fc-client-docker":
     setup(
         **common_setup,
         name="fc-client-docker",
```

