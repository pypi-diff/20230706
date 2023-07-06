# Comparing `tmp/pyreference-0.7.2.tar.gz` & `tmp/pyreference-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreference-0.7.2.tar", last modified: Mon Nov 21 06:21:19 2022, max compression
+gzip compressed data, was "pyreference-0.7.3.tar", last modified: Thu Jul  6 06:44:42 2023, max compression
```

## Comparing `pyreference-0.7.2.tar` & `pyreference-0.7.3.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-21 06:21:19.753033 pyreference-0.7.2/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1092 2022-11-18 06:19:30.000000 pyreference-0.7.2/LICENSE.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3237 2022-11-21 06:21:19.753033 pyreference-0.7.2/PKG-INFO
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2465 2022-11-21 06:01:21.000000 pyreference-0.7.2/README.md
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-21 06:21:19.753033 pyreference-0.7.2/bin/
--rwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)     8179 2022-11-18 06:19:30.000000 pyreference-0.7.2/bin/pyreference_biotype.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-21 06:21:19.753033 pyreference-0.7.2/pyreference/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      188 2022-11-21 06:07:36.000000 pyreference-0.7.2/pyreference/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2673 2022-11-21 06:06:43.000000 pyreference-0.7.2/pyreference/gene.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2216 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/genomic_region.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      746 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/mirna.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2102 2022-11-21 04:39:59.000000 pyreference-0.7.2/pyreference/pyreference_config.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)    20070 2022-11-21 06:08:16.000000 pyreference-0.7.2/pyreference/reference.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1246 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/referenceargparse.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      325 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/settings.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     9533 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/transcript.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-21 06:21:19.753033 pyreference-0.7.2/pyreference/utils/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/utils/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1173 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/utils/file_utils.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3631 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/utils/genomics_utils.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1295 2022-11-18 06:19:30.000000 pyreference-0.7.2/pyreference/utils/iv_iterators.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-21 06:21:19.753033 pyreference-0.7.2/pyreference.egg-info/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3237 2022-11-21 06:21:19.000000 pyreference-0.7.2/pyreference.egg-info/PKG-INFO
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      642 2022-11-21 06:21:19.000000 pyreference-0.7.2/pyreference.egg-info/SOURCES.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        1 2022-11-21 06:21:19.000000 pyreference-0.7.2/pyreference.egg-info/dependency_links.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       84 2022-11-21 06:21:19.000000 pyreference-0.7.2/pyreference.egg-info/requires.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       18 2022-11-21 06:21:19.000000 pyreference-0.7.2/pyreference.egg-info/top_level.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       38 2022-11-21 06:21:19.753033 pyreference-0.7.2/setup.cfg
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1798 2022-11-21 06:14:30.000000 pyreference-0.7.2/setup.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-21 06:21:19.753033 pyreference-0.7.2/tests/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-18 06:19:30.000000 pyreference-0.7.2/tests/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     9217 2022-11-21 04:49:47.000000 pyreference-0.7.2/tests/test_reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/
+-rw-rw-r--   0 root         (0) root         (0)     1092 2023-03-21 01:08:04.000000 pyreference-0.7.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-07-06 06:44:42.961318 pyreference-0.7.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2465 2023-03-21 01:08:04.000000 pyreference-0.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/bin/
+-rwxrwxr-x   0 root         (0) root         (0)     8179 2023-03-21 01:08:04.000000 pyreference-0.7.3/bin/pyreference_biotype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/pyreference/
+-rw-rw-r--   0 root         (0) root         (0)      188 2023-07-06 06:39:49.000000 pyreference-0.7.3/pyreference/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2818 2023-07-06 06:33:40.000000 pyreference-0.7.3/pyreference/gene.py
+-rw-rw-r--   0 root         (0) root         (0)     2216 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/genomic_region.py
+-rw-rw-r--   0 root         (0) root         (0)      746 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/mirna.py
+-rw-rw-r--   0 root         (0) root         (0)     2102 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/pyreference_config.py
+-rw-rw-r--   0 root         (0) root         (0)    20304 2023-07-06 05:45:06.000000 pyreference-0.7.3/pyreference/reference.py
+-rw-rw-r--   0 root         (0) root         (0)     1246 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/referenceargparse.py
+-rw-rw-r--   0 root         (0) root         (0)      325 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/settings.py
+-rw-rw-r--   0 root         (0) root         (0)     9533 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/transcript.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/pyreference/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1173 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/utils/file_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3631 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/utils/genomics_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1295 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/utils/iv_iterators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/pyreference.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 06:44:42.961318 pyreference-0.7.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1815 2023-03-21 01:08:04.000000 pyreference-0.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/tests/
+-rw-rw-r--   0 root         (0) root         (0)     9509 2023-07-06 06:31:17.000000 pyreference-0.7.3/tests/test_reference.py
```

### Comparing `pyreference-0.7.2/LICENSE.txt` & `pyreference-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/PKG-INFO` & `pyreference-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreference
-Version: 0.7.2
+Version: 0.7.3
 Summary: Library for working with reference genomes and gene GTF/GFFs
 Home-page: https://github.com/SACGF/pyreference
 Author: David Lawrence
 Author-email: davmlaw@gmail.com
 Keywords: genomics,gtf,gff,genome,genes
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyreference-0.7.2/README.md` & `pyreference-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/bin/pyreference_biotype.py` & `pyreference-0.7.3/bin/pyreference_biotype.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference/gene.py` & `pyreference-0.7.3/pyreference/gene.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     @lazy
     def representative_transcript(self):
         """ Returns longest coding transcript if gene is coding, otherwise longest transcript
             Sort transcript ID alphabetically if equal length """
         
         transcript = self.get_longest_coding_transcript()
-        if transcript == None:
+        if transcript is None:
             transcript = self.get_longest_transcript()
         return transcript
 
     def get_representative_transcript(self):
         return self.representative_transcript
 
     def get_longest_coding_transcript(self):
@@ -67,19 +67,24 @@
     def get_longest_transcript(self, coding_only=False):
         transcripts = self.transcripts
         if coding_only:
             transcripts = filter(lambda t: t.is_coding, transcripts)
         
         longest_transcript = None
         if transcripts:
-            # We want the MAX length - and MIN ID, so sort by min but use maxint-length  
+            try:
+                big_int = sys.maxint  # Python 2
+            except AttributeError:
+                big_int = sys.maxsize  # Python 3
+
+            # We want the MAX length - and MIN ID, so sort by min but use maxint-length
             # We also want NM_007041 (len 2209) over NM_001001976 (len 2209)
             # Which is annoyingly zero padded - so use smallest ID length, then only if equal do alpha sort 
             def min_transcript_key(t):
-                return (sys.maxint - t.length, len(t.get_id()), t.get_id())
+                return big_int - t.length, len(t.get_id()), t.get_id()
 
             longest_transcript = min(transcripts, key=min_transcript_key)
         return longest_transcript
 
     def __repr__(self):
         return "%s (%s) %d transcripts" % (self.get_gene_name(), self.accession_id, len(self.transcripts))
```

### Comparing `pyreference-0.7.2/pyreference/genomic_region.py` & `pyreference-0.7.3/pyreference/genomic_region.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference/mirna.py` & `pyreference-0.7.3/pyreference/mirna.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference/pyreference_config.py` & `pyreference-0.7.3/pyreference/pyreference_config.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference/reference.py` & `pyreference-0.7.3/pyreference/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from bioutils.assemblies import make_ac_name_map
 from collections import defaultdict
 from deprecation import deprecated
 from functools import reduce
 import gzip
 import json
 from lazy import lazy
+import logging
 import operator
 import os
 from pyreference import settings
 from pyreference.gene import Gene
 from pyreference.mirna import MiRNA
 from pyreference.pyreference_config import load_params_from_config
 from pyreference.transcript import Transcript
@@ -153,16 +154,20 @@
                     raise config_exception
                 raise ValueError(message + " config section '%s' in file '%s'" % (params['build'], params['config']))
 
         if self._genome_sequence_lookup not in FASTA_LOOKUP:
             valid_values = ','.join(str(s) for s in FASTA_LOOKUP)
             raise ValueError("genome_sequence_lookup='%s' must be one of %s" % (self._genome_sequence_lookup,
                                                                                 valid_values))
+        self.contig_to_chrom = {}
+        try:
+            self.contig_to_chrom = make_ac_name_map(self._genome_accession)
+        except FileNotFoundError:
+            logging.warning(f"Bioutils does not support genome build '{self._genome_accession}' cannot perform chrom/contig mapping")
 
-        self.contig_to_chrom = make_ac_name_map(self._genome_accession)
         # Store this so we can ask about config later
         self.build = params["build"]
         self._args = {"build": build, "config": config}
         self._build_params = params
 
     @lazy
     def _genes_dict(self):
```

### Comparing `pyreference-0.7.2/pyreference/referenceargparse.py` & `pyreference-0.7.3/pyreference/referenceargparse.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference/transcript.py` & `pyreference-0.7.3/pyreference/transcript.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference/utils/file_utils.py` & `pyreference-0.7.3/pyreference/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference/utils/genomics_utils.py` & `pyreference-0.7.3/pyreference/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference/utils/iv_iterators.py` & `pyreference-0.7.3/pyreference/utils/iv_iterators.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.2/pyreference.egg-info/PKG-INFO` & `pyreference-0.7.3/pyreference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreference
-Version: 0.7.2
+Version: 0.7.3
 Summary: Library for working with reference genomes and gene GTF/GFFs
 Home-page: https://github.com/SACGF/pyreference
 Author: David Lawrence
 Author-email: davmlaw@gmail.com
 Keywords: genomics,gtf,gff,genome,genes
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyreference-0.7.2/pyreference.egg-info/SOURCES.txt` & `pyreference-0.7.3/pyreference.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 pyreference.egg-info/dependency_links.txt
 pyreference.egg-info/requires.txt
 pyreference.egg-info/top_level.txt
 pyreference/utils/__init__.py
 pyreference/utils/file_utils.py
 pyreference/utils/genomics_utils.py
 pyreference/utils/iv_iterators.py
-tests/__init__.py
 tests/test_reference.py
```

### Comparing `pyreference-0.7.2/setup.py` & `pyreference-0.7.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 setup(name='pyreference',
-      packages=find_packages(),
+      packages=find_packages(exclude=['tests']),
       version=_get_version("pyreference/__init__.py"),
       description='Library for working with reference genomes and gene GTF/GFFs',
       long_description_content_type="text/markdown",
       long_description=open("README.md").read(),
       author='David Lawrence',
       author_email='davmlaw@gmail.com',
       url='https://github.com/SACGF/pyreference',
```

### Comparing `pyreference-0.7.2/tests/test_reference.py` & `pyreference-0.7.3/tests/test_reference.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,21 @@
 
             utr = str(transcript.get_3putr_sequence()).upper()
             self.assertTrue(utr.startswith(test["3p_utr"]), "%s should start with %s" % (utr, test["3p_utr"]))
 
             m_rna = transcript.get_transcript_sequence()
             self.assertTrue(m_rna.find(test["3p_utr"]) > 1)
 
+    def test_gene_transcript(self):
+        gene = self.reference.genes["PLCXD1"]
+        lt = gene.get_longest_transcript()
+        self.assertEqual(lt.accession_id, "NM_018390_2")
+        lct = gene.get_longest_coding_transcript()
+        self.assertEqual(lct.accession_id, "NM_018390_2")
+
     def test_get_transcript_length(self):
         transcript_id = "NM_018390_2"
         transcript = self.reference.transcripts[transcript_id]
 
         seq = transcript.get_transcript_sequence()
         #        print "**** transcript_id = %s - sequence = %s" % (transcript_id, seq)
         sequence_length = len(seq)
```

