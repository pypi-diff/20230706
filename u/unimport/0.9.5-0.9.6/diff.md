# Comparing `tmp/unimport-0.9.5.tar.gz` & `tmp/unimport-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimport-0.9.5.tar", last modified: Wed Mar  9 23:11:19 2022, max compression
+gzip compressed data, was "unimport-0.9.6.tar", last modified: Wed May  4 12:33:50 2022, max compression
```

## Comparing `unimport-0.9.5.tar` & `unimport-0.9.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 23:11:19.683234 unimport-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-03-09 23:11:19.000000 unimport-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-03-09 23:11:19.683234 unimport-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-03-09 23:11:19.000000 unimport-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-09 23:11:19.683234 unimport-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-03-09 23:11:19.000000 unimport-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 23:11:19.679234 unimport-0.9.5/unimport/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16345 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/color.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 23:11:19.683234 unimport-0.9.5/unimport/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/commands/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/commands/permission.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     4397 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/refactor.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/relate.py
--rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     4935 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 23:11:19.679234 unimport-0.9.5/unimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-09 23:11:19.000000 unimport-0.9.5/unimport.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:50.089495 unimport-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-05-04 12:33:49.000000 unimport-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-05-04 12:33:50.089495 unimport-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-05-04 12:33:49.000000 unimport-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-04 12:33:50.089495 unimport-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-05-04 12:33:49.000000 unimport-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:50.085495 unimport-0.9.6/unimport/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16345 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/color.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:50.089495 unimport-0.9.6/unimport/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/permission.py
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4397 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/refactor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/relate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4935 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:50.089495 unimport-0.9.6/unimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-05-04 12:33:50.000000 unimport-0.9.6/unimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/zip-safe
```

### Comparing `unimport-0.9.5/LICENSE` & `unimport-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/PKG-INFO` & `unimport-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimport
-Version: 0.9.5
+Version: 0.9.6
 Summary: A linter, formatter for finding and removing unused import statements.
 Home-page: https://github.com/hakancelik96/unimport
 Author: Hakan Çelik
 Author-email: hakancelik96@outlook.com
 License: MIT
 Project-URL: Documentation, https://unimport.hakancelik.dev/
 Project-URL: Issues, https://github.com/hakancelik96/unimport/issues
@@ -40,12 +40,13 @@
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
```

### Comparing `unimport-0.9.5/README.md` & `unimport-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/setup.py` & `unimport-0.9.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with open(readme_md, encoding="utf8") as ld_file:
         return ld_file.read()
 
 
 DESCRIPTION = (
     "A linter, formatter for finding and removing unused import statements."
 )
-VERSION = "0.9.5"
+VERSION = "0.9.6"
 
 
 setup(
     name="unimport",
     version=VERSION,
     description=DESCRIPTION,
     long_description=get_long_description(),
@@ -71,11 +71,12 @@
         "Environment :: Console",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     entry_points={"console_scripts": ["unimport = unimport.__main__:main"]},
 )
```

### Comparing `unimport-0.9.5/unimport/analyzer.py` & `unimport-0.9.6/unimport/analyzer.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/color.py` & `unimport-0.9.6/unimport/color.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/commands/check.py` & `unimport-0.9.6/unimport/commands/check.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/commands/options.py` & `unimport-0.9.6/unimport/commands/options.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/commands/permission.py` & `unimport-0.9.6/unimport/commands/permission.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/commands/remove.py` & `unimport-0.9.6/unimport/commands/remove.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/config.py` & `unimport-0.9.6/unimport/config.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/constants.py` & `unimport-0.9.6/unimport/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import libcst as cst
 
 from unimport.statement import Import, ImportFrom, Name
 
 DESCRIPTION = (
     "A linter, formatter for finding and removing unused import statements."
 )
-VERSION = "0.9.5"
+VERSION = "0.9.6"
 
 __all__ = (
     "BUILTINS",
     "BUILTIN_MODULE_NAMES",
     "CFNT",
     "DESCRIPTION",
     "EXCLUDE_REGEX_PATTERN",
```

### Comparing `unimport-0.9.5/unimport/main.py` & `unimport-0.9.6/unimport/main.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/refactor.py` & `unimport-0.9.6/unimport/refactor.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/relate.py` & `unimport-0.9.6/unimport/relate.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/statement.py` & `unimport-0.9.6/unimport/statement.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport/utils.py` & `unimport-0.9.6/unimport/utils.py`

 * *Files identical despite different names*

### Comparing `unimport-0.9.5/unimport.egg-info/PKG-INFO` & `unimport-0.9.6/unimport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimport
-Version: 0.9.5
+Version: 0.9.6
 Summary: A linter, formatter for finding and removing unused import statements.
 Home-page: https://github.com/hakancelik96/unimport
 Author: Hakan Çelik
 Author-email: hakancelik96@outlook.com
 License: MIT
 Project-URL: Documentation, https://unimport.hakancelik.dev/
 Project-URL: Issues, https://github.com/hakancelik96/unimport/issues
@@ -40,12 +40,13 @@
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
```

### Comparing `unimport-0.9.5/unimport.egg-info/SOURCES.txt` & `unimport-0.9.6/unimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

