# Comparing `tmp/querychart_package-1.0.4.tar.gz` & `tmp/querychart_package-2.0.0.tar.gz`

## Comparing `querychart_package-1.0.4.tar` & `querychart_package-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-1.0.4/src/querychart_package/.schemawiz_config3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 querychart_package-1.0.4/src/querychart_package/__init__.py
--rw-r--r--   0        0        0    81920 2020-02-02 00:00:00.000000 querychart_package-1.0.4/src/querychart_package/local_sqlite_db
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 querychart_package-1.0.4/src/querychart_package/querychart.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-1.0.4/src/querychart_package/sales.csv
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-1.0.4/src/querychart_package/widesales.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-1.0.4/tests/.schemawiz_config3
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 querychart_package-1.0.4/tests/chart_csv_columns.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 querychart_package-1.0.4/tests/chart_csv_rows.py
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 querychart_package-1.0.4/tests/local_sqlite_db
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-1.0.4/tests/sales.csv
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-1.0.4/tests/widesales.csv
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 querychart_package-1.0.4/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 querychart_package-1.0.4/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 querychart_package-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 querychart_package-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 querychart_package-2.0.0/test.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/.schemawiz_config3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/data.csv
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/fieldcounts.tsv
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/gant_data.csv
+-rw-r--r--   0        0        0    11206 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/ganter.py
+-rw-r--r--   0        0        0   180224 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/local_sqlite_db
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/plan.xlsx
+-rw-r--r--   0        0        0    14251 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/querychart.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/sales.csv
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/sampledata.csv
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.0/src/querychart_package/widesales.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.0/tests/.schemawiz_config3
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 querychart_package-2.0.0/tests/chart_csv_columns.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 querychart_package-2.0.0/tests/chart_csv_rows.py
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 querychart_package-2.0.0/tests/local_sqlite_db
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.0/tests/sales.csv
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.0/tests/widesales.csv
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 querychart_package-2.0.0/.gitignore
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 querychart_package-2.0.0/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 querychart_package-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 querychart_package-2.0.0/PKG-INFO
```

### Comparing `querychart_package-1.0.4/src/querychart_package/sales.csv` & `querychart_package-2.0.0/src/querychart_package/sales.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-1.0.4/tests/local_sqlite_db` & `querychart_package-2.0.0/tests/local_sqlite_db`

 * *Format-specific differences are supported for SQLite databases but no file-specific differences were detected; falling back to a binary diff. file(1) reports: SQLite 3.x database, last written using SQLite version 3038004, file counter 23, database pages 3, 1st free page 3, free pages 1, cookie 0xb, schema 4, UTF-8, version-valid-for 23*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5351 4c69 7465 2066 6f72 6d61 7420 3300  SQLite format 3.
-00000010: 1000 0101 0040 2020 0000 0017 0000 0003  .....@  ........
-00000020: 0000 0003 0000 0001 0000 000b 0000 0004  ................
+00000010: 1000 0101 0040 2020 0000 0023 0000 0003  .....@  ...#....
+00000020: 0000 0003 0000 0001 0000 0011 0000 0004  ................
 00000030: 0000 0000 0000 0000 0000 0001 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0000 0000 0000 0000 0000 0017  ................
+00000050: 0000 0000 0000 0000 0000 0000 0000 0023  ...............#
 00000060: 002e 5b34 0d00 0000 010f 0000 0f00 0df0  ..[4............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -219,18 +219,18 @@
 00000da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000df0: 0000 0110 1731 3101 8345 7461 626c 6574  .....11..Etablet
 00000e00: 626c 6373 765f 3230 3233 3034 3231 3035  blcsv_2023042105
-00000e10: 3174 626c 6373 765f 3230 3233 3034 3231  1tblcsv_20230421
-00000e20: 3035 3103 4352 4541 5445 2054 4142 4c45  051.CREATE TABLE
+00000e10: 3874 626c 6373 765f 3230 3233 3034 3231  8tblcsv_20230421
+00000e20: 3035 3803 4352 4541 5445 2054 4142 4c45  058.CREATE TABLE
 00000e30: 2074 626c 6373 765f 3230 3233 3034 3231   tblcsv_20230421
-00000e40: 3035 3128 0a09 6c65 6765 6e64 2074 6578  051(..legend tex
+00000e40: 3035 3828 0a09 6c65 6765 6e64 2074 6578  058(..legend tex
 00000e50: 7420 0909 2f2a 2065 672e 2063 6f73 7420  t ../* eg. cost 
 00000e60: 2a2f 202c 0a09 2232 3032 332f 3033 2f32  */ ,.."2023/03/2
 00000e70: 3922 2072 6561 6c20 0909 2f2a 2065 672e  9" real ../* eg.
 00000e80: 2038 2e35 3520 2a2f 202c 0a09 2232 3032   8.55 */ ,.."202
 00000e90: 332f 3033 2f33 3022 2072 6561 6c20 0909  3/03/30" real ..
 00000ea0: 2f2a 2065 672e 2031 382e 3435 202a 2f20  /* eg. 18.45 */ 
 00000eb0: 2c0a 0922 3230 3233 2f30 332f 3331 2220  ,.."2023/03/31"
```

### Comparing `querychart_package-1.0.4/tests/sales.csv` & `querychart_package-2.0.0/tests/sales.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-1.0.4/pyproject.toml` & `querychart_package-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","schemawizard_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "querychart_package"
-version = "1.0.4"
+version = "2.0.0"
 dependencies = [
   'schemawizard_package >= 2.3.5'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
 description = "A wrapper for simplified matplotlib usage"
```

### Comparing `querychart_package-1.0.4/PKG-INFO` & `querychart_package-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querychart_package
-Version: 1.0.4
+Version: 2.0.0
 Summary: A wrapper for simplified matplotlib usage
 Project-URL: Homepage, https://github.com/daveskura/querychart
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -16,13 +16,9 @@
 sql graphs based on matplotlib
 
 ## install matplotlib
 ```
 pip install matplotlib
 ```
 
-
-
-
-
 ### marker ref 
 https://www.w3schools.com/python/matplotlib_markers.asp
```

