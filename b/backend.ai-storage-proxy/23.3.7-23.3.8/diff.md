# Comparing `tmp/backend.ai-storage-proxy-23.3.7.tar.gz` & `tmp/backend.ai-storage-proxy-23.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-23.3.7.tar", last modified: Mon Jul  3 16:26:22 2023, max compression
+gzip compressed data, was "backend.ai-storage-proxy-23.3.8.tar", last modified: Thu Jul  6 04:38:10 2023, max compression
```

## Comparing `backend.ai-storage-proxy-23.3.7.tar` & `backend.ai-storage-proxy-23.3.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33435 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/onefs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/netappclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/subproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/vfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.192323 backend.ai-storage-proxy-23.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.184323 backend.ai-storage-proxy-23.3.8/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.184323 backend.ai-storage-proxy-23.3.8/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33435 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/dellemc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/dellemc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/dellemc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/dellemc/onefs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (123)    20782 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/netapp/netappclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    22488 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:10.188323 backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-06 04:38:10.000000 backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 04:38:10.000000 backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:10.000000 backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:10.000000 backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:10.000000 backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 04:38:10.000000 backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 04:38:10.000000 backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:38:10.192323 backend.ai-storage-proxy-23.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-06 04:38:09.000000 backend.ai-storage-proxy-23.3.8/setup.py
```

### Comparing `backend.ai-storage-proxy-23.3.7/PKG-INFO` & `backend.ai-storage-proxy-23.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.7
+Version: 23.3.8
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/abc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/cephfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/config.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/context.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/__init__.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/dellemc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     ) -> None:
         super().__init__(mount_path)
         self.api_client = api_client
 
     async def create_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
-        config: Optional[QuotaConfig] = None,
+        options: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         await aiofiles.os.makedirs(qspath, exist_ok=True)
-        if config is not None:
-            await self.update_quota_scope(quota_scope_id, config)
+        if options is not None:
+            await self.update_quota_scope(quota_scope_id, options)
 
     async def describe_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
     ) -> Optional[QuotaUsage]:
         qspath = self.mangle_qspath(quota_scope_id)
         quota_id_path = qspath / ".quota_id"
```

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/exceptions.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/dellemc/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/onefs_client.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/dellemc/onefs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
         self.api_client = api_client
         self.fs = fs
         self.gpfs_owner = gpfs_owner
 
     async def create_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
-        config: Optional[QuotaConfig] = None,
+        options: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         await self.api_client.create_fileset(
             self.fs,
             quota_scope_id.pathname,
             path=qspath,
             owner=self.gpfs_owner,
         )
-        if config is not None:
-            await self.update_quota_scope(quota_scope_id, config)
+        if options is not None:
+            await self.update_quota_scope(quota_scope_id, options)
 
     async def update_quota_scope(self, quota_scope_id: QuotaScopeID, config: QuotaConfig) -> None:
         await self.api_client.set_quota(self.fs, quota_scope_id.pathname, config.limit_bytes)
 
     async def describe_quota_scope(self, quota_scope_id: QuotaScopeID) -> Optional[QuotaUsage]:
         if not self.mangle_qspath(quota_scope_id).exists():
             return None
@@ -184,15 +184,18 @@
         free, total = 0, 0
         for _pool in storage_pools:
             pool = await self.api_client.get_fs_pool(self.fs, _pool.storagePoolName)
             if pool.totalDataInKB is None or pool.freeDataInKB is None:
                 continue
             total += pool.totalDataInKB
             free += pool.freeDataInKB
-        return CapacityUsage(BinarySize(total - free) * 1024, BinarySize(total) * 1024)
+        return CapacityUsage(
+            used_bytes=BinarySize(total - free) * 1024,
+            capacity_bytes=BinarySize(total) * 1024,
+        )
 
     async def get_performance_metric(self) -> FSPerfMetric:
         # ref: https://www.ibm.com/docs/en/spectrum-scale/5.0.3?topic=2-perfmondata-get
         query = (
             "metrics "
             "avg(gpfs_ns_read_ops),"
             "avg(gpfs_ns_write_ops),"
```

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/migration.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/migration.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/netapp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,21 +68,21 @@
         self.netapp_client = netapp_client
         self.svm_id = svm_id
         self.volume_id = volume_id
 
     async def create_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
-        config: Optional[QuotaConfig] = None,
+        options: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         result = await self.netapp_client.create_qtree(self.svm_id, self.volume_id, qspath.name)
         self.netapp_client.check_job_result(result, [])
-        if config is not None:
-            await self.update_quota_scope(quota_scope_id, config)
+        if options is not None:
+            await self.update_quota_scope(quota_scope_id, options)
 
     async def describe_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
     ) -> Optional[QuotaUsage]:
         qspath = self.mangle_qspath(quota_scope_id)
         if not qspath.exists():
```

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/netapp/netappclient.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/purestorage/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/server.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/subproc.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/subproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/types.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/vfs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                     )
         except t.DataError:
             raise InvalidQuotaScopeError(f"Invalid value format for quota scope ID: {ref!r}")
 
     async def create_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
-        config: Optional[QuotaConfig] = None,
+        options: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
             lambda: qspath.mkdir(0o755, parents=True, exist_ok=False),
         )
@@ -133,15 +133,15 @@
     with setgid on the first-level namespace directories for each user
     or each project.
     """
 
     async def create_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
-        config: Optional[QuotaConfig] = None,
+        options: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
             lambda: qspath.mkdir(0o755, parents=True, exist_ok=False),
         )
```

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/weka/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,29 +37,31 @@
             None,
             lambda: os.stat(path).st_ino,
         )
 
     async def create_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
-        config: Optional[QuotaConfig] = None,
+        options: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         await aiofiles.os.makedirs(qspath)
         assert self.fs_uid is not None
-        if config is not None:
-            await self.update_quota_scope(quota_scope_id, config)
+        if options is not None:
+            await self.update_quota_scope(quota_scope_id, options)
 
     async def update_quota_scope(self, quota_scope_id: QuotaScopeID, config: QuotaConfig) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         inode_id = await self._get_inode_id(qspath)
         qs_relpath = qspath.relative_to(self.mount_path).as_posix()
         if not qs_relpath.startswith("/"):
             qs_relpath = "/" + qs_relpath
-        await self.api_client.set_quota_v1(qs_relpath, inode_id, hard_limit=config.limit_bytes)
+        await self.api_client.set_quota_v1(
+            qs_relpath, inode_id, soft_limit=config.limit_bytes, hard_limit=config.limit_bytes
+        )
 
     async def describe_quota_scope(self, quota_scope_id: QuotaScopeID) -> Optional[QuotaUsage]:
         qspath = self.mangle_qspath(quota_scope_id)
         if not qspath.exists():
             return None
 
         inode_id = await self._get_inode_id(qspath)
@@ -147,16 +149,16 @@
                 "metadata": {},
             }
 
     async def get_fs_usage(self) -> CapacityUsage:
         assert self._fs_uid is not None
         fs = await self.api_client.get_fs(self._fs_uid)
         return CapacityUsage(
-            fs.total_budget,
-            fs.used_total,
+            capacity_bytes=fs.total_budget,
+            used_bytes=fs.used_total,
         )
 
     async def get_performance_metric(self) -> FSPerfMetric:
         start_time = datetime.now().replace(second=0, microsecond=0) - timedelta(
             minutes=1,
         )
```

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-23.3.8/ai/backend/storage/xfs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,36 +153,40 @@
         self.project_registry = project_registry
         stat_vfs = os.statvfs(mount_path)
         self.block_size = stat_vfs.f_bsize
 
     async def create_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
-        config: Optional[QuotaConfig] = None,
+        options: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         try:
-            if config is None:
+            if options is None:
                 # Set the limit as the filesystem size
                 vfs_stat = os.statvfs(self.mount_path)
-                config = QuotaConfig(vfs_stat.f_blocks * self.block_size)
+                options = QuotaConfig(vfs_stat.f_blocks * self.block_size)
             async with FileLock(LOCK_FILE):
-                log.info("creating project quota (qs:{}, q:{})", quota_scope_id, config.limit_bytes)
+                log.info(
+                    "creating project quota (qs:{}, q:{})",
+                    quota_scope_id,
+                    (options.limit_bytes if options else None),
+                )
                 await aiofiles.os.makedirs(qspath)
                 await self.project_registry.read_project_info()
                 await self.project_registry.add_project_entry(quota_scope_id, qspath)
                 await self.project_registry.read_project_info()
         except (asyncio.CancelledError, asyncio.TimeoutError):
             log.exception("quota-scope creation timeout")
             raise
         except Exception:
             log.exception("quota-scope creation error")
             raise
-        if config is not None:
-            await self.update_quota_scope(quota_scope_id, config)
+        if options is not None:
+            await self.update_quota_scope(quota_scope_id, options)
 
     async def describe_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
     ) -> Optional[QuotaUsage]:
         if not self.mangle_qspath(quota_scope_id).exists():
             return None
```

### Comparing `backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.7
+Version: 23.3.8
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-23.3.8/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/backend_shim.py` & `backend.ai-storage-proxy-23.3.8/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.7/setup.py` & `backend.ai-storage-proxy-23.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'asyncpg>=0.27.0',
         'attrs>=20.3',
-        """backend.ai-common==23.03.7
+        """backend.ai-common==23.03.8
 """,
         'click>=7.1.2',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
         'more-itertools~=8.13.0',
         'setproctitle~=1.3.2',
         'tenacity>=8.0',
@@ -250,11 +250,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.7
+    'version': """23.03.8
 """,
     'zip_safe': False,
 })
```

