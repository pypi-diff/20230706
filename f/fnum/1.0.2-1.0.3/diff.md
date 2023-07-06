# Comparing `tmp/fnum-1.0.2-py3-none-any.whl.zip` & `tmp/fnum-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16096 bytes, number of entries: 10
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 04:11 fnum/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-06 04:11 fnum/__main__.py
--rw-r--r--  2.0 unx     2235 b- defN 23-Jul-06 04:11 fnum/actions.py
--rw-r--r--  2.0 unx     1793 b- defN 23-Jul-06 04:11 fnum/cli.py
--rw-r--r--  2.0 unx    35141 b- defN 23-Jul-06 04:12 fnum-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1055 b- defN 23-Jul-06 04:12 fnum-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 04:12 fnum-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-06 04:12 fnum-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-06 04:12 fnum-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      745 b- defN 23-Jul-06 04:12 fnum-1.0.2.dist-info/RECORD
-10 files, 41185 bytes uncompressed, 14836 bytes compressed:  64.0%
+Zip file size: 16169 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-06 04:33 fnum/__init__.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-06 04:33 fnum/__main__.py
+-rw-r--r--  2.0 unx     2699 b- defN 23-Jul-06 04:33 fnum/actions.py
+-rw-r--r--  2.0 unx     1793 b- defN 23-Jul-06 04:33 fnum/cli.py
+-rw-r--r--  2.0 unx    35141 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1055 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      745 b- defN 23-Jul-06 04:33 fnum-1.0.3.dist-info/RECORD
+10 files, 41649 bytes uncompressed, 14909 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: fnum/actions.py
 Comment: 
 
 Filename: fnum/cli.py
 Comment: 
 
-Filename: fnum-1.0.2.dist-info/LICENSE
+Filename: fnum-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.0.2.dist-info/METADATA
+Filename: fnum-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.0.2.dist-info/WHEEL
+Filename: fnum-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.0.2.dist-info/entry_points.txt
+Filename: fnum-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.0.2.dist-info/top_level.txt
+Filename: fnum-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.0.2.dist-info/RECORD
+Filename: fnum-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.2"
+__version__ = "1.0.3"
```

## fnum/actions.py

```diff
@@ -50,23 +50,34 @@
         progressbar = noop_progessbar
     with progressbar(files, length=len(files), label="Processing files") as bar:
         for filepath in bar:
             if not filepath.is_file() or filepath.suffix not in suffixes:
                 continue
 
             try:
-                if int(filepath.stem) < num:
+                if int(filepath.stem) <= num:
                     continue
             except ValueError:
                 pass
 
             newpath = numpath(filepath.suffix)
             num += 1
-            metadata["originals"][filepath.name] = newpath.name
-            metadata["order"].append(newpath.name)
+
+            try:
+                order_index = metadata["order"].index(filepath.name)
+                metadata["order"][order_index] = newpath.name
+            except ValueError:
+                metadata["order"].append(newpath.name)
+            try:
+                original_index = metadata["originals"].values().index(filepath.name)
+                original_key = metadata["originals"].keys(original_index)
+                metadata["originals"][original_key] = newpath.name
+            except ValueError:
+                metadata["originals"][filepath.name] = newpath.name
+
             filepath.rename(newpath)
 
     metadata["max"] = num - 1
     return metadata
 
 
 def write_max(dirpath, metadata):
```

## Comparing `fnum-1.0.2.dist-info/LICENSE` & `fnum-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.0.2.dist-info/METADATA` & `fnum-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.0.2
+Version: 1.0.3
 Summary: Renames files in a directory to be named using sequential integers starting with 1
 Author-email: Matt Wisniewski <fnum@mattw.life>
 License: GPLv3
 Project-URL: homepage, https://github.com/polishmatt/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

## Comparing `fnum-1.0.2.dist-info/RECORD` & `fnum-1.0.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-fnum/__init__.py,sha256=Y3LSfRioSl2xch70pq_ULlvyECXyEtN3krVaWeGyaxk,22
+fnum/__init__.py,sha256=2plzdEEb24FLjE2I2XyBBcJEPYWHccNL4SgtLC_6erg,22
 fnum/__main__.py,sha256=8hDtWlaFZK24KhfNq_ZKgtXqYHsDQDetukOCMlsbW0Q,59
-fnum/actions.py,sha256=e2UoyzOpnJ4xwLrzElSfxEb0InoiwZx03c-yg3ehoQA,2235
+fnum/actions.py,sha256=z4Aaluvjr1wZLJzHDshYdjsNBAvTwauTL150pFJjVOs,2699
 fnum/cli.py,sha256=4kvhG47vsJKIFWjpBKr2ZNPsnpHyVrEI_xwhUMEdPPY,1793
-fnum-1.0.2.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
-fnum-1.0.2.dist-info/METADATA,sha256=Vmx9Rl2-AnHqxcLEGgqp9ptnIgy4nrgw_NePl530nnU,1055
-fnum-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fnum-1.0.2.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
-fnum-1.0.2.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
-fnum-1.0.2.dist-info/RECORD,,
+fnum-1.0.3.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
+fnum-1.0.3.dist-info/METADATA,sha256=Y1cWvPdlVnn_w_ElZdKMEpGO0Ve0t3_2QVMfm6mUHnY,1055
+fnum-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fnum-1.0.3.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
+fnum-1.0.3.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
+fnum-1.0.3.dist-info/RECORD,,
```

