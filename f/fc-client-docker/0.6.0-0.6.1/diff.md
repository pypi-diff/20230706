# Comparing `tmp/fc-client-docker-0.6.0.tar.gz` & `tmp/fc-client-docker-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-client-docker-0.6.0.tar", last modified: Wed Jul  5 06:32:30 2023, max compression
+gzip compressed data, was "dist/fc-client-docker-0.6.1.tar", last modified: Thu Jul  6 05:55:14 2023, max compression
```

## Comparing `fc-client-docker-0.6.0.tar` & `fc-client-docker-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-03-29 08:28:44.000000 fc-client-docker-0.6.0/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      675 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2022-08-17 06:53:34.000000 fc-client-docker-0.6.0/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/fc_client_docker/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      331 2023-07-05 06:29:40.000000 fc-client-docker-0.6.0/fc_client_docker/__init__.py
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)      102 2023-07-05 06:29:40.000000 fc-client-docker-0.6.0/fc_client_docker/fc_client_docker
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/fc_client_docker.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      675 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/fc_client_docker.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      422 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/fc_client_docker.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/fc_client_docker.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       59 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/fc_client_docker.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       27 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/fc_client_docker.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/fc_common/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-05 06:30:26.000000 fc-client-docker-0.6.0/fc_common/VERSION
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-06-30 05:19:57.000000 fc-client-docker-0.6.0/fc_common/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-06-30 05:20:06.000000 fc-client-docker-0.6.0/fc_common/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-06-30 05:20:06.000000 fc-client-docker-0.6.0/fc_common/etcd.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-05 06:29:52.000000 fc-client-docker-0.6.0/fc_common/logger.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-06-30 05:19:57.000000 fc-client-docker-0.6.0/fc_common/version.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-05 06:32:30.000000 fc-client-docker-0.6.0/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3859 2023-07-05 06:29:52.000000 fc-client-docker-0.6.0/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:14.000000 fc-client-docker-0.6.1/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      675 2023-07-06 05:55:14.000000 fc-client-docker-0.6.1/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:14.000000 fc-client-docker-0.6.1/fc_client_docker/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      331 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/fc_client_docker/__init__.py
+-rwxr-xr-x   0 nxa13855  (1001) atg       (1001)      102 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/fc_client_docker/fc_client_docker
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:14.000000 fc-client-docker-0.6.1/fc_client_docker.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      675 2023-07-06 05:55:13.000000 fc-client-docker-0.6.1/fc_client_docker.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      422 2023-07-06 05:55:14.000000 fc-client-docker-0.6.1/fc_client_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-06 05:55:13.000000 fc-client-docker-0.6.1/fc_client_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       59 2023-07-06 05:55:13.000000 fc-client-docker-0.6.1/fc_client_docker.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       27 2023-07-06 05:55:13.000000 fc-client-docker-0.6.1/fc_client_docker.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:14.000000 fc-client-docker-0.6.1/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/fc_common/version.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-06 05:55:14.000000 fc-client-docker-0.6.1/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-06 05:53:39.000000 fc-client-docker-0.6.1/setup.py
```

### Comparing `fc-client-docker-0.6.0/LICENSE` & `fc-client-docker-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.0/PKG-INFO` & `fc-client-docker-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client-docker
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

### Comparing `fc-client-docker-0.6.0/README.rst` & `fc-client-docker-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.0/fc_client_docker.egg-info/PKG-INFO` & `fc-client-docker-0.6.1/fc_client_docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client-docker
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

### Comparing `fc-client-docker-0.6.0/fc_common/config.py` & `fc-client-docker-0.6.1/fc_common/config.py`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.0/fc_common/etcd.py` & `fc-client-docker-0.6.1/fc_common/etcd.py`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.0/fc_common/logger.py` & `fc-client-docker-0.6.1/fc_common/logger.py`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.0/fc_common/version.py` & `fc-client-docker-0.6.1/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.0/setup.cfg` & `fc-client-docker-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.0/setup.py` & `fc-client-docker-0.6.1/setup.py`

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

