# Comparing `tmp/agamprimer-0.6.4.tar.gz` & `tmp/agamprimer-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agamprimer-0.6.4.tar", max compression
+gzip compressed data, was "agamprimer-0.6.5.tar", max compression
```

## Comparing `agamprimer-0.6.4.tar` & `agamprimer-0.6.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    41549 2023-07-06 15:41:49.480582 agamprimer-0.6.4/AgamPrimer/AgamPrimer.py
--rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.4/AgamPrimer/__init__.py
--rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.4/AgamPrimer/agamPrimer.egg-info/PKG-INFO
--rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.4/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.4/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.4/AgamPrimer/agamPrimer.egg-info/top_level.txt
--rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.4/LICENSE
--rw-r--r--   0        0        0      730 2023-07-06 15:41:22.128394 agamprimer-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 agamprimer-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    41554 2023-07-06 16:00:16.369636 agamprimer-0.6.5/AgamPrimer/AgamPrimer.py
+-rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.5/AgamPrimer/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.5/AgamPrimer/agamPrimer.egg-info/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.5/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.5/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.5/AgamPrimer/agamPrimer.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.5/LICENSE
+-rw-r--r--   0        0        0      730 2023-07-06 16:00:53.845966 agamprimer-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 agamprimer-0.6.5/PKG-INFO
```

### Comparing `agamprimer-0.6.4/AgamPrimer/AgamPrimer.py` & `agamprimer-0.6.5/AgamPrimer/AgamPrimer.py`

 * *Files 0% similar despite different names*

```diff
@@ -730,15 +730,15 @@
     # run primer3
     primer_dict = primer3.designPrimers(
         seq_args=seq_parameters, global_args=primer_parameters
     )
 
     if assay_type != "probe":
         # check if primer3 has returned any primers
-        if int(extract_trailing_digits(primer_dict["PRIMER_PAIR_EXPLAIN"])):
+        if int(extract_trailing_digits(primer_dict["PRIMER_PAIR_EXPLAIN"])) == 0:
             print(
                 f"No primers found for {assay_name}. For cDNA primers, this is more likely to occur if the target contains only one exon-exon junction. see troubleshooting below for more information. We suggest relaxing the primer parameters \n"
             )
             print(primer3_run_statistics(primer_dict, assay_type))
             return (None, None)
 
     # AgamPrimer.primer3_run_statistics(primer_dict, assay_type)
```

### Comparing `agamprimer-0.6.4/AgamPrimer/agamPrimer.egg-info/PKG-INFO` & `agamprimer-0.6.5/AgamPrimer/agamPrimer.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `agamprimer-0.6.4/LICENSE` & `agamprimer-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agamprimer-0.6.4/pyproject.toml` & `agamprimer-0.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AgamPrimer"
-version = "0.6.4"
+version = "0.6.5"
 description = "A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "AgamPrimer" }
 ]
```

### Comparing `agamprimer-0.6.4/PKG-INFO` & `agamprimer-0.6.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agamprimer
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

