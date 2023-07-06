# Comparing `tmp/findpydeps-0.2.5.tar.gz` & `tmp/findpydeps-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findpydeps-0.2.5.tar", last modified: Tue Nov 23 22:54:01 2021, max compression
+gzip compressed data, was "findpydeps-0.2.6.tar", last modified: Thu Jul  6 16:47:53 2023, max compression
```

## Comparing `findpydeps-0.2.5.tar` & `findpydeps-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-23 22:54:02.481812 findpydeps-0.2.5/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1072 2021-08-22 20:32:24.000000 findpydeps-0.2.5/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4347 2021-11-23 22:54:02.481812 findpydeps-0.2.5/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2375 2021-09-16 18:12:19.000000 findpydeps-0.2.5/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      112 2021-08-26 19:03:43.000000 findpydeps-0.2.5/pyproject.toml
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1067 2021-11-23 22:54:02.497439 findpydeps-0.2.5/setup.cfg
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-23 22:54:02.075580 findpydeps-0.2.5/src/
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-23 22:54:02.247435 findpydeps-0.2.5/src/findpydeps/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       53 2021-11-23 22:53:54.000000 findpydeps-0.2.5/src/findpydeps/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       99 2021-11-23 22:53:54.000000 findpydeps-0.2.5/src/findpydeps/__main__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    28296 2021-11-23 22:53:54.000000 findpydeps-0.2.5/src/findpydeps/findpydeps.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-23 22:54:02.434936 findpydeps-0.2.5/src/findpydeps.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4347 2021-11-23 22:54:01.000000 findpydeps-0.2.5/src/findpydeps.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      318 2021-11-23 22:54:02.000000 findpydeps-0.2.5/src/findpydeps.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2021-11-23 22:54:01.000000 findpydeps-0.2.5/src/findpydeps.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       57 2021-11-23 22:54:01.000000 findpydeps-0.2.5/src/findpydeps.egg-info/entry_points.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       11 2021-11-23 22:54:01.000000 findpydeps-0.2.5/src/findpydeps.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1001)        0 2023-07-06 16:47:53.743260 findpydeps-0.2.6/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)     1072 2023-07-05 17:03:47.000000 findpydeps-0.2.6/LICENSE
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)     4827 2023-07-06 16:47:53.743260 findpydeps-0.2.6/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)     2875 2023-07-05 22:30:01.000000 findpydeps-0.2.6/README.md
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)      112 2023-07-05 17:03:47.000000 findpydeps-0.2.6/pyproject.toml
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)     1067 2023-07-06 16:47:53.743260 findpydeps-0.2.6/setup.cfg
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1001)        0 2023-07-06 16:47:53.739925 findpydeps-0.2.6/src/
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1001)        0 2023-07-06 16:47:53.739925 findpydeps-0.2.6/src/findpydeps/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)       90 2023-07-06 16:47:13.000000 findpydeps-0.2.6/src/findpydeps/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)       99 2023-07-05 17:03:47.000000 findpydeps-0.2.6/src/findpydeps/__main__.py
+-rwxr-xr-x   0 nicolas   (1000) nicolas   (1001)    28732 2023-07-06 16:47:13.000000 findpydeps-0.2.6/src/findpydeps/findpydeps.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1001)        0 2023-07-06 16:47:53.743260 findpydeps-0.2.6/src/findpydeps.egg-info/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)     4827 2023-07-06 16:47:53.000000 findpydeps-0.2.6/src/findpydeps.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)      318 2023-07-06 16:47:53.000000 findpydeps-0.2.6/src/findpydeps.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)        1 2023-07-06 16:47:53.000000 findpydeps-0.2.6/src/findpydeps.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)       56 2023-07-06 16:47:53.000000 findpydeps-0.2.6/src/findpydeps.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1001)       11 2023-07-06 16:47:53.000000 findpydeps-0.2.6/src/findpydeps.egg-info/top_level.txt
```

### Comparing `findpydeps-0.2.5/LICENSE` & `findpydeps-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `findpydeps-0.2.5/PKG-INFO` & `findpydeps-0.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: findpydeps
-Version: 0.2.5
+Version: 0.2.6
 Summary: Find the python dependencies used by your python files and projects
 Home-page: https://github.com/Nicolas-Reyland/findpydeps
 Author: Nicolas Reyland
 Author-email: nicolas@reyland.dev
 Maintainer: Nicolas Reyland
 Maintainer-email: nicolas@reyland.dev
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/Nicolas-Reyland/findpydeps/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Downloads](https://static.pepy.tech/badge/findpydeps)](https://pepy.tech/project/findpydeps)
+[![Downloads](https://static.pepy.tech/badge/findpydeps/month)](https://pepy.tech/project/findpydeps)
+[![Downloads](https://static.pepy.tech/badge/findpydeps/week)](https://pepy.tech/project/findpydeps)
+
 # findpydeps
 Find the python dependencies used by your python files and projects.
 
 ## Installation
 Simply install it via pip:
 ```bash
 pip install findpydeps
@@ -57,42 +60,44 @@
 cd your_python_project
 findpydeps -i main.py --follow-local-imports > requirements.txt
 pip install -r requirements.txt
 ```
 
 For exhaustive usage information, please refer to the `findpydeps -h` output (or `python3 -m findpydeps -h`) :
 ```
-usage: findpydeps [-h] [-i input [input ...]] [-d expr] [-r policy] [-l] [-s] [--blocks] [--no-blocks] [--functions] [--no-functions] [-v] [--header] [--no-header]
+usage: findpydeps.py [-h] [-i input [input ...]] [-d expr] [-r policy] [-l] [-s] [--blocks] [--no-blocks] [--functions] [--no-functions] [--submodules-as-modules] [-v] [--header]
+                     [--no-header]
 
 Find the python dependencies used by your python files
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -i input [input ...], --input input [input ...]
                         input files and/or directories (directories will be scanned for *.py files)
   -d expr, --dir-scanning-expr expr
                         only process files with this expression in scanned directories [default: *.py]
   -r policy, --removal-policy policy
                         removal policy for modules (0: local & stdlib, 1: local only, 2: stdlib only, 3: no removal) [default: 0]
   -l, --follow-local-imports
-                        follow imports for local files
+                        also scan files which are imported locally (not libraries)
   -s, --strict          raise an error on SyntaxErrors in the input python files
   --blocks              scan contents of 'if', 'try' and 'with' blocks
   --no-blocks           don't scan contents of 'if', 'try' and 'with' blocks
   --functions           scan contents of functions
   --no-functions        don't scan contents of functions
+  --submodules-as-modules
+                        submodule imports are treated as module-imports (e.g. "import random.shuffle" generates "random.shuffle", not "random", which is the default behavior)
   -v, --verbose         verbose mode (all messages prepended with '#')
   --header              show the greeting header
   --no-header           don't show the greeting header
 ```
 
 
 ## Todo
- * Verify package names on pypi.org (check if installable via pip)
- * Exclude/Include custom package names option
+ * Option to manually exclude/include modules
 
 MIT License
 
 Copyright (c) 2021 Nicolas Reyland
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
@@ -107,9 +112,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
-
```

### Comparing `findpydeps-0.2.5/README.md` & `findpydeps-0.2.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![Downloads](https://static.pepy.tech/badge/findpydeps)](https://pepy.tech/project/findpydeps)
+[![Downloads](https://static.pepy.tech/badge/findpydeps/month)](https://pepy.tech/project/findpydeps)
+[![Downloads](https://static.pepy.tech/badge/findpydeps/week)](https://pepy.tech/project/findpydeps)
+
 # findpydeps
 Find the python dependencies used by your python files and projects.
 
 ## Installation
 Simply install it via pip:
 ```bash
 pip install findpydeps
@@ -33,35 +37,37 @@
 cd your_python_project
 findpydeps -i main.py --follow-local-imports > requirements.txt
 pip install -r requirements.txt
 ```
 
 For exhaustive usage information, please refer to the `findpydeps -h` output (or `python3 -m findpydeps -h`) :
 ```
-usage: findpydeps [-h] [-i input [input ...]] [-d expr] [-r policy] [-l] [-s] [--blocks] [--no-blocks] [--functions] [--no-functions] [-v] [--header] [--no-header]
+usage: findpydeps.py [-h] [-i input [input ...]] [-d expr] [-r policy] [-l] [-s] [--blocks] [--no-blocks] [--functions] [--no-functions] [--submodules-as-modules] [-v] [--header]
+                     [--no-header]
 
 Find the python dependencies used by your python files
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -i input [input ...], --input input [input ...]
                         input files and/or directories (directories will be scanned for *.py files)
   -d expr, --dir-scanning-expr expr
                         only process files with this expression in scanned directories [default: *.py]
   -r policy, --removal-policy policy
                         removal policy for modules (0: local & stdlib, 1: local only, 2: stdlib only, 3: no removal) [default: 0]
   -l, --follow-local-imports
-                        follow imports for local files
+                        also scan files which are imported locally (not libraries)
   -s, --strict          raise an error on SyntaxErrors in the input python files
   --blocks              scan contents of 'if', 'try' and 'with' blocks
   --no-blocks           don't scan contents of 'if', 'try' and 'with' blocks
   --functions           scan contents of functions
   --no-functions        don't scan contents of functions
+  --submodules-as-modules
+                        submodule imports are treated as module-imports (e.g. "import random.shuffle" generates "random.shuffle", not "random", which is the default behavior)
   -v, --verbose         verbose mode (all messages prepended with '#')
   --header              show the greeting header
   --no-header           don't show the greeting header
 ```
 
 
 ## Todo
- * Verify package names on pypi.org (check if installable via pip)
- * Exclude/Include custom package names option
+ * Option to manually exclude/include modules
```

### Comparing `findpydeps-0.2.5/setup.cfg` & `findpydeps-0.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = findpydeps
-version = 0.2.5
+version = 0.2.6
 author = Nicolas Reyland
 author_email = nicolas@reyland.dev
 maintainer = Nicolas Reyland
 maintainer_email = nicolas@reyland.dev
 description = Find the python dependencies used by your python files and projects
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
```

### Comparing `findpydeps-0.2.5/src/findpydeps/findpydeps.py` & `findpydeps-0.2.6/src/findpydeps/findpydeps.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 from __future__ import print_function
 from __future__ import with_statement
 
 """ Python Script to find dependencies/modules from import-statements in python files
 
-usage: findpydeps [-h] [-i input [input ...]] [-d expr] [-r policy] [-l] [-s] [--blocks] [--no-blocks] [--functions] [--no-functions] [-v] [--header] [--no-header]
+usage: findpydeps.py [-h] [-i input [input ...]] [-d expr] [-r policy] [-l] [-s] [--blocks] [--no-blocks] [--functions] [--no-functions] [--submodules-as-modules] [-v] [--header]
+                     [--no-header]
 
 Find the python dependencies used by your python files
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -i input [input ...], --input input [input ...]
                         input files and/or directories (directories will be scanned for *.py files)
   -d expr, --dir-scanning-expr expr
                         only process files with this expression in scanned directories [default: *.py]
   -r policy, --removal-policy policy
                         removal policy for modules (0: local & stdlib, 1: local only, 2: stdlib only, 3: no removal) [default: 0]
   -l, --follow-local-imports
                         follow imports for local files
   -s, --strict          raise an error on SyntaxErrors in the input python files
   --blocks              scan contents of 'if', 'try' and 'with' blocks
   --no-blocks           don't scan contents of 'if', 'try' and 'with' blocks
   --functions           scan contents of functions
   --no-functions        don't scan contents of functions
+  --submodules-as-modules
+                        submodule imports are treated as module-imports (e.g. "import random.shuffle" generates "random.shuffle", not "random", which is the default behavior)
   -v, --verbose         verbose mode (all messages prepended with '#')
   --header              show the greeting header
   --no-header           don't show the greeting header
 
 """
 
 # Python Dependencies
 from argparse import ArgumentParser
-import os, sys, fnmatch
+import os
+import sys
+import fnmatch
 import ast
 
+from typing import Iterable, AnyStr
 
 # Argument Parser
 
 # rename __main__ ?
 renamed_sys_argv0: bool = False
 if sys.argv[0].endswith("__main__.py"):
     sys.argv[0] = sys.argv[0][:-11] + "findpydeps"
@@ -71,22 +77,23 @@
 
 parser.add_argument(
     "-r",
     "--removal-policy",
     metavar="policy",
     type=int,
     default=0,
-    help="removal policy for modules (0: local & stdlib, 1: local only, 2: stdlib only, 3: no removal) [default: %(default)s]",
+    help="removal policy for modules (0: local & stdlib, 1: local only, 2: stdlib only, 3: no removal) [default: %("
+         "default)s]",
 )
 
 parser.add_argument(
     "-l",
     "--follow-local-imports",
     action="store_true",
-    help="follow imports for local files",
+    help="also scan files which are imported locally (not libraries)",
 )
 
 parser.add_argument(
     "-s",
     "--strict",
     action="store_true",
     help="raise an error on SyntaxErrors in the input python files",
@@ -118,14 +125,22 @@
 parser.add_argument(
     "--no-functions",
     dest="functions",
     action="store_false",
     help="don't scan contents of functions",
 )
 
+parser.add_argument(
+    "--submodules-as-modules",
+    dest="submodules",
+    action="store_true",
+    help='submodule imports are treated as module-imports (e.g. "import random.shuffle" generates "random.shuffle", '
+         'not "random", which is the default behavior)',
+)
+
 parser.set_defaults(functions=True)
 
 parser.add_argument(
     "-v",
     "--verbose",
     action="store_true",
     help="verbose mode (all messages prepended with '#')",
@@ -140,20 +155,19 @@
     dest="header",
     action="store_false",
     help="don't show the greeting header",
 )
 
 parser.set_defaults(header=True)
 
-
-# Contsants
+# Constants
 HEADER: str = "# Generated by https://github.com/Nicolas-Reyland/findpydeps"
 USAGE_MSG: str = 'Try "python3 -m findpydeps -h" to get help.'
 
-PYTHON_STANDARD_MODULES: set[str] = {
+PYTHON_STANDARD_MODULES: frozenset[str] = getattr(sys, "stdlib_module_names", frozenset({
     "__future__",
     "__main__",
     "_thread",
     "abc",
     "aifc",
     "argparse",
     "array",
@@ -356,23 +370,25 @@
     "xml",
     "xmlrpc",
     "zipapp",
     "zipfile",
     "zipimport",
     "zlib",
     "zoneinfo",
-}  # this set was definately not written manually. I love selenium !!!
+}))
 
 DEPENDENCIES: set[str] = set()
 READ_FILES: set[str] = set()
 
 ROOT_DIR: str = os.path.dirname(os.path.abspath(__file__))
 
+
 # Lambdas
-vprint = lambda *a, **k: None
+def vprint(*__, **___):
+    ...
 
 
 # Custom Exception
 class ArgumentError(Exception):
     """
     A class used for custom Argument Errors
 
@@ -398,15 +414,15 @@
             if self.message
             else "ArgumentError has been raised"
         )
 
 
 # Functions
 def path_from_relative_import(base_path: str, import_str: str) -> tuple[bool, str]:
-    """Builds the path corresponging to a python relative import string
+    """Builds the path corresponding to a python relative import string
 
     Relative imports in python often have dots "." in them. Calculations of
     import paths starting with double dots ".." or more are done using the
     relative import value (ast.ImportFrom.level).
 
     Parameters
     ---------
@@ -475,15 +491,15 @@
     A simple import is a python import in the form of /import .* (as .*)/
     Returns the name of the main module. Remember that you can do imports such as
     "import numpy.random as rd", where you would only want the "numpy" part, not
     "numpy.random" or "random".
 
     Parameters
     ---------
-    import_str : str
+    import_name : str
         Import string (e.g. "math", "matplotlib.pylab")
 
     Returns
     -------
     module_name : str
         Name of the python module
 
@@ -510,22 +526,22 @@
         List containing (num_dots - 1) times the ".." string
 
     """
 
     return [".." for _ in range(num_dots - 1)]
 
 
-def get_module_names_in_importfrom_obj(
-    obj: ast.ImportFrom, current_path: str, args: dict[str, bool]
+def get_module_names_in_import_from_obj(
+        obj: ast.ImportFrom, current_path: str, args: dict[str, bool]
 ) -> tuple[set[str], set[str]]:
-    """Get the names of the modules that are used in an from-import statement
+    """Get the names of the modules that are used in a from-import statement
 
     The from-import statement in python (e.g. "from math import sin, cos") lets you
     import python objects (variables, classes, functions, modules) from the import source.
-    The source is, most of the time, referrning a python source file. You therefore often
+    The source is, most of the time, referring to a python source file. You therefore often
     only import from a single python source file when doing a from import. But newer python
     import syntax lets you import multiple files from a directory using the from statement
     (e.g. "from .folder import file1, file2", "from .. import *"). You therefore can have
     multiple module imports in a single from-import.
 
     Parameters
     ----------
@@ -537,25 +553,26 @@
         The command-line arguments given to this script
 
     Returns
     -------
     all_imports : tuple[set[str], set[str]]
         global_imports : set[str]
             Global imports, not referring to a local file (except you played with the sys.path or
-            other inpredictable pythonic sutff)
+            other unpredictable pythonic stuff)
         local_import_files : set[str]
             Set of the files that are imported locally. Their extension (".py") is stripped from
             the string value
 
     """
 
     if not obj.module:
         if obj.level == 0:
             vprint(
-                f"WARNING: Bizarre import with level {obj.level}, but no module name ({obj.module}). Alias-names are {[alias.name for alias in obj.names]}. For more debugging: {obj.__dict__}"
+                f"WARNING: Bizarre import with level {obj.level}, but no module name ({obj.module}). "
+                f"Alias-names are {[alias.name for alias in obj.names]}. For more debugging: {obj.__dict__}"
             )
             return set(), set()
         obj.module = "." * obj.level
         vprint("NONE: Changing obj.module to", obj.module)
 
     elif obj.level != 0:
         obj.module = "." * obj.level + obj.module
@@ -566,52 +583,46 @@
     potential_path_dirname = os.path.dirname(potential_path)
     potential_path_filename = os.path.basename(potential_path)
     # to check if file exists:
     #  - make sure it can be a file, looking at the python import string (`not must_be_dir`)
     #  - check if directory which it should be in exists
     #  - check if any of the files in this directory are in this format: /(filename)(.py[^\.]*)/
     if (
-        not must_be_dir
-        and os.path.isdir(potential_path_dirname)
-        and any(
-            map(
-                lambda fn: os.path.basename(fn).split(".py")[0]
-                == potential_path_filename
-                if fn.count(".py") > 0
-                else False,
-                files_in_dir(potential_path_dirname),
-            )
-        )
+            not must_be_dir
+            and os.path.isdir(potential_path_dirname)
+            and any(os.path.basename(fn).partition(".py")[0] == potential_path_filename for fn in
+                    files_in_dir(potential_path_dirname) if ".py" in fn)
     ):
         vprint(f"import refers to a file: {potential_path_filename}")
         return set(), {potential_path}
     if os.path.isdir(potential_path):
         vprint(f"import refers to a directory: {potential_path}")
 
         if len(obj.names) == 1 and obj.names[0].name == "*":
-            # python 3.9 : return set(), set(map(lambda fp: fp.removesuffix(".py"), fnmatch.filter(files_in_dir(potential_path), "*.py")))
+            # python 3.9 : return set(), set(map(lambda fp: fp.removesuffix(".py"), fnmatch.filter(files_in_dir(
+            # potential_path), "*.py")))
             return set(), set(
                 map(
                     lambda fp: fp[:-3],
                     fnmatch.filter(files_in_dir(potential_path), "*.py"),
                 )
             )
 
         return set(), set(
             [os.path.join(potential_path, alias.name) for alias in obj.names]
         )
 
-    global_import = get_module_name_in_simple_import(obj.module)
+    global_import = obj.module if args["submodules"] else get_module_name_in_simple_import(obj.module)
     vprint(f"import is global: {global_import}")
 
     return {global_import}, set()
 
 
 def modules_from_ast_import_object(
-    obj: ast.Import | ast.ImportFrom, current_path: str, args: dict[str, bool]
+        obj: ast.Import | ast.ImportFrom, current_path: str, args: dict[str, bool]
 ) -> tuple[set[str], set[str]]:
     """Get the modules that are imported in a python import object
 
     There are two types of python imports: simple imports (import .* as .*) and
     from-imports (from .* import .*). This function returns the set of global and
     local imports
 
@@ -625,75 +636,61 @@
         The command-line arguments given to this script
 
     Returns
     -------
     all_imports : tuple[set[str], set[str]]
         global_imports : set[str]
             Global imports, not referring to a local file (except you played with the sys.path or
-            other inpredictable pythonic sutff)
+            other unpredictable pythonic stuff)
         local_import_files : set[str]
             Set of the files that are imported locally. Their extension (".py") is stripped from
             the string value
 
     Raises
     ------
     AssertionError
-        The `obj` is neither a ast.Import, nor a ast.ImportFrom
+        The `obj` is neither an ast.Import, nor an ast.ImportFrom
 
     """
 
-    global vprint
-
-    T = type(obj)
-    if T is ast.ImportFrom:
+    t = type(obj)
+    if t is ast.ImportFrom:
         # from abc import xyz (as ijk)
-        import_set = set()
-
-        global_imports, local_import_files = get_module_names_in_importfrom_obj(
+        global_imports, local_imports = get_module_names_in_import_from_obj(
             obj, current_path, args
         )
 
-        vprint(f"from import: {global_imports}, {local_import_files}")
-        return global_imports, local_import_files
+        vprint(f"from import: {global_imports}, {local_imports}")
+        return global_imports, local_imports
     else:
         # import abc (as xyz)
-        assert T is ast.Import
-        # TODO: check for local import
+        assert t is ast.Import
         global_imports = set()
-        local_import_files = set()
+        local_imports = set()
         for alias in obj.names:
             import_name = alias.name
             # check for local import
             file_path = path_from_relative_import(current_path, import_name)[1]
             file_path_dir = os.path.dirname(file_path)
-            if (
-                os.path.isfile(file_path + ".py")
-                or os.path.isdir(file_path_dir)
-                and any(
-                    map(
-                        lambda fn: os.path.basename(fn).split(".py")[0] == import_name
-                        if fn.count(".py") > 0
-                        else False,
-                        files_in_dir(file_path_dir),
-                    )
-                )
-            ):
+            if (os.path.isfile(file_path + ".py") or os.path.isdir(file_path_dir) and any(
+                    os.path.basename(fn).partition(".py")[0] == import_name for fn in files_in_dir(file_path_dir) if
+                    ".py" in fn)):
                 # simple local import
-                local_import_files.add(file_path)
+                local_imports.add(file_path)
                 continue
 
             # default step
-            global_imports.add(get_module_name_in_simple_import(import_name))
+            global_imports.add(import_name if args["submodules"] else get_module_name_in_simple_import(import_name))
 
-        vprint(f"simple import: {global_imports}, {local_import_files}")
-        return global_imports, local_import_files
+        vprint(f"simple import: {global_imports}, {local_imports}")
+        return global_imports, local_imports
 
 
 def handle_ast_object(
-    obj: ast.AST, ast_path: str, args: dict[str, bool]
+        obj: ast.AST, ast_path: str, args: dict[str, bool]
 ) -> tuple[set[str], set[str]]:
     """Go through an abstract ast.AST (derived or not) objects
 
     To go through ast.AST object, looking for ast.Import and
     ast.ImportFrom objects. It is looking for objects derived
     from the `ast.AST` class. Then, we iterate through the attributes
     and their values, if iterable.
@@ -708,77 +705,75 @@
         The command-line arguments given to this script
 
     Returns
     -------
     all_imports : tuple[set[str], set[str]]
         global_imports : set[str]
             Global imports, not referring to a local file (except you played with the sys.path or
-            other inpredictable pythonic sutff)
+            other unpredictable pythonic stuff)
         local_import_files : set[str]
             Set of the files that are imported locally. Their extension (".py") is stripped from
             the string value
 
     Raises
     ------
     AssertionError
         The `obj` is not derived from the ast.AST abstract class
 
     """
 
-    global vprint
+    t = type(obj)
+    assert issubclass(t, ast.AST)
 
-    T = type(obj)
-    assert issubclass(T, ast.AST)
-
-    if not args["blocks"] and T in [ast.If, ast.With, ast.Try]:
+    if not args["blocks"] and t in [ast.If, ast.With, ast.Try]:
         return set(), set()
-    if not args["functions"] and T is ast.FunctionDef:
+    if not args["functions"] and t is ast.FunctionDef:
         return set(), set()
 
     # is the current ast object an import ?
-    if T is ast.Import or T is ast.ImportFrom:
+    if t is ast.Import or t is ast.ImportFrom:
+        # declare 'obj' of being of one of those two types
+        obj: ast.Import | ast.ImportFrom
         global_deps, local_deps_files = modules_from_ast_import_object(
             obj, ast_path, args
         )
         vprint(f"global: {global_deps}, local files: {local_deps_files}")
         return global_deps, local_deps_files
 
-    modules: set[str] = set()
-    # try to iterate through python object properties that could, somewhere deeply nested, have ast-import objects in them
+    # try to iterate through python object properties that could,
+    # somewhere deeply nested, have ast-import objects in them
     global_deps, local_deps_files = set(), set()
     for attr_name, attr_value in filter(
-        lambda key_value: not key_value[0].startswith("_"), obj.__dict__.items()
+            lambda key_value: not key_value[0].startswith("_"), obj.__dict__.items()
     ):
         # attributes are lists of ast.AST derivatives ? iterating through them could be wise, when searching for imports
         if (
-            attr_value
-            and type(attr_value) is list
-            and issubclass(type(attr_value[0]), ast.AST)
+                attr_value
+                and type(attr_value) is list
+                and issubclass(type(attr_value[0]), ast.AST)
         ):
             for sub_obj in attr_value:
                 sub_global_deps, sub_local_deps_files = handle_ast_object(
                     sub_obj, ast_path, args
                 )
                 global_deps |= sub_global_deps
                 local_deps_files |= sub_local_deps_files
     return global_deps, local_deps_files
 
 
-def files_in_dir(dirpath: str) -> filter[str]:
-    return filter(
-        os.path.isfile, map(lambda fn: os.path.join(dirpath, fn), os.listdir(dirpath))
-    )
+def files_in_dir(dir_path: str) -> Iterable[str]:
+    return filter(os.path.isfile, (os.path.join(dir_path, fn) for fn in os.listdir(dir_path)))
 
 
 def find_file_dependencies(
-    input_file: str, as_tree: ast.AST, args: dict[str, bool]
+        input_file: str, as_tree: ast.AST, args: dict[str, bool]
 ) -> set[str]:
     """Find the python dependencies used in a python file
 
-    Searches through a python file, using it's AST, looking for
+    Searches through a python file, using its AST, looking for
     dependencies. Local imports can be filtered out. They can also
     be `followed`. This can be configured with the `args`.
 
     Parameters
     ----------
     input_file : str
         Input python file
@@ -795,27 +790,27 @@
     Raises
     ------
     AssertionError
         The `input_file` is not an absolute path
 
     """
 
-    global READ_FILES, vprint
+    global READ_FILES
 
     # assert this so we know the path is unique
     assert os.path.isabs(input_file)
 
     # add file to the read files
     if input_file in READ_FILES:
         return set()
     READ_FILES.add(input_file)
 
-    dirpath = os.path.dirname(input_file)
+    dir_path = os.path.dirname(input_file)
     global_dependencies, local_dependencies_file_set = handle_ast_object(
-        as_tree, dirpath, args
+        as_tree, dir_path, args
     )
 
     # remove local imports? && following local imports?
     if not args["remove_local_imports"] or args["follow_local_imports"]:
         # go through each file
         while local_dependencies_file_set:
             # take next file path
@@ -827,27 +822,27 @@
             # add the local import ?
             if not args["remove_local_imports"]:
                 vprint(f"adding local import: {local_import_name}")
                 global_dependencies.add(local_import_name)
 
             # follow the local import ?
             if args["follow_local_imports"] and (
-                as_tree := parse_python_file(local_import_file_path + ".py")
+                    as_tree := parse_python_file(local_import_file_path + ".py")
             ):
                 # TODO: make sure we don't follow circular imports
                 # python only seems to accept *.py files
                 vprint(f"following local import: {local_import_name}")
                 global_dependencies |= find_file_dependencies(
                     local_import_file_path, as_tree, args
                 )
 
     return global_dependencies
 
 
-def parse_python_file(file_path: str) -> ast.AST:
+def parse_python_file(file_path: str) -> ast.AST | None:
     """Parse the input file into an AST
 
     Parse the python source code input file into a python
     Abstract Syntax Tree (from ast.AST).
 
     Parameters
     ----------
@@ -857,16 +852,14 @@
     Returns
     -------
     tree : ast.AST
         Abstract Syntax Tree of the python file `file_path`
 
     """
 
-    global vprint
-
     if not os.path.isfile(file_path):
         vprint(f"WARNING: input file does not exist: {file_path}")
         return None
 
     with open(file_path, "r") as file:
         try:
             content = file.read()
@@ -878,57 +871,28 @@
             vprint(f"Failed: {se}")
             return None
 
     return as_tree
 
 
 # - Main function -
-def main() -> None:
-    """Main function for the findpydeps script
-
-    Those are the steps by this function :
-     * Parse and validate the command line arguments
-     * Scan the directories that were given, if any
-     * Print the header, unless asked not to
-     * Setup the verbose context
-     * Parse all the input files into trees (AST)
-     * Find all the dependencies (`find_file_dependencies`)
-     * Remove the python std libraries, except not asked to (arg removal_policy)
-
-    Raises
-    ------
-    ArgumentError
-        No input given (arg input) || Invalid repoval policy
-    OSError
-        One of the inputs (arg input) is neither a file, nor a directory
-        (e.g. ~broken symlink ?)
-
-    """
-
-    global parser, DEPENDENCIES, USAGE_MSG, ROOT_DIR, PYPI_MODULES_LIST_FILE_NAME, vprint
-
-    # no args ?
-    if len(sys.argv) == 1:
-        parser.print_help(sys.stderr)
-        sys.exit(1)
-
-    # parse the command line arguments
-    args = vars(parser.parse_args())
+def run(args: dict[str, bool | AnyStr | Iterable[AnyStr]]) -> None:
+    global DEPENDENCIES, USAGE_MSG, ROOT_DIR, PYTHON_STANDARD_MODULES, vprint
 
     # assert input was given
     if not args["input"]:
         raise ArgumentError(f'Missing argument "input" (-i/--input). {USAGE_MSG}')
 
     # validate removal policy
     if args["removal_policy"] < 0 or args["removal_policy"] > 3:
         raise ArgumentError(
             f'Invalid removal policy: {args["removal_policy"]}. {USAGE_MSG}'
         )
 
-    # setup args missng values
+    # setup args missing values
     args["remove_local_imports"] = args["removal_policy"] < 2
 
     # init files & directories
     input_files = list()
     input_directories = list()
 
     # evaluate the paths & check their existence
@@ -937,15 +901,15 @@
         if not os.path.exists(abs_path):
             raise OSError(f'Input path: "{abs_path}" does not exist')
         if os.path.isfile(abs_path):
             input_files.append(abs_path)
         elif os.path.isdir(abs_path):
             input_directories.append(abs_path)
         else:
-            raise OSError(f'Unhandeled object at "{abs_path}"')
+            raise OSError(f'Unhandled object at "{abs_path}"')
 
     # scan the folders
     for folder in input_directories:
         for path, _, files in os.walk(folder):
             filtered_files = fnmatch.filter(files, args["dir_scanning_expr"])
             input_files.extend(map(lambda fn: os.path.join(path, fn), filtered_files))
 
@@ -962,27 +926,27 @@
         vprint("verbose mode")
         vprint(f"args: {args}")
 
     # parse the input files into abstract syntax trees
     vprint()
     vprint("Parsing the files ...")
 
-    file_path_tree_pairs: list[tuple[str & ast.AST]] = list()
+    file_path_tree_pairs: list[tuple[str, ast.AST]] = list()
     for input_file in input_files:
         vprint(f'Parsing tree for: "{input_file}"')
         if as_tree := parse_python_file(input_file):
             file_path_tree_pairs.append((input_file, as_tree))
 
     vprint()
     vprint("Searching for imports ...")
 
     # add all the dependency-sets
     num_pairs = len(file_path_tree_pairs)
     for i in range(num_pairs):
-        vprint(f"Doing AST {i+1}/{num_pairs}")
+        vprint(f"Doing AST {i + 1}/{num_pairs}")
         file_path, as_tree = file_path_tree_pairs[i]
         DEPENDENCIES |= find_file_dependencies(file_path, as_tree, args)
 
     # remove the python stdlib dependencies ?
     if args["removal_policy"] % 2 == 0:
         vprint("Removing imports from the python stdlib")
         global PYTHON_STANDARD_MODULES
@@ -994,10 +958,45 @@
 
     for dep in list(DEPENDENCIES):
         print(dep)
 
     sys.exit(0)
 
 
+def main() -> None:
+    """Main function for the findpydeps script
+
+    Those are the steps by this function :
+     * Parse and validate the command line arguments
+     * Scan the directories that were given, if any
+     * Print the header, unless asked not to
+     * Set up the verbose context
+     * Parse all the input files into trees (AST)
+     * Find all the dependencies (`find_file_dependencies`)
+     * Remove the python std libraries, except not asked to (arg removal_policy)
+
+    Raises
+    ------
+    ArgumentError
+        No input given (arg input) || Invalid removal policy
+    OSError
+        One of the inputs (arg input) is neither a file, nor a directory
+        (e.g. ~broken symlink ?)
+
+    """
+
+    global parser
+
+    # no args ?
+    if len(sys.argv) == 1:
+        parser.print_help(sys.stderr)
+        sys.exit(1)
+
+    # parse the command line arguments
+    args = vars(parser.parse_args())
+
+    run(args)
+
+
 # Used as the main file: run the main function
 if __name__ == "__main__":
     main()
```

### Comparing `findpydeps-0.2.5/src/findpydeps.egg-info/PKG-INFO` & `findpydeps-0.2.6/src/findpydeps.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: findpydeps
-Version: 0.2.5
+Version: 0.2.6
 Summary: Find the python dependencies used by your python files and projects
 Home-page: https://github.com/Nicolas-Reyland/findpydeps
 Author: Nicolas Reyland
 Author-email: nicolas@reyland.dev
 Maintainer: Nicolas Reyland
 Maintainer-email: nicolas@reyland.dev
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/Nicolas-Reyland/findpydeps/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Downloads](https://static.pepy.tech/badge/findpydeps)](https://pepy.tech/project/findpydeps)
+[![Downloads](https://static.pepy.tech/badge/findpydeps/month)](https://pepy.tech/project/findpydeps)
+[![Downloads](https://static.pepy.tech/badge/findpydeps/week)](https://pepy.tech/project/findpydeps)
+
 # findpydeps
 Find the python dependencies used by your python files and projects.
 
 ## Installation
 Simply install it via pip:
 ```bash
 pip install findpydeps
@@ -57,42 +60,44 @@
 cd your_python_project
 findpydeps -i main.py --follow-local-imports > requirements.txt
 pip install -r requirements.txt
 ```
 
 For exhaustive usage information, please refer to the `findpydeps -h` output (or `python3 -m findpydeps -h`) :
 ```
-usage: findpydeps [-h] [-i input [input ...]] [-d expr] [-r policy] [-l] [-s] [--blocks] [--no-blocks] [--functions] [--no-functions] [-v] [--header] [--no-header]
+usage: findpydeps.py [-h] [-i input [input ...]] [-d expr] [-r policy] [-l] [-s] [--blocks] [--no-blocks] [--functions] [--no-functions] [--submodules-as-modules] [-v] [--header]
+                     [--no-header]
 
 Find the python dependencies used by your python files
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -i input [input ...], --input input [input ...]
                         input files and/or directories (directories will be scanned for *.py files)
   -d expr, --dir-scanning-expr expr
                         only process files with this expression in scanned directories [default: *.py]
   -r policy, --removal-policy policy
                         removal policy for modules (0: local & stdlib, 1: local only, 2: stdlib only, 3: no removal) [default: 0]
   -l, --follow-local-imports
-                        follow imports for local files
+                        also scan files which are imported locally (not libraries)
   -s, --strict          raise an error on SyntaxErrors in the input python files
   --blocks              scan contents of 'if', 'try' and 'with' blocks
   --no-blocks           don't scan contents of 'if', 'try' and 'with' blocks
   --functions           scan contents of functions
   --no-functions        don't scan contents of functions
+  --submodules-as-modules
+                        submodule imports are treated as module-imports (e.g. "import random.shuffle" generates "random.shuffle", not "random", which is the default behavior)
   -v, --verbose         verbose mode (all messages prepended with '#')
   --header              show the greeting header
   --no-header           don't show the greeting header
 ```
 
 
 ## Todo
- * Verify package names on pypi.org (check if installable via pip)
- * Exclude/Include custom package names option
+ * Option to manually exclude/include modules
 
 MIT License
 
 Copyright (c) 2021 Nicolas Reyland
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
@@ -107,9 +112,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
-
```

