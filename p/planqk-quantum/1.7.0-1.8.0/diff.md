# Comparing `tmp/planqk-quantum-1.7.0.tar.gz` & `tmp/planqk-quantum-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-1.7.0.tar", last modified: Wed May 17 13:27:47 2023, max compression
+gzip compressed data, was "planqk-quantum-1.8.0.tar", last modified: Thu Jul  6 07:38:17 2023, max compression
```

## Comparing `planqk-quantum-1.7.0.tar` & `planqk-quantum-1.8.0.tar`

### file list

```diff
@@ -1,28 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/planqk/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3069 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3679 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5848 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.820867 planqk-quantum-1.7.0/planqk/qiskit/providers/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6170 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     4906 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_target_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-17 13:27:47.000000 planqk-quantum-1.7.0/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 13:27:47.824867 planqk-quantum-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-17 13:27:38.000000 planqk-quantum-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.550334 planqk-quantum-1.8.0/planqk/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3679 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.550334 planqk-quantum-1.8.0/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.550334 planqk-quantum-1.8.0/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4177 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/client/client_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4138 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.550334 planqk-quantum-1.8.0/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/planqk/qiskit/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6021 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/azure/planqk_azure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8556 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/azure/planqk_azure_job.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/planqk/qiskit/providers/braket/
+-rw-r--r--   0 runner    (1001) docker     (122)     4256 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/braket/braket_job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/braket/planqk_braket_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/planqk/qiskit/providers/helper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/helper/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/planqk/qiskit/providers/helper/job_input_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-06 07:38:17.000000 planqk-quantum-1.8.0/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 07:38:17.554334 planqk-quantum-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-06 07:38:00.000000 planqk-quantum-1.8.0/setup.py
```

### Comparing `planqk-quantum-1.7.0/LICENSE` & `planqk-quantum-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.7.0/PKG-INFO` & `planqk-quantum-1.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,29 +12,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python library for the PlanQK Platform
 
 [![PyPI version](https://badge.fury.io/py/planqk-quantum.svg)](https://badge.fury.io/py/planqk-quantum)
 
-The `planqk-quantum` library is a SDK for developing quantum circuits using [Qiskit](https://pypi.org/project/qiskit) to be run on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de).
+The `planqk-quantum` library is an SDK for developing quantum circuits using [Qiskit](https://pypi.org/project/qiskit) to be run on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de).
 
 ## Getting Started
 
 Check out the following guides on how to get started with PlanQK:
 
-- [Tutorial on how to create a PlanQK Service using the `planqk-quantum` library](https://docs.platform.planqk.de/tutorials/tutorial-qiskit.html)
-- [General guide on how to create and deploy PlanQK Services](https://docs.platform.planqk.de/docs/service-platform/managed-services.html)
+- [PlanQK Quickstart Guide](https://docs.platform.planqk.de/tutorials/tutorial-qiskit.html)
+- [Using the `planqk-quantum` SDK](https://docs.platform.planqk.de/docs/getting-started/using-sdk.html)
 
 ## Installation
 
 The package is released on PyPI and can be installed via `pip`:
 
 ```bash
-pip install planqk-quantum
+pip install --upgrade planqk-quantum
 ```
 
 ## Development
 
 To create a new Conda environment, run:
 
 ```bash
```

### Comparing `planqk-quantum-1.7.0/README.md` & `planqk-quantum-1.8.0/planqk_quantum.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,40 @@
+Metadata-Version: 2.1
+Name: planqk-quantum
+Version: 1.8.0
+Summary: Python library for the PlanQK Quantum Platform
+Home-page: https://github.com/planqk/planqk-quantum
+Author: StoneOne AG
+Author-email: info@stoneone.de
+License: apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Python library for the PlanQK Platform
 
 [![PyPI version](https://badge.fury.io/py/planqk-quantum.svg)](https://badge.fury.io/py/planqk-quantum)
 
-The `planqk-quantum` library is a SDK for developing quantum circuits using [Qiskit](https://pypi.org/project/qiskit) to be run on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de).
+The `planqk-quantum` library is an SDK for developing quantum circuits using [Qiskit](https://pypi.org/project/qiskit) to be run on quantum devices provided by the [PlanQK Platform](https://docs.platform.planqk.de).
 
 ## Getting Started
 
 Check out the following guides on how to get started with PlanQK:
 
-- [Tutorial on how to create a PlanQK Service using the `planqk-quantum` library](https://docs.platform.planqk.de/tutorials/tutorial-qiskit.html)
-- [General guide on how to create and deploy PlanQK Services](https://docs.platform.planqk.de/docs/service-platform/managed-services.html)
+- [PlanQK Quickstart Guide](https://docs.platform.planqk.de/tutorials/tutorial-qiskit.html)
+- [Using the `planqk-quantum` SDK](https://docs.platform.planqk.de/docs/getting-started/using-sdk.html)
 
 ## Installation
 
 The package is released on PyPI and can be installed via `pip`:
 
 ```bash
-pip install planqk-quantum
+pip install --upgrade planqk-quantum
 ```
 
 ## Development
 
 To create a new Conda environment, run:
 
 ```bash
```

### Comparing `planqk-quantum-1.7.0/planqk/credentials.py` & `planqk-quantum-1.8.0/planqk/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 class StaticCredential(CredentialProvider):
     def __init__(self, access_token=None):
         self.access_token = access_token
 
     def get_access_token(self) -> str:
         if not self.access_token:
-            raise CredentialUnavailableError(f'Access Token not set')
+            raise CredentialUnavailableError(f'Access token not set')
         return self.access_token
 
 
 class DefaultCredentialsProvider(CredentialProvider):
     def __init__(self, access_token=None):
         self.credentials = [
             StaticCredential(access_token),
```

### Comparing `planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_backend.py` & `planqk-quantum-1.8.0/planqk/qiskit/providers/azure/planqk_azure_backend.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 import logging
 
 from azure.quantum.qiskit.backends.backend import AzureBackend
 from qiskit.providers import Backend
 from qiskit.qobj import Qobj, QasmQobj
 
-from planqk.client import _PlanqkClient
 from planqk.qiskit.job import PlanqkJob
 from planqk.qiskit.providers.azure.planqk_azure_job import _PlanqkAzureJob
 
 logger = logging.getLogger(__name__)
 
 
 class _PlanqkAzureBackend(Backend):
     backend_name = None
 
-    def __init__(self, client: _PlanqkClient, azure_backend: AzureBackend):
-        self._client = client
+    def __init__(self, azure_backend: AzureBackend):
         self.backend = azure_backend
 
     def run(self, circuit, **kwargs):
         """
-        Submits the given circuit to run on an Azure Quantum backend.
+        Submits the given input to run on an Azure Quantum backend.
         """
 
         # Some Qiskit features require passing lists of circuits, so unpack those here.
         # We currently only support single-experiment jobs.
         if isinstance(circuit, (list, tuple)):
             if len(circuit) > 1:
                 raise NotImplementedError("Multi-experiment jobs are not supported!")
             circuit = circuit[0]
 
-        # If the circuit was created using qiskit.assemble,
+        # If the input was created using qiskit.assemble,
         # disassemble into QASM here
         if isinstance(circuit, QasmQobj) or isinstance(circuit, Qobj):
             from qiskit.assembler import disassemble
             circuits, run, _ = disassemble(circuit)
             circuit = circuits[0]
             if kwargs.get("shots") is None:
                 # Note that the default number of shots for QObj is 1024
@@ -44,53 +42,52 @@
         # The default of these job parameters come from the AzureBackend configuration:
         config = self.configuration()
         provider_id = kwargs.pop("provider_id", config.azure["provider_id"])
         input_data_format = kwargs.pop("input_data_format", config.azure["input_data_format"])
         output_data_format = kwargs.pop("output_data_format", config.azure["output_data_format"])
 
         # If not provided as kwargs, the values of these parameters
-        # are calculated from the circuit itself:
+        # are calculated from the input itself:
         job_name = kwargs.pop("job_name", circuit.name)
         input_data = self.backend._translate_circuit(circuit, **kwargs)
         metadata = kwargs.pop("metadata") if "metadata" in kwargs else self.backend._job_metadata(circuit, **kwargs)
 
-        # Backend options are mapped to input_params.
-        # Take also into consideration options passed in the kwargs, as the take precedence
+        # Backend kwargs are mapped to input_params.
+        # Take also into consideration kwargs passed in the kwargs, as the take precedence
         # over default values:
         input_params = vars(self.backend.options)
         for opt in kwargs.copy():
             if opt in input_params:
                 input_params[opt] = kwargs.pop(opt)
 
         logger.info(f"Submitting new job for backend {self.name()}")
         job = _PlanqkAzureJob(
-            client=self._client,
             backend=self,
             target=self.name(),
             name=job_name,
             provider_id=provider_id,
             input_data=input_data.decode("utf-8"),
             input_data_format=input_data_format,
             output_data_format=output_data_format,
             input_params=input_params,
             metadata=metadata,
             **kwargs
         )
 
-        logger.info(f"Submitted job with id '{job.id()}' for circuit '{circuit.name}':")
+        logger.info(f"Submitted job with id '{job.id()}' for input '{circuit.name}':")
         logger.info(input_data)
 
         return job
 
     def retrieve_job(self, job_id) -> _PlanqkAzureJob:
         """
         Returns the Job instance associated with the given id.
         """
-        planqk_job = PlanqkJob(self._client, job_id=job_id)
-        return _PlanqkAzureJob(client=self._client, backend=self, planqk_job=planqk_job)
+        planqk_job = PlanqkJob(job_id=job_id)
+        return _PlanqkAzureJob(backend=self, planqk_job=planqk_job)
 
     def name(self):
         """
         Return the backend name.
 
         Returns:
             str: the name of the backend.
@@ -126,17 +123,17 @@
            BackendConfiguration: the configuration for the backend.
        """
         return self.backend.configuration
 
     @property
     def options(self):
         """
-        Return the options for the backend.
+        Return the kwargs for the backend.
 
-        The options of a backend are the dynamic parameters defining
+        The kwargs of a backend are the dynamic parameters defining
         how the backend is used. These are used to control the :meth:`run` method.
         """
         return self.backend.options
 
     @property
     def properties(self):
         """
@@ -146,35 +143,35 @@
             BackendProperties: the configuration for the backend. If the backend
             does not support properties, it returns ``None``.
         """
         return self.backend.properties
 
     def provider(self):
         """
-        Return the backend Provider.
+        Return the backend SupportedProviders.
 
         Returns:
-            Provider: the Provider responsible for the backend.
+            SupportedProviders: the SupportedProviders responsible for the backend.
         """
         return self.backend.provider()
 
     def set_options(self, **fields):
         """
-        Set the options fields for the backend.
+        Set the kwargs fields for the backend.
 
-        This method is used to update the options of a backend. If
-        you need to change any of the options prior to running just
-        pass in the kwarg with the new value for the options.
+        This method is used to update the kwargs of a backend. If
+        you need to change any of the kwargs prior to running just
+        pass in the kwarg with the new value for the kwargs.
 
         Args:
-            fields: The fields to update the options
+            fields: The fields to update the kwargs
 
         Raises:
             AttributeError: If the field passed in is not part of the
-                options
+                kwargs
         """
         self.backend.set_options(**fields)
 
     def status(self):
         """
         Return the backend status.
```

### Comparing `planqk-quantum-1.7.0/planqk/qiskit/providers/azure/planqk_azure_job.py` & `planqk-quantum-1.8.0/planqk/qiskit/providers/azure/planqk_azure_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 import json
 from collections import defaultdict
 
 import numpy as np
 from qiskit.providers import JobV1, JobStatus
 from qiskit.result import Result
 
-from planqk.client import _PlanqkClient
 from planqk.qiskit.job import PlanqkJob
 
 # Azure status codes being used here
 AzureJobStatusMap = {
-    "Succeeded": JobStatus.DONE,
-    "Waiting": JobStatus.QUEUED,
-    "Executing": JobStatus.RUNNING,
-    "Failed": JobStatus.ERROR,
-    "Cancelled": JobStatus.CANCELLED,
-    "Finishing": JobStatus.RUNNING
+    "COMPLETED": JobStatus.DONE,
+    "PENDING": JobStatus.QUEUED,
+    "RUNNING": JobStatus.RUNNING,
+    "FAILED": JobStatus.ERROR,
+    "CANCELLED": JobStatus.CANCELLED,
 }
 
 # Constants for output data format
 MICROSOFT_OUTPUT_DATA_FORMAT = "microsoft.quantum-results.v1"
 IONQ_OUTPUT_DATA_FORMAT = "ionq.quantum-results.v1"
 HONEYWELL_OUTPUT_DATA_FORMAT = "honeywell.quantum-results.v1"
 
 
 class _PlanqkAzureJob(JobV1):
 
     def __init__(
             self,
-            client: _PlanqkClient,
             backend,  # TODO _PlanqkAzureBackend causes circular dependency -> use job details
             planqk_job: PlanqkJob = None,
             **kwargs
     ) -> None:
         if planqk_job is None:
             self._planqk_job = PlanqkJob(
-                client=client,
                 **kwargs
             )
             self.submit()
         else:
             self._planqk_job = planqk_job
 
         super().__init__(backend, self._planqk_job.id, **kwargs)
@@ -49,17 +45,17 @@
         """
         self._planqk_job.submit()
 
     def result(self, timeout=None, sampler_seed=None):
         """
         Return the results of the job.
         """
-        self._planqk_job.wait_until_completed(timeout_secs=timeout)
+        self._planqk_job.wait_for_final_state(timeout_secs=timeout)
 
-        success = self._planqk_job.status == "Succeeded"
+        success = self._planqk_job.status == "COMPLETED"
         results = self._format_results(sampler_seed=sampler_seed)
 
         return Result.from_dict(
             {
                 "results": [results],
                 "job_id": self._planqk_job.id,
                 "backend_name": self._backend.name(),
@@ -72,15 +68,15 @@
     def cancel(self):
         self._planqk_job.cancel()
 
     def status(self):
         """
         Return the status of the job, among the values of ``JobStatus``.
         """
-        self._planqk_job.refresh()
+        self._planqk_job._refresh()
         status = AzureJobStatusMap[self._planqk_job.status]
         return status
 
     def job_id(self):
         """
         This job's id.
         """
@@ -98,15 +94,15 @@
         """
         return None
 
     def _format_results(self, sampler_seed=None):
         """
         Populates the results datastructures in a format that is compatible with qiskit libraries.
         """
-        success = self._planqk_job.status == "Succeeded"
+        success = self._planqk_job.status == "COMPLETED"
         shots_key = "shots"
 
         job_result = {
             "data": {},
             "success": success,
             "header": {},
         }
```

### Comparing `planqk-quantum-1.7.0/setup.py` & `planqk-quantum-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="1.7.0",
+    version="1.8.0",
     author='StoneOne AG',
     author_email='info@stoneone.de',
     url='https://github.com/planqk/planqk-quantum',
     description='Python library for the PlanQK Quantum Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

