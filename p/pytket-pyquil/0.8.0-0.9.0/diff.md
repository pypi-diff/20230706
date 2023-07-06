# Comparing `tmp/pytket-pyquil-0.8.0.tar.gz` & `tmp/pytket-pyquil-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-pyquil-0.8.0.tar", last modified: Tue Mar  2 14:34:42 2021, max compression
+gzip compressed data, was "pytket-pyquil-0.9.0.tar", last modified: Thu Apr  1 10:57:41 2021, max compression
```

## Comparing `pytket-pyquil-0.8.0.tar` & `pytket-pyquil-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:34:42.635419 pytket-pyquil-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-02 14:31:41.000000 pytket-pyquil-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2021-03-02 14:34:42.635419 pytket-pyquil-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      626 2021-03-02 14:31:41.000000 pytket-pyquil-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-03-02 14:31:41.000000 pytket-pyquil-0.8.0/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:34:42.631419 pytket-pyquil-0.8.0/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:34:42.631419 pytket-pyquil-0.8.0/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:34:42.631419 pytket-pyquil-0.8.0/pytket/extensions/pyquil/
--rw-r--r--   0 runner    (1001) docker     (121)      946 2021-03-02 14:31:41.000000 pytket-pyquil-0.8.0/pytket/extensions/pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-03-02 14:34:42.000000 pytket-pyquil-0.8.0/pytket/extensions/pyquil/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:34:42.631419 pytket-pyquil-0.8.0/pytket/extensions/pyquil/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-02 14:31:41.000000 pytket-pyquil-0.8.0/pytket/extensions/pyquil/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13158 2021-03-02 14:31:41.000000 pytket-pyquil-0.8.0/pytket/extensions/pyquil/backends/forest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11707 2021-03-02 14:31:41.000000 pytket-pyquil-0.8.0/pytket/extensions/pyquil/pyquil_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:34:42.635419 pytket-pyquil-0.8.0/pytket_pyquil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2021-03-02 14:34:42.000000 pytket-pyquil-0.8.0/pytket_pyquil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      471 2021-03-02 14:34:42.000000 pytket-pyquil-0.8.0/pytket_pyquil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-02 14:34:42.000000 pytket-pyquil-0.8.0/pytket_pyquil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-02 14:34:42.000000 pytket-pyquil-0.8.0/pytket_pyquil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-03-02 14:34:42.000000 pytket-pyquil-0.8.0/pytket_pyquil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-02 14:34:42.000000 pytket-pyquil-0.8.0/pytket_pyquil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-02 14:34:42.635419 pytket-pyquil-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2021-03-02 14:31:41.000000 pytket-pyquil-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:41.732063 pytket-pyquil-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-04-01 10:54:45.000000 pytket-pyquil-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2021-04-01 10:57:41.732063 pytket-pyquil-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2021-04-01 10:54:45.000000 pytket-pyquil-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-04-01 10:54:45.000000 pytket-pyquil-0.9.0/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:41.732063 pytket-pyquil-0.9.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:41.732063 pytket-pyquil-0.9.0/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:41.732063 pytket-pyquil-0.9.0/pytket/extensions/pyquil/
+-rw-r--r--   0 runner    (1001) docker     (121)      946 2021-04-01 10:54:45.000000 pytket-pyquil-0.9.0/pytket/extensions/pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-04-01 10:57:41.000000 pytket-pyquil-0.9.0/pytket/extensions/pyquil/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:41.732063 pytket-pyquil-0.9.0/pytket/extensions/pyquil/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-04-01 10:54:45.000000 pytket-pyquil-0.9.0/pytket/extensions/pyquil/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13142 2021-04-01 10:54:45.000000 pytket-pyquil-0.9.0/pytket/extensions/pyquil/backends/forest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11714 2021-04-01 10:54:45.000000 pytket-pyquil-0.9.0/pytket/extensions/pyquil/pyquil_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:41.732063 pytket-pyquil-0.9.0/pytket_pyquil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2021-04-01 10:57:41.000000 pytket-pyquil-0.9.0/pytket_pyquil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2021-04-01 10:57:41.000000 pytket-pyquil-0.9.0/pytket_pyquil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:57:41.000000 pytket-pyquil-0.9.0/pytket_pyquil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:57:41.000000 pytket-pyquil-0.9.0/pytket_pyquil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-04-01 10:57:41.000000 pytket-pyquil-0.9.0/pytket_pyquil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-01 10:57:41.000000 pytket-pyquil-0.9.0/pytket_pyquil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-01 10:57:41.732063 pytket-pyquil-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-04-01 10:54:45.000000 pytket-pyquil-0.9.0/setup.py
```

### Comparing `pytket-pyquil-0.8.0/PKG-INFO` & `pytket-pyquil-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytket-pyquil
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing translation to and from the pyQuil framework
-Home-page: https://github.com/CQCL/pytket
+Home-page: https://github.com/CQCL/pytket-extensions
 Author: Will Simmons
 Author-email: will.simmons@cambridgequantum.com
 License: Apache 2
 Description: # pytket-pyquil
         
         [Pytket](https://cqcl.github.io/pytket) is a Python module for interfacing
         with CQC tket, a set of quantum programming tools.
```

### Comparing `pytket-pyquil-0.8.0/README.md` & `pytket-pyquil-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytket-pyquil-0.8.0/pytket/extensions/pyquil/__init__.py` & `pytket-pyquil-0.9.0/pytket/extensions/pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-pyquil-0.8.0/pytket/extensions/pyquil/backends/__init__.py` & `pytket-pyquil-0.9.0/pytket/extensions/pyquil/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-pyquil-0.8.0/pytket/extensions/pyquil/backends/forest.py` & `pytket-pyquil-0.9.0/pytket/extensions/pyquil/backends/forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from copy import copy
 from typing import Iterable, List, Optional
 from uuid import uuid4
 from logging import warning
 
-import numpy as np  # type: ignore
+import numpy as np
 from pyquil import get_qc
 from pyquil.api import QuantumComputer, WavefunctionSimulator
 from pyquil.gates import I
 from pyquil.paulis import ID, PauliSum, PauliTerm
 from pyquil.quilatom import Qubit as Qubit_
 
 from pytket.circuit import Circuit, OpType, Qubit  # type: ignore
```

### Comparing `pytket-pyquil-0.8.0/pytket/extensions/pyquil/pyquil_convert.py` & `pytket-pyquil-0.9.0/pytket/extensions/pyquil/pyquil_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 )
 
         return to_pyquil(ppi)
 
 
 def param_from_pyquil(p: Union[float, Expression]) -> Expr:
     def to_sympy(e: Union[float, Expression]) -> Expr:
-        if isinstance(e, float):
+        if isinstance(e, (float, int)):
             return e
         elif isinstance(e, MemoryReference):
             return Symbol(e.name)
         elif isinstance(e, Function_):
             if e.name == "SIN":
                 return sin(to_sympy(e.expression))  # type: ignore
             elif e.name == "COS":
```

### Comparing `pytket-pyquil-0.8.0/pytket_pyquil.egg-info/PKG-INFO` & `pytket-pyquil-0.9.0/pytket_pyquil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytket-pyquil
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing translation to and from the pyQuil framework
-Home-page: https://github.com/CQCL/pytket
+Home-page: https://github.com/CQCL/pytket-extensions
 Author: Will Simmons
 Author-email: will.simmons@cambridgequantum.com
 License: Apache 2
 Description: # pytket-pyquil
         
         [Pytket](https://cqcl.github.io/pytket) is a Python module for interfacing
         with CQC tket, a set of quantum programming tools.
```

### Comparing `pytket-pyquil-0.8.0/setup.py` & `pytket-pyquil-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 
 setup(
     name=metadata["__extension_name__"],
     version=metadata["__extension_version__"],
     author="Will Simmons",
     author_email="will.simmons@cambridgequantum.com",
     python_requires=">=3.7",
-    url="https://github.com/CQCL/pytket",
+    url="https://github.com/CQCL/pytket-extensions",
     description="Extension for pytket, providing translation to and from the pyQuil "
     "framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
-    install_requires=["pytket ~= 0.8.0", "pyquil ~= 2.28", "typing-extensions ~= 3.7"],
+    install_requires=["pytket ~= 0.9.0", "pyquil ~= 2.28", "typing-extensions ~= 3.7"],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
         "Operating System :: MacOS :: MacOS X",
```

