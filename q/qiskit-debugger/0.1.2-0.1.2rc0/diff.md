# Comparing `tmp/qiskit_debugger-0.1.2.tar.gz` & `tmp/qiskit_debugger-0.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_debugger-0.1.2.tar", last modified: Thu Jul  6 03:36:29 2023, max compression
+gzip compressed data, was "qiskit_debugger-0.1.2rc0.tar", last modified: Thu Jul  6 03:28:32 2023, max compression
```

## Comparing `qiskit_debugger-0.1.2.tar` & `qiskit_debugger-0.1.2rc0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:36:29.981810 qiskit_debugger-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 03:26:20.000000 qiskit_debugger-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8388 2023-07-06 03:36:29.981810 qiskit_debugger-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6276 2023-07-06 03:35:11.000000 qiskit_debugger-0.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1114 2023-07-06 03:35:24.000000 qiskit_debugger-0.1.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:36:29.971810 qiskit_debugger-0.1.2/qiskit_debugger/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:36:29.981810 qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8388 2023-07-06 03:36:29.000000 qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-06 03:36:29.000000 qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 03:36:29.000000 qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 03:36:29.000000 qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 03:36:29.000000 qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5133 2023-07-06 01:22:17.000000 qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 03:36:29.981810 qiskit_debugger-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-06 03:15:41.000000 qiskit_debugger-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:28:32.251826 qiskit_debugger-0.1.2rc0/
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 03:26:20.000000 qiskit_debugger-0.1.2rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8732 2023-07-06 03:28:32.251826 qiskit_debugger-0.1.2rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-07-06 01:22:17.000000 qiskit_debugger-0.1.2rc0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-06 03:28:12.000000 qiskit_debugger-0.1.2rc0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:28:32.241826 qiskit_debugger-0.1.2rc0/qiskit_debugger/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:28:32.241826 qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8732 2023-07-06 03:28:32.000000 qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-06 03:28:32.000000 qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 03:28:32.000000 qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 03:28:32.000000 qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 03:28:32.000000 qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5133 2023-07-06 01:22:17.000000 qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 03:28:32.251826 qiskit_debugger-0.1.2rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-06 03:15:41.000000 qiskit_debugger-0.1.2rc0/setup.py
```

### Comparing `qiskit_debugger-0.1.2/LICENSE` & `qiskit_debugger-0.1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_debugger-0.1.2/PKG-INFO` & `qiskit_debugger-0.1.2rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_debugger
-Version: 0.1.2
+Version: 0.1.2rc0
 Summary: Quantum Circuit debugger for the Qiskit SDK.
 Author-email: Sirajus Salekin <ssalekin14@gmail.com>, Palvit Garg <pgarg5@ncsu.edu>, Harshwardhan Joshi <hjoshi2@ncsu.edu>
 Maintainer-email: Sirajus Salekin <ssalekin14@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Sirajus Salekin, Harsh Joshi, & Palvit Garg]
         
@@ -57,26 +57,36 @@
 - Palvit Garg (pgarg5)
 - Harshwardhan Joshi (hjoshi2)
 - Shawn Salekin (ssaleki)
 
 #### Presentation
 [URL](https://docs.google.com/presentation/d/1SCwHKmPCc7U0Hl_CVZLNMto9HAEyD_zuz_fqGwnIzuc/edit?usp=sharing)
 
-## Quickstart
-1. Install with pip 
+## How To Test
+We are assuming you are faimilar with Qiskit and git. We'd also assume you have
+jupyter notebook installed on your system. 
+
+1. Install this library via pip
 ```
 pip install qiskit_debugger
 ``` 
 
-2. Import the following the classes to experiment with the debugger like this:
+2. Ensure the following python libraries are installed in either a) python virtual environment, or b) jupyter notebook kernel.
+```
+qiskit-ibm-runtime==0.6.2
+qiskit-aer==0.11.0
+matplotlib==3.6.0
+```
+
+3. Import the following the classes to experiment with the debugger like this:
 ```
 from qiskit_debugger import QuantumDebugCircuit, QCDebugger, run_circuit
 ```
 
-3. A motivating example of how to use the debugger classes:
+4. A motivating example of how to use the debugger classes:
 
 ```
 qc = QuantumDebugCircuit(2)
 qc.x(0)
 qc.h(range(2))
 qc.cx(0, 1)
 qc.h(range(2))
@@ -94,24 +104,23 @@
 qdb = QCDebugger(qc)
 qdb.c()
 qdb.c()
 qdb.c()
 qdb.c()
 ```
 
-
-Run the circuit as a whole w/o debugger
+5. Run the circuit as a whole w/o debugger
 
 ```
 qc.measure_all()
 result = run_circuit(qc)
 print(result.get_counts())
 ```
 
-If you want to use hardware you have to initiate the `QCDebugger` like so:
+6. If you want to use hardware you have to initiate the `QCDebugger` like so:
 
 ```
 from qiskit import IBMQ
 
 # loading IBMQ account
 IBMQ.load_account()
 provider = IBMQ.get_provider(hub='ibm-q-ncsu', group='nc-state', project='grad-qc-class')
```

### Comparing `qiskit_debugger-0.1.2/README.md` & `qiskit_debugger-0.1.2rc0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,36 @@
 - Palvit Garg (pgarg5)
 - Harshwardhan Joshi (hjoshi2)
 - Shawn Salekin (ssaleki)
 
 #### Presentation
 [URL](https://docs.google.com/presentation/d/1SCwHKmPCc7U0Hl_CVZLNMto9HAEyD_zuz_fqGwnIzuc/edit?usp=sharing)
 
-## Quickstart
-1. Install with pip 
+## How To Test
+We are assuming you are faimilar with Qiskit and git. We'd also assume you have
+jupyter notebook installed on your system. 
+
+1. Install this library via pip
 ```
 pip install qiskit_debugger
 ``` 
 
-2. Import the following the classes to experiment with the debugger like this:
+2. Ensure the following python libraries are installed in either a) python virtual environment, or b) jupyter notebook kernel.
+```
+qiskit-ibm-runtime==0.6.2
+qiskit-aer==0.11.0
+matplotlib==3.6.0
+```
+
+3. Import the following the classes to experiment with the debugger like this:
 ```
 from qiskit_debugger import QuantumDebugCircuit, QCDebugger, run_circuit
 ```
 
-3. A motivating example of how to use the debugger classes:
+4. A motivating example of how to use the debugger classes:
 
 ```
 qc = QuantumDebugCircuit(2)
 qc.x(0)
 qc.h(range(2))
 qc.cx(0, 1)
 qc.h(range(2))
@@ -54,24 +64,23 @@
 qdb = QCDebugger(qc)
 qdb.c()
 qdb.c()
 qdb.c()
 qdb.c()
 ```
 
-
-Run the circuit as a whole w/o debugger
+5. Run the circuit as a whole w/o debugger
 
 ```
 qc.measure_all()
 result = run_circuit(qc)
 print(result.get_counts())
 ```
 
-If you want to use hardware you have to initiate the `QCDebugger` like so:
+6. If you want to use hardware you have to initiate the `QCDebugger` like so:
 
 ```
 from qiskit import IBMQ
 
 # loading IBMQ account
 IBMQ.load_account()
 provider = IBMQ.get_provider(hub='ibm-q-ncsu', group='nc-state', project='grad-qc-class')
```

### Comparing `qiskit_debugger-0.1.2/pyproject.toml` & `qiskit_debugger-0.1.2rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 	{name = "Sirajus Salekin", email = "ssalekin14@gmail.com"},
 	{name = "Palvit Garg", email = "pgarg5@ncsu.edu"},
 	{name = "Harshwardhan Joshi", email = "hjoshi2@ncsu.edu"},
 ]
 maintainers = [
   {name = "Sirajus Salekin", email = "ssalekin14@gmail.com"}
 ]
-version = "0.1.2"
+version = "0.1.2rc0"
 description = "Quantum Circuit debugger for the Qiskit SDK."
 keywords = ["quantum", "computing", "debugger", "qiskit"]
 readme = "README.md"
 license = { file = "LICENSE"}
 requires-python = ">=3.6"
 dependencies = [
 	"qiskit==0.43.2"
```

### Comparing `qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.egg-info/PKG-INFO` & `qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-debugger
-Version: 0.1.2
+Version: 0.1.2rc0
 Summary: Quantum Circuit debugger for the Qiskit SDK.
 Author-email: Sirajus Salekin <ssalekin14@gmail.com>, Palvit Garg <pgarg5@ncsu.edu>, Harshwardhan Joshi <hjoshi2@ncsu.edu>
 Maintainer-email: Sirajus Salekin <ssalekin14@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Sirajus Salekin, Harsh Joshi, & Palvit Garg]
         
@@ -57,26 +57,36 @@
 - Palvit Garg (pgarg5)
 - Harshwardhan Joshi (hjoshi2)
 - Shawn Salekin (ssaleki)
 
 #### Presentation
 [URL](https://docs.google.com/presentation/d/1SCwHKmPCc7U0Hl_CVZLNMto9HAEyD_zuz_fqGwnIzuc/edit?usp=sharing)
 
-## Quickstart
-1. Install with pip 
+## How To Test
+We are assuming you are faimilar with Qiskit and git. We'd also assume you have
+jupyter notebook installed on your system. 
+
+1. Install this library via pip
 ```
 pip install qiskit_debugger
 ``` 
 
-2. Import the following the classes to experiment with the debugger like this:
+2. Ensure the following python libraries are installed in either a) python virtual environment, or b) jupyter notebook kernel.
+```
+qiskit-ibm-runtime==0.6.2
+qiskit-aer==0.11.0
+matplotlib==3.6.0
+```
+
+3. Import the following the classes to experiment with the debugger like this:
 ```
 from qiskit_debugger import QuantumDebugCircuit, QCDebugger, run_circuit
 ```
 
-3. A motivating example of how to use the debugger classes:
+4. A motivating example of how to use the debugger classes:
 
 ```
 qc = QuantumDebugCircuit(2)
 qc.x(0)
 qc.h(range(2))
 qc.cx(0, 1)
 qc.h(range(2))
@@ -94,24 +104,23 @@
 qdb = QCDebugger(qc)
 qdb.c()
 qdb.c()
 qdb.c()
 qdb.c()
 ```
 
-
-Run the circuit as a whole w/o debugger
+5. Run the circuit as a whole w/o debugger
 
 ```
 qc.measure_all()
 result = run_circuit(qc)
 print(result.get_counts())
 ```
 
-If you want to use hardware you have to initiate the `QCDebugger` like so:
+6. If you want to use hardware you have to initiate the `QCDebugger` like so:
 
 ```
 from qiskit import IBMQ
 
 # loading IBMQ account
 IBMQ.load_account()
 provider = IBMQ.get_provider(hub='ibm-q-ncsu', group='nc-state', project='grad-qc-class')
```

### Comparing `qiskit_debugger-0.1.2/qiskit_debugger/qiskit_debugger.py` & `qiskit_debugger-0.1.2rc0/qiskit_debugger/qiskit_debugger.py`

 * *Files identical despite different names*

