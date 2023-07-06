# Comparing `tmp/planqk-quantum-1.8.2.tar.gz` & `tmp/planqk-quantum-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-1.8.2.tar", last modified: Thu Jul  6 09:31:20 2023, max compression
+gzip compressed data, was "planqk-quantum-1.8.3.tar", last modified: Thu Jul  6 09:54:34 2023, max compression
```

## Comparing `planqk-quantum-1.8.2.tar` & `planqk-quantum-1.8.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/planqk/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3679 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (122)     4177 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/client/client_dtos.py
--rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/planqk/qiskit/providers/helper/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/providers/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/providers/helper/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/planqk/qiskit/providers/helper/job_input_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 09:31:20.000000 planqk-quantum-1.8.2/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-06 09:31:20.000000 planqk-quantum-1.8.2/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 09:31:20.000000 planqk-quantum-1.8.2/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-06 09:31:20.000000 planqk-quantum-1.8.2/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-06 09:31:20.000000 planqk-quantum-1.8.2/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 09:31:20.924893 planqk-quantum-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-06 09:31:09.000000 planqk-quantum-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:34.541679 planqk-quantum-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 09:54:34.541679 planqk-quantum-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:34.537679 planqk-quantum-1.8.3/planqk/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3679 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:34.537679 planqk-quantum-1.8.3/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:34.537679 planqk-quantum-1.8.3/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4177 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/client/client_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:34.537679 planqk-quantum-1.8.3/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:34.541679 planqk-quantum-1.8.3/planqk/qiskit/providers/helper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/providers/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/providers/helper/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/planqk/qiskit/providers/helper/job_input_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 09:54:34.541679 planqk-quantum-1.8.3/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-06 09:54:34.000000 planqk-quantum-1.8.3/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-06 09:54:34.000000 planqk-quantum-1.8.3/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 09:54:34.000000 planqk-quantum-1.8.3/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-06 09:54:34.000000 planqk-quantum-1.8.3/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-06 09:54:34.000000 planqk-quantum-1.8.3/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 09:54:34.541679 planqk-quantum-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-06 09:54:20.000000 planqk-quantum-1.8.3/setup.py
```

### Comparing `planqk-quantum-1.8.2/LICENSE` & `planqk-quantum-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/PKG-INFO` & `planqk-quantum-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.8.2
+Version: 1.8.3
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `planqk-quantum-1.8.2/README.md` & `planqk-quantum-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/credentials.py` & `planqk-quantum-1.8.3/planqk/credentials.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/qiskit/backend.py` & `planqk-quantum-1.8.3/planqk/qiskit/backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/qiskit/client/backend_dtos.py` & `planqk-quantum-1.8.3/planqk/qiskit/client/backend_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/qiskit/client/client.py` & `planqk-quantum-1.8.3/planqk/qiskit/client/client.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/qiskit/client/client_dtos.py` & `planqk-quantum-1.8.3/planqk/qiskit/client/client_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/qiskit/job.py` & `planqk-quantum-1.8.3/planqk/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/qiskit/provider.py` & `planqk-quantum-1.8.3/planqk/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/qiskit/providers/helper/adapter.py` & `planqk-quantum-1.8.3/planqk/qiskit/providers/helper/adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk/qiskit/providers/helper/job_input_converter.py` & `planqk-quantum-1.8.3/planqk/qiskit/providers/helper/job_input_converter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-1.8.3/planqk_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 1.8.2
+Version: 1.8.3
 Summary: Python library for the PlanQK Quantum Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: StoneOne AG
 Author-email: info@stoneone.de
 License: apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `planqk-quantum-1.8.2/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-1.8.3/planqk_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planqk-quantum-1.8.2/setup.py` & `planqk-quantum-1.8.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="1.8.2",
+    version="1.8.3",
     author='StoneOne AG',
     author_email='info@stoneone.de',
     url='https://github.com/planqk/planqk-quantum',
     description='Python library for the PlanQK Quantum Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

