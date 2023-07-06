# Comparing `tmp/dithering-0.1.20.tar.gz` & `tmp/dithering-0.1.21.tar.gz`

## Comparing `dithering-0.1.20.tar` & `dithering-0.1.21.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 dithering-0.1.20/Cargo.toml
--rw-r--r--   0     1001      123     2805 2023-07-06 08:42:43.000000 dithering-0.1.20/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-06 08:42:43.000000 dithering-0.1.20/.gitignore
--rw-r--r--   0     1001      123     1067 2023-07-06 08:42:43.000000 dithering-0.1.20/LICENSE
--rw-r--r--   0     1001      123      720 2023-07-06 08:42:43.000000 dithering-0.1.20/README.md
--rw-r--r--   0     1001      123      103 2023-07-06 08:42:43.000000 dithering-0.1.20/dithering.pyi
--rw-r--r--   0     1001      123      369 2023-07-06 08:42:43.000000 dithering-0.1.20/pyproject.toml
--rw-r--r--   0     1001      123     8863 2023-07-06 08:42:43.000000 dithering-0.1.20/resources/dithering.png
--rw-r--r--   0     1001      123    57228 2023-07-06 08:42:43.000000 dithering-0.1.20/resources/dithering.svg
--rw-r--r--   0     1001      123      212 2023-07-06 08:42:43.000000 dithering-0.1.20/src/lib.rs
--rw-r--r--   0     1001      123       51 2023-07-06 08:42:43.000000 dithering-0.1.20/src/methods/mod.rs
--rw-r--r--   0     1001      123      888 2023-07-06 08:42:43.000000 dithering-0.1.20/src/methods/ordered.rs
--rw-r--r--   0     1001      123     9356 2023-07-06 08:42:43.000000 dithering-0.1.20/Cargo.lock
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 dithering-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 dithering-0.1.21/Cargo.toml
+-rw-r--r--   0     1001      123     2805 2023-07-06 14:05:10.000000 dithering-0.1.21/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-06 14:05:10.000000 dithering-0.1.21/.gitignore
+-rw-r--r--   0     1001      123     1067 2023-07-06 14:05:10.000000 dithering-0.1.21/LICENSE
+-rw-r--r--   0     1001      123      758 2023-07-06 14:05:10.000000 dithering-0.1.21/README.md
+-rw-r--r--   0     1001      123      103 2023-07-06 14:05:10.000000 dithering-0.1.21/dithering.pyi
+-rw-r--r--   0     1001      123      369 2023-07-06 14:05:10.000000 dithering-0.1.21/pyproject.toml
+-rw-r--r--   0     1001      123     8863 2023-07-06 14:05:10.000000 dithering-0.1.21/resources/dithering.png
+-rw-r--r--   0     1001      123    57228 2023-07-06 14:05:10.000000 dithering-0.1.21/resources/dithering.svg
+-rw-r--r--   0     1001      123      212 2023-07-06 14:05:10.000000 dithering-0.1.21/src/lib.rs
+-rw-r--r--   0     1001      123       51 2023-07-06 14:05:10.000000 dithering-0.1.21/src/methods/mod.rs
+-rw-r--r--   0     1001      123      888 2023-07-06 14:05:10.000000 dithering-0.1.21/src/methods/ordered.rs
+-rw-r--r--   0     1001      123     9356 2023-07-06 14:05:10.000000 dithering-0.1.21/Cargo.lock
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 dithering-0.1.21/PKG-INFO
```

### Comparing `dithering-0.1.20/.github/workflows/CI.yml` & `dithering-0.1.21/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dithering-0.1.20/.gitignore` & `dithering-0.1.21/.gitignore`

 * *Files identical despite different names*

### Comparing `dithering-0.1.20/LICENSE` & `dithering-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `dithering-0.1.20/README.md` & `dithering-0.1.21/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <p align="center">
     <br>
-    <img src="https://github.com/BackyardML/dithering/blob/main/resources/dithering.png?raw=true" width="600"/>
+    <img src="https://raw.githubusercontent.com/BackyardML/dithering/72ea732b8c7372af6f427a5f8244af158d80d208/resources/dithering.svg" width="600"/>
     <br>
 <p>
 
 ![CI](https://github.com/BackyardML/dithering/actions/workflows/CI.yml/badge.svg)
 
+
 ## Overview
 Welcome to Dithering, a project that brings efficient Rust implementation of various image dithering methods to be used in Python!
 
 ## Installation
 ```
 pip install dithering
 ```
```

### Comparing `dithering-0.1.20/resources/dithering.png` & `dithering-0.1.21/resources/dithering.png`

 * *Files identical despite different names*

### Comparing `dithering-0.1.20/resources/dithering.svg` & `dithering-0.1.21/resources/dithering.svg`

 * *Files identical despite different names*

### Comparing `dithering-0.1.20/src/methods/ordered.rs` & `dithering-0.1.21/src/methods/ordered.rs`

 * *Files identical despite different names*

### Comparing `dithering-0.1.20/Cargo.lock` & `dithering-0.1.21/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "dithering"
-version = "0.1.20"
+version = "0.1.21"
 dependencies = [
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
```

### Comparing `dithering-0.1.20/PKG-INFO` & `dithering-0.1.21/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: dithering
-Version: 0.1.20
+Version: 0.1.21
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Efficient implementations of various image dithering methods.
 Home-Page: https://backyardml.github.io/
 Author: Patrik Larsson <patrik@backyardml.se>
 Author-email: Patrik Larsson <patrik@backyardml.se>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/BackyardML/dithering
 
 <p align="center">
     <br>
-    <img src="https://github.com/BackyardML/dithering/blob/main/resources/dithering.png?raw=true" width="600"/>
+    <img src="https://raw.githubusercontent.com/BackyardML/dithering/72ea732b8c7372af6f427a5f8244af158d80d208/resources/dithering.svg" width="600"/>
     <br>
 <p>
 
 ![CI](https://github.com/BackyardML/dithering/actions/workflows/CI.yml/badge.svg)
 
+
 ## Overview
 Welcome to Dithering, a project that brings efficient Rust implementation of various image dithering methods to be used in Python!
 
 ## Installation
 ```
 pip install dithering
 ```
```

