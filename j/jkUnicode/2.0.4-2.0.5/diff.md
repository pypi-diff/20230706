# Comparing `tmp/jkUnicode-2.0.4.tar.gz` & `tmp/jkUnicode-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jkUnicode-2.0.4.tar", last modified: Tue Jul  4 10:24:31 2023, max compression
+gzip compressed data, was "jkUnicode-2.0.5.tar", last modified: Thu Jul  6 12:46:46 2023, max compression
```

## Comparing `jkUnicode-2.0.4.tar` & `jkUnicode-2.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:31.926380 jkUnicode-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-04 10:24:31.926380 jkUnicode-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:31.914380 jkUnicode-2.0.4/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:31.922380 jkUnicode-2.0.4/lib/jkUnicode/
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/aglfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/aglfnData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:31.922380 jkUnicode-2.0.4/lib/jkUnicode/cmdline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/cmdline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/cmdline/ortho.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/cmdline/uniinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:31.926380 jkUnicode-2.0.4/lib/jkUnicode/json/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/json/ignored_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/json/ignored_languages.json
--rw-r--r--   0 runner    (1001) docker     (123)  1404126 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/json/language_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/json/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/json/scripts.json
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/json/territories.json
--rw-r--r--   0 runner    (1001) docker     (123)    31126 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/orthography.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:31.926380 jkUnicode-2.0.4/lib/jkUnicode/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/tools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/tools/jsonhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/tools/xmlhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)    58924 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniCase.py
--rw-r--r--   0 runner    (1001) docker     (123)   646770 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniCat.py
--rw-r--r--   0 runner    (1001) docker     (123)    54403 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniDecomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)  1478896 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniName.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniNiceName.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniRangesBits.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniScript.py
--rw-r--r--   0 runner    (1001) docker     (123)    74012 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/lib/jkUnicode/uniScriptData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:24:31.922380 jkUnicode-2.0.4/lib/jkUnicode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-04 10:24:31.000000 jkUnicode-2.0.4/lib/jkUnicode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-04 10:24:31.000000 jkUnicode-2.0.4/lib/jkUnicode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:24:31.000000 jkUnicode-2.0.4/lib/jkUnicode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 10:24:31.000000 jkUnicode-2.0.4/lib/jkUnicode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-04 10:24:31.000000 jkUnicode-2.0.4/lib/jkUnicode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 10:24:31.000000 jkUnicode-2.0.4/lib/jkUnicode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:24:31.000000 jkUnicode-2.0.4/lib/jkUnicode.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-04 10:24:31.930380 jkUnicode-2.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-07-04 10:24:13.000000 jkUnicode-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:46.175592 jkUnicode-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-06 12:46:46.175592 jkUnicode-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:46.163592 jkUnicode-2.0.5/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:46.167592 jkUnicode-2.0.5/lib/jkUnicode/
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/aglfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/aglfnData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:46.171592 jkUnicode-2.0.5/lib/jkUnicode/cmdline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/cmdline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/cmdline/ortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/cmdline/uniinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:46.175592 jkUnicode-2.0.5/lib/jkUnicode/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/json/ignored_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/json/ignored_languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1404126 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/json/language_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/json/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/json/scripts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/json/territories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31485 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/orthography.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:46.175592 jkUnicode-2.0.5/lib/jkUnicode/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/tools/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/tools/jsonhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/tools/xmlhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58924 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   646770 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniCat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54403 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniDecomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1478896 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniNiceName.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniRangesBits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74012 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/lib/jkUnicode/uniScriptData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:46:46.171592 jkUnicode-2.0.5/lib/jkUnicode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-06 12:46:46.000000 jkUnicode-2.0.5/lib/jkUnicode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-06 12:46:46.000000 jkUnicode-2.0.5/lib/jkUnicode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:46:46.000000 jkUnicode-2.0.5/lib/jkUnicode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 12:46:46.000000 jkUnicode-2.0.5/lib/jkUnicode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 12:46:46.000000 jkUnicode-2.0.5/lib/jkUnicode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 12:46:46.000000 jkUnicode-2.0.5/lib/jkUnicode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:46:45.000000 jkUnicode-2.0.5/lib/jkUnicode.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-06 12:46:46.175592 jkUnicode-2.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-07-06 12:46:35.000000 jkUnicode-2.0.5/setup.py
```

### Comparing `jkUnicode-2.0.4/LICENSE` & `jkUnicode-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/PKG-INFO` & `jkUnicode-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jkUnicode
-Version: 2.0.4
+Version: 2.0.5
 Summary: Unicode support libraries
 Home-page: https://pypi.org/project/jkUnicode/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Documentation, https://jkunicode.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/jenskutilek/jkUnicode
 Project-URL: Tracker, https://github.com/jenskutilek/jkUnicode/issues
```

### Comparing `jkUnicode-2.0.4/README.md` & `jkUnicode-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/__init__.py` & `jkUnicode-2.0.5/lib/jkUnicode/__init__.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/aglfn.py` & `jkUnicode-2.0.5/lib/jkUnicode/aglfn.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/aglfnData.py` & `jkUnicode-2.0.5/lib/jkUnicode/aglfnData.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/cmdline/ortho.py` & `jkUnicode-2.0.5/lib/jkUnicode/cmdline/ortho.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/cmdline/uniinfo.py` & `jkUnicode-2.0.5/lib/jkUnicode/cmdline/uniinfo.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/json/ignored_languages.json` & `jkUnicode-2.0.5/lib/jkUnicode/json/ignored_languages.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/json/language_characters.json` & `jkUnicode-2.0.5/lib/jkUnicode/json/language_characters.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/json/languages.json` & `jkUnicode-2.0.5/lib/jkUnicode/json/languages.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/json/scripts.json` & `jkUnicode-2.0.5/lib/jkUnicode/json/scripts.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/json/territories.json` & `jkUnicode-2.0.5/lib/jkUnicode/json/territories.json`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/orthography.py` & `jkUnicode-2.0.5/lib/jkUnicode/orthography.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from jkUnicode import UniInfo
 from jkUnicode.tools.jsonhelpers import dict_from_file
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Tuple
+from typing import Any, Dict, FrozenSet, List, Optional, Set, Tuple
 
 
 class Orthography:
     """
     The Orthography object represents an orthography. You usually don't deal
     with this object directly, it is used internally by the
     :py:class:`jkUnicode.orthography.OrthographyInfo` object.
@@ -709,15 +709,15 @@
         ]
 
     def get_almost_supported_punctuation(self) -> List[Orthography]:
         return [
             o for o in self.orthographies if o.almost_supported_punctuation()
         ]
 
-    def get_kern_list(self, include_optional=False) -> Set[Tuple[int, ...]]:
+    def get_kern_list(self, include_optional=False) -> Set[FrozenSet[int]]:
         """
         Return a list of character pairs that may appear in any supported
         orthography for the current cmap.
 
         :param include_optional: Include optional characters.
         :type include_optional: bool
         """
@@ -726,17 +726,29 @@
         m = self.get_supported_orthographies_minimum_inclusive()
         possible_pairs = set()
         for ot in m:
             if include_optional:
                 unicodes = ot.unicodes_base | ot.unicodes_optional
             else:
                 unicodes = ot.unicodes_base
-            ot_pairs = set(itertools.combinations_with_replacement(unicodes, 2))
+            ot_pairs = frozenset(
+                [
+                    frozenset(sorted(list(pair)))
+                    for pair in itertools.combinations_with_replacement(
+                        unicodes, 2
+                    )
+                ]
+            )
             possible_pairs |= ot_pairs
-        # print([(chr(L), chr(R)) for L, R in sorted(possible_pairs)])
+        # for pair in sorted([sorted(p) for p in possible_pairs]):
+        #     try:
+        #         L, R = pair
+        #         print(chr(L), chr(R))
+        #     except ValueError:
+        #         print(chr(next(iter(pair))))
         return possible_pairs
 
     def __len__(self) -> int:
         """
         Return the number of known orthographies.
         """
         return len(self.orthographies)
```

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/tools/helpers.py` & `jkUnicode-2.0.5/lib/jkUnicode/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/tools/jsonhelpers.py` & `jkUnicode-2.0.5/lib/jkUnicode/tools/jsonhelpers.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/tools/xmlhelpers.py` & `jkUnicode-2.0.5/lib/jkUnicode/tools/xmlhelpers.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniBlock.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniBlock.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniBlockData.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniBlockData.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniCase.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniCase.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniCat.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniCat.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniDecomposition.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniDecomposition.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniName.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniName.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniNiceName.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniNiceName.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniRangesBits.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniRangesBits.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode/uniScriptData.py` & `jkUnicode-2.0.5/lib/jkUnicode/uniScriptData.py`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/lib/jkUnicode.egg-info/PKG-INFO` & `jkUnicode-2.0.5/lib/jkUnicode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jkUnicode
-Version: 2.0.4
+Version: 2.0.5
 Summary: Unicode support libraries
 Home-page: https://pypi.org/project/jkUnicode/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Documentation, https://jkunicode.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/jenskutilek/jkUnicode
 Project-URL: Tracker, https://github.com/jenskutilek/jkUnicode/issues
```

### Comparing `jkUnicode-2.0.4/lib/jkUnicode.egg-info/SOURCES.txt` & `jkUnicode-2.0.5/lib/jkUnicode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jkUnicode-2.0.4/setup.cfg` & `jkUnicode-2.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jkUnicode
-version = 2.0.4
+version = 2.0.5
 description = Unicode support libraries
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://pypi.org/project/jkUnicode/
 author = Jens Kutilek
 license = MIT
 license_files = LICENSE
```

