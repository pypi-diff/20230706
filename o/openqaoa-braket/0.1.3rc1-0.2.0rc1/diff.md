# Comparing `tmp/openqaoa-braket-0.1.3rc1.tar.gz` & `tmp/openqaoa-braket-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqaoa-braket-0.1.3rc1.tar", last modified: Fri Jun 30 09:17:34 2023, max compression
+gzip compressed data, was "openqaoa-braket-0.2.0rc1.tar", last modified: Thu Jul  6 05:59:25 2023, max compression
```

## Comparing `openqaoa-braket-0.1.3rc1.tar` & `openqaoa-braket-0.2.0rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:34.702823 openqaoa-braket-0.1.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-30 09:17:34.702823 openqaoa-braket-0.1.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:34.698823 openqaoa-braket-0.1.3rc1/openqaoa_braket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:34.698823 openqaoa-braket-0.1.3rc1/openqaoa_braket/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:34.702823 openqaoa-braket-0.1.3rc1/openqaoa_braket/algorithms/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/algorithms/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/algorithms/jobs/managed_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:34.702823 openqaoa-braket-0.1.3rc1/openqaoa_braket/backends/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/backends/gates_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket/backends/qaoa_braket_qpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:34.698823 openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-30 09:17:34.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-30 09:17:34.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:17:34.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 09:17:34.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 09:17:34.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 09:17:34.000000 openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:17:34.702823 openqaoa-braket-0.1.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:34.702823 openqaoa-braket-0.1.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/tests/test_aws_managed_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/tests/test_devices_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/tests/test_gate_applicators_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/tests/test_gates_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-06-30 09:15:43.000000 openqaoa-braket-0.1.3rc1/tests/test_qpu_braket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/openqaoa_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/openqaoa_braket/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/openqaoa_braket/algorithms/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/algorithms/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/algorithms/jobs/managed_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/openqaoa_braket/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/backends/gates_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket/backends/qaoa_braket_qpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-06 05:59:25.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-06 05:59:25.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:59:25.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 05:59:25.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 05:59:25.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 05:59:25.000000 openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:25.865871 openqaoa-braket-0.2.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/tests/test_aws_managed_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/tests/test_devices_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/tests/test_gate_applicators_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/tests/test_gates_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-06 05:57:36.000000 openqaoa-braket-0.2.0rc1/tests/test_qpu_braket.py
```

### Comparing `openqaoa-braket-0.1.3rc1/LICENSE` & `openqaoa-braket-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/PKG-INFO` & `openqaoa-braket-0.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-braket
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: Braket Plug-in for OpenQAOA
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-braket-0.1.3rc1/README.md` & `openqaoa-braket-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/openqaoa_braket/algorithms/jobs/managed_job.py` & `openqaoa-braket-0.2.0rc1/openqaoa_braket/algorithms/jobs/managed_job.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/openqaoa_braket/backends/devices.py` & `openqaoa-braket-0.2.0rc1/openqaoa_braket/backends/devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/openqaoa_braket/backends/gates_braket.py` & `openqaoa-braket-0.2.0rc1/openqaoa_braket/backends/gates_braket.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/openqaoa_braket/backends/qaoa_braket_qpu.py` & `openqaoa-braket-0.2.0rc1/openqaoa_braket/backends/qaoa_braket_qpu.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/PKG-INFO` & `openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-braket
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: Braket Plug-in for OpenQAOA
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-braket-0.1.3rc1/openqaoa_braket.egg-info/SOURCES.txt` & `openqaoa-braket-0.2.0rc1/openqaoa_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/setup.py` & `openqaoa-braket-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/tests/test_aws_managed_jobs.py` & `openqaoa-braket-0.2.0rc1/tests/test_aws_managed_jobs.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/tests/test_devices_braket.py` & `openqaoa-braket-0.2.0rc1/tests/test_devices_braket.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/tests/test_gate_applicators_braket.py` & `openqaoa-braket-0.2.0rc1/tests/test_gate_applicators_braket.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/tests/test_gates_braket.py` & `openqaoa-braket-0.2.0rc1/tests/test_gates_braket.py`

 * *Files identical despite different names*

### Comparing `openqaoa-braket-0.1.3rc1/tests/test_qpu_braket.py` & `openqaoa-braket-0.2.0rc1/tests/test_qpu_braket.py`

 * *Files identical despite different names*

