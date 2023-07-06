# Comparing `tmp/bblocks-1.1.0.tar.gz` & `tmp/bblocks-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblocks-1.1.0.tar", max compression
+gzip compressed data, was "bblocks-1.1.1.tar", max compression
```

## Comparing `bblocks-1.1.0.tar` & `bblocks-1.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1074 2023-03-09 10:54:28.197317 bblocks-1.1.0/LICENSE
--rw-r--r--   0        0        0    17113 2023-03-09 10:54:28.197317 bblocks-1.1.0/README.md
--rw-r--r--   0        0        0      138 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/.raw_data/README.md
--rw-r--r--   0        0        0     1223 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/analysis_tools/__init__.py
--rw-r--r--   0        0        0     4421 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/analysis_tools/get.py
--rw-r--r--   0        0        0        0 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/cleaning_tools/__init__.py
--rw-r--r--   0        0        0     7803 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/cleaning_tools/clean.py
--rw-r--r--   0        0        0     5259 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/cleaning_tools/filter.py
--rw-r--r--   0        0        0      573 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/config.py
--rw-r--r--   0        0        0        0 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/dataframe_tools/__init__.py
--rw-r--r--   0        0        0    25590 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/dataframe_tools/add.py
--rw-r--r--   0        0        0     3561 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/dataframe_tools/common.py
--rw-r--r--   0        0        0        0 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/__init__.py
--rw-r--r--   0        0        0     2644 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/common.py
--rw-r--r--   0        0        0      140 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/debt/__init__.py
--rw-r--r--   0        0        0     2518 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/debt/common.py
--rw-r--r--   0        0        0     3298 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/debt/get_data.py
--rw-r--r--   0        0        0     1116 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/debt/settings/debt_service_indicators.json
--rw-r--r--   0        0        0      541 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/debt/settings/debt_stocks_indicators.json
--rw-r--r--   0        0        0   306280 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/debt/settings/ids_indicators.json
--rw-r--r--   0        0        0     9461 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/debt/wb_ids.py
--rw-r--r--   0        0        0     1800 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/fao.py
--rw-r--r--   0        0        0     8253 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/hdr.py
--rw-r--r--   0        0        0     8325 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/ilo.py
--rw-r--r--   0        0        0     7328 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/imf.py
--rw-r--r--   0        0        0     9000 2023-03-09 10:54:28.197317 bblocks-1.1.0/bblocks/import_tools/sdr.py
--rw-r--r--   0        0        0     4200 2023-03-09 10:54:28.201317 bblocks-1.1.0/bblocks/import_tools/settings/aids_indicators.json
--rw-r--r--   0        0        0  2744667 2023-03-09 10:54:28.213317 bblocks-1.1.0/bblocks/import_tools/settings/flourish_geometries.csv
--rw-r--r--   0        0        0     6288 2023-03-09 10:54:28.213317 bblocks-1.1.0/bblocks/import_tools/settings/ids_codes.csv
--rw-r--r--   0        0        0      450 2023-03-09 10:54:28.213317 bblocks-1.1.0/bblocks/import_tools/settings/oecd_codes.csv
--rw-r--r--   0        0        0     9495 2023-03-09 10:54:28.213317 bblocks-1.1.0/bblocks/import_tools/unaids.py
--rw-r--r--   0        0        0      739 2023-03-09 10:54:28.213317 bblocks-1.1.0/bblocks/import_tools/unzip.py
--rw-r--r--   0        0        0     6793 2023-03-09 10:54:28.217317 bblocks-1.1.0/bblocks/import_tools/wfp.py
--rw-r--r--   0        0        0     4675 2023-03-09 10:54:28.217317 bblocks-1.1.0/bblocks/import_tools/who.py
--rw-r--r--   0        0        0     9937 2023-03-09 10:54:28.217317 bblocks-1.1.0/bblocks/import_tools/world_bank.py
--rw-r--r--   0        0        0      571 2023-03-09 10:54:28.217317 bblocks-1.1.0/bblocks/logger.py
--rw-r--r--   0        0        0        0 2023-03-09 10:54:28.217317 bblocks-1.1.0/bblocks/other_tools/__init__.py
--rw-r--r--   0        0        0     1080 2023-03-09 10:54:28.217317 bblocks-1.1.0/bblocks/other_tools/common.py
--rw-r--r--   0        0        0     3951 2023-03-09 10:54:28.217317 bblocks-1.1.0/bblocks/other_tools/dictionaries.py
--rw-r--r--   0        0        0     1234 2023-03-09 10:54:28.217317 bblocks-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    18424 1970-01-01 00:00:00.000000 bblocks-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 12:15:51.080281 bblocks-1.1.1/LICENSE
+-rw-r--r--   0        0        0    17113 2023-07-06 12:15:51.080281 bblocks-1.1.1/README.md
+-rw-r--r--   0        0        0      138 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/.raw_data/README.md
+-rw-r--r--   0        0        0     1223 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/analysis_tools/__init__.py
+-rw-r--r--   0        0        0     4421 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/analysis_tools/get.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0     7803 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/cleaning_tools/clean.py
+-rw-r--r--   0        0        0     5259 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/cleaning_tools/filter.py
+-rw-r--r--   0        0        0      573 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/config.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/dataframe_tools/__init__.py
+-rw-r--r--   0        0        0    25590 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/dataframe_tools/add.py
+-rw-r--r--   0        0        0     3561 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/dataframe_tools/common.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/import_tools/__init__.py
+-rw-r--r--   0        0        0     2644 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/import_tools/common.py
+-rw-r--r--   0        0        0      140 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/import_tools/debt/__init__.py
+-rw-r--r--   0        0        0     2518 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/import_tools/debt/common.py
+-rw-r--r--   0        0        0     3298 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/import_tools/debt/get_data.py
+-rw-r--r--   0        0        0     1116 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/import_tools/debt/settings/debt_service_indicators.json
+-rw-r--r--   0        0        0      541 2023-07-06 12:15:51.080281 bblocks-1.1.1/bblocks/import_tools/debt/settings/debt_stocks_indicators.json
+-rw-r--r--   0        0        0   306280 2023-07-06 12:15:51.084281 bblocks-1.1.1/bblocks/import_tools/debt/settings/ids_indicators.json
+-rw-r--r--   0        0        0     9461 2023-07-06 12:15:51.084281 bblocks-1.1.1/bblocks/import_tools/debt/wb_ids.py
+-rw-r--r--   0        0        0     1800 2023-07-06 12:15:51.084281 bblocks-1.1.1/bblocks/import_tools/fao.py
+-rw-r--r--   0        0        0     8253 2023-07-06 12:15:51.084281 bblocks-1.1.1/bblocks/import_tools/hdr.py
+-rw-r--r--   0        0        0     8325 2023-07-06 12:15:51.084281 bblocks-1.1.1/bblocks/import_tools/ilo.py
+-rw-r--r--   0        0        0     7328 2023-07-06 12:15:51.084281 bblocks-1.1.1/bblocks/import_tools/imf.py
+-rw-r--r--   0        0        0     9000 2023-07-06 12:15:51.084281 bblocks-1.1.1/bblocks/import_tools/sdr.py
+-rw-r--r--   0        0        0     4200 2023-07-06 12:15:51.084281 bblocks-1.1.1/bblocks/import_tools/settings/aids_indicators.json
+-rw-r--r--   0        0        0  2744667 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/import_tools/settings/flourish_geometries.csv
+-rw-r--r--   0        0        0     6288 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/import_tools/settings/ids_codes.csv
+-rw-r--r--   0        0        0      450 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/import_tools/settings/oecd_codes.csv
+-rw-r--r--   0        0        0     9495 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/import_tools/unaids.py
+-rw-r--r--   0        0        0      739 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/import_tools/unzip.py
+-rw-r--r--   0        0        0     6793 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/import_tools/wfp.py
+-rw-r--r--   0        0        0     4675 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/import_tools/who.py
+-rw-r--r--   0        0        0     9937 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/import_tools/world_bank.py
+-rw-r--r--   0        0        0      571 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/logger.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/other_tools/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/other_tools/common.py
+-rw-r--r--   0        0        0     3951 2023-07-06 12:15:51.100281 bblocks-1.1.1/bblocks/other_tools/dictionaries.py
+-rw-r--r--   0        0        0     1228 2023-07-06 12:15:51.100281 bblocks-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    18313 1970-01-01 00:00:00.000000 bblocks-1.1.1/PKG-INFO
```

### Comparing `bblocks-1.1.0/LICENSE` & `bblocks-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/README.md` & `bblocks-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/__init__.py` & `bblocks-1.1.1/bblocks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 # Easy access to importers
 from bblocks.import_tools.world_bank import WorldBankData
 from bblocks.import_tools.who import GHED
 from bblocks.import_tools.wfp import WFPData
 from bblocks.import_tools.imf import WorldEconomicOutlook
 from bblocks.import_tools.unaids import Aids
```

### Comparing `bblocks-1.1.0/bblocks/analysis_tools/get.py` & `bblocks-1.1.1/bblocks/analysis_tools/get.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/cleaning_tools/clean.py` & `bblocks-1.1.1/bblocks/cleaning_tools/clean.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/cleaning_tools/filter.py` & `bblocks-1.1.1/bblocks/cleaning_tools/filter.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/config.py` & `bblocks-1.1.1/bblocks/config.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/dataframe_tools/add.py` & `bblocks-1.1.1/bblocks/dataframe_tools/add.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/dataframe_tools/common.py` & `bblocks-1.1.1/bblocks/dataframe_tools/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/common.py` & `bblocks-1.1.1/bblocks/import_tools/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/debt/common.py` & `bblocks-1.1.1/bblocks/import_tools/debt/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/debt/get_data.py` & `bblocks-1.1.1/bblocks/import_tools/debt/get_data.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/debt/settings/debt_service_indicators.json` & `bblocks-1.1.1/bblocks/import_tools/debt/settings/debt_service_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/debt/settings/debt_stocks_indicators.json` & `bblocks-1.1.1/bblocks/import_tools/debt/settings/debt_stocks_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/debt/settings/ids_indicators.json` & `bblocks-1.1.1/bblocks/import_tools/debt/settings/ids_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/debt/wb_ids.py` & `bblocks-1.1.1/bblocks/import_tools/debt/wb_ids.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/fao.py` & `bblocks-1.1.1/bblocks/import_tools/fao.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/hdr.py` & `bblocks-1.1.1/bblocks/import_tools/hdr.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/ilo.py` & `bblocks-1.1.1/bblocks/import_tools/ilo.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/imf.py` & `bblocks-1.1.1/bblocks/import_tools/imf.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/sdr.py` & `bblocks-1.1.1/bblocks/import_tools/sdr.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/settings/aids_indicators.json` & `bblocks-1.1.1/bblocks/import_tools/settings/aids_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/settings/flourish_geometries.csv` & `bblocks-1.1.1/bblocks/import_tools/settings/flourish_geometries.csv`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/settings/ids_codes.csv` & `bblocks-1.1.1/bblocks/import_tools/settings/ids_codes.csv`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/unaids.py` & `bblocks-1.1.1/bblocks/import_tools/unaids.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/unzip.py` & `bblocks-1.1.1/bblocks/import_tools/unzip.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/wfp.py` & `bblocks-1.1.1/bblocks/import_tools/wfp.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/who.py` & `bblocks-1.1.1/bblocks/import_tools/who.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/import_tools/world_bank.py` & `bblocks-1.1.1/bblocks/import_tools/world_bank.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/logger.py` & `bblocks-1.1.1/bblocks/logger.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/other_tools/common.py` & `bblocks-1.1.1/bblocks/other_tools/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/bblocks/other_tools/dictionaries.py` & `bblocks-1.1.1/bblocks/other_tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.1.0/pyproject.toml` & `bblocks-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblocks"
-version = "1.1.0"
+version = "1.1.1"
 description = "A package with tools to download and analyse international development data. These tools are meant to be the building blocks of further analysis."
 authors = ["The ONE Campaign <data@one.org>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
@@ -17,22 +17,22 @@
     { include = "bblocks" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^1.5.3"
 numpy = "^1.24.1"
-country-converter = "^0.8.0"
+country-converter = "^1.0"
 openpyxl = "^3.0.10"
 requests = "^2.28.2"
 opencv-python = "^4.7.0"
 weo = "^0.7.4"
-beautifulsoup4 = "^4.11.1"
+beautifulsoup4 = "^4.12"
 pyjstat = "^2.3.0"
-pyarrow = "^11.0.0"
+pyarrow = "^12.0"
 wbgapi = "<1.1"
 PyPDF2 = "^2"
 camelot-py = "^0.10.1"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 black = "^22.12.0"
```

### Comparing `bblocks-1.1.0/PKG-INFO` & `bblocks-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: bblocks
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package with tools to download and analyse international development data. These tools are meant to be the building blocks of further analysis.
 License: MIT
 Author: The ONE Campaign
 Author-email: data@one.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyPDF2 (>=2,<3)
-Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12,<5.0)
 Requires-Dist: camelot-py (>=0.10.1,<0.11.0)
-Requires-Dist: country-converter (>=0.8.0,<0.9.0)
+Requires-Dist: country-converter (>=1.0,<2.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: pyarrow (>=12.0,<13.0)
 Requires-Dist: pyjstat (>=2.3.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: wbgapi (<1.1)
 Requires-Dist: weo (>=0.7.4,<0.8.0)
 Description-Content-Type: text/markdown
 
 [![pypi](https://img.shields.io/pypi/v/bblocks.svg)](https://pypi.org/project/bblocks/)
```

