# Comparing `tmp/openqaoa-pyquil-0.1.3rc1.tar.gz` & `tmp/openqaoa-pyquil-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqaoa-pyquil-0.1.3rc1.tar", last modified: Fri Jun 30 09:18:01 2023, max compression
+gzip compressed data, was "openqaoa-pyquil-0.2.0rc1.tar", last modified: Thu Jul  6 05:59:52 2023, max compression
```

## Comparing `openqaoa-pyquil-0.1.3rc1.tar` & `openqaoa-pyquil-0.2.0rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:01.263860 openqaoa-pyquil-0.1.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-30 09:18:01.263860 openqaoa-pyquil-0.1.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:01.263860 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:01.263860 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/gates_pyquil.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/qaoa_pyquil_qpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/qaoa_pyquil_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:01.263860 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-30 09:18:01.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 09:18:01.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:18:01.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 09:18:01.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 09:18:01.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 09:18:01.000000 openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:18:01.263860 openqaoa-pyquil-0.1.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:18:01.263860 openqaoa-pyquil-0.1.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30520 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/tests/test_circuit_routing_pyquil.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/tests/test_gate_applicators_pyquil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/tests/test_gates_pyquil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/tests/test_pyquil_backend_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/tests/test_pyquil_qvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-30 09:15:43.000000 openqaoa-pyquil-0.1.3rc1/tests/test_workflows_pyquil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:52.741776 openqaoa-pyquil-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-06 05:59:52.741776 openqaoa-pyquil-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:52.737776 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:52.737776 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/gates_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/qaoa_pyquil_qpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/qaoa_pyquil_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:52.737776 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-06 05:59:52.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-06 05:59:52.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:59:52.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 05:59:52.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 05:59:52.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 05:59:52.000000 openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:59:52.741776 openqaoa-pyquil-0.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:59:52.741776 openqaoa-pyquil-0.2.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30520 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/tests/test_circuit_routing_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/tests/test_gate_applicators_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/tests/test_gates_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/tests/test_pyquil_backend_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/tests/test_pyquil_qvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-06 05:57:36.000000 openqaoa-pyquil-0.2.0rc1/tests/test_workflows_pyquil.py
```

### Comparing `openqaoa-pyquil-0.1.3rc1/LICENSE` & `openqaoa-pyquil-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/PKG-INFO` & `openqaoa-pyquil-0.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-pyquil
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: Pyquil Plug-in for OpenQAOA
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-pyquil-0.1.3rc1/README.md` & `openqaoa-pyquil-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backend_config.py` & `openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backend_config.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/devices.py` & `openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/gates_pyquil.py` & `openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/gates_pyquil.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/qaoa_pyquil_qpu.py` & `openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/qaoa_pyquil_qpu.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil/backends/qaoa_pyquil_sim.py` & `openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil/backends/qaoa_pyquil_sim.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/PKG-INFO` & `openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-pyquil
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: Pyquil Plug-in for OpenQAOA
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-pyquil-0.1.3rc1/openqaoa_pyquil.egg-info/SOURCES.txt` & `openqaoa-pyquil-0.2.0rc1/openqaoa_pyquil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/setup.py` & `openqaoa-pyquil-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/tests/test_circuit_routing_pyquil.py` & `openqaoa-pyquil-0.2.0rc1/tests/test_circuit_routing_pyquil.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/tests/test_gate_applicators_pyquil.py` & `openqaoa-pyquil-0.2.0rc1/tests/test_gate_applicators_pyquil.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/tests/test_gates_pyquil.py` & `openqaoa-pyquil-0.2.0rc1/tests/test_gates_pyquil.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/tests/test_pyquil_backend_wrapper.py` & `openqaoa-pyquil-0.2.0rc1/tests/test_pyquil_backend_wrapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/tests/test_pyquil_qvm.py` & `openqaoa-pyquil-0.2.0rc1/tests/test_pyquil_qvm.py`

 * *Files identical despite different names*

### Comparing `openqaoa-pyquil-0.1.3rc1/tests/test_workflows_pyquil.py` & `openqaoa-pyquil-0.2.0rc1/tests/test_workflows_pyquil.py`

 * *Files identical despite different names*

