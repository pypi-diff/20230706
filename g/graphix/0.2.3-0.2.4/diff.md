# Comparing `tmp/graphix-0.2.3.tar.gz` & `tmp/graphix-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphix-0.2.3.tar", last modified: Sun Jun 25 12:44:31 2023, max compression
+gzip compressed data, was "graphix-0.2.4.tar", last modified: Thu Jul  6 17:52:23 2023, max compression
```

## Comparing `graphix-0.2.3.tar` & `graphix-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.013814 graphix-0.2.3/
--rw-r--r--   0 sunami     (501) staff       (20)    10761 2023-06-25 12:12:17.000000 graphix-0.2.3/LICENSE
--rw-r--r--   0 sunami     (501) staff       (20)       94 2023-06-25 12:12:17.000000 graphix-0.2.3/MANIFEST.in
--rw-r--r--   0 sunami     (501) staff       (20)     5510 2023-06-25 12:44:31.013613 graphix-0.2.3/PKG-INFO
--rw-r--r--   0 sunami     (501) staff       (20)     4576 2023-06-25 12:12:17.000000 graphix-0.2.3/README.md
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.009542 graphix-0.2.3/graphix/
--rw-r--r--   0 sunami     (501) staff       (20)      247 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/__init__.py
--rw-r--r--   0 sunami     (501) staff       (20)     7451 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/clifford.py
--rw-r--r--   0 sunami     (501) staff       (20)     4173 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/generator.py
--rw-r--r--   0 sunami     (501) staff       (20)    13035 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/gflow.py
--rw-r--r--   0 sunami     (501) staff       (20)    14059 2023-06-25 12:16:17.000000 graphix-0.2.3/graphix/graphsim.py
--rw-r--r--   0 sunami     (501) staff       (20)     2463 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/ops.py
--rw-r--r--   0 sunami     (501) staff       (20)    68268 2023-06-25 12:16:17.000000 graphix-0.2.3/graphix/pattern.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.010939 graphix-0.2.3/graphix/sim/
--rw-r--r--   0 sunami     (501) staff       (20)        0 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/sim/__init__.py
--rw-r--r--   0 sunami     (501) staff       (20)    11396 2023-06-25 12:16:17.000000 graphix-0.2.3/graphix/sim/statevec.py
--rw-r--r--   0 sunami     (501) staff       (20)    26314 2023-06-25 12:16:17.000000 graphix-0.2.3/graphix/sim/tensornet.py
--rw-r--r--   0 sunami     (501) staff       (20)     2269 2023-06-25 12:41:22.000000 graphix-0.2.3/graphix/simulator.py
--rw-r--r--   0 sunami     (501) staff       (20)    37241 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/transpiler.py
--rw-r--r--   0 sunami     (501) staff       (20)       22 2023-06-25 12:41:33.000000 graphix-0.2.3/graphix/version.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.010354 graphix-0.2.3/graphix.egg-info/
--rw-r--r--   0 sunami     (501) staff       (20)     5510 2023-06-25 12:44:30.000000 graphix-0.2.3/graphix.egg-info/PKG-INFO
--rw-r--r--   0 sunami     (501) staff       (20)      631 2023-06-25 12:44:31.000000 graphix-0.2.3/graphix.egg-info/SOURCES.txt
--rw-r--r--   0 sunami     (501) staff       (20)        1 2023-06-25 12:44:30.000000 graphix-0.2.3/graphix.egg-info/dependency_links.txt
--rw-r--r--   0 sunami     (501) staff       (20)       85 2023-06-25 12:44:30.000000 graphix-0.2.3/graphix.egg-info/requires.txt
--rw-r--r--   0 sunami     (501) staff       (20)        8 2023-06-25 12:44:30.000000 graphix-0.2.3/graphix.egg-info/top_level.txt
--rw-r--r--   0 sunami     (501) staff       (20)       81 2023-06-25 12:12:17.000000 graphix-0.2.3/pyproject.toml
--rw-r--r--   0 sunami     (501) staff       (20)       38 2023-06-25 12:44:31.013918 graphix-0.2.3/setup.cfg
--rw-r--r--   0 sunami     (501) staff       (20)     1488 2023-06-25 12:12:17.000000 graphix-0.2.3/setup.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.013250 graphix-0.2.3/tests/
--rw-r--r--   0 sunami     (501) staff       (20)     2904 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_clifford.py
--rw-r--r--   0 sunami     (501) staff       (20)     2986 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_generator.py
--rw-r--r--   0 sunami     (501) staff       (20)     2479 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_gflow.py
--rw-r--r--   0 sunami     (501) staff       (20)     3974 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_graphsim.py
--rw-r--r--   0 sunami     (501) staff       (20)    15447 2023-06-25 12:16:17.000000 graphix-0.2.3/tests/test_pattern.py
--rw-r--r--   0 sunami     (501) staff       (20)    15771 2023-06-25 12:16:17.000000 graphix-0.2.3/tests/test_tnsim.py
--rw-r--r--   0 sunami     (501) staff       (20)     5102 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_transpiler.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-07-06 17:52:23.397570 graphix-0.2.4/
+-rw-r--r--   0 sunami     (501) staff       (20)    10761 2023-06-25 12:12:17.000000 graphix-0.2.4/LICENSE
+-rw-r--r--   0 sunami     (501) staff       (20)       94 2023-06-25 12:12:17.000000 graphix-0.2.4/MANIFEST.in
+-rw-r--r--   0 sunami     (501) staff       (20)     6049 2023-07-06 17:52:23.397287 graphix-0.2.4/PKG-INFO
+-rw-r--r--   0 sunami     (501) staff       (20)     5072 2023-07-04 22:20:33.000000 graphix-0.2.4/README.md
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-07-06 17:52:23.388060 graphix-0.2.4/graphix/
+-rw-r--r--   0 sunami     (501) staff       (20)      247 2023-06-25 12:12:17.000000 graphix-0.2.4/graphix/__init__.py
+-rw-r--r--   0 sunami     (501) staff       (20)     7451 2023-06-25 12:12:17.000000 graphix-0.2.4/graphix/clifford.py
+-rw-r--r--   0 sunami     (501) staff       (20)     3749 2023-07-04 22:20:33.000000 graphix-0.2.4/graphix/device_interface.py
+-rw-r--r--   0 sunami     (501) staff       (20)     4173 2023-06-25 12:12:17.000000 graphix-0.2.4/graphix/generator.py
+-rw-r--r--   0 sunami     (501) staff       (20)    13035 2023-06-25 12:12:17.000000 graphix-0.2.4/graphix/gflow.py
+-rw-r--r--   0 sunami     (501) staff       (20)    14059 2023-06-25 12:16:17.000000 graphix-0.2.4/graphix/graphsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2463 2023-06-25 12:12:17.000000 graphix-0.2.4/graphix/ops.py
+-rw-r--r--   0 sunami     (501) staff       (20)    68918 2023-07-04 22:20:33.000000 graphix-0.2.4/graphix/pattern.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-07-06 17:52:23.393753 graphix-0.2.4/graphix/sim/
+-rw-r--r--   0 sunami     (501) staff       (20)        0 2023-06-25 12:12:17.000000 graphix-0.2.4/graphix/sim/__init__.py
+-rw-r--r--   0 sunami     (501) staff       (20)    11396 2023-06-25 12:16:17.000000 graphix-0.2.4/graphix/sim/statevec.py
+-rw-r--r--   0 sunami     (501) staff       (20)    26314 2023-06-25 12:16:17.000000 graphix-0.2.4/graphix/sim/tensornet.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2269 2023-07-06 14:15:57.000000 graphix-0.2.4/graphix/simulator.py
+-rw-r--r--   0 sunami     (501) staff       (20)    37241 2023-06-25 12:12:17.000000 graphix-0.2.4/graphix/transpiler.py
+-rw-r--r--   0 sunami     (501) staff       (20)       22 2023-07-06 17:48:31.000000 graphix-0.2.4/graphix/version.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-07-06 17:52:23.392905 graphix-0.2.4/graphix.egg-info/
+-rw-r--r--   0 sunami     (501) staff       (20)     6049 2023-07-06 17:52:23.000000 graphix-0.2.4/graphix.egg-info/PKG-INFO
+-rw-r--r--   0 sunami     (501) staff       (20)      680 2023-07-06 17:52:23.000000 graphix-0.2.4/graphix.egg-info/SOURCES.txt
+-rw-r--r--   0 sunami     (501) staff       (20)        1 2023-07-06 17:52:23.000000 graphix-0.2.4/graphix.egg-info/dependency_links.txt
+-rw-r--r--   0 sunami     (501) staff       (20)      128 2023-07-06 17:52:23.000000 graphix-0.2.4/graphix.egg-info/requires.txt
+-rw-r--r--   0 sunami     (501) staff       (20)        8 2023-07-06 17:52:23.000000 graphix-0.2.4/graphix.egg-info/top_level.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       81 2023-06-25 12:12:17.000000 graphix-0.2.4/pyproject.toml
+-rw-r--r--   0 sunami     (501) staff       (20)       38 2023-07-06 17:52:23.397683 graphix-0.2.4/setup.cfg
+-rw-r--r--   0 sunami     (501) staff       (20)     1565 2023-07-04 22:20:33.000000 graphix-0.2.4/setup.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-07-06 17:52:23.396792 graphix-0.2.4/tests/
+-rw-r--r--   0 sunami     (501) staff       (20)     2904 2023-06-25 12:12:17.000000 graphix-0.2.4/tests/test_clifford.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2986 2023-06-25 12:12:17.000000 graphix-0.2.4/tests/test_generator.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2479 2023-06-25 12:12:17.000000 graphix-0.2.4/tests/test_gflow.py
+-rw-r--r--   0 sunami     (501) staff       (20)     3974 2023-06-25 12:12:17.000000 graphix-0.2.4/tests/test_graphsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)    15447 2023-06-25 12:16:17.000000 graphix-0.2.4/tests/test_pattern.py
+-rw-r--r--   0 sunami     (501) staff       (20)     1388 2023-07-04 22:20:33.000000 graphix-0.2.4/tests/test_runner.py
+-rw-r--r--   0 sunami     (501) staff       (20)    15771 2023-06-25 12:16:17.000000 graphix-0.2.4/tests/test_tnsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)     5102 2023-06-25 12:12:17.000000 graphix-0.2.4/tests/test_transpiler.py
```

### Comparing `graphix-0.2.3/LICENSE` & `graphix-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/PKG-INFO` & `graphix-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.3
+Version: 0.2.4
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
@@ -16,24 +16,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
+Provides-Extra: extra
+Provides-Extra: test
 License-File: LICENSE
 
 <img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="550">
 
-[![Documentation Status](https://readthedocs.org/projects/graphix/badge/?version=latest)](https://graphix.readthedocs.io/en/latest/?badge=latest)
-![GitHub](https://img.shields.io/github/license/TeamGraphix/graphix)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix)
 ![PyPI](https://img.shields.io/pypi/v/graphix)
 [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg)](https://unitary.fund/)
 [![DOI](https://zenodo.org/badge/573466585.svg)](https://zenodo.org/badge/latestdoi/573466585)
+[![Documentation Status](https://readthedocs.org/projects/graphix/badge/?version=latest)](https://graphix.readthedocs.io/en/latest/?badge=latest)
+![GitHub](https://img.shields.io/github/license/TeamGraphix/graphix)
+[![Downloads](https://static.pepy.tech/badge/graphix)](https://pepy.tech/project/graphix)
 
 **Graphix** is a measurement-based quantum computing (MBQC) compiler, which makes it easier to generate, optimize and simulate MBQC *measurement patterns*.
 
 ## Feature
 
 - We integrate an efficient [graph state simulator](https://graphix.readthedocs.io/en/latest/lc-mbqc.html) as an optimization routine of MBQC *measurement pattern*, with which we can classically [preprocess all Pauli measurements](https://graphix.readthedocs.io/en/latest/tutorial.html#performing-pauli-measurements) (corresponding to the elimination of all Clifford gates in the gate network - c.f. [Gottesman-Knill theorem](https://en.wikipedia.org/wiki/Gottesman–Knill_theorem)), significantly reducing the required size of graph state to run the computation.
 - We implement tensor-network simulation of MBQC with which thousands of qubits (graph nodes) can be simulated with modest computing resources (e.g. laptop), without approximation.
@@ -42,14 +45,24 @@
 ## Installation
 Install `graphix` with `pip`:
 
 ```bash
 $ pip install graphix
 ```
 
+Install together with device interface:
+```bash
+$ pip install graphix[extra]
+```
+this will install `graphix` and [IBMQ interface](https://github.com/TeamGraphix/graphix-ibmq) to run MBQC patterns on IBM devices and Aer simulator.
+
+We are currently adding more quantum device interfaces.
+Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind!
+
+
 ## Next Steps
 
 - We have a few [demos](https://graphix.readthedocs.io/en/latest/gallery/index.html) showing basic usages of `Graphix`.
 - You can run demos on your browser:
   - Preprocessing Clifford gates: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=deutsch-jozsa.ipynb)
   - Using tensor-network simulator backend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qft_with_tn.ipynb)
   - QAOA circuit: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qaoa.ipynb)
```

### Comparing `graphix-0.2.3/README.md` & `graphix-0.2.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="550">
 
-[![Documentation Status](https://readthedocs.org/projects/graphix/badge/?version=latest)](https://graphix.readthedocs.io/en/latest/?badge=latest)
-![GitHub](https://img.shields.io/github/license/TeamGraphix/graphix)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix)
 ![PyPI](https://img.shields.io/pypi/v/graphix)
 [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg)](https://unitary.fund/)
 [![DOI](https://zenodo.org/badge/573466585.svg)](https://zenodo.org/badge/latestdoi/573466585)
+[![Documentation Status](https://readthedocs.org/projects/graphix/badge/?version=latest)](https://graphix.readthedocs.io/en/latest/?badge=latest)
+![GitHub](https://img.shields.io/github/license/TeamGraphix/graphix)
+[![Downloads](https://static.pepy.tech/badge/graphix)](https://pepy.tech/project/graphix)
 
 **Graphix** is a measurement-based quantum computing (MBQC) compiler, which makes it easier to generate, optimize and simulate MBQC *measurement patterns*.
 
 ## Feature
 
 - We integrate an efficient [graph state simulator](https://graphix.readthedocs.io/en/latest/lc-mbqc.html) as an optimization routine of MBQC *measurement pattern*, with which we can classically [preprocess all Pauli measurements](https://graphix.readthedocs.io/en/latest/tutorial.html#performing-pauli-measurements) (corresponding to the elimination of all Clifford gates in the gate network - c.f. [Gottesman-Knill theorem](https://en.wikipedia.org/wiki/Gottesman–Knill_theorem)), significantly reducing the required size of graph state to run the computation.
 - We implement tensor-network simulation of MBQC with which thousands of qubits (graph nodes) can be simulated with modest computing resources (e.g. laptop), without approximation.
@@ -18,14 +19,24 @@
 ## Installation
 Install `graphix` with `pip`:
 
 ```bash
 $ pip install graphix
 ```
 
+Install together with device interface:
+```bash
+$ pip install graphix[extra]
+```
+this will install `graphix` and [IBMQ interface](https://github.com/TeamGraphix/graphix-ibmq) to run MBQC patterns on IBM devices and Aer simulator.
+
+We are currently adding more quantum device interfaces.
+Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind!
+
+
 ## Next Steps
 
 - We have a few [demos](https://graphix.readthedocs.io/en/latest/gallery/index.html) showing basic usages of `Graphix`.
 - You can run demos on your browser:
   - Preprocessing Clifford gates: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=deutsch-jozsa.ipynb)
   - Using tensor-network simulator backend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qft_with_tn.ipynb)
   - QAOA circuit: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qaoa.ipynb)
```

### Comparing `graphix-0.2.3/graphix/clifford.py` & `graphix-0.2.4/graphix/clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix/generator.py` & `graphix-0.2.4/graphix/generator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix/gflow.py` & `graphix-0.2.4/graphix/gflow.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix/graphsim.py` & `graphix-0.2.4/graphix/graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix/ops.py` & `graphix-0.2.4/graphix/ops.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix/pattern.py` & `graphix-0.2.4/graphix/pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """MBQC pattern according to Measurement Calculus
 ref: V. Danos, E. Kashefi and P. Panangaden. J. ACM 54.2 8 (2007)
 """
 import numpy as np
 import networkx as nx
 from graphix.simulator import PatternSimulator
+from graphix.device_interface import PatternRunner
 from graphix.graphsim import GraphState
 from graphix.gflow import flow, gflow, get_layers
 from graphix.clifford import CLIFFORD_CONJ, CLIFFORD_TO_QASM3, CLIFFORD_MEASURE
 from copy import deepcopy
 
 
 class Pattern:
@@ -1162,14 +1163,34 @@
 
         .. seealso:: :class:`graphix.simulator.PatternSimulator`
         """
         sim = PatternSimulator(self, backend=backend, **kwargs)
         state = sim.run()
         return state
 
+    def run_pattern(self, backend, **kwargs):
+        """run the pattern on cloud-based quantum devices and their simulators.
+        Available backend: ['ibmq']
+
+        Parameters
+        ----------
+        backend : str
+            parameter to select executor backend.
+        kwargs: keyword args for specified backend.
+
+        Returns
+        -------
+        result :
+            the measurement result,
+            in the representation depending on the backend used.
+        """
+        exe = PatternRunner(self, backend=backend, **kwargs)
+        result = exe.run()
+        return result
+
     def perform_pauli_measurements(self):
         """Perform Pauli measurements in the pattern using
         efficient stabilizer simulator.
 
         .. seealso:: :func:`measure_pauli`
 
         """
```

### Comparing `graphix-0.2.3/graphix/sim/statevec.py` & `graphix-0.2.4/graphix/sim/statevec.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix/sim/tensornet.py` & `graphix-0.2.4/graphix/sim/tensornet.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix/simulator.py` & `graphix-0.2.4/graphix/simulator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix/transpiler.py` & `graphix-0.2.4/graphix/transpiler.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/graphix.egg-info/PKG-INFO` & `graphix-0.2.4/graphix.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.3
+Version: 0.2.4
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
@@ -16,24 +16,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
+Provides-Extra: extra
+Provides-Extra: test
 License-File: LICENSE
 
 <img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="550">
 
-[![Documentation Status](https://readthedocs.org/projects/graphix/badge/?version=latest)](https://graphix.readthedocs.io/en/latest/?badge=latest)
-![GitHub](https://img.shields.io/github/license/TeamGraphix/graphix)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix)
 ![PyPI](https://img.shields.io/pypi/v/graphix)
 [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg)](https://unitary.fund/)
 [![DOI](https://zenodo.org/badge/573466585.svg)](https://zenodo.org/badge/latestdoi/573466585)
+[![Documentation Status](https://readthedocs.org/projects/graphix/badge/?version=latest)](https://graphix.readthedocs.io/en/latest/?badge=latest)
+![GitHub](https://img.shields.io/github/license/TeamGraphix/graphix)
+[![Downloads](https://static.pepy.tech/badge/graphix)](https://pepy.tech/project/graphix)
 
 **Graphix** is a measurement-based quantum computing (MBQC) compiler, which makes it easier to generate, optimize and simulate MBQC *measurement patterns*.
 
 ## Feature
 
 - We integrate an efficient [graph state simulator](https://graphix.readthedocs.io/en/latest/lc-mbqc.html) as an optimization routine of MBQC *measurement pattern*, with which we can classically [preprocess all Pauli measurements](https://graphix.readthedocs.io/en/latest/tutorial.html#performing-pauli-measurements) (corresponding to the elimination of all Clifford gates in the gate network - c.f. [Gottesman-Knill theorem](https://en.wikipedia.org/wiki/Gottesman–Knill_theorem)), significantly reducing the required size of graph state to run the computation.
 - We implement tensor-network simulation of MBQC with which thousands of qubits (graph nodes) can be simulated with modest computing resources (e.g. laptop), without approximation.
@@ -42,14 +45,24 @@
 ## Installation
 Install `graphix` with `pip`:
 
 ```bash
 $ pip install graphix
 ```
 
+Install together with device interface:
+```bash
+$ pip install graphix[extra]
+```
+this will install `graphix` and [IBMQ interface](https://github.com/TeamGraphix/graphix-ibmq) to run MBQC patterns on IBM devices and Aer simulator.
+
+We are currently adding more quantum device interfaces.
+Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind!
+
+
 ## Next Steps
 
 - We have a few [demos](https://graphix.readthedocs.io/en/latest/gallery/index.html) showing basic usages of `Graphix`.
 - You can run demos on your browser:
   - Preprocessing Clifford gates: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=deutsch-jozsa.ipynb)
   - Using tensor-network simulator backend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qft_with_tn.ipynb)
   - QAOA circuit: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qaoa.ipynb)
```

### Comparing `graphix-0.2.3/graphix.egg-info/SOURCES.txt` & `graphix-0.2.4/graphix.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 graphix/__init__.py
 graphix/clifford.py
+graphix/device_interface.py
 graphix/generator.py
 graphix/gflow.py
 graphix/graphsim.py
 graphix/ops.py
 graphix/pattern.py
 graphix/simulator.py
 graphix/transpiler.py
@@ -22,9 +23,10 @@
 graphix/sim/statevec.py
 graphix/sim/tensornet.py
 tests/test_clifford.py
 tests/test_generator.py
 tests/test_gflow.py
 tests/test_graphsim.py
 tests/test_pattern.py
+tests/test_runner.py
 tests/test_tnsim.py
 tests/test_transpiler.py
```

### Comparing `graphix-0.2.3/setup.py` & `graphix-0.2.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,10 +32,11 @@
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Physics",
     ],
     "python_requires": ">=3.8,<3.11",
     "install_requires": requirements,
+    "extras_require": {'extra': ['graphix-ibmq'], 'test': ['graphix-ibmq']},
 }
 
 setup(**(info))
```

### Comparing `graphix-0.2.3/tests/test_clifford.py` & `graphix-0.2.4/tests/test_clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/tests/test_generator.py` & `graphix-0.2.4/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/tests/test_gflow.py` & `graphix-0.2.4/tests/test_gflow.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/tests/test_graphsim.py` & `graphix-0.2.4/tests/test_graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/tests/test_pattern.py` & `graphix-0.2.4/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/tests/test_tnsim.py` & `graphix-0.2.4/tests/test_tnsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.3/tests/test_transpiler.py` & `graphix-0.2.4/tests/test_transpiler.py`

 * *Files identical despite different names*

