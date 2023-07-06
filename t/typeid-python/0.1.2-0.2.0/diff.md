# Comparing `tmp/typeid_python-0.1.2.tar.gz` & `tmp/typeid_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeid_python-0.1.2.tar", max compression
+gzip compressed data, was "typeid_python-0.2.0.tar", max compression
```

## Comparing `typeid_python-0.1.2.tar` & `typeid_python-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-02 21:35:38.940939 typeid_python-0.1.2/LICENSE
--rw-r--r--   0        0        0     2469 2023-06-30 11:13:15.292795 typeid_python-0.1.2/README.md
--rw-r--r--   0        0        0     1392 2023-06-30 19:03:55.130105 typeid_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-29 20:43:34.998392 typeid_python-0.1.2/typeid/__init__.py
--rw-r--r--   0        0        0     6545 2023-06-30 10:48:55.361603 typeid_python-0.1.2/typeid/base32.py
--rw-r--r--   0        0        0       37 2023-06-30 09:52:48.383251 typeid_python-0.1.2/typeid/constants.py
--rw-r--r--   0        0        0      207 2023-06-29 20:16:47.263968 typeid_python-0.1.2/typeid/errors.py
--rw-r--r--   0        0        0     1660 2023-06-30 19:03:52.462137 typeid_python-0.1.2/typeid/typeid.py
--rw-r--r--   0        0        0      823 2023-06-30 19:03:52.462137 typeid_python-0.1.2/typeid/validation.py
--rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 typeid_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-02 21:35:38.940939 typeid_python-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2469 2023-06-30 11:13:15.292795 typeid_python-0.2.0/README.md
+-rw-r--r--   0        0        0     1450 2023-07-06 12:47:21.595852 typeid_python-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-29 20:43:34.998392 typeid_python-0.2.0/typeid/__init__.py
+-rw-r--r--   0        0        0     6469 2023-07-06 12:42:30.775952 typeid_python-0.2.0/typeid/base32.py
+-rw-r--r--   0        0        0       37 2023-06-30 09:52:48.383251 typeid_python-0.2.0/typeid/constants.py
+-rw-r--r--   0        0        0      207 2023-06-29 20:16:47.263968 typeid_python-0.2.0/typeid/errors.py
+-rw-r--r--   0        0        0     1660 2023-06-30 19:03:52.462137 typeid_python-0.2.0/typeid/typeid.py
+-rw-r--r--   0        0        0      899 2023-07-06 12:44:57.757807 typeid_python-0.2.0/typeid/validation.py
+-rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 typeid_python-0.2.0/PKG-INFO
```

### Comparing `typeid_python-0.1.2/LICENSE` & `typeid_python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typeid_python-0.1.2/README.md` & `typeid_python-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `typeid_python-0.1.2/pyproject.toml` & `typeid_python-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 [tool.poetry]
 name = "typeid-python"
-version = "0.1.2"
+version = "0.2.0"
 description = "Python implementation of TypeIDs: type-safe, K-sortable, and globally unique identifiers inspired by Stripe IDs"
 authors = ["Murad Akhundov <akhundov1murad@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/akhundMurad/typeid-python"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
 ]
-
 keywords = ["typeid", "uuid", "uuid6", "guid"]
+packages = [{ include = "typeid" }]
 
-packages = [
-    { include = "typeid" }
-]
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
   "/docs",
   "/examples",
   "/deps",
@@ -40,24 +37,30 @@
   "requirements.txt",
   "mypy.ini",
   "pytest.ini",
   ".flake8",
   "pytest.ini",
 ]
 
+
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 uuid6 = "^2023.5.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 black = "^23.3.0"
 flake8 = "^5.0.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 requests = "^2.31.0"
 pyyaml = "^6.0"
 
+
+[tool.pylint]
+disable = ["C0111", "C0116", "C0114", "R0903"]
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `typeid_python-0.1.2/typeid/base32.py` & `typeid_python-0.2.0/typeid/base32.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,17 +299,14 @@
     dst[24] = ALPHABET[((src[14] & 3) << 3) | ((src[15] & 224) >> 5)]
     dst[25] = ALPHABET[src[15] & 31]
 
     return "".join(dst)
 
 
 def decode(s: str) -> list:
-    if len(s) != SUFFIX_LEN:
-        raise RuntimeError("Invalid length.")
-
     v = bytes(s, encoding="utf-8")
 
     if (
         TABLE[v[0]] == 0xFF
         and TABLE[v[1]] == 0xFF
         and TABLE[v[2]] == 0xFF
         and TABLE[v[3]] == 0xFF
```

### Comparing `typeid_python-0.1.2/typeid/typeid.py` & `typeid_python-0.2.0/typeid/typeid.py`

 * *Files identical despite different names*

### Comparing `typeid_python-0.1.2/typeid/validation.py` & `typeid_python-0.2.0/typeid/validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from typeid import base32
-from typeid.constants import PREFIX_MAX_LEN
+from typeid.constants import PREFIX_MAX_LEN, SUFFIX_LEN
 from typeid.errors import PrefixValidationException, SuffixValidationException
 
 
 def validate_prefix(prefix: str) -> None:
     if not prefix.islower() or not prefix.isascii() or len(prefix) > PREFIX_MAX_LEN or not prefix.isalpha():
         raise PrefixValidationException(f"Invalid prefix: {prefix}.")
 
 
 def validate_suffix(suffix: str) -> None:
     if (
-        suffix == ""
+        len(suffix) != SUFFIX_LEN
+        or suffix == ""
         or " " in suffix
         or (not suffix.isdigit() and not suffix.islower())
         or any([symbol not in base32.ALPHABET for symbol in suffix])
+        or suffix[0] > "7"
     ):
         raise SuffixValidationException(f"Invalid suffix: {suffix}.")
     try:
         base32.decode(suffix)
     except Exception as exc:
         raise SuffixValidationException(f"Invalid suffix: {suffix}.") from exc
```

### Comparing `typeid_python-0.1.2/PKG-INFO` & `typeid_python-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeid-python
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python implementation of TypeIDs: type-safe, K-sortable, and globally unique identifiers inspired by Stripe IDs
 Home-page: https://github.com/akhundMurad/typeid-python
 License: MIT
 Keywords: typeid,uuid,uuid6,guid
 Author: Murad Akhundov
 Author-email: akhundov1murad@gmail.com
 Requires-Python: >=3.8,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: typeid-python Version: 0.1.2 Summary: Python
+Metadata-Version: 2.1 Name: typeid-python Version: 0.2.0 Summary: Python
 implementation of TypeIDs: type-safe, K-sortable, and globally unique
 identifiers inspired by Stripe IDs Home-page: https://github.com/akhundMurad/
 typeid-python License: MIT Keywords: typeid,uuid,uuid6,guid Author: Murad
 Akhundov Author-email: akhundov1murad@gmail.com Requires-Python: >=3.8,<4
 Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

