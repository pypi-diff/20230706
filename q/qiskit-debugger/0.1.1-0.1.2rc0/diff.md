# Comparing `tmp/qiskit_debugger-0.1.1.tar.gz` & `tmp/qiskit_debugger-0.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_debugger-0.1.1.tar", last modified: Wed Jul  5 14:11:32 2023, max compression
+gzip compressed data, was "qiskit_debugger-0.1.2rc0.tar", last modified: Thu Jul  6 03:28:32 2023, max compression
```

## Comparing `qiskit_debugger-0.1.1.tar` & `qiskit_debugger-0.1.2rc0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-05 22:01:01.000000 qiskit_debugger-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7050 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6617 2023-07-05 14:10:54.000000 qiskit_debugger-0.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       87 2023-05-05 22:01:58.000000 qiskit_debugger-0.1.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/qiskit_debugger/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7050 2023-07-05 14:11:32.000000 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2023-07-05 14:11:32.000000 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 14:11:32.000000 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-05 14:11:32.000000 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      982 2023-07-04 21:50:24.000000 qiskit_debugger-0.1.1/setup.py
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

### Comparing `qiskit_debugger-0.1.1/LICENSE` & `qiskit_debugger-0.1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_debugger-0.1.1/PKG-INFO` & `qiskit_debugger-0.1.2rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: qiskit_debugger
-Version: 0.1.1
-Summary: Quantum Circuit debugger for the Qiskit SDK.
-Author: Sirajus Salekin
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Breakpoint Debugging on a Physical Qunatum Circuit
 
 ## Problem Description
 In classical computing, debugging with breakpoint means halting the program
 execution at any given point and freezing the program state. This allows
 programmers to examine the program internals mid-execution (as in, what
 variables contain which values, analyze control flow etc.) Unfortunately, in
```

### Comparing `qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/PKG-INFO` & `qiskit_debugger-0.1.2rc0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,43 @@
 Metadata-Version: 2.1
-Name: qiskit-debugger
-Version: 0.1.1
+Name: qiskit_debugger
+Version: 0.1.2rc0
 Summary: Quantum Circuit debugger for the Qiskit SDK.
-Author: Sirajus Salekin
-License: MIT
+Author-email: Sirajus Salekin <ssalekin14@gmail.com>, Palvit Garg <pgarg5@ncsu.edu>, Harshwardhan Joshi <hjoshi2@ncsu.edu>
+Maintainer-email: Sirajus Salekin <ssalekin14@gmail.com>
+License: MIT License
+        
+        Copyright (c) [2023] [Sirajus Salekin, Harsh Joshi, & Palvit Garg]
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/salekinsirajus/quantum_circuit_debugger
+Project-URL: repository, https://github.com/salekinsirajus/quantum_circuit_debugger
+Keywords: quantum,computing,debugger,qiskit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Breakpoint Debugging on a Physical Qunatum Circuit
 
 ## Problem Description
```

