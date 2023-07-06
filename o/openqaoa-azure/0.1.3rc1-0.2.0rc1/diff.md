# Comparing `tmp/openqaoa-azure-0.1.3rc1.tar.gz` & `tmp/openqaoa-azure-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqaoa-azure-0.1.3rc1.tar", last modified: Fri Jun 30 09:18:58 2023, max compression
+gzip compressed data, was "openqaoa-azure-0.2.0rc1.tar", last modified: Thu Jul  6 06:00:50 2023, max compression
```

## Comparing `openqaoa-azure-0.1.3rc1.tar` & `openqaoa-azure-0.2.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:58.254079 openqaoa-azure-0.1.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-30 09:18:58.250079 openqaoa-azure-0.1.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:58.250079 openqaoa-azure-0.1.3rc1/openqaoa_azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:58.250079 openqaoa-azure-0.1.3rc1/openqaoa_azure/backends/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure/backends/devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:58.250079 openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-30 09:18:58.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-30 09:18:58.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:18:58.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 09:18:58.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 09:18:58.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 09:18:58.000000 openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:18:58.254079 openqaoa-azure-0.1.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:58.250079 openqaoa-azure-0.1.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/tests/test_devices_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-30 09:15:43.000000 openqaoa-azure-0.1.3rc1/tests/test_qpu_qiskit_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:00:50.977571 openqaoa-azure-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-06 06:00:50.977571 openqaoa-azure-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:00:50.973571 openqaoa-azure-0.2.0rc1/openqaoa_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:00:50.977571 openqaoa-azure-0.2.0rc1/openqaoa_azure/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure/backends/devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:00:50.977571 openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-06 06:00:50.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-06 06:00:50.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:00:50.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-06 06:00:50.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 06:00:50.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 06:00:50.000000 openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:00:50.977571 openqaoa-azure-0.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:00:50.977571 openqaoa-azure-0.2.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/tests/test_devices_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-06 05:57:36.000000 openqaoa-azure-0.2.0rc1/tests/test_qpu_qiskit_azure.py
```

### Comparing `openqaoa-azure-0.1.3rc1/LICENSE` & `openqaoa-azure-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openqaoa-azure-0.1.3rc1/PKG-INFO` & `openqaoa-azure-0.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-azure
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: Azure Plug-in for OpenQAOA
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-azure-0.1.3rc1/README.md` & `openqaoa-azure-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `openqaoa-azure-0.1.3rc1/openqaoa_azure/backends/devices.py` & `openqaoa-azure-0.2.0rc1/openqaoa_azure/backends/devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/PKG-INFO` & `openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-azure
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: Azure Plug-in for OpenQAOA
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-azure-0.1.3rc1/openqaoa_azure.egg-info/SOURCES.txt` & `openqaoa-azure-0.2.0rc1/openqaoa_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openqaoa-azure-0.1.3rc1/setup.py` & `openqaoa-azure-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `openqaoa-azure-0.1.3rc1/tests/test_devices_azure.py` & `openqaoa-azure-0.2.0rc1/tests/test_devices_azure.py`

 * *Files identical despite different names*

### Comparing `openqaoa-azure-0.1.3rc1/tests/test_qpu_qiskit_azure.py` & `openqaoa-azure-0.2.0rc1/tests/test_qpu_qiskit_azure.py`

 * *Files identical despite different names*

