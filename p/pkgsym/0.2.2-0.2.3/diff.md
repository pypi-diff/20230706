# Comparing `tmp/pkgsym-0.2.2.tar.gz` & `tmp/pkgsym-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgsym-0.2.2.tar", last modified: Thu Feb  9 19:54:31 2023, max compression
+gzip compressed data, was "pkgsym-0.2.3.tar", last modified: Thu Jul  6 18:28:23 2023, max compression
```

## Comparing `pkgsym-0.2.2.tar` & `pkgsym-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 qyriad    (1000) qyriad    (1000)        0 2023-02-09 19:54:31.803278 pkgsym-0.2.2/
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)     1072 2023-02-07 19:02:18.000000 pkgsym-0.2.2/LICENSE.txt
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)     3076 2023-02-09 19:54:31.803278 pkgsym-0.2.2/PKG-INFO
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)     2794 2023-02-07 19:02:18.000000 pkgsym-0.2.2/README.md
-drwxr-xr-x   0 qyriad    (1000) qyriad    (1000)        0 2023-02-09 19:54:31.799945 pkgsym-0.2.2/pkgsym/
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)     9656 2023-02-07 19:09:58.000000 pkgsym-0.2.2/pkgsym/__init__.py
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)       49 2023-02-07 19:02:18.000000 pkgsym-0.2.2/pkgsym/__main__.py
-drwxr-xr-x   0 qyriad    (1000) qyriad    (1000)        0 2023-02-09 19:54:31.803278 pkgsym-0.2.2/pkgsym.egg-info/
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)     3076 2023-02-09 19:54:31.000000 pkgsym-0.2.2/pkgsym.egg-info/PKG-INFO
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)      237 2023-02-09 19:54:31.000000 pkgsym-0.2.2/pkgsym.egg-info/SOURCES.txt
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)        1 2023-02-09 19:54:31.000000 pkgsym-0.2.2/pkgsym.egg-info/dependency_links.txt
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)       39 2023-02-09 19:54:31.000000 pkgsym-0.2.2/pkgsym.egg-info/entry_points.txt
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)        7 2023-02-09 19:54:31.000000 pkgsym-0.2.2/pkgsym.egg-info/top_level.txt
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)       90 2023-02-07 19:02:18.000000 pkgsym-0.2.2/pyproject.toml
--rw-r--r--   0 qyriad    (1000) qyriad    (1000)      390 2023-02-09 19:54:31.803278 pkgsym-0.2.2/setup.cfg
+drwxr-xr-x   0 qyriad    (1000) users      (985)        0 2023-07-06 18:28:23.913973 pkgsym-0.2.3/
+-rw-r--r--   0 qyriad    (1000) users      (985)     1072 2023-07-06 12:37:04.000000 pkgsym-0.2.3/LICENSE.txt
+-rw-r--r--   0 qyriad    (1000) users      (985)     3076 2023-07-06 18:28:23.913973 pkgsym-0.2.3/PKG-INFO
+-rw-r--r--   0 qyriad    (1000) users      (985)     2794 2023-07-06 12:37:04.000000 pkgsym-0.2.3/README.md
+drwxr-xr-x   0 qyriad    (1000) users      (985)        0 2023-07-06 18:28:23.913973 pkgsym-0.2.3/pkgsym/
+-rw-r--r--   0 qyriad    (1000) users      (985)     9776 2023-07-06 18:17:12.000000 pkgsym-0.2.3/pkgsym/__init__.py
+-rw-r--r--   0 qyriad    (1000) users      (985)       49 2022-09-28 05:01:13.000000 pkgsym-0.2.3/pkgsym/__main__.py
+drwxr-xr-x   0 qyriad    (1000) users      (985)        0 2023-07-06 18:28:23.913973 pkgsym-0.2.3/pkgsym.egg-info/
+-rw-r--r--   0 qyriad    (1000) users      (985)     3076 2023-07-06 18:28:23.000000 pkgsym-0.2.3/pkgsym.egg-info/PKG-INFO
+-rw-r--r--   0 qyriad    (1000) users      (985)      237 2023-07-06 18:28:23.000000 pkgsym-0.2.3/pkgsym.egg-info/SOURCES.txt
+-rw-r--r--   0 qyriad    (1000) users      (985)        1 2023-07-06 18:28:23.000000 pkgsym-0.2.3/pkgsym.egg-info/dependency_links.txt
+-rw-r--r--   0 qyriad    (1000) users      (985)       39 2023-07-06 18:28:23.000000 pkgsym-0.2.3/pkgsym.egg-info/entry_points.txt
+-rw-r--r--   0 qyriad    (1000) users      (985)        7 2023-07-06 18:28:23.000000 pkgsym-0.2.3/pkgsym.egg-info/top_level.txt
+-rw-r--r--   0 qyriad    (1000) users      (985)       90 2022-09-28 05:01:13.000000 pkgsym-0.2.3/pyproject.toml
+-rw-r--r--   0 qyriad    (1000) users      (985)      390 2023-07-06 18:28:23.913973 pkgsym-0.2.3/setup.cfg
```

### Comparing `pkgsym-0.2.2/LICENSE.txt` & `pkgsym-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkgsym-0.2.2/PKG-INFO` & `pkgsym-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgsym
-Version: 0.2.2
+Version: 0.2.3
 Summary: Poor man's package manager (like brew link without the brew)
 Home-page: https://github.com/Qyriad/pkgsym
 Author: Mikaela Szekely
 Author-email: mikaela.szekely@qyriad.me
 License: MIT
 Platform: any
 License-File: LICENSE.txt
```

### Comparing `pkgsym-0.2.2/README.md` & `pkgsym-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pkgsym-0.2.2/pkgsym/__init__.py` & `pkgsym-0.2.3/pkgsym/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import errno
 import argparse
 import itertools
 import traceback
 from dataclasses import dataclass
 from typing import Tuple, List
 
+VERSION = "0.2.3"
+
 
 HOME_DIR = os.path.expanduser('~')
 DEFAULT_PREFIX = os.path.join(HOME_DIR, '.local')
 DEFAULT_OPT = "opt"
 
 
 @dataclass
@@ -178,15 +180,16 @@
 
 
     return (symlink_operations, directory_operations)
 
 
 def main():
 
-    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser = argparse.ArgumentParser(prog='pkgsym', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('--version', action='version', version=f'%(prog)s {VERSION}')
     parser.add_argument('action', choices=['link', 'unlink'],
         help="Link or unlink a package under the self-contained directory to the prefix",
     )
     parser.add_argument('package', action='store', type=str,
         help="The package name to link or unlink -- should be the directory under $prefix/opt that contains the package",
     )
     parser.add_argument('--prefix', type=str, default=DEFAULT_PREFIX,
```

### Comparing `pkgsym-0.2.2/pkgsym.egg-info/PKG-INFO` & `pkgsym-0.2.3/pkgsym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgsym
-Version: 0.2.2
+Version: 0.2.3
 Summary: Poor man's package manager (like brew link without the brew)
 Home-page: https://github.com/Qyriad/pkgsym
 Author: Mikaela Szekely
 Author-email: mikaela.szekely@qyriad.me
 License: MIT
 Platform: any
 License-File: LICENSE.txt
```

