# Comparing `tmp/merkly-0.7.1.tar.gz` & `tmp/merkly-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkly-0.7.1.tar", max compression
+gzip compressed data, was "merkly-0.7.2.tar", max compression
```

## Comparing `merkly-0.7.1.tar` & `merkly-0.7.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-23 19:07:33.847162 merkly-0.7.1/LICENSE
--rw-r--r--   0        0        0     5392 2023-06-23 19:07:33.847162 merkly-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-06-23 19:07:33.851163 merkly-0.7.1/merkly/__init__.py
--rw-r--r--   0        0        0     4549 2023-06-23 19:07:33.851163 merkly-0.7.1/merkly/mtree.py
--rw-r--r--   0        0        0     2769 2023-06-23 19:07:33.851163 merkly-0.7.1/merkly/utils.py
--rw-r--r--   0        0        0      878 2023-06-23 19:07:33.851163 merkly-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 merkly-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-06 03:26:05.839926 merkly-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5392 2023-07-06 03:26:05.839926 merkly-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 03:26:05.839926 merkly-0.7.2/merkly/__init__.py
+-rw-r--r--   0        0        0     4554 2023-07-06 03:26:05.839926 merkly-0.7.2/merkly/mtree.py
+-rw-r--r--   0        0        0     2769 2023-07-06 03:26:05.839926 merkly-0.7.2/merkly/utils.py
+-rw-r--r--   0        0        0      878 2023-07-06 03:26:05.839926 merkly-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 merkly-0.7.2/PKG-INFO
```

### Comparing `merkly-0.7.1/LICENSE` & `merkly-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `merkly-0.7.1/README.md` & `merkly-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `merkly-0.7.1/merkly/mtree.py` & `merkly-0.7.2/merkly/mtree.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self, leafs: List[str], hash_function: Callable[[str], str] = keccak
     ) -> None:
         is_power_2(len(leafs))
         hash_function_type_checking(hash_function)
         self.hash_function: Callable[[str], str] = hash_function
         self.raw_leafs: List[str] = leafs
         self.leafs: List[str] = self.__hash_leafs(leafs)
-        self.short_leafs: List[str] = self.short(leafs)
+        self.short_leafs: List[str] = self.short(self.leafs)
 
     def __hash_leafs(self, leafs: List[str]) -> List[str]:
         return list(map(self.hash_function, leafs))
 
     def __repr__(self) -> str:
         return f"""MerkleTree(\nraw_leafs: {self.raw_leafs}\nleafs: {self.leafs}\nshort_leafs: {self.short(self.leafs)})"""
```

### Comparing `merkly-0.7.1/merkly/utils.py` & `merkly-0.7.2/merkly/utils.py`

 * *Files identical despite different names*

### Comparing `merkly-0.7.1/pyproject.toml` & `merkly-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merkly"
-version = "0.7.1"
+version = "0.7.2"
 description = "🌳 The simple and easy implementation of Merkle Tree"
 authors = ["Lucas Oliveira <olivmath@protonmail.com>"]
 repository = "https://github.com/olivmath/merkly.git"
 documentation = "https://pypi.org/project/merkly/"
 readme = "README.md"
 license = "MIT"
 keywords = [
```

### Comparing `merkly-0.7.1/PKG-INFO` & `merkly-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkly
-Version: 0.7.1
+Version: 0.7.2
 Summary: 🌳 The simple and easy implementation of Merkle Tree
 Home-page: https://github.com/olivmath/merkly.git
 License: MIT
 Keywords: merkle-tree,merkle-proof,merkle-root,keccak256,blockchain
 Author: Lucas Oliveira
 Author-email: olivmath@protonmail.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: merkly Version: 0.7.1 Summary: ð³ The simple and
+Metadata-Version: 2.1 Name: merkly Version: 0.7.2 Summary: ð³ The simple and
 easy implementation of Merkle Tree Home-page: https://github.com/olivmath/
 merkly.git License: MIT Keywords: merkle-tree,merkle-proof,merkle-
 root,keccak256,blockchain Author: Lucas Oliveira Author-email:
 olivmath@protonmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

