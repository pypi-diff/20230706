# Comparing `tmp/rpds_py-0.8.6.tar.gz` & `tmp/rpds_py-0.8.7.tar.gz`

## Comparing `rpds_py-0.8.6.tar` & `rpds_py-0.8.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.6/Cargo.toml
--rw-r--r--   0        0        0      219 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.github/dependabot.yml
--rw-r--r--   0        0        0       81 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.github/release.yml
--rw-r--r--   0        0        0     5012 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.gitignore
--rw-r--r--   0        0        0     1050 2023-07-06 13:16:53.000000 rpds_py-0.8.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1076 2023-07-06 13:16:53.000000 rpds_py-0.8.6/LICENSE
--rw-r--r--   0        0        0     1739 2023-07-06 13:16:53.000000 rpds_py-0.8.6/README.rst
--rw-r--r--   0        0        0     1043 2023-07-06 13:16:53.000000 rpds_py-0.8.6/noxfile.py
--rw-r--r--   0        0        0     1406 2023-07-06 13:16:53.000000 rpds_py-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     1697 2023-07-06 13:16:53.000000 rpds_py-0.8.6/rpds.pyi
--rw-r--r--   0        0        0    17578 2023-07-06 13:16:53.000000 rpds_py-0.8.6/src/lib.rs
--rw-r--r--   0        0        0       20 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/requirements.in
--rw-r--r--   0        0        0      484 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/requirements.txt
--rw-r--r--   0        0        0     8653 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/test_hash_trie_map.py
--rw-r--r--   0        0        0     5098 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/test_hash_trie_set.py
--rw-r--r--   0        0        0     3533 2023-07-06 13:16:53.000000 rpds_py-0.8.6/tests/test_list.py
--rw-r--r--   0        0        0     8633 2023-07-06 13:16:53.000000 rpds_py-0.8.6/Cargo.lock
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 rpds_py-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.7/Cargo.toml
+-rw-r--r--   0        0        0      219 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.github/dependabot.yml
+-rw-r--r--   0        0        0       81 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.github/release.yml
+-rw-r--r--   0        0        0     5075 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.gitignore
+-rw-r--r--   0        0        0     1050 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1076 2023-07-06 13:57:08.000000 rpds_py-0.8.7/LICENSE
+-rw-r--r--   0        0        0     1739 2023-07-06 13:57:08.000000 rpds_py-0.8.7/README.rst
+-rw-r--r--   0        0        0     1043 2023-07-06 13:57:08.000000 rpds_py-0.8.7/noxfile.py
+-rw-r--r--   0        0        0     1406 2023-07-06 13:57:08.000000 rpds_py-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     1697 2023-07-06 13:57:08.000000 rpds_py-0.8.7/rpds.pyi
+-rw-r--r--   0        0        0    17578 2023-07-06 13:57:08.000000 rpds_py-0.8.7/src/lib.rs
+-rw-r--r--   0        0        0       20 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/requirements.in
+-rw-r--r--   0        0        0      484 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/requirements.txt
+-rw-r--r--   0        0        0     8653 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/test_hash_trie_map.py
+-rw-r--r--   0        0        0     5098 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/test_hash_trie_set.py
+-rw-r--r--   0        0        0     3533 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/test_list.py
+-rw-r--r--   0        0        0     8633 2023-07-06 13:57:08.000000 rpds_py-0.8.7/Cargo.lock
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 rpds_py-0.8.7/PKG-INFO
```

### Comparing `rpds_py-0.8.6/.github/workflows/CI.yml` & `rpds_py-0.8.7/.github/workflows/CI.yml`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,18 @@
           path: dist
 
   musllinux:
     needs: test
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        target: [x86_64-unknown-linux-musl, i686-unknown-linux-musl]
+        target:
+          - aarch64-unknown-linux-musl
+          - i686-unknown-linux-musl
+          - x86_64-unknown-linux-musl
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
```

### Comparing `rpds_py-0.8.6/.gitignore` & `rpds_py-0.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/.pre-commit-config.yaml` & `rpds_py-0.8.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/LICENSE` & `rpds_py-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/README.rst` & `rpds_py-0.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/noxfile.py` & `rpds_py-0.8.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/pyproject.toml` & `rpds_py-0.8.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/rpds.pyi` & `rpds_py-0.8.7/rpds.pyi`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/src/lib.rs` & `rpds_py-0.8.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/tests/test_hash_trie_map.py` & `rpds_py-0.8.7/tests/test_hash_trie_map.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/tests/test_hash_trie_set.py` & `rpds_py-0.8.7/tests/test_hash_trie_set.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/tests/test_list.py` & `rpds_py-0.8.7/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.6/Cargo.lock` & `rpds_py-0.8.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 checksum = "9bd6ce569b15c331b1e5fd8cf6adb0bf240678b5f0cdc4d0f41e11683f6feba9"
 dependencies = [
  "archery",
 ]
 
 [[package]]
 name = "rpds-py"
-version = "0.8.6"
+version = "0.8.7"
 dependencies = [
  "archery",
  "pyo3",
  "rpds",
 ]
 
 [[package]]
```

### Comparing `rpds_py-0.8.6/PKG-INFO` & `rpds_py-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpds-py
-Version: 0.8.6
+Version: 0.8.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

