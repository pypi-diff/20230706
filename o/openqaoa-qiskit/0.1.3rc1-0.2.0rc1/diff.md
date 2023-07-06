# Comparing `tmp/openqaoa-qiskit-0.1.3rc1.tar.gz` & `tmp/openqaoa-qiskit-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqaoa-qiskit-0.1.3rc1.tar", last modified: Fri Jun 30 09:17:06 2023, max compression
+gzip compressed data, was "openqaoa-qiskit-0.2.0rc1.tar", last modified: Thu Jul  6 05:58:57 2023, max compression
```

## Comparing `openqaoa-qiskit-0.1.3rc1.tar` & `openqaoa-qiskit-0.2.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:06.885727 openqaoa-qiskit-0.1.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-30 09:17:06.885727 openqaoa-qiskit-0.1.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:06.881727 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:06.885727 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/gates_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/qaoa_qiskit_qpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/qaoa_qiskit_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:06.881727 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-30 09:17:06.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-30 09:17:06.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:17:06.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 09:17:06.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 09:17:06.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 09:17:06.000000 openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:17:06.885727 openqaoa-qiskit-0.1.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:06.885727 openqaoa-qiskit-0.1.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_backends_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_circuit_routing_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_devices_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_gate_applicators_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_gates_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_qiskit_backend_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_qpu_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_result_object_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_sample_from_wavefunction_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30609 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_sim_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    48166 2023-06-30 09:15:43.000000 openqaoa-qiskit-0.1.3rc1/tests/test_workflows_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:57.393970 openqaoa-qiskit-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-06 05:58:57.393970 openqaoa-qiskit-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:57.389970 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:57.393970 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/gates_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/qaoa_qiskit_qpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/qaoa_qiskit_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:57.389970 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-06 05:58:57.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-06 05:58:57.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:58:57.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 05:58:57.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 05:58:57.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 05:58:57.000000 openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:58:57.393970 openqaoa-qiskit-0.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:57.393970 openqaoa-qiskit-0.2.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_backends_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_circuit_routing_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_devices_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_gate_applicators_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_gates_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_qiskit_backend_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_qpu_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_result_object_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_sample_from_wavefunction_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30609 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_sim_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48166 2023-07-06 05:57:36.000000 openqaoa-qiskit-0.2.0rc1/tests/test_workflows_qiskit.py
```

### Comparing `openqaoa-qiskit-0.1.3rc1/LICENSE` & `openqaoa-qiskit-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/PKG-INFO` & `openqaoa-qiskit-0.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-qiskit
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: Qiskit Plug-in for OpenQAOA
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-qiskit-0.1.3rc1/README.md` & `openqaoa-qiskit-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backend_config.py` & `openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backend_config.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/devices.py` & `openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/gates_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/gates_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/qaoa_qiskit_qpu.py` & `openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/qaoa_qiskit_qpu.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit/backends/qaoa_qiskit_sim.py` & `openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit/backends/qaoa_qiskit_sim.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/PKG-INFO` & `openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-qiskit
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: Qiskit Plug-in for OpenQAOA
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-qiskit-0.1.3rc1/openqaoa_qiskit.egg-info/SOURCES.txt` & `openqaoa-qiskit-0.2.0rc1/openqaoa_qiskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/setup.py` & `openqaoa-qiskit-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_backends_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_backends_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_circuit_routing_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_circuit_routing_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_devices_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_devices_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_gate_applicators_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_gate_applicators_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_gates_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_gates_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_qiskit_backend_wrapper.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_qiskit_backend_wrapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_qpu_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_qpu_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_result_object_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_result_object_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_sample_from_wavefunction_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_sample_from_wavefunction_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_sim_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_sim_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-qiskit-0.1.3rc1/tests/test_workflows_qiskit.py` & `openqaoa-qiskit-0.2.0rc1/tests/test_workflows_qiskit.py`

 * *Files identical despite different names*

