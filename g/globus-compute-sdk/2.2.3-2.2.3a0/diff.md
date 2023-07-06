# Comparing `tmp/globus-compute-sdk-2.2.3.tar.gz` & `tmp/globus-compute-sdk-2.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.2.3.tar", last modified: Thu Jul  6 20:21:49 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.2.3a0.tar", last modified: Wed Jul  5 15:36:03 2023, max compression
```

## Comparing `globus-compute-sdk-2.2.3.tar` & `globus-compute-sdk-2.2.3a0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.583593 globus-compute-sdk-2.2.3/
--rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/LICENSE
--rw-r--r--   0 yadu       (501) staff       (20)       16 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/MANIFEST.in
--rw-r--r--   0 yadu       (501) staff       (20)     1819 2023-07-06 20:21:49.583697 globus-compute-sdk-2.2.3/PKG-INFO
--rw-r--r--   0 yadu       (501) staff       (20)      816 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/PyPI.md
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.573451 globus-compute-sdk-2.2.3/globus_compute_sdk/
--rw-r--r--   0 yadu       (501) staff       (20)      433 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.574962 globus-compute-sdk-2.2.3/globus_compute_sdk/errors/
--rw-r--r--   0 yadu       (501) staff       (20)      320 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     1921 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.577736 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     1384 2023-07-05 15:19:44.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.578780 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)      648 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 yadu       (501) staff       (20)      724 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 yadu       (501) staff       (20)    11458 2023-04-24 17:52:07.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-r--r--   0 yadu       (501) staff       (20)     2262 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 yadu       (501) staff       (20)    27050 2023-06-30 20:13:26.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 yadu       (501) staff       (20)     2400 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 yadu       (501) staff       (20)    46344 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.581709 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 yadu       (501) staff       (20)      237 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     1787 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 yadu       (501) staff       (20)      855 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 yadu       (501) staff       (20)      373 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 yadu       (501) staff       (20)      954 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 yadu       (501) staff       (20)     7287 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 yadu       (501) staff       (20)      710 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 yadu       (501) staff       (20)     3012 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 yadu       (501) staff       (20)     2190 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.582215 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 yadu       (501) staff       (20)      212 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     1207 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 yadu       (501) staff       (20)     8561 2023-07-05 15:19:44.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.583342 globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/
--rw-r--r--   0 yadu       (501) staff       (20)      603 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     1412 2023-06-16 15:43:21.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 yadu       (501) staff       (20)     7869 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 yadu       (501) staff       (20)     4848 2023-06-16 15:43:21.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/utils.py
--rw-r--r--   0 yadu       (501) staff       (20)      832 2023-07-06 20:21:28.000000 globus-compute-sdk-2.2.3/globus_compute_sdk/version.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:21:49.574420 globus-compute-sdk-2.2.3/globus_compute_sdk.egg-info/
--rw-r--r--   0 yadu       (501) staff       (20)     1819 2023-07-06 20:21:49.000000 globus-compute-sdk-2.2.3/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yadu       (501) staff       (20)     1577 2023-07-06 20:21:49.000000 globus-compute-sdk-2.2.3/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-06 20:21:49.000000 globus-compute-sdk-2.2.3/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yadu       (501) staff       (20)      397 2023-07-06 20:21:49.000000 globus-compute-sdk-2.2.3/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 yadu       (501) staff       (20)       19 2023-07-06 20:21:49.000000 globus-compute-sdk-2.2.3/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 yadu       (501) staff       (20)      282 2023-07-06 20:21:49.584103 globus-compute-sdk-2.2.3/setup.cfg
--rw-r--r--   0 yadu       (501) staff       (20)     3161 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3/setup.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.453345 globus-compute-sdk-2.2.3a0/
+-rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/LICENSE
+-rw-r--r--   0 yadu       (501) staff       (20)       16 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/MANIFEST.in
+-rw-r--r--   0 yadu       (501) staff       (20)     1821 2023-07-05 15:36:03.453443 globus-compute-sdk-2.2.3a0/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)      816 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/PyPI.md
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.445677 globus-compute-sdk-2.2.3a0/globus_compute_sdk/
+-rw-r--r--   0 yadu       (501) staff       (20)      433 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.446898 globus-compute-sdk-2.2.3a0/globus_compute_sdk/errors/
+-rw-r--r--   0 yadu       (501) staff       (20)      320 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1921 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.448628 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1384 2023-07-05 15:19:44.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.449560 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      648 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 yadu       (501) staff       (20)      724 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 yadu       (501) staff       (20)    11458 2023-04-24 17:52:07.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2262 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 yadu       (501) staff       (20)    27050 2023-06-30 20:13:26.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2400 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 yadu       (501) staff       (20)    46344 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.451776 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 yadu       (501) staff       (20)      237 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1787 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 yadu       (501) staff       (20)      855 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 yadu       (501) staff       (20)      373 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 yadu       (501) staff       (20)      954 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7287 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)      710 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3012 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2190 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.452128 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 yadu       (501) staff       (20)      212 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1207 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 yadu       (501) staff       (20)     8561 2023-07-05 15:19:44.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.453067 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/
+-rw-r--r--   0 yadu       (501) staff       (20)      603 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1412 2023-06-16 15:43:21.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7869 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 yadu       (501) staff       (20)     4848 2023-06-16 15:43:21.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/utils.py
+-rw-r--r--   0 yadu       (501) staff       (20)      834 2023-07-05 15:25:26.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/version.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.446516 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/
+-rw-r--r--   0 yadu       (501) staff       (20)     1821 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)     1577 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      397 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 yadu       (501) staff       (20)       19 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      282 2023-07-05 15:36:03.453803 globus-compute-sdk-2.2.3a0/setup.cfg
+-rw-r--r--   0 yadu       (501) staff       (20)     3161 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3a0/setup.py
```

### Comparing `globus-compute-sdk-2.2.3/LICENSE` & `globus-compute-sdk-2.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/PKG-INFO` & `globus-compute-sdk-2.2.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.2.3
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.2.3/PyPI.md` & `globus-compute-sdk-2.2.3a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/_environments.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/__init__.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk/version.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.3"
+__version__ = "2.2.3a0"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.2.3
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.2.3/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.3/setup.py` & `globus-compute-sdk-2.2.3a0/setup.py`

 * *Files identical despite different names*

