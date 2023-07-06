# Comparing `tmp/rpds_py-0.8.4.tar.gz` & `tmp/rpds_py-0.8.6.tar.gz`

## Comparing `rpds_py-0.8.4.tar` & `rpds_py-0.8.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.4/Cargo.toml
--rw-r--r--   0        0        0      219 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.github/dependabot.yml
--rw-r--r--   0        0        0       81 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.github/release.yml
--rw-r--r--   0        0        0     4321 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.gitignore
--rw-r--r--   0        0        0     1050 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1076 2023-07-06 11:57:04.000000 rpds_py-0.8.4/LICENSE
--rw-r--r--   0        0        0     1739 2023-07-06 11:57:04.000000 rpds_py-0.8.4/README.rst
--rw-r--r--   0        0        0     1043 2023-07-06 11:57:04.000000 rpds_py-0.8.4/noxfile.py
--rw-r--r--   0        0        0     1406 2023-07-06 11:57:04.000000 rpds_py-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     1697 2023-07-06 11:57:04.000000 rpds_py-0.8.4/rpds.pyi
--rw-r--r--   0        0        0    17578 2023-07-06 11:57:04.000000 rpds_py-0.8.4/src/lib.rs
--rw-r--r--   0        0        0       20 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/requirements.in
--rw-r--r--   0        0        0      484 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/requirements.txt
--rw-r--r--   0        0        0     8653 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/test_hash_trie_map.py
--rw-r--r--   0        0        0     5098 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/test_hash_trie_set.py
--rw-r--r--   0        0        0     3533 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/test_list.py
--rw-r--r--   0        0        0     8633 2023-07-06 11:57:04.000000 rpds_py-0.8.4/Cargo.lock
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 rpds_py-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.6/Cargo.toml
+-rw-r--r--   0        0        0      219 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.github/dependabot.yml
+-rw-r--r--   0        0        0       81 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.github/release.yml
+-rw-r--r--   0        0        0     5012 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1050 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1076 2023-07-06 13:16:53.000000 rpds_py-0.8.6/LICENSE
+-rw-r--r--   0        0        0     1739 2023-07-06 13:16:53.000000 rpds_py-0.8.6/README.rst
+-rw-r--r--   0        0        0     1043 2023-07-06 13:16:53.000000 rpds_py-0.8.6/noxfile.py
+-rw-r--r--   0        0        0     1406 2023-07-06 13:16:53.000000 rpds_py-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1697 2023-07-06 13:16:53.000000 rpds_py-0.8.6/rpds.pyi
+-rw-r--r--   0        0        0    17578 2023-07-06 13:16:53.000000 rpds_py-0.8.6/src/lib.rs
+-rw-r--r--   0        0        0       20 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/requirements.in
+-rw-r--r--   0        0        0      484 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/requirements.txt
+-rw-r--r--   0        0        0     8653 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/test_hash_trie_map.py
+-rw-r--r--   0        0        0     5098 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/test_hash_trie_set.py
+-rw-r--r--   0        0        0     3533 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/test_list.py
+-rw-r--r--   0        0        0     8633 2023-07-06 13:16:53.000000 rpds_py-0.8.6/Cargo.lock
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 rpds_py-0.8.6/PKG-INFO
```

### Comparing `rpds_py-0.8.4/.github/workflows/CI.yml` & `rpds_py-0.8.6/.github/workflows/CI.yml`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         with:
           python-version: "3.x"
       - name: Set up nox
         uses: wntrblm/nox@2023.04.22
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}"
 
-  linux:
+  manylinux:
     needs: test
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
     steps:
       - uses: actions/checkout@v3
@@ -88,14 +88,37 @@
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
+  musllinux:
+    needs: test
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        target: [x86_64-unknown-linux-musl, i686-unknown-linux-musl]
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.x"
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          target: ${{ matrix.target }}
+          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 pypy3.8 pypy3.9'
+          manylinux: musllinux_1_2
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels
+          path: dist
+
   windows:
     needs: test
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64, x86]
     steps:
@@ -137,15 +160,15 @@
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos]
+    needs: [manylinux, musllinux, windows, macos]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
```

### Comparing `rpds_py-0.8.4/.gitignore` & `rpds_py-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/.pre-commit-config.yaml` & `rpds_py-0.8.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/LICENSE` & `rpds_py-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/README.rst` & `rpds_py-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/noxfile.py` & `rpds_py-0.8.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/pyproject.toml` & `rpds_py-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/rpds.pyi` & `rpds_py-0.8.6/rpds.pyi`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/src/lib.rs` & `rpds_py-0.8.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/tests/test_hash_trie_map.py` & `rpds_py-0.8.6/tests/test_hash_trie_map.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/tests/test_hash_trie_set.py` & `rpds_py-0.8.6/tests/test_hash_trie_set.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/tests/test_list.py` & `rpds_py-0.8.6/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.4/Cargo.lock` & `rpds_py-0.8.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 checksum = "9bd6ce569b15c331b1e5fd8cf6adb0bf240678b5f0cdc4d0f41e11683f6feba9"
 dependencies = [
  "archery",
 ]
 
 [[package]]
 name = "rpds-py"
-version = "0.8.4"
+version = "0.8.6"
 dependencies = [
  "archery",
  "pyo3",
  "rpds",
 ]
 
 [[package]]
```

### Comparing `rpds_py-0.8.4/PKG-INFO` & `rpds_py-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpds-py
-Version: 0.8.4
+Version: 0.8.6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

