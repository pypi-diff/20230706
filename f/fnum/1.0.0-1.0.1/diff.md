# Comparing `tmp/fnum-1.0.0-py3-none-any.whl.zip` & `tmp/fnum-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16086 bytes, number of entries: 10
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 03:51 fnum/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-06 03:51 fnum/__main__.py
--rw-r--r--  2.0 unx     2235 b- defN 23-Jul-06 03:51 fnum/actions.py
--rw-r--r--  2.0 unx     1793 b- defN 23-Jul-06 03:51 fnum/cli.py
--rw-r--r--  2.0 unx    35141 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1043 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      745 b- defN 23-Jul-06 03:51 fnum-1.0.0.dist-info/RECORD
-10 files, 41173 bytes uncompressed, 14826 bytes compressed:  64.0%
+Zip file size: 16095 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 03:58 fnum/__init__.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-06 03:58 fnum/__main__.py
+-rw-r--r--  2.0 unx     2235 b- defN 23-Jul-06 03:58 fnum/actions.py
+-rw-r--r--  2.0 unx     1793 b- defN 23-Jul-06 03:58 fnum/cli.py
+-rw-r--r--  2.0 unx    35141 b- defN 23-Jul-06 03:58 fnum-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1055 b- defN 23-Jul-06 03:58 fnum-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 03:58 fnum-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-06 03:58 fnum-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-06 03:58 fnum-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      745 b- defN 23-Jul-06 03:58 fnum-1.0.1.dist-info/RECORD
+10 files, 41185 bytes uncompressed, 14835 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: fnum/actions.py
 Comment: 
 
 Filename: fnum/cli.py
 Comment: 
 
-Filename: fnum-1.0.0.dist-info/LICENSE
+Filename: fnum-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.0.0.dist-info/METADATA
+Filename: fnum-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.0.0.dist-info/WHEEL
+Filename: fnum-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.0.0.dist-info/entry_points.txt
+Filename: fnum-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.0.0.dist-info/top_level.txt
+Filename: fnum-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.0.0.dist-info/RECORD
+Filename: fnum-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

## Comparing `fnum-1.0.0.dist-info/LICENSE` & `fnum-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.0.0.dist-info/METADATA` & `fnum-1.0.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.0.0
+Version: 1.0.1
 Summary: Renames files in a directory to be named using sequential integers starting with 1
 Author-email: Matt Wisniewski <fnum@mattw.life>
 License: GPLv3
 Project-URL: homepage, https://github.com/polishmatt/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `fnum-1.0.0.dist-info/RECORD` & `fnum-1.0.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-fnum/__init__.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
+fnum/__init__.py,sha256=d4QHYmS_30j0hPN8NmNPnQ_Z0TphDRbu4MtQj9cT9e8,22
 fnum/__main__.py,sha256=8hDtWlaFZK24KhfNq_ZKgtXqYHsDQDetukOCMlsbW0Q,59
 fnum/actions.py,sha256=e2UoyzOpnJ4xwLrzElSfxEb0InoiwZx03c-yg3ehoQA,2235
 fnum/cli.py,sha256=4kvhG47vsJKIFWjpBKr2ZNPsnpHyVrEI_xwhUMEdPPY,1793
-fnum-1.0.0.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
-fnum-1.0.0.dist-info/METADATA,sha256=fj4H_F8RHrVoQ13LgOwBne9CmdBtoH3FqkQ8fwGZGQk,1043
-fnum-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fnum-1.0.0.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
-fnum-1.0.0.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
-fnum-1.0.0.dist-info/RECORD,,
+fnum-1.0.1.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
+fnum-1.0.1.dist-info/METADATA,sha256=_bnYIAvDn27zOxcjyCvjErCl82Gaz-8GVLAvC--x75I,1055
+fnum-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fnum-1.0.1.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
+fnum-1.0.1.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
+fnum-1.0.1.dist-info/RECORD,,
```

