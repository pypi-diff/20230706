# Comparing `tmp/planqk-quantum-1.8.0.tar.gz` & `tmp/planqk-quantum-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-1.8.0.tar", last modified: Thu Jul  6 07:38:17 2023, max compression
+gzip compressed data, was "planqk-quantum-1.8.1.tar", last modified: Thu Jul  6 09:22:52 2023, max compression
```

## Comparing `planqk-quantum-1.8.0.tar` & `planqk-quantum-1.8.1.tar`

### file list

```diff
@@ -1,39 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.550334 planqk-quantum-1.8.0/planqk/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3679 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.550334 planqk-quantum-1.8.0/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.550334 planqk-quantum-1.8.0/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (122)     4177 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/client/client_dtos.py
--rw-r--r--   0 runner    (1001) docker     (122)     4138 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.550334 planqk-quantum-1.8.0/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/planqk/qiskit/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6021 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/azure/planqk_azure_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     8556 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/azure/planqk_azure_job.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/planqk/qiskit/providers/braket/
--rw-r--r--   0 runner    (1001) docker     (122)     4256 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/braket/braket_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/braket/planqk_braket_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/planqk/qiskit/providers/helper/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/helper/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/helper/job_input_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/planqk/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3679 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4177 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/client/client_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/planqk/qiskit/providers/helper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/providers/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/providers/helper/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/planqk/qiskit/providers/helper/job_input_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 09:22:52.000000 planqk-quantum-1.8.1/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-06 09:22:52.000000 planqk-quantum-1.8.1/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 09:22:52.000000 planqk-quantum-1.8.1/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-06 09:22:52.000000 planqk-quantum-1.8.1/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-06 09:22:52.000000 planqk-quantum-1.8.1/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 09:22:52.554553 planqk-quantum-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-06 09:22:38.000000 planqk-quantum-1.8.1/setup.py
```

### Comparing `planqk-quantum-1.8.0/LICENSE` & `planqk-quantum-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/PKG-INFO` & `planqk-quantum-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `planqk-quantum-1.8.0/README.md` & `planqk-quantum-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk/credentials.py` & `planqk-quantum-1.8.1/planqk/credentials.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk/qiskit/backend.py` & `planqk-quantum-1.8.1/planqk/qiskit/backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk/qiskit/client/backend_dtos.py` & `planqk-quantum-1.8.1/planqk/qiskit/client/backend_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk/qiskit/client/client.py` & `planqk-quantum-1.8.1/planqk/qiskit/client/client.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk/qiskit/client/client_dtos.py` & `planqk-quantum-1.8.1/planqk/qiskit/client/client_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk/qiskit/job.py` & `planqk-quantum-1.8.1/planqk/qiskit/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-import time
-from dataclasses import asdict
-from typing import Optional, Union
+from typing import Optional
 
-from qiskit import QiskitError
-from qiskit.providers import JobV1, BackendV2, JobStatus, Backend
+from qiskit.providers import JobV1, JobStatus, Backend
 from qiskit.result import Result
 from qiskit.result.models import ExperimentResult, ExperimentResultData
 
-from planqk.qiskit.client.client import logger, _PlanqkClient
+from planqk.qiskit.client.client import _PlanqkClient
 from planqk.qiskit.client.client_dtos import JobDto
 
 
 class ErrorData(object):
     def __init__(self, code: str, message: str):
         self.code = code
         self.message = message
 
 
 JobStatusMap = {
-    "COMPLETED": JobStatus.DONE,
+    "CREATED": JobStatus.INITIALIZING,
     "PENDING": JobStatus.QUEUED,
     "RUNNING": JobStatus.RUNNING,
+    "COMPLETED": JobStatus.DONE,
     "FAILED": JobStatus.ERROR,
     "CANCELLING": JobStatus.RUNNING,
     "CANCELLED": JobStatus.CANCELLED,
 }
 
 
 class PlanqkJob(JobV1):
```

### Comparing `planqk-quantum-1.8.0/planqk/qiskit/provider.py` & `planqk-quantum-1.8.1/planqk/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk/qiskit/providers/helper/adapter.py` & `planqk-quantum-1.8.1/planqk/qiskit/providers/helper/adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk/qiskit/providers/helper/job_input_converter.py` & `planqk-quantum-1.8.1/planqk/qiskit/providers/helper/job_input_converter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.0/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-1.8.1/planqk_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `planqk-quantum-1.8.0/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-1.8.1/planqk_quantum.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 planqk/qiskit/job.py
 planqk/qiskit/provider.py
 planqk/qiskit/client/__init__.py
 planqk/qiskit/client/backend_dtos.py
 planqk/qiskit/client/client.py
 planqk/qiskit/client/client_dtos.py
 planqk/qiskit/providers/__init__.py
-planqk/qiskit/providers/azure/__init__.py
-planqk/qiskit/providers/azure/planqk_azure_backend.py
-planqk/qiskit/providers/azure/planqk_azure_job.py
-planqk/qiskit/providers/braket/braket_job.py
-planqk/qiskit/providers/braket/planqk_braket_backend.py
 planqk/qiskit/providers/helper/__init__.py
 planqk/qiskit/providers/helper/adapter.py
 planqk/qiskit/providers/helper/job_input_converter.py
 planqk_quantum.egg-info/PKG-INFO
 planqk_quantum.egg-info/SOURCES.txt
 planqk_quantum.egg-info/dependency_links.txt
 planqk_quantum.egg-info/requires.txt
```

### Comparing `planqk-quantum-1.8.0/setup.py` & `planqk-quantum-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="1.8.0",
+    version="1.8.1",
     author='StoneOne AG',
     author_email='info@stoneone.de',
     url='https://github.com/planqk/planqk-quantum',
     description='Python library for the PlanQK Quantum Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

