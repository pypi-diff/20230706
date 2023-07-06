# Comparing `tmp/windows_control-0.0.6.tar.gz` & `tmp/windows_control-0.0.7.tar.gz`

## Comparing `windows_control-0.0.6.tar` & `windows_control-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 windows_control-0.0.6/Cargo.toml
--rw-r--r--   0        0        0     2807 2023-06-28 03:33:37.000000 windows_control-0.0.6/.github/workflows/CI.yml
--rw-r--r--   0        0        0      756 2023-06-28 03:33:37.000000 windows_control-0.0.6/.gitignore
--rw-r--r--   0        0        0     2450 2023-06-28 09:04:22.000000 windows_control-0.0.6/README.md
--rw-r--r--   0        0        0      485 2023-06-28 09:06:30.000000 windows_control-0.0.6/README_PUB.md
--rw-r--r--   0        0        0      679 2023-06-28 09:02:28.000000 windows_control-0.0.6/justfile
--rw-r--r--   0        0        0      820 2023-06-28 09:06:55.000000 windows_control-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       90 2023-06-28 05:39:06.000000 windows_control-0.0.6/src/keyboard/mod.rs
--rw-r--r--   0        0        0     1201 2023-06-28 05:51:30.000000 windows_control-0.0.6/src/lib.rs
--rw-r--r--   0        0        0      508 2023-06-28 05:39:46.000000 windows_control-0.0.6/test.py
--rw-r--r--   0        0        0     7435 2023-06-28 06:00:28.000000 windows_control-0.0.6/Cargo.lock
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 windows_control-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 windows_control-0.0.7/Cargo.toml
+-rw-r--r--   0        0        0     2807 2023-06-28 03:33:37.000000 windows_control-0.0.7/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      756 2023-06-28 03:33:37.000000 windows_control-0.0.7/.gitignore
+-rw-r--r--   0        0        0     2753 2023-07-02 15:41:49.000000 windows_control-0.0.7/README.md
+-rw-r--r--   0        0        0      469 2023-06-28 09:07:29.000000 windows_control-0.0.7/README_PUB.md
+-rw-r--r--   0        0        0      679 2023-06-28 09:02:28.000000 windows_control-0.0.7/justfile
+-rw-r--r--   0        0        0      820 2023-07-06 02:44:17.000000 windows_control-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      585 2023-07-03 08:24:56.000000 windows_control-0.0.7/src/clean_up.rs
+-rw-r--r--   0        0        0    14532 2023-07-03 03:45:51.000000 windows_control-0.0.7/src/keyboard/key_map.rs
+-rw-r--r--   0        0        0     3495 2023-07-03 08:17:50.000000 windows_control-0.0.7/src/keyboard/mod.rs
+-rw-r--r--   0        0        0     2240 2023-07-06 02:42:06.000000 windows_control-0.0.7/src/lib.rs
+-rw-r--r--   0        0        0      840 2023-07-03 07:25:23.000000 windows_control-0.0.7/src/mouse/mod.rs
+-rw-r--r--   0        0        0     5609 2023-07-06 02:42:06.000000 windows_control-0.0.7/src/window/mod.rs
+-rw-r--r--   0        0        0     2844 2023-07-06 02:41:24.000000 windows_control-0.0.7/src/window/private.rs
+-rw-r--r--   0        0        0     4254 2023-07-06 02:39:35.000000 windows_control-0.0.7/test.py
+-rw-r--r--   0        0        0    65561 2023-07-06 02:39:21.000000 windows_control-0.0.7/Cargo.lock
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 windows_control-0.0.7/PKG-INFO
```

### Comparing `windows_control-0.0.6/.github/workflows/CI.yml` & `windows_control-0.0.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.6/.gitignore` & `windows_control-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.6/README.md` & `windows_control-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,40 +15,47 @@
 
 ## Examples
 
 (TODO)
 
 ## Contributing
 
+### TODO
+windows module
+add opencv support,after that pub a new version: https://www.perplexity.ai/search/bc8f7e79-b31a-4ba6-8a7f-f94e239f4c77?s=u
+
 ### Prerequisites
 
-Before contributing to the project, you need to know about PyO3. You can follow the instructions in the [PyO3 getting start](https://pyo3.rs/v0.19.0/getting_started), [PyO3 guide](https://pyo3.rs/v0.19.0/building_and_distribution#manual-builds) and [How to use maturin to publish a python package](https://www.maturin.rs/tutorial.html).
+Before contributing to the project, you need to know about PyO3. You can follow the instructions:
+- [PyO3 getting start](https://pyo3.rs/v0.19.0/getting_started);
+- [PyO3 guide](https://pyo3.rs/v0.19.0/building_and_distribution#manual-builds);
+- [How to use maturin to publish a python package](https://www.maturin.rs/tutorial.html);
+- [PyO3 Define a Class/Struct/Enum](https://pyo3.rs/v0.19.0/class.html#attribute-access).
 
 ### Manual Development
 
-First, install python package `maturin` by running `pip install maturin` in terminal.
-
-Second, make sure there is an virtual env at your project root directory. You can do it by running `python -m venv .venv` in terminal---the name `.venv` is specified for `maturin`.
-
-Then, to add new features(like new funcs or new modules), modify the `src/lib.rs` file. After making changes, generate the Python module by running `maturin develop`. This command generates a library in `target/debug`. On Windows, rename the generated library file `[your_module].dll` to `[your_module].pyd`.
-
-Finally, to test the generated library, run `python test.py` in the root directory to verify that the newly added features work correctly in Python.
+1. Install the python package `maturin` by running `pip install maturin` in terminal.
+2. Make sure there is a virtual env at your project root directory. You can do it by running `python -m venv .venv` in terminal---the name `.venv` is specified for `maturin`. NOTE: please restart your terminal after creating the virtual env.
+3. To add new features (like new funcs or new modules), modify the `src/lib.rs` file.
+4. After making changes, generate the Python module by running `maturin develop`. This command generates a library in `target/debug`.
+5. On Windows, rename the generated library file `[your_module].dll` to `[your_module].pyd`.
+6. Finally, to test the generated library, run `python test.py` in the root directory to verify that the newly added features work correctly in Python.
 
 ### Automatic Development
 
 If you have [just](https://crates.io/crates/just) installed, run just to automatically generate and test the project. The justfile contains specific commands for this purpose.
 
 ### Publish
 First, update the field `version` in file `pyproject.toml`.
 Then, use `maturin publish`(in powershell,not git bash) to publish the package to PyPI(or just run `just pub` with [just](https://crates.io/crates/just)).When you see:
 ```bash
 🚀 Uploading 2 packages
 ✨ Packages uploaded successfully
 ```
 This means it's published successfully, and you can check it in [PyPi](https://pypi.org/project/windows-control/).
 
-Finally, update section `Examples` in both `README.md`(this file) and `README.rst`.
+Finally, update section `Examples` in both `README.md`(this file) and `README_PUB.md`.
 
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `windows_control-0.0.6/justfile` & `windows_control-0.0.7/justfile`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.6/pyproject.toml` & `windows_control-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "windows_control"
-version = "0.0.6"
+version = "0.0.7"
 description = "It is used to do some control with keyboard/mouse on windows (especially on win10)."
 readme = "README_PUB.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

### Comparing `windows_control-0.0.6/PKG-INFO` & `windows_control-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: windows_control
-Version: 0.0.6
+Version: 0.0.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: It is used to do some control with keyboard/mouse on windows (especially on win10).
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/dbsxdbsx/windows_control
 
-# Project Name
-
 [windows_control](https://pypi.org/project/windows-control/) is a package named with a root Python module `windows_control`.
 It provides some simple and efficient ways to do manipulations on Windows systems(Especially on Win10) efficiently, since it is written in Rust using [PyO3](https://crates.io/crates/pyo3).
 
 ## Installation
 
 ```bash
 pip install windows_control
```

