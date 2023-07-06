# Comparing `tmp/proteus_preprocessing-0.2.9.tar.gz` & `tmp/proteus_preprocessing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_preprocessing-0.2.9.tar", max compression
+gzip compressed data, was "proteus_preprocessing-0.3.0.tar", max compression
```

## Comparing `proteus_preprocessing-0.2.9.tar` & `proteus_preprocessing-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       43 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/deck/__init__.py
--rw-r--r--   0        0        0      909 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/deck/ecl_deck.py
--rw-r--r--   0        0        0     8550 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/deck/runspec.py
--rw-r--r--   0        0        0     4028 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/deck/section.py
--rw-r--r--   0        0        0        0 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/modular/__init__.py
--rw-r--r--   0        0        0      594 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/modular/dat.py
--rw-r--r--   0        0        0    16684 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/modular/data.py
--rw-r--r--   0        0        0      415 2023-03-15 15:25:43.097318 proteus_preprocessing-0.2.9/preprocessing/modular/egrid.py
--rw-r--r--   0        0        0      365 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/modular/grdecl.py
--rw-r--r--   0        0        0     2123 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/modular/init.py
--rw-r--r--   0        0        0     5402 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/modular/s.py
--rw-r--r--   0        0        0      178 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/modular/x.py
--rw-r--r--   0        0        0      221 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/patches.py
--rw-r--r--   0        0        0       71 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/utils/__init__.py
--rw-r--r--   0        0        0     1062 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/utils/expand_dates.py
--rw-r--r--   0        0        0      901 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/preprocessing/utils/expand_wcon.py
--rw-r--r--   0        0        0     1513 2023-03-15 15:25:43.101318 proteus_preprocessing-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 proteus_preprocessing-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-07-06 16:07:26.456689 proteus_preprocessing-0.3.0/preprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:07:26.456689 proteus_preprocessing-0.3.0/preprocessing/deck/__init__.py
+-rw-r--r--   0        0        0      909 2023-07-06 16:07:26.456689 proteus_preprocessing-0.3.0/preprocessing/deck/ecl_deck.py
+-rw-r--r--   0        0        0     8837 2023-07-06 16:07:26.456689 proteus_preprocessing-0.3.0/preprocessing/deck/runspec.py
+-rw-r--r--   0        0        0     2999 2023-07-06 16:07:26.456689 proteus_preprocessing-0.3.0/preprocessing/deck/section.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/modular/__init__.py
+-rw-r--r--   0        0        0      548 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/modular/dat.py
+-rw-r--r--   0        0        0    16684 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/modular/data.py
+-rw-r--r--   0        0        0      415 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/modular/egrid.py
+-rw-r--r--   0        0        0      365 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/modular/grdecl.py
+-rw-r--r--   0        0        0     2123 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/modular/init.py
+-rw-r--r--   0        0        0     5402 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/modular/s.py
+-rw-r--r--   0        0        0      178 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/modular/x.py
+-rw-r--r--   0        0        0      221 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/patches.py
+-rw-r--r--   0        0        0       71 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/utils/__init__.py
+-rw-r--r--   0        0        0     1062 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/utils/expand_dates.py
+-rw-r--r--   0        0        0      901 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/preprocessing/utils/expand_wcon.py
+-rw-r--r--   0        0        0     1526 2023-07-06 16:07:26.460689 proteus_preprocessing-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 proteus_preprocessing-0.3.0/PKG-INFO
```

### Comparing `proteus_preprocessing-0.2.9/preprocessing/deck/ecl_deck.py` & `proteus_preprocessing-0.3.0/preprocessing/deck/ecl_deck.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.9/preprocessing/deck/runspec.py` & `proteus_preprocessing-0.3.0/preprocessing/deck/runspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from functools import reduce
 
 import numpy as np
 from ecl.eclfile import EclInitFile, EclKW
 from ecl.grid import EclGrid
 from ecl.summary import EclSum
 from ecl2df import EclFiles
-from preprocessing.deck.section import get_includes
+
+from preprocessing.deck.section import find_includes
 from preprocessing.modular.data import WellSpecsProcessor
 
 SMSPEC_WELL_KEYWORDS = {
     "WOPR",
     "WOPRH",
     "WWPR",
     "WWPRH",
@@ -24,22 +25,21 @@
     "WWIRH",
 }
 SMSPEC_FIELD_KEYWORDS = ["FOPR", "FWPR", "FGPR", "FOPRH", "FWPRH", "FGPRH"]
 
 
 def preprocess(
     data_file_loc,
-    egrid_file_loc=None,
-    smspec_file_loc=None,
-    init_file_loc=None,
-    download_func=None,
+    egrid_file_loc,
+    smspec_file_loc,
+    init_file_loc,
+    download_func,
     allow_missing_files=tuple(),
-    base_dir=None,
 ):
-    get_includes(data_file_loc, download_func, allow_missing_files=allow_missing_files, base_dir=base_dir)
+    find_includes(data_file_loc, download_func, allow_missing_files=allow_missing_files)
 
     preprocessor = WellSpecsProcessor(data_file_loc)
     data = preprocessor.process()
 
     if smspec_file_loc:
         smry = EclSum(str(smspec_file_loc))
         wnames = OrderedDict((wname, {"injector": None, "type": None}) for wname in smry.wells())
@@ -89,20 +89,21 @@
         field_keywords = set(SMSPEC_FIELD_KEYWORDS).intersection(list(smry))
 
     else:
         wnames = {}
         extractor_keywords = []
         injector_keywords = []
         field_keywords = []
+        smry = None
 
     def get_ecl(data):
         import opm.io
         from pathlib import Path
 
-        section_list = [opm.io.parser.eclSectionType.SCHEDULE]
+        section_list = [opm.io.parser.eclSectionType.SCHEDULE, opm.io.parser.eclSectionType.GRID]
 
         if Path(data._eclbase + ".DATA").is_file():
             deckfile = data._eclbase + ".DATA"
         else:
             deckfile = data._eclbase
         builtin = opm.io.Builtin()
 
@@ -181,14 +182,15 @@
         init_keywords = sorted(set(x.name for x in init if isinstance(x, EclKW)))
     else:
         init_keywords = []
 
     return {
         "phases": preprocess_phases(ecldeck),
         "start": preprocess_start(ecldeck),
+        "timestep": preprocess_timestep(smry),
         "endscale": find_keyword(ecldeck, "ENDSCALE"),
         "multout": find_keyword(ecldeck, "MULTOUT"),
         "dimens": preprocess_dimens(ecldeck),
         "wnames": wnames,
         "wkeywords": {"injector": injector_keywords, "extractor": extractor_keywords},
         "fkeywords": sorted(field_keywords),
         "data_keywords": data_keywords,
@@ -202,14 +204,25 @@
     try:
         start = str(ecldeck["START"][0]).strip(" \n/")
         return datetime.strptime(start, "%d '%b' %Y")
     except Exception:
         return False
 
 
+def preprocess_timestep(smry):
+    from datetime import timedelta
+
+    try:
+        data = smry["TIMESTEP"]
+        unit = data.unit.lower()
+        return timedelta(**{unit: int(data[0].value)})
+    except Exception:
+        return None
+
+
 def preprocess_phases(ecldeck):
     return {
         "gas": find_keyword(ecldeck, "GAS"),
         "oil": find_keyword(ecldeck, "OIL"),
         "water": find_keyword(ecldeck, "WATER"),
     }
```

### Comparing `proteus_preprocessing-0.2.9/preprocessing/modular/data.py` & `proteus_preprocessing-0.3.0/preprocessing/modular/data.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.9/preprocessing/modular/init.py` & `proteus_preprocessing-0.3.0/preprocessing/modular/init.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.9/preprocessing/modular/s.py` & `proteus_preprocessing-0.3.0/preprocessing/modular/s.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.9/preprocessing/utils/expand_dates.py` & `proteus_preprocessing-0.3.0/preprocessing/utils/expand_dates.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.9/preprocessing/utils/expand_wcon.py` & `proteus_preprocessing-0.3.0/preprocessing/utils/expand_wcon.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.2.9/pyproject.toml` & `proteus_preprocessing-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-preprocessing"
-version = "0.2.9"
+version = "0.3.0"
 description = ""
 authors = []
 packages = [
     { include = "preprocessing/modular" },
     { include = "preprocessing/deck" },
     { include = "preprocessing/utils" },
     { include = "preprocessing/patches.py" },
@@ -13,18 +13,19 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-json-logger = "^2.0.1"
 tqdm = "^4.61.0"
 tabulate = "^0.8.9"
 readchar = "^3.0.4"
-libecl = "^2.13.1"
+libecl = "2.13.2"
 h5py = "^3.6.0"
 pandas = "^1.4.1"
-ecl2df = "^0.16.1"
+ecl2df = "0.16.1"
+opm = "2022.4"
 tables = "^3.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pre-commit = "^2.9.3"
 poethepoet = "^0.16.0"
 black = "^22.6.0"
```

### Comparing `proteus_preprocessing-0.2.9/PKG-INFO` & `proteus_preprocessing-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: proteus-preprocessing
-Version: 0.2.9
+Version: 0.3.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ecl2df (>=0.16.1,<0.17.0)
+Requires-Dist: ecl2df (==0.16.1)
 Requires-Dist: h5py (>=3.6.0,<4.0.0)
-Requires-Dist: libecl (>=2.13.1,<3.0.0)
+Requires-Dist: libecl (==2.13.2)
+Requires-Dist: opm (==2022.4)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Requires-Dist: python-json-logger (>=2.0.1,<3.0.0)
 Requires-Dist: readchar (>=3.0.4,<4.0.0)
 Requires-Dist: tables (>=3.7.0,<4.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: tqdm (>=4.61.0,<5.0.0)
```

