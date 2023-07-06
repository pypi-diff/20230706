# Comparing `tmp/fnum-0.2.0-py3-none-any.whl.zip` & `tmp/fnum-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16087 bytes, number of entries: 10
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 03:45 fnum/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-06 03:45 fnum/__main__.py
--rw-r--r--  2.0 unx     2235 b- defN 23-Jul-06 03:45 fnum/actions.py
--rw-r--r--  2.0 unx     1793 b- defN 23-Jul-06 03:45 fnum/cli.py
--rw-r--r--  2.0 unx    35141 b- defN 23-Jul-06 03:45 fnum-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1043 b- defN 23-Jul-06 03:45 fnum-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 03:45 fnum-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-06 03:45 fnum-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-06 03:45 fnum-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      745 b- defN 23-Jul-06 03:45 fnum-0.2.0.dist-info/RECORD
-10 files, 41173 bytes uncompressed, 14827 bytes compressed:  64.0%
+Zip file size: 16086 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 03:51 fnum/__init__.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-06 03:51 fnum/__main__.py
+-rw-r--r--  2.0 unx     2235 b- defN 23-Jul-06 03:51 fnum/actions.py
+-rw-r--r--  2.0 unx     1793 b- defN 23-Jul-06 03:51 fnum/cli.py
+-rw-r--r--  2.0 unx    35141 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1043 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      745 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/RECORD
+10 files, 41173 bytes uncompressed, 14826 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: fnum/actions.py
 Comment: 
 
 Filename: fnum/cli.py
 Comment: 
 
-Filename: fnum-0.2.0.dist-info/LICENSE
+Filename: fnum-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-0.2.0.dist-info/METADATA
+Filename: fnum-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: fnum-0.2.0.dist-info/WHEEL
+Filename: fnum-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-0.2.0.dist-info/entry_points.txt
+Filename: fnum-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-0.2.0.dist-info/top_level.txt
+Filename: fnum-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-0.2.0.dist-info/RECORD
+Filename: fnum-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0"
+__version__ = "1.0.0"
```

## Comparing `fnum-0.2.0.dist-info/LICENSE` & `fnum-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-0.2.0.dist-info/METADATA` & `fnum-1.0.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 0.2.0
+Version: 1.0.0
 Summary: Renames files in a directory to be named using sequential integers starting with 1
 Author-email: Matt Wisniewski <fnum@mattw.life>
 License: GPLv3
 Project-URL: homepage, https://github.com/polishmatt/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

## Comparing `fnum-0.2.0.dist-info/RECORD` & `fnum-1.0.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-fnum/__init__.py,sha256=Zn1KFblwuFHiDRdRAiRnDBRkbPttWh44jKa5zG2ov0E,22
+fnum/__init__.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
 fnum/__main__.py,sha256=8hDtWlaFZK24KhfNq_ZKgtXqYHsDQDetukOCMlsbW0Q,59
 fnum/actions.py,sha256=e2UoyzOpnJ4xwLrzElSfxEb0InoiwZx03c-yg3ehoQA,2235
 fnum/cli.py,sha256=4kvhG47vsJKIFWjpBKr2ZNPsnpHyVrEI_xwhUMEdPPY,1793
-fnum-0.2.0.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
-fnum-0.2.0.dist-info/METADATA,sha256=PjZwMHqoIxRMz1tWn_VI2ihe2WboiwQSXBmVjl-zeLI,1043
-fnum-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fnum-0.2.0.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
-fnum-0.2.0.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
-fnum-0.2.0.dist-info/RECORD,,
+fnum-1.0.0.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
+fnum-1.0.0.dist-info/METADATA,sha256=fj4H_F8RHrVoQ13LgOwBne9CmdBtoH3FqkQ8fwGZGQk,1043
+fnum-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fnum-1.0.0.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
+fnum-1.0.0.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
+fnum-1.0.0.dist-info/RECORD,,
```

