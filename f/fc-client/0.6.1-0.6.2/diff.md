# Comparing `tmp/fc-client-0.6.1.tar.gz` & `tmp/fc-client-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-client-0.6.1.tar", last modified: Thu Jul  6 05:55:13 2023, max compression
+gzip compressed data, was "dist/fc-client-0.6.2.tar", last modified: Thu Jul  6 08:49:04 2023, max compression
```

## Comparing `fc-client-0.6.1.tar` & `fc-client-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:13.000000 fc-client-0.6.1/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-06 05:53:39.000000 fc-client-0.6.1/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 05:55:13.000000 fc-client-0.6.1/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-06 05:53:39.000000 fc-client-0.6.1/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    14077 2023-07-06 05:53:39.000000 fc-client-0.6.1/fc_client/client.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      410 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       92 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client.egg-info/requires.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_client_daemon/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     7064 2023-07-06 05:53:39.000000 fc-client-0.6.1/fc_client_daemon/client_daemon.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:13.000000 fc-client-0.6.1/fc_common/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-06 05:53:39.000000 fc-client-0.6.1/fc_common/VERSION
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-06 05:53:39.000000 fc-client-0.6.1/fc_common/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-06 05:53:39.000000 fc-client-0.6.1/fc_common/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-06 05:53:39.000000 fc-client-0.6.1/fc_common/etcd.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-06 05:53:39.000000 fc-client-0.6.1/fc_common/logger.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-06 05:53:39.000000 fc-client-0.6.1/fc_common/version.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-06 05:55:13.000000 fc-client-0.6.1/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-06 05:53:39.000000 fc-client-0.6.1/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-06 08:48:52.000000 fc-client-0.6.2/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 08:49:04.000000 fc-client-0.6.2/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-06 08:48:52.000000 fc-client-0.6.2/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    14077 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_client/client.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      410 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       92 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client_daemon/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     7064 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_client_daemon/client_daemon.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/version.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-06 08:49:04.000000 fc-client-0.6.2/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-06 08:48:52.000000 fc-client-0.6.2/setup.py
```

### Comparing `fc-client-0.6.1/LICENSE` & `fc-client-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/PKG-INFO` & `fc-client-0.6.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.6.1
+Version: 0.6.2
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-client-0.6.1/README.rst` & `fc-client-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/fc_client/client.py` & `fc-client-0.6.2/fc_client/client.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/fc_client.egg-info/PKG-INFO` & `fc-client-0.6.2/fc_client.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.6.1
+Version: 0.6.2
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-client-0.6.1/fc_client_daemon/client_daemon.py` & `fc-client-0.6.2/fc_client_daemon/client_daemon.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/fc_common/config.py` & `fc-client-0.6.2/fc_common/config.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/fc_common/etcd.py` & `fc-client-0.6.2/fc_common/etcd.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/fc_common/logger.py` & `fc-client-0.6.2/fc_common/logger.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/fc_common/version.py` & `fc-client-0.6.2/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/setup.cfg` & `fc-client-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.1/setup.py` & `fc-client-0.6.2/setup.py`

 * *Files identical despite different names*

