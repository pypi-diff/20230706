# Comparing `tmp/planqk-quantum-1.8.5.tar.gz` & `tmp/planqk-quantum-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-1.8.5.tar", last modified: Thu Jul  6 10:50:28 2023, max compression
+gzip compressed data, was "planqk-quantum-1.8.6.tar", last modified: Thu Jul  6 10:51:58 2023, max compression
```

## Comparing `planqk-quantum-1.8.5.tar` & `planqk-quantum-1.8.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/planqk/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3679 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/client/client_dtos.py
--rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/planqk/qiskit/providers/helper/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/providers/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/providers/helper/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/planqk/qiskit/providers/helper/job_input_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 10:50:28.000000 planqk-quantum-1.8.5/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-06 10:50:28.000000 planqk-quantum-1.8.5/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 10:50:28.000000 planqk-quantum-1.8.5/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-06 10:50:28.000000 planqk-quantum-1.8.5/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-06 10:50:28.000000 planqk-quantum-1.8.5/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 10:50:28.177511 planqk-quantum-1.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-06 10:50:17.000000 planqk-quantum-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:58.812274 planqk-quantum-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 10:51:58.812274 planqk-quantum-1.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:58.808274 planqk-quantum-1.8.6/planqk/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:58.808274 planqk-quantum-1.8.6/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:58.808274 planqk-quantum-1.8.6/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/client/client_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:58.808274 planqk-quantum-1.8.6/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:58.808274 planqk-quantum-1.8.6/planqk/qiskit/providers/helper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/providers/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/providers/helper/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/planqk/qiskit/providers/helper/job_input_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 10:51:58.812274 planqk-quantum-1.8.6/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 10:51:58.000000 planqk-quantum-1.8.6/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-06 10:51:58.000000 planqk-quantum-1.8.6/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 10:51:58.000000 planqk-quantum-1.8.6/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-06 10:51:58.000000 planqk-quantum-1.8.6/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-06 10:51:58.000000 planqk-quantum-1.8.6/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 10:51:58.812274 planqk-quantum-1.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-06 10:51:47.000000 planqk-quantum-1.8.6/setup.py
```

### Comparing `planqk-quantum-1.8.5/LICENSE` & `planqk-quantum-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/PKG-INFO` & `planqk-quantum-1.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.8.5
+Version: 1.8.6
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `planqk-quantum-1.8.5/README.md` & `planqk-quantum-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk/credentials.py` & `planqk-quantum-1.8.6/planqk/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import os
 import platform
 from abc import ABC, abstractmethod
 from json import JSONDecodeError
 
-from planqk.exceptions import CredentialUnavailableError, PlanqkClientError
+from planqk.exceptions import CredentialUnavailableError
 
 _TOKEN_ENV_VARIABLE = 'PLANQK_QUANTUM_ACCESS_TOKEN'
 
 logger = logging.getLogger(__name__)
 
 
 class CredentialProvider(ABC):
@@ -90,8 +90,8 @@
                 logger.debug('%s - %s is unavailable', self.__class__.__name__, credential.__class__.__name__)
             except Exception as e:
                 logger.error('%s.get_access_token() failed: %s raised unexpected error "%s"', self.__class__.__name__,
                              credential.__class__.__name__, e, exc_info=logger.isEnabledFor(logging.DEBUG))
 
         message = f'{self.__class__.__name__} failed to retrieve an access token'
         logger.warning(message)
-        raise PlanqkClientError(message)
+        raise CredentialUnavailableError(message)
```

### Comparing `planqk-quantum-1.8.5/planqk/qiskit/backend.py` & `planqk-quantum-1.8.6/planqk/qiskit/backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk/qiskit/client/backend_dtos.py` & `planqk-quantum-1.8.6/planqk/qiskit/client/backend_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk/qiskit/client/client.py` & `planqk-quantum-1.8.6/planqk/qiskit/client/client.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk/qiskit/client/client_dtos.py` & `planqk-quantum-1.8.6/planqk/qiskit/client/client_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk/qiskit/job.py` & `planqk-quantum-1.8.6/planqk/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk/qiskit/provider.py` & `planqk-quantum-1.8.6/planqk/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk/qiskit/providers/helper/adapter.py` & `planqk-quantum-1.8.6/planqk/qiskit/providers/helper/adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk/qiskit/providers/helper/job_input_converter.py` & `planqk-quantum-1.8.6/planqk/qiskit/providers/helper/job_input_converter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-1.8.6/planqk_quantum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.8.5
+Version: 1.8.6
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `planqk-quantum-1.8.5/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-1.8.6/planqk_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.5/setup.py` & `planqk-quantum-1.8.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="1.8.5",
+    version="1.8.6",
     author='StoneOne AG',
     author_email='info@stoneone.de',
     url='https://github.com/planqk/planqk-quantum',
     description='Python library for the PlanQK Quantum Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

