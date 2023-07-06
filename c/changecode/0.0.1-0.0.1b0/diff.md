# Comparing `tmp/changecode-0.0.1.tar.gz` & `tmp/changecode-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changecode-0.0.1.tar", max compression
+gzip compressed data, was "changecode-0.0.1b0.tar", max compression
```

## Comparing `changecode-0.0.1.tar` & `changecode-0.0.1b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       64 2023-06-22 12:46:10.476826 changecode-0.0.1/changecode/__init__.py
--rw-r--r--   0        0        0      181 2023-03-08 08:17:16.620095 changecode-0.0.1/changecode/baseparse.py
--rw-r--r--   0        0        0       57 2023-03-08 08:15:46.971025 changecode-0.0.1/changecode/classes.py
--rw-r--r--   0        0        0     1615 2023-06-22 16:23:06.251443 changecode-0.0.1/changecode/code.py
--rw-r--r--   0        0        0       62 2023-03-08 08:21:27.997927 changecode-0.0.1/changecode/functions.py
--rw-r--r--   0        0        0      379 2023-03-08 08:17:20.320221 changecode-0.0.1/changecode/imports.py
--rw-r--r--   0        0        0     1126 2023-02-10 12:44:45.759881 changecode-0.0.1/LICENSE.md
--rw-r--r--   0        0        0      373 2023-07-06 21:20:31.744854 changecode-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-21 20:27:30.635151 changecode-0.0.1/README.md
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 changecode-0.0.1/setup.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 changecode-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-05 10:05:04.588415 changecode-0.0.1b0/changecode/__init__.py
+-rw-r--r--   0        0        0      181 2023-03-08 08:17:16.620095 changecode-0.0.1b0/changecode/baseparse.py
+-rw-r--r--   0        0        0       57 2023-03-08 08:15:46.971025 changecode-0.0.1b0/changecode/classes.py
+-rw-r--r--   0        0        0     1654 2023-03-08 08:21:27.997927 changecode-0.0.1b0/changecode/code.py
+-rw-r--r--   0        0        0       62 2023-03-08 08:21:27.997927 changecode-0.0.1b0/changecode/functions.py
+-rw-r--r--   0        0        0      379 2023-03-08 08:17:20.320221 changecode-0.0.1b0/changecode/imports.py
+-rw-r--r--   0        0        0     1126 2023-02-10 12:44:45.759881 changecode-0.0.1b0/LICENSE.md
+-rw-r--r--   0        0        0      374 2023-06-21 20:36:09.612560 changecode-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-21 20:27:30.635151 changecode-0.0.1b0/README.md
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 changecode-0.0.1b0/setup.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 changecode-0.0.1b0/PKG-INFO
```

### Comparing `changecode-0.0.1/changecode/code.py` & `changecode-0.0.1b0/changecode/code.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """Код должен быть по PEP8 чтобы все работало!"""
 
 from typing import List
 
+from .imports import ImportParse
+
 
 class CodeParse:
     def __init__(self, file):
         self._file = file
-        self.code_strings: List[str] = file.read().split("\n")
+        self.code_strings = file.read().split("\n")
 
         self.imports_parse = None
         self.functions_parse = None
         self.classes_parse = None
 
-    def search(self, text: str) -> List:
+    def _search(self, text) -> List:
         return [(num, string) for num, string in enumerate(self.code_strings) if text in string]
     
     def _get_imports(self, code_strings):
         pass
 
-    def add_code_line(self, string: str, index: int = 0) -> None:
-        self.code_strings.insert(index, string)
-
-    def add_import_from(self, from_: str, import_: str) -> None:
-        self.add_code_line(f"from {from_} import {import_}")
-
-    def add_import_from_as(self, from_: str, import_: str, as_: str) -> None:
-        self.add_code_line(f"from {from_} import {import_} as {as_}")
-
-    def add_import(self, import_: str) -> None:
-        self.add_code_line(f"import {import_}")
-
-    def add_import_as(self, import_: str, as_: str) -> None:
-        self.add_code_line(f"import {import_} as {as_}")
+    def add_import_from(self, from_, import_) -> None:
+        import_code = f"from {from_} import {import_}"
+        self.code_strings.insert(0, import_code)
+
+    def add_import_from_as(self, from_, import_, as_) -> None:
+        import_code = f"from {from_} import {import_} as {as_}"
+        self.code_strings.insert(0, import_code)
+
+    def add_import(self, import_) -> None:
+        import_code = f"import {import_}"
+        self.code_strings.insert(0, import_code)
+
+    def add_import_as(self, import_, as_) -> None:
+        import_code = f"import {import_} as {as_}"
+        self.code_strings.insert(0, import_code)
 
     def append_in_lists(self, var: str, value: str):
         strings = self._search(var + " = ")
 
         for num, string in strings:
             var_values = string[string.find("[")+1:string.find("]")]
             self.code_strings[num] = f"{var} = [{var_values}, {value}]"
```

### Comparing `changecode-0.0.1/LICENSE.md` & `changecode-0.0.1b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `changecode-0.0.1/setup.py` & `changecode-0.0.1b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['changecode']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'changecode',
-    'version': '0.0.1',
+    'version': '0.0.1b0',
     'description': 'Change python code',
     'long_description': '# Changecode\n\n___\n',
     'author': 'BulatXam',
     'author_email': 'Khamdbulat@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `changecode-0.0.1/PKG-INFO` & `changecode-0.0.1b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changecode
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: Change python code
 License: MIT
 Author: BulatXam
 Author-email: Khamdbulat@yandex.ru
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

