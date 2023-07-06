# Comparing `tmp/rpds_py-0.8.3.tar.gz` & `tmp/rpds_py-0.8.4.tar.gz`

## Comparing `rpds_py-0.8.3.tar` & `rpds_py-0.8.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.3/Cargo.toml
--rw-r--r--   0        0        0      219 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.github/dependabot.yml
--rw-r--r--   0        0        0       81 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.github/release.yml
--rw-r--r--   0        0        0     4321 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.gitignore
--rw-r--r--   0        0        0     1050 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1076 2023-07-06 11:45:33.000000 rpds_py-0.8.3/LICENSE
--rw-r--r--   0        0        0     1741 2023-07-06 11:45:33.000000 rpds_py-0.8.3/README.rst
--rw-r--r--   0        0        0     1043 2023-07-06 11:45:33.000000 rpds_py-0.8.3/noxfile.py
--rw-r--r--   0        0        0     1406 2023-07-06 11:45:33.000000 rpds_py-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     1697 2023-07-06 11:45:33.000000 rpds_py-0.8.3/rpds.pyi
--rw-r--r--   0        0        0    17578 2023-07-06 11:45:33.000000 rpds_py-0.8.3/src/lib.rs
--rw-r--r--   0        0        0       20 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/requirements.in
--rw-r--r--   0        0        0      484 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/requirements.txt
--rw-r--r--   0        0        0     8653 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/test_hash_trie_map.py
--rw-r--r--   0        0        0     5098 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/test_hash_trie_set.py
--rw-r--r--   0        0        0     3533 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/test_list.py
--rw-r--r--   0        0        0     8325 2023-07-06 11:46:07.000000 rpds_py-0.8.3/Cargo.lock
--rw-r--r--   0        0        0     2924 1970-01-01 00:00:00.000000 rpds_py-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.4/Cargo.toml
+-rw-r--r--   0        0        0      219 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.github/dependabot.yml
+-rw-r--r--   0        0        0       81 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.github/release.yml
+-rw-r--r--   0        0        0     4321 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1050 2023-07-06 11:57:04.000000 rpds_py-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1076 2023-07-06 11:57:04.000000 rpds_py-0.8.4/LICENSE
+-rw-r--r--   0        0        0     1739 2023-07-06 11:57:04.000000 rpds_py-0.8.4/README.rst
+-rw-r--r--   0        0        0     1043 2023-07-06 11:57:04.000000 rpds_py-0.8.4/noxfile.py
+-rw-r--r--   0        0        0     1406 2023-07-06 11:57:04.000000 rpds_py-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     1697 2023-07-06 11:57:04.000000 rpds_py-0.8.4/rpds.pyi
+-rw-r--r--   0        0        0    17578 2023-07-06 11:57:04.000000 rpds_py-0.8.4/src/lib.rs
+-rw-r--r--   0        0        0       20 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/requirements.in
+-rw-r--r--   0        0        0      484 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/requirements.txt
+-rw-r--r--   0        0        0     8653 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/test_hash_trie_map.py
+-rw-r--r--   0        0        0     5098 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/test_hash_trie_set.py
+-rw-r--r--   0        0        0     3533 2023-07-06 11:57:04.000000 rpds_py-0.8.4/tests/test_list.py
+-rw-r--r--   0        0        0     8633 2023-07-06 11:57:04.000000 rpds_py-0.8.4/Cargo.lock
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 rpds_py-0.8.4/PKG-INFO
```

### Comparing `rpds_py-0.8.3/.github/workflows/CI.yml` & `rpds_py-0.8.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/.gitignore` & `rpds_py-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/.pre-commit-config.yaml` & `rpds_py-0.8.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/LICENSE` & `rpds_py-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/README.rst` & `rpds_py-0.8.4/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,17 @@
   :alt: PyPI version
   :target: https://pypi.org/project/rpds-py/
 
 .. |Pythons| image:: https://img.shields.io/pypi/pyversions/rpds-py.svg
   :alt: Supported Python versions
   :target: https://pypi.org/project/rpds-py/
 
-.. |CI| image:: https://github.com/Julian/rpds.py/workflows/CI/badge.svg
+.. |CI| image:: https://github.com/crate-py/rpds/workflows/CI/badge.svg
   :alt: Build status
-  :target: https://github.com/Julian/rpds.py/actions?query=workflow%3ACI
+  :target: https://github.com/crate-py/rpds/actions?query=workflow%3ACI
 
 
 Python bindings to the Rust ``rpds`` crate.
 
 What's here is quite minimal (in transparency, it was written initially to support replacing ``pyrsistent`` in the `referencing library <https://github.com/python-jsonschema/referencing>`_).
 If you see something missing (which is very likely), a PR is definitely welcome to add it.
```

### Comparing `rpds_py-0.8.3/noxfile.py` & `rpds_py-0.8.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/pyproject.toml` & `rpds_py-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/rpds.pyi` & `rpds_py-0.8.4/rpds.pyi`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/src/lib.rs` & `rpds_py-0.8.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/tests/test_hash_trie_map.py` & `rpds_py-0.8.4/tests/test_hash_trie_map.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/tests/test_hash_trie_set.py` & `rpds_py-0.8.4/tests/test_hash_trie_set.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/tests/test_list.py` & `rpds_py-0.8.4/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.3/PKG-INFO` & `rpds_py-0.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpds-py
-Version: 0.8.3
+Version: 0.8.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,17 +36,17 @@
   :alt: PyPI version
   :target: https://pypi.org/project/rpds-py/
 
 .. |Pythons| image:: https://img.shields.io/pypi/pyversions/rpds-py.svg
   :alt: Supported Python versions
   :target: https://pypi.org/project/rpds-py/
 
-.. |CI| image:: https://github.com/Julian/rpds.py/workflows/CI/badge.svg
+.. |CI| image:: https://github.com/crate-py/rpds/workflows/CI/badge.svg
   :alt: Build status
-  :target: https://github.com/Julian/rpds.py/actions?query=workflow%3ACI
+  :target: https://github.com/crate-py/rpds/actions?query=workflow%3ACI
 
 
 Python bindings to the Rust ``rpds`` crate.
 
 What's here is quite minimal (in transparency, it was written initially to support replacing ``pyrsistent`` in the `referencing library <https://github.com/python-jsonschema/referencing>`_).
 If you see something missing (which is very likely), a PR is definitely welcome to add it.
```

