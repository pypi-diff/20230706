# Comparing `tmp/microhapdb-0.7rc1.tar.gz` & `tmp/microhapdb-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microhapdb-0.7rc1.tar", last modified: Thu Jan 20 20:46:06 2022, max compression
+gzip compressed data, was "microhapdb-0.9.tar", last modified: Thu Jul  6 17:16:47 2023, max compression
```

## Comparing `microhapdb-0.7rc1.tar` & `microhapdb-0.9.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 standage   (502) staff       (20)        0 2022-01-20 20:46:06.106614 microhapdb-0.7rc1/
--rw-r--r--   0 standage   (502) staff       (20)     1859 2021-12-23 15:09:33.000000 microhapdb-0.7rc1/LICENSE.txt
--rw-r--r--   0 standage   (502) staff       (20)      115 2021-12-23 15:09:33.000000 microhapdb-0.7rc1/MANIFEST.in
--rw-r--r--   0 standage   (502) staff       (20)    12359 2022-01-20 20:46:06.106848 microhapdb-0.7rc1/PKG-INFO
--rw-r--r--   0 standage   (502) staff       (20)    11639 2022-01-20 20:38:12.000000 microhapdb-0.7rc1/README.md
-drwxr-xr-x   0 standage   (502) staff       (20)        0 2022-01-20 20:46:06.108076 microhapdb-0.7rc1/microhapdb/
--rw-r--r--   0 standage   (502) staff       (20)     2563 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/__init__.py
--rw-r--r--   0 standage   (502) staff       (20)      500 2022-01-20 20:46:06.108228 microhapdb-0.7rc1/microhapdb/_version.py
-drwxr-xr-x   0 standage   (502) staff       (20)        0 2022-01-20 20:46:06.069897 microhapdb-0.7rc1/microhapdb/cli/
--rw-r--r--   0 standage   (502) staff       (20)     3097 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/cli/__init__.py
--rw-r--r--   0 standage   (502) staff       (20)     4996 2022-01-20 20:38:12.000000 microhapdb-0.7rc1/microhapdb/cli/frequency.py
--rw-r--r--   0 standage   (502) staff       (20)     1074 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/cli/lookup.py
--rw-r--r--   0 standage   (502) staff       (20)     5715 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/cli/marker.py
--rw-r--r--   0 standage   (502) staff       (20)     1803 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/cli/population.py
--rw-r--r--   0 standage   (502) staff       (20)      589 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/conftest.py
-drwxr-xr-x   0 standage   (502) staff       (20)        0 2022-01-20 20:46:06.098806 microhapdb-0.7rc1/microhapdb/data/
--rw-r--r--   0 standage   (502) staff       (20)  4651679 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/data/frequency.tsv
--rw-r--r--   0 standage   (502) staff       (20)     4530 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/data/idmap.tsv
--rw-r--r--   0 standage   (502) staff       (20)      201 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/data/indels.tsv
--rw-r--r--   0 standage   (502) staff       (20)   256353 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/data/marker-aes.tsv
--rw-r--r--   0 standage   (502) staff       (20)    30081 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/data/marker-offsets-GRCh37.tsv
--rw-r--r--   0 standage   (502) staff       (20)    59873 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/data/marker.tsv
--rw-r--r--   0 standage   (502) staff       (20)     3538 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/data/population.tsv
--rw-r--r--   0 standage   (502) staff       (20)   580583 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/data/sequences.tsv
-drwxr-xr-x   0 standage   (502) staff       (20)        0 2022-01-20 20:46:06.101019 microhapdb-0.7rc1/microhapdb/data/tests/
--rw-r--r--   0 standage   (502) staff       (20)     7964 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/data/tests/panel-alpha.fasta
--rw-r--r--   0 standage   (502) staff       (20)    17862 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/data/tests/panel-beta.fasta
--rw-r--r--   0 standage   (502) staff       (20)    49017 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/data/variantmap.tsv
--rw-r--r--   0 standage   (502) staff       (20)    13155 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/marker.py
--rw-r--r--   0 standage   (502) staff       (20)     4795 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/panel.py
--rw-r--r--   0 standage   (502) staff       (20)     1906 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/population.py
--rw-r--r--   0 standage   (502) staff       (20)     6655 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/retrieve.py
-drwxr-xr-x   0 standage   (502) staff       (20)        0 2022-01-20 20:46:06.106048 microhapdb-0.7rc1/microhapdb/tests/
--rw-r--r--   0 standage   (502) staff       (20)    20449 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/tests/test_cli.py
--rw-r--r--   0 standage   (502) staff       (20)     6770 2022-01-20 20:38:12.000000 microhapdb-0.7rc1/microhapdb/tests/test_frequency.py
--rw-r--r--   0 standage   (502) staff       (20)    30510 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/tests/test_marker.py
--rw-r--r--   0 standage   (502) staff       (20)     6603 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/microhapdb/tests/test_population.py
--rw-r--r--   0 standage   (502) staff       (20)     2452 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/tests/test_retrieve.py
--rw-r--r--   0 standage   (502) staff       (20)     1561 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/microhapdb/util.py
-drwxr-xr-x   0 standage   (502) staff       (20)        0 2022-01-20 20:46:06.065211 microhapdb-0.7rc1/microhapdb.egg-info/
--rw-r--r--   0 standage   (502) staff       (20)    12359 2022-01-20 20:46:05.000000 microhapdb-0.7rc1/microhapdb.egg-info/PKG-INFO
--rw-r--r--   0 standage   (502) staff       (20)     1132 2022-01-20 20:46:05.000000 microhapdb-0.7rc1/microhapdb.egg-info/SOURCES.txt
--rw-r--r--   0 standage   (502) staff       (20)        1 2022-01-20 20:46:05.000000 microhapdb-0.7rc1/microhapdb.egg-info/dependency_links.txt
--rw-r--r--   0 standage   (502) staff       (20)       52 2022-01-20 20:46:05.000000 microhapdb-0.7rc1/microhapdb.egg-info/entry_points.txt
--rw-r--r--   0 standage   (502) staff       (20)       12 2022-01-20 20:46:05.000000 microhapdb-0.7rc1/microhapdb.egg-info/requires.txt
--rw-r--r--   0 standage   (502) staff       (20)       11 2022-01-20 20:46:05.000000 microhapdb-0.7rc1/microhapdb.egg-info/top_level.txt
--rw-r--r--   0 standage   (502) staff       (20)        1 2021-12-23 15:09:49.000000 microhapdb-0.7rc1/microhapdb.egg-info/zip-safe
--rw-r--r--   0 standage   (502) staff       (20)      209 2022-01-20 20:46:06.107534 microhapdb-0.7rc1/setup.cfg
--rw-r--r--   0 standage   (502) staff       (20)     1658 2021-12-31 01:54:03.000000 microhapdb-0.7rc1/setup.py
--rw-r--r--   0 standage   (502) staff       (20)    68611 2021-12-23 15:09:34.000000 microhapdb-0.7rc1/versioneer.py
+drwxr-xr-x   0 daniel.standage (1653330546) staff       (20)        0 2023-07-06 17:16:47.609129 microhapdb-0.9/
+-rw-------   0 daniel.standage (1653330546) staff       (20)     1859 2022-03-07 18:42:13.000000 microhapdb-0.9/LICENSE.txt
+-rw-------   0 daniel.standage (1653330546) staff       (20)      116 2023-03-01 20:48:53.000000 microhapdb-0.9/MANIFEST.in
+-rw-r--r--   0 daniel.standage (1653330546) staff       (20)     3908 2023-07-06 17:16:47.609320 microhapdb-0.9/PKG-INFO
+-rw-------   0 daniel.standage (1653330546) staff       (20)     3228 2023-07-03 19:44:11.000000 microhapdb-0.9/README.md
+drwxr-xr-x   0 daniel.standage (1653330546) staff       (20)        0 2023-07-06 17:16:47.610494 microhapdb-0.9/microhapdb/
+-rw-------   0 daniel.standage (1653330546) staff       (20)     3456 2023-06-30 17:28:47.000000 microhapdb-0.9/microhapdb/__init__.py
+-rw-r--r--   0 daniel.standage (1653330546) staff       (20)      495 2023-07-06 17:16:47.610627 microhapdb-0.9/microhapdb/_version.py
+drwxr-xr-x   0 daniel.standage (1653330546) staff       (20)        0 2023-07-06 17:16:47.585006 microhapdb-0.9/microhapdb/cli/
+-rw-------   0 daniel.standage (1653330546) staff       (20)     3989 2023-03-13 14:27:00.000000 microhapdb-0.9/microhapdb/cli/__init__.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     5388 2023-02-22 21:24:52.000000 microhapdb-0.9/microhapdb/cli/frequency.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     1379 2022-11-15 20:05:04.000000 microhapdb-0.9/microhapdb/cli/lookup.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     7941 2023-05-01 16:35:17.000000 microhapdb-0.9/microhapdb/cli/marker.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     2085 2022-11-15 20:05:04.000000 microhapdb-0.9/microhapdb/cli/population.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     1482 2023-06-16 18:03:38.000000 microhapdb-0.9/microhapdb/cli/summarize.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)      891 2022-11-14 17:21:34.000000 microhapdb-0.9/microhapdb/conftest.py
+drwxr-xr-x   0 daniel.standage (1653330546) staff       (20)        0 2023-07-06 17:16:47.603967 microhapdb-0.9/microhapdb/data/
+-rw-------   0 daniel.standage (1653330546) staff       (20)  5244486 2023-06-30 17:28:47.000000 microhapdb-0.9/microhapdb/data/frequency.csv.gz
+-rw-------   0 daniel.standage (1653330546) staff       (20)     1071 2023-06-28 11:41:06.000000 microhapdb-0.9/microhapdb/data/indels.csv
+-rw-------   0 daniel.standage (1653330546) staff       (20)  2121662 2023-06-30 17:28:47.000000 microhapdb-0.9/microhapdb/data/marker-aes.csv
+-rw-------   0 daniel.standage (1653330546) staff       (20)   560278 2023-06-30 17:28:47.000000 microhapdb-0.9/microhapdb/data/marker.csv
+-rw-------   0 daniel.standage (1653330546) staff       (20)    12197 2023-06-30 17:28:47.000000 microhapdb-0.9/microhapdb/data/merged.csv
+-rw-------   0 daniel.standage (1653330546) staff       (20)     4389 2023-06-28 11:41:06.000000 microhapdb-0.9/microhapdb/data/population.csv
+-rw-------   0 daniel.standage (1653330546) staff       (20)    17185 2023-06-22 18:57:41.000000 microhapdb-0.9/microhapdb/marker.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     7598 2023-06-16 18:03:38.000000 microhapdb-0.9/microhapdb/nomenclature.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     6452 2023-02-28 19:39:08.000000 microhapdb-0.9/microhapdb/panel.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     4142 2023-02-28 19:39:08.000000 microhapdb-0.9/microhapdb/population.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     1620 2023-06-16 18:03:38.000000 microhapdb-0.9/microhapdb/tables.py
+drwxr-xr-x   0 daniel.standage (1653330546) staff       (20)        0 2023-07-06 17:16:47.607418 microhapdb-0.9/microhapdb/tests/
+drwxr-xr-x   0 daniel.standage (1653330546) staff       (20)        0 2023-07-06 17:16:47.608609 microhapdb-0.9/microhapdb/tests/data/
+-rw-------   0 daniel.standage (1653330546) staff       (20)     7238 2023-05-01 16:35:17.000000 microhapdb-0.9/microhapdb/tests/data/panel-alpha.fasta
+-rw-------   0 daniel.standage (1653330546) staff       (20)    16201 2023-05-01 16:35:17.000000 microhapdb-0.9/microhapdb/tests/data/panel-beta.fasta
+-rw-------   0 daniel.standage (1653330546) staff       (20)    30701 2023-06-30 17:28:47.000000 microhapdb-0.9/microhapdb/tests/test_cli.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     3473 2023-06-30 17:28:47.000000 microhapdb-0.9/microhapdb/tests/test_frequency.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)    30343 2023-06-30 17:28:47.000000 microhapdb-0.9/microhapdb/tests/test_marker.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     5649 2023-06-16 18:03:38.000000 microhapdb-0.9/microhapdb/tests/test_nomenclature.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     6386 2023-02-28 19:39:08.000000 microhapdb-0.9/microhapdb/tests/test_population.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)     1717 2023-02-23 20:09:25.000000 microhapdb-0.9/microhapdb/tests/test_retrieve.py
+drwxr-xr-x   0 daniel.standage (1653330546) staff       (20)        0 2023-07-06 17:16:47.581825 microhapdb-0.9/microhapdb.egg-info/
+-rw-------   0 daniel.standage (1653330546) staff       (20)     3908 2023-07-06 17:16:47.000000 microhapdb-0.9/microhapdb.egg-info/PKG-INFO
+-rw-------   0 daniel.standage (1653330546) staff       (20)     1105 2023-07-06 17:16:47.000000 microhapdb-0.9/microhapdb.egg-info/SOURCES.txt
+-rw-------   0 daniel.standage (1653330546) staff       (20)        1 2023-07-06 17:16:47.000000 microhapdb-0.9/microhapdb.egg-info/dependency_links.txt
+-rw-------   0 daniel.standage (1653330546) staff       (20)       51 2023-07-06 17:16:47.000000 microhapdb-0.9/microhapdb.egg-info/entry_points.txt
+-rw-------   0 daniel.standage (1653330546) staff       (20)       25 2023-07-06 17:16:47.000000 microhapdb-0.9/microhapdb.egg-info/requires.txt
+-rw-------   0 daniel.standage (1653330546) staff       (20)       11 2023-07-06 17:16:47.000000 microhapdb-0.9/microhapdb.egg-info/top_level.txt
+-rw-------   0 daniel.standage (1653330546) staff       (20)        1 2022-03-07 19:02:11.000000 microhapdb-0.9/microhapdb.egg-info/zip-safe
+-rw-------   0 daniel.standage (1653330546) staff       (20)      209 2023-07-06 17:16:47.610078 microhapdb-0.9/setup.cfg
+-rw-------   0 daniel.standage (1653330546) staff       (20)     1940 2023-06-30 17:47:33.000000 microhapdb-0.9/setup.py
+-rw-------   0 daniel.standage (1653330546) staff       (20)    68448 2022-11-14 17:21:34.000000 microhapdb-0.9/versioneer.py
```

### Comparing `microhapdb-0.7rc1/LICENSE.txt` & `microhapdb-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `microhapdb-0.7rc1/microhapdb/cli/frequency.py` & `microhapdb-0.9/microhapdb/cli/frequency.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,101 @@
-# -----------------------------------------------------------------------------
-# Copyright (c) 2019, Battelle National Biodefense Institute.
+# -------------------------------------------------------------------------------------------------
+# Copyright (c) 2019, DHS.
 #
-# This file is part of MicroHapDB (http://github.com/bioforensics/microhapdb)
-# and is licensed under the BSD license: see LICENSE.txt.
-# -----------------------------------------------------------------------------
+# This file is part of MicroHapDB (http://github.com/bioforensics/MicroHapDB) and is licensed under
+# the BSD license: see LICENSE.txt.
+#
+# This software was prepared for the Department of Homeland Security (DHS) by the Battelle National
+# Biodefense Institute, LLC (BNBI) as part of contract HSHQDC-15-C-00064 to manage and operate the
+# National Biodefense Analysis and Countermeasures Center (NBACC), a Federally Funded Research and
+# Development Center.
+# -------------------------------------------------------------------------------------------------
 
 from argparse import RawDescriptionHelpFormatter
 import microhapdb
-from microhapdb.retrieve import standardize_marker_ids, standardize_population_ids
+from microhapdb import Marker, Population
 from numpy import float64
 import pandas as pd
 import sys
 from textwrap import dedent
+from warnings import warn
+
+
+def main(args):
+    markers = args.marker
+    if args.panel:
+        with open(args.panel, "r") as fh:
+            markers = fh.read().strip().split()
+    result = apply_filters(markers, args.population, args.allele)
+    if len(result) == 0:
+        return
+    display(result, args.format, args.population)
+
+
+def apply_filters(markers=None, populations=None, allele=None):
+    result = microhapdb.frequencies
+    if markers:
+        markers = Marker.standardize_ids(markers)
+        result = result[result.Marker.isin(markers)]
+    if populations:
+        populations = Population.standardize_ids(populations)
+        result = result[result.Population.isin(populations)]
+    if allele:
+        result = result[result.Allele == allele]
+    return result
+
+
+def display(result, view_format, population):
+    if view_format == "table":
+        result.to_csv(sys.stdout, sep="\t", index=False)
+    elif view_format == "detail":
+        raise NotImplementedError("detail format not yet implemented")
+    elif view_format == "mhpl8r":
+        npop = len(result.Population.unique())
+        if npop > 1:
+            warn(f"frequencies for {npop} populations recovered, expected only 1", UserWarning)
+        result = result[["Marker", "Allele", "Frequency"]].rename(columns={"Allele": "Haplotype"})
+        result.to_csv(sys.stdout, sep="\t", index=False)
+    elif view_format == "efm":
+        if population is None or len(population) != 1:
+            raise ValueError("must specify one and only one population with --format=efm")
+        result = construct_frequency_table(population[0], result.Marker.unique())
+        result.to_csv(sys.stdout)
+    else:
+        raise ValueError(f'unsupported view format "{view_format}"')
 
 
 def subparser(subparsers):
-    desc = microhapdb.cli.bubbletext + '\nRetrieve population allele frequencies'
     epilog = """\
     Examples::
 
         microhapdb frequency --marker=mh22KK-060 --population=SA000001B
         microhapdb frequency --marker=mh22KK-060 --allele=C,A
     """
     epilog = dedent(epilog)
     subparser = subparsers.add_parser(
-        'frequency', description=desc, epilog=epilog, formatter_class=RawDescriptionHelpFormatter,
+        "frequency",
+        description="Retrieve population allele frequencies",
+        epilog=epilog,
+        formatter_class=RawDescriptionHelpFormatter,
+    )
+    subparser.add_argument(
+        "--format", choices=["table", "detail", "mhpl8r", "efm"], default="table"
     )
-    subparser.add_argument('--format', choices=['table', 'detail', 'mhpl8r', 'efm'], default='table')
     meg = subparser.add_mutually_exclusive_group()
-    meg.add_argument('--marker', metavar='ID', nargs='+', help='restrict frequencies by marker')
-    meg.add_argument('--panel', metavar='FILE', help='restrict frequencies to markers listed in FILE, one ID per line')
-    subparser.add_argument('--population', metavar='ID', nargs='+', help='restrict frequencies by population')
-    subparser.add_argument('--allele', metavar='ID', help='restrict frequencies by allele')
-
-
-def order_haplotypes(markers, pop, frequencies):
-    """Retrieve all unique haplotype designators and order by marker occurrence
-
-    This ordering creates a pleasing arrangement of blocks of data along a single diagonal in the
-    final output table, whereas other orderings result in a more chaotic organization.
-    """
-    haplotypes = list()
-    for marker in sorted(markers):
-        # print("DEBUG", frequencies.shape, len(frequencies.Marker == marker), len(frequencies.Population))
-        subset = frequencies[(frequencies.Marker == marker) & (frequencies.Population == pop)]
-        for haplotype in sorted(subset.Allele):
-            if haplotype not in haplotypes:
-                haplotypes.append(haplotype)
-    print(
-        f"[microhapdb] retrieved and ordered {len(haplotypes)} distinct haplotypes",
-        file=sys.stderr,
+    meg.add_argument("--marker", metavar="ID", nargs="+", help="restrict frequencies by marker")
+    meg.add_argument(
+        "--panel",
+        metavar="FILE",
+        help="restrict frequencies to markers listed in FILE, one ID per line",
     )
-    return haplotypes
+    subparser.add_argument(
+        "--population", metavar="ID", nargs="+", help="restrict frequencies by population"
+    )
+    subparser.add_argument("--allele", metavar="ID", help="restrict frequencies by allele")
 
 
 def construct_frequency_table(pop, panel):
     frequencies = microhapdb.frequencies
     frequencies = frequencies[frequencies.Marker.isin(panel)]
     marker_indices = {marker: i for i, marker in enumerate(panel)}
     haplotypes = order_haplotypes(panel, pop, frequencies)
@@ -72,40 +112,24 @@
     print(
         f"[microhapdb] constructed frequency table for {nrows} haplotypes and {ncols} markers",
         file=sys.stderr,
     )
     return table.round(3)
 
 
-def main(args):
-    query_args = list()
-    result = microhapdb.frequencies
-    if args.marker:
-        markerids = standardize_marker_ids(args.marker)
-        result = result[result.Marker.isin(markerids)]
-    if args.panel:
-        with open(args.panel, 'r') as fh:
-            markerids = fh.read().strip().split()
-            markerids = standardize_marker_ids(markerids)
-        result = result[result.Marker.isin(markerids)]
-    if args.population:
-        popids = standardize_population_ids(args.population)
-        result = result[result.Population.isin(popids)]
-    if args.allele:
-        result = result[result.Allele == args.allele]
-    if args.format == 'table':
-        print(result.to_string(index=False))
-    elif args.format == 'detail':
-        raise NotImplementedError('detail format not yet implemented')
-    elif args.format == 'mhpl8r':
-        npop = len(result.Population.unique())
-        if npop > 1:
-            print(f'warning: frequencies for {npop} populations recovered, expected only 1', file=sys.stderr)
-        result = result[['Marker', 'Allele', 'Frequency']].rename(columns={'Allele': 'Haplotype'})
-        result.to_csv(sys.stdout, sep="\t", index=False)
-    elif args.format == 'efm':
-        if args.population is None or len(args.population) != 1:
-            raise ValueError("must specify one and only one population with --format=efm")
-        result = construct_frequency_table(args.population[0], markerids)
-        result.to_csv(sys.stdout)
-    else:
-        raise ValueError(f'unsupported view format "{args.format}"')
+def order_haplotypes(markers, pop, frequencies):
+    """Retrieve all unique haplotype designators and order by marker occurrence
+
+    This ordering creates a pleasing arrangement of blocks of data along a single diagonal in the
+    final output table, whereas other orderings result in a more chaotic organization.
+    """
+    haplotypes = list()
+    for marker in sorted(markers):
+        subset = frequencies[(frequencies.Marker == marker) & (frequencies.Population == pop)]
+        for haplotype in sorted(subset.Allele):
+            if haplotype not in haplotypes:
+                haplotypes.append(haplotype)
+    print(
+        f"[microhapdb] retrieved and ordered {len(haplotypes)} distinct haplotypes",
+        file=sys.stderr,
+    )
+    return haplotypes
```

### Comparing `microhapdb-0.7rc1/microhapdb/cli/lookup.py` & `microhapdb-0.9/microhapdb/cli/lookup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-# -----------------------------------------------------------------------------
-# Copyright (c) 2019, Battelle National Biodefense Institute.
+# -------------------------------------------------------------------------------------------------
+# Copyright (c) 2019, DHS.
 #
-# This file is part of MicroHapDB (http://github.com/bioforensics/microhapdb)
-# and is licensed under the BSD license: see LICENSE.txt.
-# -----------------------------------------------------------------------------
+# This file is part of MicroHapDB (http://github.com/bioforensics/MicroHapDB) and is licensed under
+# the BSD license: see LICENSE.txt.
+#
+# This software was prepared for the Department of Homeland Security (DHS) by the Battelle National
+# Biodefense Institute, LLC (BNBI) as part of contract HSHQDC-15-C-00064 to manage and operate the
+# National Biodefense Analysis and Countermeasures Center (NBACC), a Federally Funded Research and
+# Development Center.
+# -------------------------------------------------------------------------------------------------
 
 from argparse import RawDescriptionHelpFormatter
 import microhapdb
 from textwrap import dedent
 
 
+def main(args):
+    result = microhapdb.retrieve_by_id(args.id)
+    print(result.to_string(index=False))
+
+
 def subparser(subparsers):
-    desc = microhapdb.cli.bubbletext + '\nRetrieve marker or population records by name or identifier'
     epilog = """\
     Examples::
 
         microhapdb lookup rs10815466
         microhapdb lookup mh12KK-043
         microhapdb lookup Japanese
     """
     epilog = dedent(epilog)
     subparser = subparsers.add_parser(
-        'lookup', description=desc, epilog=epilog, formatter_class=RawDescriptionHelpFormatter,
+        "lookup",
+        description="Retrieve marker or population records by name or identifier",
+        epilog=epilog,
+        formatter_class=RawDescriptionHelpFormatter,
     )
-    subparser.add_argument('id', help='record identifier')
-
-
-def main(args):
-    result = microhapdb.retrieve.by_id(args.id)
-    print(result.to_string(index=False))
+    subparser.add_argument("id", help="record identifier")
```

### Comparing `microhapdb-0.7rc1/microhapdb/data/tests/panel-alpha.fasta` & `microhapdb-0.9/microhapdb/tests/data/panel-alpha.fasta`

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,110 @@
->mh01KK-117 PermID=MHDBM-39dc025f GRCh38:chr1:204664211-204664397 variants=32,89,192,218 Xref=SI664549I
+>mh01KK-117 GRCh38:chr1:204664179-204664430 mh01KK-117.v1=32,89,192,218
 CCAGCTCTGTTTGTCTCCCCACAAAGCATTGCAGAAGAAAACACGGAAGCCGCCAGCACTATTATGCATTCATGATTCCA
 GCTTCAACCAGTCCTCTCTGCTGCAATCCCTTTATTCCTCCTCTGCAGCTGCCCCGGCACCTCTGCACAGTCCTTTTCTG
 AATCTGCCCCTCACCGTGCTCCCCACCTGCACGCCGTCCTCAGAACAGATTGCCTTGCCTGACCTCCTGAGGCCGACGGA
 GATGGTGATGT
->mh02KK-134 PermID=MHDBM-daea3d38 GRCh38:chr2:160222899-160223002 variants=73,97,112,176 Xref=SI664557H
+>mh02KK-134 GRCh38:chr2:160222826-160223076 mh02KK-134.v1=73,97,112,176
 CAGTACTTTTGTGGCACTGGAGAACTGCAGGCCTTGGGGACAGGCAGGAACTGTACCCTTGGCAGGAACCCTCACTACCT
 AAGGATGGGCAATGGCTTATGAGTGAGAAACACGGAGCCGTGGGAACTCAGAATGACATGCTACCTGGAGATTGTGGTAA
 CGCCCTGTTTTTTTGTGGGCATATCTACGAGCCTCAAGGACATTGGAGACAGCCACCTAGCAAGAGCTGGGGGCCTGTGG
 GGGAAGCTGG
->mh03CP-005 PermID=MHDBM-18771df9 GRCh38:chr3:15643038-15643049 variants=119,121,122,130 Xref=SI664935H
+>mh03CP-005 GRCh38:chr3:15642919-15643169 mh03CP-005=119,121,122,130
 TGGGAGGCTGAGGCAGGAGAATCACTTGAACCTGGGAGGCAGGAGTTGCGGTGAGAAAGATCGCGCCACTGCATTCCAGC
 CTGGACAACAGGAGCAAAACTCTGCCTCAAAAAAAAAAAAAAAAATAAAATAAAATAAAGAAATGGAATCCCTCAAAGGA
 TATGTACATTTTAAATTATATTAAAGAGTACCAAATTTCCCGCTTAAAAAACTTTGATTTCACTTTACAGCCCCAGTCAT
 ACAGTATGAG
->mh04KK-030 PermID=MHDBM-1e252b7e GRCh38:chr4:3664642-3664756 variants=68,101,169,182 Xref=SI664727G
+>mh04KK-030 GRCh38:chr4:3664574-3664825 mh04KK-030.v1=68,101,169,182
 ACAGTGGTGTGGTCTGATTTGTGTCTTCTGCATTCACAGCTGAATATAGGCCCAGGGGCTTTCTGAACTGGACTCAGTGA
 CAAGGGCCTGACTCCCGGGCACGTGGTACTATTCTTACCACAGATGTCCGTGCTCAGAGCTGGGACATGGTCACTCCTGG
 GTAAGACACATTAGGTCCTTAACTAGGAGACACTCACTGGGGATTTTCTCGTGGTTCTGCTGTGCAAGTTGGAGGCAGTT
 GGGAGGTTGCC
->mh05KK-170 PermID=MHDBM-22ddbb7d GRCh38:chr5:2447909-2448045 variants=57,85,179,193 Xref=SI664573F
+>mh05KK-170 GRCh38:chr5:2447852-2448103 mh05KK-170.v1=57,85,179,193
 GAGACCTTGACACATGGAGGACAAAAGTGAACTTGATTTTCTTAACAAAACTGAAGGCCACAGTTGAAGAGAGAGAGCAT
 GAGACAGCTTGATCGAAATGGTGAAGCTTTGGAGAGATTTTGCGGGGAATGCACTGGAGAACCATGAAGATGTGGAAACA
 AACAAACAAACAAAAAACCGCTTTTGCATCTTCAGACATCTCACTTGTCATCACCAGCACAGTGCCATGCATGAGTGACC
 CATTGCAGGGA
->mh06KK-008 PermID=MHDBM-ed9ca745 GRCh38:chr6:169255933-169256152 variants=25,75,116,244 Xref=SI664725E
+>mh06KK-008 GRCh38:chr6:169255908-169256178 mh06KK-008.v1=25,75,116,244
 ATGACTCCACGTGCCGATGGGCAGGTACAGAGAAGATGGGCCTCCTTCTGTAAAATCTGGCAGCCCAGAATCAGGGAAGT
 CTGTTTAGAGGAGACAGAAGGTAAGCCGATTGGAACATGGCCCGTGAATGGGGTGTCCCCAGTTGAGAAAGTATTTCAGG
 CAGAGAGAGTGGGTAGGTGTTCATGGTGCAAAGAACAGCAGGCTCCTGGTGCGGCACCCAGGCCAGGTGCATGGAATGGG
 CTTCATAGACGATGGAAGTCACAGAGAGTT
->mh07CP-004 PermID=MHDBM-9f52aec1 GRCh38:chr7:16789069-16789114 variants=102,106,109,118,147 Xref=SI664886M
+>mh07CP-004 GRCh38:chr7:16788967-16789217 mh07CP-004=102,106,109,118,147
 TAGCATAGAAGGTCTTAAATTCTTTTTTACTTAGGCCTTTTCTGTTTTGCCATTATGTTTATTATTTTTATGGATGACAA
 CATAGTGCATTTTGTCTTTTTTTTTTTTTAATTTATTTTTTTTTATTGATCATTCTTGGGTGTTTCTCGCAGAGGGGGAT
 TTGGCAGGGTCATAGGACAATAGTGGAGGGAAGGTCAGCAGATAAACAAGTGAACAAAGGTCTCTGGTTTTCCTAGGCAG
 AGTGTGTGTG
->mh08KK-039 PermID=MHDBM-5078e94d GRCh38:chr8:3659269-3659481 variants=25,69,107,156,217,237 Xref=SI664905E
+>mh08KK-039 GRCh38:chr8:3659244-3659507 mh08KK-039.v1=25,69,107,156,217,237
 TATGAGAACATGATAACAAAGACTACCAAATTGCAGAGATGATCACCTTCTTGACAAATTGTGTAGTTATTGTTACAAAG
 AAACAAATTTTCATTTTGCACTTGCCAATCTAGTTTACTACCCACTGATGAAATTTTTCACTTAGACACAGGTAACGGGT
 CTCAGTGTTTAGAATCATTGTATAATTATCTGAGACACTACTTAGTTTTCAAATCTCCGAAACACAGAAGCAGATGCGTT
 TCACTTAGCCAAGGTCAAACTGT
->mh09KK-157 PermID=MHDBM-d57c98ab GRCh38:chr9:132987091-132987244 variants=48,64,132,161,201 Xref=SI664584H
+>mh09KK-157 GRCh38:chr9:132987043-132987293 mh09KK-157.v1=48,64,132,161,201
 GCTGGAGTTGGGTTGCTCAGAAAAACAGACTGGTCCAAAGTCTTCCCCGGGGTCTCCTCCTGGCCTCTTCTTGCCGCCGC
 CTGCTCTGGGCAGAGCCCGGGAGTGTGAGCCGCCAGAAGCAGCGGCACGTGGCTGTCTCTCTGGGCCTCCTCCTCCTAGG
 AAGGGCGTGCCCTCCTTGCTCCCTCTGGGCTTCCCAGAAACCGTGGCTATTGATGCTGATGGTCCTATCTCCCCACAGTG
 CCCAGAGACC
->mh10KK-163 PermID=MHDBM-195029a7 GRCh38:chr10:3120217-3120476 variants=25,38,101,140,284 Xref=SI664592G
+>mh10KK-163 GRCh38:chr10:3120192-3120502 mh10KK-163.v1=25,38,101,140,284
 GTTTTAAGACTCTGAAAATTTTTGATCTCACTCCCAGAGAGTTTTACCACCTCTTCTTCTGTGTGGCCACCAGGGGGACG
 TAGTGTGGCCGAGACTCCAGGGGTGCCCGTGAGCACCCGAGGCGCTGAGGAGGGCTGGGTCGCAGTCTCCTGTGATTGTA
 CCAGCATTAAAAATCGCTGTGTGTGTGTGTGTGTGTGTGTGTGTGTGCTGAGCCTAAATTTTCTTTGAGCCTCCAATACC
 CATTATGATGAACCCCTGCCTTGATGCTGAGGGTAGAAATTGAACTGAATATTTTATAATTTTATTCATT
->mh11KK-180 PermID=MHDBM-6d611fb7 GRCh38:chr11:1669560-1669753 variants=28,148,206,221 Xref=SI664598M
+>mh11KK-180 GRCh38:chr11:1669532-1669782 mh11KK-180.v1=28,148,206,221
 GGCAGAGGACCTGCCTGCTTTTCCTGATAAGACCTCGTTCCATTGCCCTAGGTCAGGCATGGATTATTAACTCTCAGGGT
 TTTGGGGGACCAGCAGCCACAGATGTGGAGTCCTGGGGAAAGGGTGACAGCCTCCTCTGCCTCCGGGGATTTGTCCTTCA
 GTGACTTGACGCCCGCAAGAGTGGATGCTAATTCTCACCGTCCCCATGAAATCCCTGCTGACGCATGCTGCCCAGGAGAC
 ATCTCCACAA
->mh12CP-008 PermID=MHDBM-003a7083 GRCh38:chr12:1996655-1996688 variants=108,111,141 Xref=SI664890H
+>mh12CP-008 GRCh38:chr12:1996547-1996797 mh12CP-008=108,111,141
 GGGACACCTTGGAAAGGGAAGAATTGTCTTGGGCCACACATAAAATACACTAATAATAGCTGATGAGCTAAAAAAAAAAA
 AAAAAAAAAAAAAAAAAAAAAAAAAAAACAACAAACTCTTCTAATGTTTTAAAGAAGTTTACGAATTTCTGTCAGGCTAC
 ATTCAAAGCCATCTTGGGCCACGTGTCCTATGGGCCGTGGGTTGGACAAGCTTGCGATAAAGCCTTCCATGATCACAGCA
 GCCCATTCAT
->mh13KK-218 PermID=MHDBM-d645f595 GRCh38:chr13:53486691-53486836 variants=52,106,117,197 Xref=SI664607D
+>mh13KK-218 GRCh38:chr13:53486639-53486889 mh13KK-218.v1=52,106,117,197
 TTACTTAGGTATATCCTTTATAATAAAACTGGAATCATAAGCATAGCACATTTCCAAGTTGTTCTAGTGAATTACTGAAC
 TGGATAGGATTGTGGAAACCTGTGAATAATAGCTAGGTAGTCAGAAGACATGGTGCGCTGGGGATCCTCAAAGTGTGGCT
 GTTAACTGAAATGAAGGTACTCTTGTGGAGGACTGAGCCCTTAACATGTGAGTTCTGCATTACTCTAGTTAGTGCTAGAA
 TTGAACTGAA
->mh14CP-003 PermID=MHDBM-64b4bc49 GRCh38:chr14:32686114-32686149 variants=107,131,142 Xref=SI664892J
+>mh14CP-003 GRCh38:chr14:32686007-32686257 mh14CP-003=107,131,142
 TTCACAATAGCCAAGCTTTGGAAGCAACTTAAGTGTCCATCAGCAGATGAATGTATAAAGAAAATATAGCACTTATACAT
 GATAGAGTACTATTCAGCCATAAAAAAGAATGAACTTCTGTCATTTGCAACGACGTGATGGAGCTGGAGGTCATTATGTT
 AAGTGAAATTCGCCAGGCACAAGAAGTGAAACATTGCATGGTCTCACTTTATTTTTTGGGATCTAAAAATCAGAACAGTT
 GAAATCATGG
->mh15CP-001 PermID=MHDBM-e74afe73 GRCh38:chr15:40076158-40076162 variants=123,125,127 Xref=SI664946J
+>mh15CP-001 GRCh38:chr15:40076035-40076286 mh15CP-001=123,125,127
 AACTTAAGGTAGCTCCTTACCTCACACGTGCTAGTTAGGCTAAATAATTATTATTTTTGAAAGGAAGCAATTTAAAAAGA
 AAGAAACGAGAAGAATGTATAGGTAAAGACTTGAAAAAAAAAATATATATATATATATATAGTCAAGACAGGGTCTTGCC
 ATGCTGCCCAGACCAGAGTGCAGTGGCTATTCACAGGCATGATCATGGTGTGCTACAGCCTTAAACTCCTGGGCTCAGGT
 GATCCTCCTGA
->mh16KK-049 PermID=MHDBM-9da28473 GRCh38:chr16:7159206-7159379 variants=38,77,97,141,211 Xref=SI664617E
+>mh16KK-049 GRCh38:chr16:7159168-7159418 mh16KK-049.v1=38,77,97,141,211
 GTTTCAAGTTGTTGCATGTGCTAATAGTTGATTGTCTTAGATTGCTGAGTAGTATTCTATGGTGTCAATCTACCACCCAA
 GAATCTTTTTTCAGTAGACACCCTGAGGCTGAGCAGGAGAGGGTGCCATTGTCACTGCGTCATGCCTATCCCAGAGACAG
 GGATTGAGAGGGGTGGCAAGCCCCTGGTGAACCTGCTTGGCTTACATGTATGTGCTGATATTTGAAAGAGAATCAGAAAC
 GGGACAGGAT
->mh17CP-001 PermID=MHDBM-9d093450 GRCh38:chr17:11308466-11308502 variants=107,133,143 Xref=SI664894L
+>mh17CP-001 GRCh38:chr17:11308359-11308610 mh17CP-001=107,133,143
 TGCCCAACCCTTCCTCCTAACCTCATATGTGCACAGGAATGCAGCAAATTAACCTCCTGGAAATGGCAGGAGCGTGGTTT
 TCTCCCTTCTGCATCCAAGGATACCAACGGAGCTTTCTCTTTTCCCCTCTACCAAAGGCCACAGTATCTCAGACTTCCCA
 GTACAATTTCCAGAGTGCTTTATTAAATAACTCACTAAACACCCCAGATACTGTGATCGGCTACGTTCGCTAAGCCCTCC
 TCATTTCACAA
->mh18CP-005 PermID=MHDBM-a85754d3 GRCh38:chr18:8892864-8892907 variants=103,132,135,146 Xref=SI664898P
+>mh18CP-005 GRCh38:chr18:8892761-8893011 mh18CP-005=103,132,135,146
 TGCACTCCAGCCAGGGCAACAGAATGAGATTCTGTCTCAAAAAATAAAAAATTAAAAAAAATTTTTTTAAACCCAAAATA
 TTACTGCAGATGTCCTTATACGCAGTGGTGTTAGTTTTAGAAACTGATTCTACGGGTATGCTTGCTCGTGTGTAAAATTA
 TTCATATACAAATTATTTATGACAGTATTGTTTCTAGTAGTAAAATATCGGAAATATTCTAAATGTTCATCAGTAGGAGA
 ATGGTCAAAT
->mh19KK-299 PermID=MHDBM-8cbeb11c GRCh38:chr19:22546697-22546850 variants=48,99,130,161,201 Xref=SI664630Z
+>mh19KK-299 GRCh38:chr19:22546649-22546899 mh19KK-299.v1=48,99,130,161,201
 CCATGTTACATTGGAAAAACATTCTCTATCATGTGGCCTGGCACAAGGGTTGGCAGCAACAGAGCAGACAGAACCAAAGG
 AAGAAGGGCCTGAAAAACCCGCTAGTGCATTTGGGCTGGCATTTTGTTACAGGAGGTTCTGATCCAATTTTAAATTCTGT
 ATTGCAGTCTAGTGAGGCAGCGAGAGTTCATTATCCCAACCGCAACCTACAGTCTACCAGGAGACATGCGACCCACCAGC
 TGGTATTTGA
->mh20KK-307 PermID=MHDBM-939f71a0 GRCh38:chr20:16532614-16532754 variants=55,111,137,195 Xref=SI664633C
+>mh20KK-307 GRCh38:chr20:16532559-16532810 mh20KK-307.v1=55,111,137,195
 CATTCAATTACCAAAGCATGTCCTGCTCAACAAGAGAACAAACCACCTGGGTTTATTTATATCACAGAACACCAAACCCA
 GATTCCTCCCATTCCCACAGTGGGTCCTTTTTTCTCAATCAATCACTAACCTAATGCATCTAGAGCTTTCATCTTAAAAC
 CACTATTATCAACAAATACCTCTCAGGAACACAAAATTATCCAGCTACATAGAAATATTAGAAGTGATCGTGGTAATGCT
 CACATTGACTT
->mh21KK-320 PermID=MHDBM-c41fae2b GRCh38:chr21:41642698-41642883 variants=32,102,191,217 Xref=SI664636F
+>mh21KK-320 GRCh38:chr21:41642666-41642916 mh21KK-320.v1=32,102,191,217
 GAGGCTGTGGAGAGGGTGTGTTTAGGATGGGCGACCTTTCCTGTGGGCTAAGGTAGGAAAGCAGAAAACAGTTAGTGTGA
 GATTCTTGGTGTCCTCAAGAGCAGCCTGTGTAACAGAAAAGACCGTTCTTAGTTCCTTCACTTTTGATTAACATCGAAGG
 TATTGTTTCACATTTCTAATGTCTAGTTTTCCTTGGGTTTTTAATAGCACTTTCAGGAAGACTTAATTCAATTAATGTTT
 GGCCAGGGGA
->mh22KK-061 PermID=MHDBM-798d33f6 GRCh38:chr22:44367725-44367871 variants=52,97,198 Xref=SI664638H
+>mh22KK-061 GRCh38:chr22:44367673-44367924 mh22KK-061.v1=52,97,198
 TGGGGACAGGTGTTTTACAGGCTCCTTTAGGGGTGGCAAGTCTCCCGGAAACGTGATTAGTGAAGACACATTAACAGCGA
 AACTGACAGAGAACCTCAACATTCTCTGGTAGGAAAAGCCAGGATCCTGGCAGAGGAAGCAACGATTCGAGCAGGGAACT
 GTGCAGGACAGAGAACAATGCGGCCCCAATTTTGATCCGGGGGTAATTAGCTTAGCTAAGGAGTTCCCCAGTCCCTAAGT
 GGAGAGGGGAT
-
```

### Comparing `microhapdb-0.7rc1/microhapdb/data/tests/panel-beta.fasta` & `microhapdb-0.9/microhapdb/tests/data/panel-beta.fasta`

 * *Files 26% similar despite different names*

```diff
@@ -1,251 +1,250 @@
->mh01KK-205 PermID=MHDBM-1f7eaca2 GRCh38:chr1:18396197-18396351 variants=48,69,157,202 Xref=SI664550A
+>mh01KK-205 GRCh38:chr1:18396149-18396400 mh01KK-205.v1=48,69,157,202
 ATGGGGTAATTTGGGGTCCAGAGCACCAGTTCTCATGAATCTGAGGAATTCTTCCTCCTAGCTACTTCCTTCCTTTTCCC
 TCATTACATCCCTGCCAAGGACAAATTCTGCCATTTGCATGGCAGGACTCCTCCAAAAAGGGGCTTCCTCCCTTTCCGTT
 AGTAAAGGAAGAGGTTACCTGAGACTTGACTTAACCTCCTTGGGAGGGAACATGCTTTCACTGTTGCGAATTGTTAAGTC
 AGGTCCAGAGT
->mh01CP-016 PermID=MHDBM-021e569a GRCh38:chr1:55559012-55559056 variants=103,141,147 Xref=SI664876L
+>mh01CP-016 GRCh38:chr1:55558909-55559160 mh01CP-016=103,141,147
 TGAGAGAGCCCAGTGACCTAAGCAGCTCCAACCCTGAGACTGGATCTAATGATGATCCAGATAATCCAGTGCCCAGCTTA
 GAGCCTGGCACACAACAAGTGCTTATAATGAAAGCATTAGTGAGTAAAAGAGTGATCCCTGGCTTTGAACTCCCTCTAAG
 TGTACCCCCAGGCATCTGTTCTTCCCTCAGTCACAATGCTGACCCCACTTCATGACTGGTCTCCTCTCCTTTGATTGTGC
 ACACAAGGGCC
->mh01KK-117 PermID=MHDBM-39dc025f GRCh38:chr1:204664211-204664397 variants=32,89,192,218 Xref=SI664549I
+>mh01KK-117 GRCh38:chr1:204664179-204664430 mh01KK-117.v1=32,89,192,218
 CCAGCTCTGTTTGTCTCCCCACAAAGCATTGCAGAAGAAAACACGGAAGCCGCCAGCACTATTATGCATTCATGATTCCA
 GCTTCAACCAGTCCTCTCTGCTGCAATCCCTTTATTCCTCCTCTGCAGCTGCCCCGGCACCTCTGCACAGTCCTTTTCTG
 AATCTGCCCCTCACCGTGCTCCCCACCTGCACGCCGTCCTCAGAACAGATTGCCTTGCCTGACCTCCTGAGGCCGACGGA
 GATGGTGATGT
->mh02KK-138 PermID=MHDBM-bc9ea531 GRCh38:chr2:45964843-45965091 variants=25,59,120,134,233,273 Xref=SI664911B
+>mh02KK-138 GRCh38:chr2:45964818-45965117 mh02KK-138.v1=25,59,120,134,233,273
 TTACTCTAATGCTGCTGTGCCTACCGTATCAAAGTCTGAGATTTTCACTTTTTTTTTCCTATGTAGTGAACACTAGCTGC
 AGTTTTGTTTTCATACCTGGACAGAGCATAAATCCTGCCATGAACACAGCAAAGATCATTCAGAAAGTGAAGAGGAAGGA
 GAAACAACGGTTCATGTTAAACTTGAGATGCTAATCTTGAAATGCCACCCGTTCTCTTCTGATTAGATTACATGCAGAAT
 AAAACATGCAGGCAATCTCAAACCTCTCCTCTCAGACGTTTCTGATTCTTATTGTGTGC
->mh02KK-136 PermID=MHDBM-eb83984f GRCh38:chr2:227227672-227227742 variants=90,107,160 Xref=SI664558I
+>mh02KK-136 GRCh38:chr2:227227582-227227833 mh02KK-136.v1=90,107,160
 CTGGGTCAGACTGTCTCACCTGAATTCAGATCCCCACTCCCCATGTTCCTTACTATCCTTAGCCTCTCAAAATCCTAGGT
 TTCTCATCTATTAGATGGAGCTTATAACAGTACCTCCCTTACAGAATTGTTGTAAGATATAATGAGATAATATGAGACAG
 CCAGCACTGAAAGTGCTCAAAACATACTGAGATCATTACAGTGCTGATGGAAGTTCATTTCCTCTACCACCATCCTGATC
 AAGGGATCCCG
->mh03CP-005 PermID=MHDBM-18771df9 GRCh38:chr3:15643038-15643049 variants=119,121,122,130 Xref=SI664935H
+>mh03CP-005 GRCh38:chr3:15642919-15643169 mh03CP-005=119,121,122,130
 TGGGAGGCTGAGGCAGGAGAATCACTTGAACCTGGGAGGCAGGAGTTGCGGTGAGAAAGATCGCGCCACTGCATTCCAGC
 CTGGACAACAGGAGCAAAACTCTGCCTCAAAAAAAAAAAAAAAAATAAAATAAAATAAAGAAATGGAATCCCTCAAAGGA
 TATGTACATTTTAAATTATATTAAAGAGTACCAAATTTCCCGCTTAAAAAACTTTGATTTCACTTTACAGCCCCAGTCAT
 ACAGTATGAG
->mh03KK-007 PermID=MHDBM-095cdb0b GRCh38:chr3:46310863-46310892 variants=110,139 Xref=SI664180Z
+>mh03KK-007 GRCh38:chr3:46310753-46311003 mh03KK-007=110,139
 ACTACAGCCTGGGGCCTGACTTCTTCTATGAAACCCTCGGAAGACTTCACTTATATTTGGTATCCAGCTTTCAGTTTGTT
 CTTGGCAGCCTGGACATTGAAAAGCTTTTCTTGAGCAATTATTTCCACTTGGTTATAGGTAGCCTTGATAACATCTCCAG
 CAGCTGCAGCCTGGAAGACAATGTACATCCTGAAGAGTCCAAAATTGGAGTAACTAGCATTAAAAACAGAAATAGCAAGT
 GGCTGGTGAA
->mh03KK-150 PermID=MHDBM-31ac28b1 GRCh38:chr3:131927127-131927311 variants=33,62,148,217 Xref=SI664563E
+>mh03KK-150 GRCh38:chr3:131927094-131927345 mh03KK-150.v1=33,62,148,217
 TTTACTATCTTATTTAATATTCATAACAACCTTGCAAATAGTCATCATCATTCCTATTTTACGGATGGGTAAATTAAGAT
 TCAAAGAATCTTTTTTGTTTTCTCGTTTGTTTTTTGGTTGGTTTTGTTTTGCTTTTCAGAGAGTCATGCATCTGTCTGTC
 ATCAAAGTCTTGTGTGTTTCCAACTGTGTTGGCTAAAATACAAAAGTTATCATTTAACATCCCTCTCTAATCTTTCAGTG
 GATCCCAGGCA
->mh04KK-030 PermID=MHDBM-1e252b7e GRCh38:chr4:3664642-3664756 variants=68,101,169,182 Xref=SI664727G
+>mh04KK-030 GRCh38:chr4:3664574-3664825 mh04KK-030.v1=68,101,169,182
 ACAGTGGTGTGGTCTGATTTGTGTCTTCTGCATTCACAGCTGAATATAGGCCCAGGGGCTTTCTGAACTGGACTCAGTGA
 CAAGGGCCTGACTCCCGGGCACGTGGTACTATTCTTACCACAGATGTCCGTGCTCAGAGCTGGGACATGGTCACTCCTGG
 GTAAGACACATTAGGTCCTTAACTAGGAGACACTCACTGGGGATTTTCTCGTGGTTCTGCTGTGCAAGTTGGAGGCAGTT
 GGGAGGTTGCC
->mh04KK-013 PermID=MHDBM-33a849c2 GRCh38:chr4:67578383-67578583 variants=25,103,115,180,225 Xref=SI664566H
+>mh04KK-013 GRCh38:chr4:67578358-67578609 mh04KK-013.v1=25,103,115,180,225
 TTGCAGTCATCTGAAATAAGCACTGCACTTTACCAAGTTGATGGATGCAGGTTCTTTATTTCAGCCAGTAACAGGTAAAA
 GTTAGAGGTTCAACTATTGTGTAGGGAAGTTATATGAGGCTAGAAAAGCGGACCAGTTAAAGATGTGAAGAACATGTTGA
 CTTCTGAGAGGGAGAGGAAGGAATCCTGGGGAATTGCACTCTTTCCCTCTGTTGTGGAAAATATCTCTGAGTGGTATGGT
 GCTTCCAATAC
->mh04KK-017 PermID=MHDBM-40955830 GRCh38:chr4:99400285-99400437 variants=49,179,201 Xref=SI664199J
+>mh04KK-017 GRCh38:chr4:99400236-99400487 mh04KK-017=49,179,201
 TGTTGGCTAATACACAGGAGATGGATGACTCCAGAGATGAAGAAAAGGGGCAGAAGATGAACATGGGGGATCACAAAGTG
 AAGGCCTTCTGTGTCTCAGAGTTGCCTAAACACCCTGCTTCCATATCAACCCTTCTATGAAAAGAACATGAGTCATTGGT
 GGGAATGGAGGACATGAATTGTTGGTGGGAGTGGTACTAATACCCACTATGTTTCATGACATGTGGAGAAAGCCAGTGTA
 TAGTGAAGTAA
->mh05KK-020 PermID=MHDBM-3175540a GRCh38:chr5:38881357-38881525 variants=41,119,184,209 Xref=SI664917H
+>mh05KK-023 GRCh38:chr5:38881316-38881567 mh05KK-023.v2=41,119,184,209
 TAGCTTCTGTTTTCTCTCCCGCTTATTCCACATGAGTCCCCGGGAATTGGAAGACCATAGTGATTGGAAGCTGAGTTTTC
 AAAAGGCAGGAGGTCATAGCTGGCTCCCATGCGAGGCATCAGAACATGGGGAATTGACTAGCAGAAGTGGAATTCACTGG
 CACATATCGTGGACCTGCAATGGGGTCTTAGGTTTGTGCTTTGGGATAAGTCAAGTCAAGCTATTTTATAGGACAAGATG
 GCTATGTGTCT
->mh06CP-007 PermID=MHDBM-994edf59 GRCh38:chr6:4383078-4383120 variants=104,123,146 Xref=SI664885L
+>mh06CP-007 GRCh38:chr6:4382974-4383225 mh06CP-007=104,123,146
 GTCATGGAGCCAGCAGGAATGAAGCAACTGGTGTCCAGTAGAGAAGAGGGAGAGAAACCTCGAGGTCTTAATTTCACAGA
 GGTTCTTGACACAGGGTGGGATTCATTGCTGTCTAAGAAGGGAACTTAGGATCTTGTGGAGTTTTGTTTTTTTTTTTTCT
 GAAGCTACTTCCTCAGTGTGTTGTTTGGCCAAAATCAGGAAGAAAATAAAACCTACCTGTTAGGGTATGTTGCACTCAGA
 AAACCTGGCTC
->mh06KK-008 PermID=MHDBM-ed9ca745 GRCh38:chr6:169255933-169256152 variants=25,75,116,244 Xref=SI664725E
+>mh06KK-008 GRCh38:chr6:169255908-169256178 mh06KK-008.v1=25,75,116,244
 ATGACTCCACGTGCCGATGGGCAGGTACAGAGAAGATGGGCCTCCTTCTGTAAAATCTGGCAGCCCAGAATCAGGGAAGT
 CTGTTTAGAGGAGACAGAAGGTAAGCCGATTGGAACATGGCCCGTGAATGGGGTGTCCCCAGTTGAGAAAGTATTTCAGG
 CAGAGAGAGTGGGTAGGTGTTCATGGTGCAAAGAACAGCAGGCTCCTGGTGCGGCACCCAGGCCAGGTGCATGGAATGGG
 CTTCATAGACGATGGAAGTCACAGAGAGTT
->mh07CP-004 PermID=MHDBM-9f52aec1 GRCh38:chr7:16789069-16789114 variants=102,106,109,118,147 Xref=SI664886M
+>mh07CP-004 GRCh38:chr7:16788967-16789217 mh07CP-004=102,106,109,118,147
 TAGCATAGAAGGTCTTAAATTCTTTTTTACTTAGGCCTTTTCTGTTTTGCCATTATGTTTATTATTTTTATGGATGACAA
 CATAGTGCATTTTGTCTTTTTTTTTTTTTAATTTATTTTTTTTTATTGATCATTCTTGGGTGTTTCTCGCAGAGGGGGAT
 TTGGCAGGGTCATAGGACAATAGTGGAGGGAAGGTCAGCAGATAAACAAGTGAACAAAGGTCTCTGGTTTTCCTAGGCAG
 AGTGTGTGTG
->mh07KK-030 PermID=MHDBM-30e2d2b6 GRCh38:chr7:53594403-53594500 variants=76,110,173 Xref=SI664578K
+>mh07KK-030 GRCh38:chr7:53594327-53594577 mh07KK-030=76,110,173
 TTGGTAAGTTGAGTACATAACAGTTCCTACCTCTGTGTTGAAAGAGGATTGAATAAGATAATGCATTTAACATAATGCCT
 GACATATAGTAAGAATTCCATAACTCTGAGATAATTATAGTTTTACTACAGGAAGCATCTGGATATAAATTTTCTACCAT
 TTCTCATTATGTGCCCCCATTATATTTCCTTAGGACTGCATAAAAGCCTTTATTCATGAATACATTTCAATAATTTGATG
 AATCACTTAA
->mh07KK-031 PermID=MHDBM-b88f697f GRCh38:chr7:97104659-97104744 variants=82,167 Xref=SI664227B
+>mh07KK-031 GRCh38:chr7:97104577-97104827 mh07KK-031=82,167
 AGATGCGTGGAGAGAGAAAAGTCTTTGGAGAAAACTGATGAGTTTAGCTTGGAACAGAGACTCTGAAAGGATGACAGGAC
 ACCCAGTTTGGACTTATCCTGTGGTTATATAGAGAGCAAGACTCTTAACTGTGGAGAGGTCAGAGGTGTGTGTATGAGGC
 TTGGAACAGCTTTTTGAGAAGCTATGCTGGCGGTTTTCCAGATAAGGGTCCAGTGAGGCCTTTGAAGTGGTTAGAATGGG
 CTTGGCCAGG
->mh08KK-039 PermID=MHDBM-5078e94d GRCh38:chr8:3659269-3659481 variants=25,69,107,156,217,237 Xref=SI664905E
+>mh08KK-039 GRCh38:chr8:3659244-3659507 mh08KK-039.v1=25,69,107,156,217,237
 TATGAGAACATGATAACAAAGACTACCAAATTGCAGAGATGATCACCTTCTTGACAAATTGTGTAGTTATTGTTACAAAG
 AAACAAATTTTCATTTTGCACTTGCCAATCTAGTTTACTACCCACTGATGAAATTTTTCACTTAGACACAGGTAACGGGT
 CTCAGTGTTTAGAATCATTGTATAATTATCTGAGACACTACTTAGTTTTCAAATCTCCGAAACACAGAAGCAGATGCGTT
 TCACTTAGCCAAGGTCAAACTGT
->mh08KK-032 PermID=MHDBM-90c91a19 GRCh38:chr8:11738319-11738459 variants=55,195 Xref=SI664183C
+>mh08KK-032 GRCh38:chr8:11738264-11738515 mh08KK-032=55,195
 AAACAATGAGAAGTCCTTCCGTGAGCCACCAAGACACCTCCCTGGAAACAACCAGCATGATCAGTTTCTTGTCTGTCCTC
 CTAAAAATGTTCATTCTGTATATAAACAAATCCATGTATAGATTCTTCTCCCCTTCTTTTTGTAAGAGAATATCAATGTA
 ATGTCCATGCCTTCTAATATTTCATAGCATATACTGCAAGAATTCCATATCAGTACATCAAGATCATTGTTTATGGCTAC
 ATAGTGTGCCT
->mh09KK-033 PermID=MHDBM-8458b727 GRCh38:chr9:680713-680790 variants=86,135,163 Xref=SI664581E
+>mh09KK-033 GRCh38:chr9:680627-680877 mh09KK-033.v1=86,135,163
 GCAAAAATTTCTGCCCTCAAGGATTGTACATTCTAGGGACAGTTAAAGTCTCCTGTGTACACGGTTGCCAGAAGAAAAAA
 TACTAAGCACGTGTTCATCGTTTATCTAAAATTCGGTTTAATGGTGCTCCACTTTCGTGCGCGGCCCTACCTGTGTACCC
 CTTGCAGATTGCACCCCTGCCCTTCCTCACCGCCAGCCCATCAAAATCAATCTTCCCTCGTAGTGTTACCTCTTTTTCAC
 CAGATCCTCC
->mh09KK-153 PermID=MHDBM-1651deb9 GRCh38:chr9:101207457-101207569 variants=69,104,181 Xref=SI664583G
+>mh09KK-153 GRCh38:chr9:101207388-101207639 mh09KK-153.v1=69,104,181
 CTTCAAACCCTTTATTCCTTAGTTCAGTTTTTTTCAAAGCCCGAATGGGGATTGGCAGTCTTCATGCTCTGAACAATTGG
 GTATTCTTTTTTCTTAGAGCCCAGATGCATTTTTTTGAAAGTCGTTCCAGGGGCCTGAGATGAAGTGGGGGTGTGAGAAG
 TAAGTTGGCTAGGGCAGATAGAACCTAAGTGTCTTCTCCTTAAGTCAGCTCCCCTTACGAGGCTGTATGATACTGGGCCA
 CCCCCATTCAC
->mh09KK-157 PermID=MHDBM-d57c98ab GRCh38:chr9:132987091-132987244 variants=48,64,132,161,201 Xref=SI664584H
+>mh09KK-157 GRCh38:chr9:132987043-132987293 mh09KK-157.v1=48,64,132,161,201
 GCTGGAGTTGGGTTGCTCAGAAAAACAGACTGGTCCAAAGTCTTCCCCGGGGTCTCCTCCTGGCCTCTTCTTGCCGCCGC
 CTGCTCTGGGCAGAGCCCGGGAGTGTGAGCCGCCAGAAGCAGCGGCACGTGGCTGTCTCTCTGGGCCTCCTCCTCCTAGG
 AAGGGCGTGCCCTCCTTGCTCCCTCTGGGCTTCCCAGAAACCGTGGCTATTGATGCTGATGGTCCTATCTCCCCACAGTG
 CCCAGAGACC
->mh10CP-003 PermID=MHDBM-ff317646 GRCh38:chr10:24304121-24304146 variants=112,118,137 Xref=SI664887N
+>mh10CP-003 GRCh38:chr10:24304009-24304259 mh10CP-003=112,118,137
 AGTATTCAGACCAAATATAAGTAAATTAGCATAAATCAGCATTCTCTGATTTCCACGCCTACTTACCCAAGTTGGTTGAC
 TCAACAGCTGCTAAGACTACAGCTGTGTGAATCCTCCACATTTTTTTTTTTTTTTGCATGGAAAAGTGTTTCAGTTTGTC
 ATTGCTTCATCATTTCGAATTCCATATTAGGTTACCTTTTTTTTTTTTTTTTTGCCTGACCATAGTACTTAAGAAAAATC
 TTGCAACTGT
->mh10KK-170 PermID=MHDBM-a362392e GRCh38:chr10:77150283-77150472 variants=30,62,219 Xref=SI664728H
+>mh10KK-170 GRCh38:chr10:77150253-77150503 mh10KK-170.v1=30,62,219
 GATTATCCAATTAGAGAATGAAATAGGCCAGCCCTGTCTTCCTTCTTCTTCCATCAAATGCCATTCTTGTAGCCATTTCA
 CTGACAACATGAGGGGCCAACAGAAGAAATAAACAGGCATAAATTTCAAACCCAGGAAATTTATGTGAGCAAAGGGAAAG
 AATCCAGATATATAAAATGAATTAATCATCAATAAGTCACCACATCCCTATTACATGGTAAGTTCTTTTCTGGGAGCTGT
 TAGGGCCAGA
->mh10KK-101 PermID=MHDBM-32587a6d GRCh38:chr10:133533422-133533454 variants=109,141 Xref=SI664591F
+>mh10KK-101 GRCh38:chr10:133533313-133533564 mh10KK-101=109,141
 CTTGTCCTTTCCTATGGCTTGTGGCTCAAGAACAAATGTGGAGCCCACACTGATTTCCCAGGACTGTCTGAGCATCTTCT
 CCACCAGTTTGGCCCCTCGTGGCAGCAGACACTAGCCCTGTAGCAGGAGGGGTTAGCAGGAGCCGTTTAGCTCCTGCCTG
 AGCTATGACCAAGGTCAGGGGGATCTCACCTCTCCCAGGATGGCCCTCATGCTGTGGAGGGAGACAGAGCCCTGGCCTGC
 CCTCAGCAGAT
->mh11KK-180 PermID=MHDBM-6d611fb7 GRCh38:chr11:1669560-1669753 variants=28,148,206,221 Xref=SI664598M
+>mh11KK-180 GRCh38:chr11:1669532-1669782 mh11KK-180.v1=28,148,206,221
 GGCAGAGGACCTGCCTGCTTTTCCTGATAAGACCTCGTTCCATTGCCCTAGGTCAGGCATGGATTATTAACTCTCAGGGT
 TTTGGGGGACCAGCAGCCACAGATGTGGAGTCCTGGGGAAAGGGTGACAGCCTCCTCTGCCTCCGGGGATTTGTCCTTCA
 GTGACTTGACGCCCGCAAGAGTGGATGCTAATTCTCACCGTCCCCATGAAATCCCTGCTGACGCATGCTGCCCAGGAGAC
 ATCTCCACAA
->mh11KK-037 PermID=MHDBM-2cddd3a7 GRCh38:chr11:72558169-72558302 variants=58,146,191 Xref=SI664594I
+>mh11KK-037 GRCh38:chr11:72558111-72558361 mh11KK-037=58,146,191
 GGCATATGCTAAACTAGAGAGACAGAGGGAAACTAGTTTTCCATCTCACCAGGCATCAGATAAGAAGGTGGAATGCCCTG
 ACTCCAGGTAGGGACACATTCTTGGTGATAGATCAGGAGCTGGAGAAAGAGACTTCCACCAGGGACCCTTCTCTTCCAAG
 GAAGTATGTTAAGTTTAAACCCTAAAGACAATAATATAGTGGCTAATTTAAAATGTTTTCCCTATCTCTACATTATGATT
 TCTTTCCTGT
->mh11KK-191 PermID=MHDBM-c19be300 GRCh38:chr11:100009430-100009619 variants=30,91,149,219 Xref=SI664600W
+>mh11KK-191 GRCh38:chr11:100009400-100009650 mh11KK-191.v1=30,91,149,219
 ACCCATAGGGAAACAAAGGTATGTAAAGGCTTGGGTAACACAGCAAAGTGTAAAAAAAAAAATGGAGGGGGATTAATTAG
 TTGGAAAGAAAAGACTGGTTTAGACATATGGAAGGTTATTATCAAGAGATTGCTCACAAGCTGTTCTCCAGTTTCAACAA
 GGGAGGGAGTGAAATTCCAACAGTATGGGATTAAACTAGAAGAATTAGATTGGGTGTAATGTAGAAGTTCATGAAAAAAT
 GAGTTGTTAC
->mh12CP-008 PermID=MHDBM-003a7083 GRCh38:chr12:1996655-1996688 variants=108,111,141 Xref=SI664890H
+>mh12CP-008 GRCh38:chr12:1996547-1996797 mh12CP-008=108,111,141
 GGGACACCTTGGAAAGGGAAGAATTGTCTTGGGCCACACATAAAATACACTAATAATAGCTGATGAGCTAAAAAAAAAAA
 AAAAAAAAAAAAAAAAAAAAAAAAAAAACAACAAACTCTTCTAATGTTTTAAAGAAGTTTACGAATTTCTGTCAGGCTAC
 ATTCAAAGCCATCTTGGGCCACGTGTCCTATGGGCCGTGGGTTGGACAAGCTTGCGATAAAGCCTTCCATGATCACAGCA
 GCCCATTCAT
->mh12KK-202 PermID=MHDBM-29c66960 GRCh38:chr12:30017295-30017448 variants=48,125,178,201 Xref=SI664604A
+>mh12KK-202 GRCh38:chr12:30017247-30017497 mh12KK-202.v1=48,125,178,201
 CCTCTCCACCACCCACCTCTTCAAGGTATTTCCAGTACCCAGTACAAAATTCTATTGTTGGTCTTAACTCACTGCTTTCT
 ATCGTTTATGTTGCTGTGTTTTCTGTTACTATGTAAGTTTCTTTGGGGCATGCACCATCTATTCAAATTTCTCATCTCAG
 GAGCAGGCACATACCTAATAGGTCCTCAATAACGATCGTCCTACCACATCAATAACAATGTGATATGCTAGGAAAAATCA
 GTGGCTCAGG
->mh12KK-046 PermID=MHDBM-8a9913c2 GRCh38:chr12:118451682-118451753 variants=89,160 Xref=SI664189I
+>mh12KK-046 GRCh38:chr12:118451593-118451843 mh12KK-046.v1=89,160
 GAAGATTTGGGACATGGTTAAAATTAGAATGATGTCATCTCAAGTTTCCAAATAGGAACACTGGTATAGGAGGAGATCAT
 TTAAAAATCTGGTAGCCTGGTGGAAGGGAGGTAGCAGAACCAATGCTGATTGGGACAGGAGATTATTTCACAAATAATTC
 GTAACCTAGGTTTCTTAGAAATAAAGGTTCAGAAAAAAGCTATACCTTTACAACACAAAGGAAACAACCCTCCATGCCCC
 TGAATCCATC
->mh13KK-213 PermID=MHDBM-d5615acf GRCh38:chr13:23191401-23191541 variants=55,149,195 Xref=SI664605B
+>mh13KK-213 GRCh38:chr13:23191346-23191597 mh13KK-213.v1=55,149,195
 TGAAGAAGGAAAGGAAGAGGAGAGACAGCAAGGAGAACTTCAGTTGTCAAGGTATCGGGTGCAGGGGTCAGAAAGAAACA
 TGACTCCATGGACCACTGCTTGGCCCAAGACCAGATGTCAAAACCACAGAGCCCTGCTGTAGAGCATTACAAATGTATTC
 CACCAAATGTTGGGATGCATCCTAGACCTGTGCTGGCCAGCAGTCCCCAGCTGTGAGGAGAAGCCCGCCATTTGAGTTGA
 TCACTTGGCAG
->mh13KK-223 PermID=MHDBM-4088f2e4 GRCh38:chr13:110154351-110154504 variants=48,91,108,201 Xref=SI664608E
+>mh13KK-223 GRCh38:chr13:110154303-110154553 mh13KK-223.v1=48,91,108,201
 ATGAGTGTATCAAACAGGGGCCTTGTTTTCTGTTTCAGTTGGCTTTTGTGGGAAAGGGAAGCCCTGGGGCTAGGAGAGCA
 GTCCTTGCCCTCTGGGAAGGGTCCCAGGCGGCACTGCCCCAGGAGGGCCTTCGTGGAGGCCACGGCCAGCCCTCGGGTGT
 TCTCTCCCTAACTCAAGCTTCTGCTTTCAAGCTCGTGCATGTTGTAGTAGAATGTGTACTCCCCACGTGGAGGCTCTCTT
 CCTCCTTTCC
->mh14CP-003 PermID=MHDBM-64b4bc49 GRCh38:chr14:32686114-32686149 variants=107,131,142 Xref=SI664892J
+>mh14CP-003 GRCh38:chr14:32686007-32686257 mh14CP-003=107,131,142
 TTCACAATAGCCAAGCTTTGGAAGCAACTTAAGTGTCCATCAGCAGATGAATGTATAAAGAAAATATAGCACTTATACAT
 GATAGAGTACTATTCAGCCATAAAAAAGAATGAACTTCTGTCATTTGCAACGACGTGATGGAGCTGGAGGTCATTATGTT
 AAGTGAAATTCGCCAGGCACAAGAAGTGAAACATTGCATGGTCTCACTTTATTTTTTGGGATCTAAAAATCAGAACAGTT
 GAAATCATGG
->mh14KK-048 PermID=MHDBM-74c13a43 GRCh38:chr14:73783853-73784011 variants=46,204 Xref=SI664190A
+>mh14KK-048 GRCh38:chr14:73783807-73784058 mh14KK-048.v1=46,204
 TGCCAGCCGTGGTGTCTGGAAAACTGTAGCGTGTTCTTAAGCGACTAGAATGCCCTCTTTAGCTGGGGGTGTTCGGCCTC
 CTTTTTTGGAGGTGGGTTGTGATGTCAAAACACTGGGTTGTGGTATAGGAAGTGGGGCAGCTAGGAAGGGGCAGATTAAT
 GGAAATAGCAATACTGGGCCTGGGCAGCCTCCCTTTGAAGACCACCCTCTCCAGGAGACTCCTGCATTGGCTTCTCTCAG
 TGGCACCTCGG
->mh15KK-069 PermID=MHDBM-b18948cd GRCh38:chr15:27984950-27985037 variants=81,168 Xref=SI664916G
+>mh15KK-069 GRCh38:chr15:27984869-27985119 mh15KK-069=81,168
 GCCCCACTGCTTGTAGCATGTACTGCAGTCACACAAAGCAGACACGAGCTGGACTGGAATGCAGTGAGCTGTGGGCTCAA
 CCGCCCCCACCTTTTCATGCACCTGAGAATGGAACCTGGAGCCAGGCAGTGCAGGCAGAGCCCCTGCCTGCCAGAACCTG
 GCCGCAACTCCCACGGCAGAGGTGCTTTGCGTACCTTATGGTCACAGGCGTGAAGAGGAGCATGGTGGTGACGTTGTCCA
 AGAAGGCAGA
->mh15KK-104 PermID=MHDBM-10729ce3 GRCh38:chr15:63806357-63806494 variants=56,112,193 Xref=SI664616D
+>mh15KK-104 GRCh38:chr15:63806301-63806551 mh15KK-104=56,112,193
 AATCTTTACCTGTCAAAATCCACACTTTTCCTTCAAAGGCCTATCTCAAAGGTGACTTCTTCCATGAAGCTTTTCATGTT
 GTAATCACCCTACGCTCACCAACACAGATTTACTCACTTCCTCCTCTAACTCTCTTACTTTTGCTTACACACATGTACAT
 TTATCATACTCTGCCTGGTTTGTTATTATTTGCGTACCTGTCTTCATCACTACTGCTCCATCCACCCCACAACCAGACTC
 ATGCTTTGCA
->mh16KK-255 PermID=MHDBM-d61ecba6 GRCh38:chr16:81936747-81936889 variants=54,67,108,196 Xref=SI664619G
+>mh16KK-255 GRCh38:chr16:81936693-81936944 mh16KK-255.v1=54,67,108,196
 CCTGTTGCTGTGTGAGGGCTTTCTGCTCAGACTTTCTTCCAGAGACATTTACATGCTGGCATAACTAACATACACAAACT
 TCTGGACACAAAGTGATCGCATAAATCACGGGGCTTTGTGCTTTTGTTGTTGTTATTTAAGACCTCTTTCGAGGGATCTA
 TTCATCAGTAGCCTCCTTTACATTCTTTTTATAGCCACATCGGATTCCACAGAATGGAACAATCATTTATTTAATAAGTC
 CCCGTGGAGGC
->mh17CP-001 PermID=MHDBM-9d093450 GRCh38:chr17:11308466-11308502 variants=107,133,143 Xref=SI664894L
+>mh17CP-001 GRCh38:chr17:11308359-11308610 mh17CP-001=107,133,143
 TGCCCAACCCTTCCTCCTAACCTCATATGTGCACAGGAATGCAGCAAATTAACCTCCTGGAAATGGCAGGAGCGTGGTTT
 TCTCCCTTCTGCATCCAAGGATACCAACGGAGCTTTCTCTTTTCCCCTCTACCAAAGGCCACAGTATCTCAGACTTCCCA
 GTACAATTTCCAGAGTGCTTTATTAAATAACTCACTAAACACCCCAGATACTGTGATCGGCTACGTTCGCTAAGCCCTCC
 TCATTTCACAA
->mh17KK-052 PermID=MHDBM-c36ecfec GRCh38:chr17:45394954-45395140 variants=32,218 Xref=SI664191B
+>mh17KK-052 GRCh38:chr17:45394922-45395173 mh17KK-052=32,218
 GAGGCCTGAGGAGGATAGCTTCAGCAGCCCACACTGAAGGCTGGGTCAGTCCTGTTTCCACAGTGGGGAAGTGATCAGAG
 CTGCCTCATGACTGGCACAGTGCCAGCACAGGGCCAGGGCCCACAGGGTCTCTGTGAAGGCCTCCACGAGGTGAGGGCCA
 GAAGCAGCCAGGAAGCCCTCCATCAAACTCCTCCTCCCAGCACCTACCATTCCAGAAAACAAACTCTCACCCCCACACAC
 GCTATCGCACA
->mh17KK-055 PermID=MHDBM-97f41f6a GRCh38:chr17:78232489-78232548 variants=95,154 Xref=SI664231W
+>mh17KK-055 GRCh38:chr17:78232394-78232644 mh17KK-055.v1=95,154
 GACAGCCCAAGGGCTACAGGAGGGAGGGAGCCCAGTTCGGGGCCCCTCACAGCCGGAGGAGGGGGCTGTGGGGCGACAGT
 GGGGGAGGGAAGCCTAGAGGTGTGTAGTTGGGGGGCCTCATCCAAGTCACCAGGGGTTGTTTCTTGATCACGCTCCCCGG
 GGTTTGGGCCTGGCAGCCCCTTGTCCCCGTCCCTGTCAGGCACTGTCAGAGCTGTTCACCCCACACCTCCTGATGCCGCG
 GGGGCAGGGG
->mh18CP-005 PermID=MHDBM-a85754d3 GRCh38:chr18:8892864-8892907 variants=103,132,135,146 Xref=SI664898P
+>mh18CP-005 GRCh38:chr18:8892761-8893011 mh18CP-005=103,132,135,146
 TGCACTCCAGCCAGGGCAACAGAATGAGATTCTGTCTCAAAAAATAAAAAATTAAAAAAAATTTTTTTAAACCCAAAATA
 TTACTGCAGATGTCCTTATACGCAGTGGTGTTAGTTTTAGAAACTGATTCTACGGGTATGCTTGCTCGTGTGTAAAATTA
 TTCATATACAAATTATTTATGACAGTATTGTTTCTAGTAGTAAAATATCGGAAATATTCTAAATGTTCATCAGTAGGAGA
 ATGGTCAAAT
->mh18KK-293 PermID=MHDBM-13ed6da8 GRCh38:chr18:78329885-78329967 variants=84,105,143,166 Xref=SI664628G
+>mh18KK-293 GRCh38:chr18:78329801-78330052 mh18KK-293.v1=84,105,143,166
 CACCTCCACCCGTGGCTTGTTGGGGGAAAGTACCAGATGGGTCAGATTCTGTGACCACCCACTGAAGTTTGAGCAGAACT
 GGAGAGCAGGTGGATTAAATCTGGGTGGTGACTCCAGCACATCTCTAATGAACACTTCTTAACGTTTAATTTCAAAGGGC
 CTGGTGACCCTCGGATGTGTCAGTGTGGAGAAGAGATAGGTATCCATAGCCTTGATTAGGATCACATGCCAGTTACCCAG
 AAATATAACAG
->mh19KK-299 PermID=MHDBM-8cbeb11c GRCh38:chr19:22546697-22546850 variants=48,99,130,161,201 Xref=SI664630Z
+>mh19KK-299 GRCh38:chr19:22546649-22546899 mh19KK-299.v1=48,99,130,161,201
 CCATGTTACATTGGAAAAACATTCTCTATCATGTGGCCTGGCACAAGGGTTGGCAGCAACAGAGCAGACAGAACCAAAGG
 AAGAAGGGCCTGAAAAACCCGCTAGTGCATTTGGGCTGGCATTTTGTTACAGGAGGTTCTGATCCAATTTTAAATTCTGT
 ATTGCAGTCTAGTGAGGCAGCGAGAGTTCATTATCCCAACCGCAACCTACAGTCTACCAGGAGACATGCGACCCACCAGC
 TGGTATTTGA
->mh19KK-057 PermID=MHDBM-eb558c37 GRCh38:chr19:51654948-51655062 variants=68,145,182 Xref=SI664629H
+>mh19KK-057 GRCh38:chr19:51654880-51655131 mh19KK-057=68,145,182
 GGTGGGGACATGAGCTGGTGTTCTCTTTTGATAGATGGGACCCCAGCAGCCTGGTGACAGCAGACATACAGCCGGTACCA
 GGTTCTGTGGCGTGGAGATGGATGGTGGAGATTAATGTCCCATGTAGGTTGCTCTGTTAGGGCTCTGCCTACTGGACCTG
 GTGAGCTCAGCATTTTTGACACGTCTTTTGGGACCATTCACTACTGCTTTCCCCAAACTTTCTGTATGTTTTACACAATA
 TCACTGGATTA
->mh20KK-307 PermID=MHDBM-939f71a0 GRCh38:chr20:16532614-16532754 variants=55,111,137,195 Xref=SI664633C
+>mh20KK-307 GRCh38:chr20:16532559-16532810 mh20KK-307.v1=55,111,137,195
 CATTCAATTACCAAAGCATGTCCTGCTCAACAAGAGAACAAACCACCTGGGTTTATTTATATCACAGAACACCAAACCCA
 GATTCCTCCCATTCCCACAGTGGGTCCTTTTTTCTCAATCAATCACTAACCTAATGCATCTAGAGCTTTCATCTTAAAAC
 CACTATTATCAACAAATACCTCTCAGGAACACAAAATTATCCAGCTACATAGAAATATTAGAAGTGATCGTGGTAATGCT
 CACATTGACTT
->mh20KK-058 PermID=MHDBM-a5b17521 GRCh38:chr20:50227722-50227827 variants=72,105,177 Xref=SI664632B
+>mh20KK-058 GRCh38:chr20:50227650-50227900 mh20KK-058.v1=72,105,177
 GGTGTGGTGATGACTGAGAGATGATGCAGATGAAGTATATAGAGCAGGGCCAGGCATATAGCTGGTGCACAATACATGCT
 AGCTATTTTCATTCTTACTAGTGGCATAGTAGAAAGCACTGGAATTTTAGCTTCAGACAGACCTGGGTGTACATTTCAGT
 GTTCTGCATCTCCCTGTTCTTGAGCAAGCTCCTCGCCTGTTTGAGCCTCAGTGTTCTCACCTGGACTTGGAGATGGTTTC
 ACTTCATGAG
->mh21KK-315 PermID=MHDBM-e965ffea GRCh38:chr21:20507773-20507918 variants=52,157,197 Xref=SI664634D
+>mh21KK-315 GRCh38:chr21:20507721-20507971 mh21KK-315.v1=52,157,197
 CAGGCAGAAAGCTTATGTGGTAGGAGCCTAAAAGAAGGTCACAGACCTATAGGGTAGGGTTTTCAGGAGGGCTTAGCTGA
 CTTCAGCTGAAATGCTCAGGTTGGGGCAGGGTGTTGGAGGTGTGAGAAAGCCTTCAGCTTCTCTGTTCCCTCCCTAGCCT
 GAGGGCAGTGGTGGCAGGGGCCTTCCACAGTCACAGCTGCACTGCCCCAAAGTGTTCAGGCAGGGGTGGGGCGGGTGCAC
 TGGGAGTCCA
->mh22KK-060 PermID=MHDBM-e1ccbf64 GRCh38:chr22:19963683-19963747 variants=93,157 Xref=SI664251Y
+>mh22KK-060 GRCh38:chr22:19963590-19963841 mh22KK-060.v1=93,157
 GGAGCACCAGCCCTCCGTGCTGCTGGAGCTGGGGGCCTACTGTGGCTACTCAGCTGTGCGCATGGCCCGCCTGCTGTCAC
 CAGGGGCGAGGCTCATCACCATCGAGATCAACCCCGACTGTGCCGCCATCACCCAGCGGATGGTGGATTTCGCTGGCGTG
 AAGGACAAGGTGTGCATGCCTGACCCGTTGTCAGACCTGGAAAAAGGGCCGGCTGTGGGCAGGGAGGGCATGCGCACTTT
 GTCCTCCCCAC
->mh22KK-061 PermID=MHDBM-798d33f6 GRCh38:chr22:44367725-44367871 variants=52,97,198 Xref=SI664638H
+>mh22KK-061 GRCh38:chr22:44367673-44367924 mh22KK-061.v1=52,97,198
 TGGGGACAGGTGTTTTACAGGCTCCTTTAGGGGTGGCAAGTCTCCCGGAAACGTGATTAGTGAAGACACATTAACAGCGA
 AACTGACAGAGAACCTCAACATTCTCTGGTAGGAAAAGCCAGGATCCTGGCAGAGGAAGCAACGATTCGAGCAGGGAACT
 GTGCAGGACAGAGAACAATGCGGCCCCAATTTTGATCCGGGGGTAATTAGCTTAGCTAAGGAGTTCCCCAGTCCCTAAGT
 GGAGAGGGGAT
-
```

### Comparing `microhapdb-0.7rc1/microhapdb/tests/test_marker.py` & `microhapdb-0.9/microhapdb/tests/test_marker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,594 +1,701 @@
-# -----------------------------------------------------------------------------
-# Copyright (c) 2019, Battelle National Biodefense Institute.
+# -------------------------------------------------------------------------------------------------
+# Copyright (c) 2019, DHS.
 #
-# This file is part of MicroHapDB (http://github.com/bioforensics/microhapdb)
-# and is licensed under the BSD license: see LICENSE.txt.
-# -----------------------------------------------------------------------------
+# This file is part of MicroHapDB (http://github.com/bioforensics/MicroHapDB) and is licensed under
+# the BSD license: see LICENSE.txt.
+#
+# This software was prepared for the Department of Homeland Security (DHS) by the Battelle National
+# Biodefense Institute, LLC (BNBI) as part of contract HSHQDC-15-C-00064 to manage and operate the
+# National Biodefense Analysis and Countermeasures Center (NBACC), a Federally Funded Research and
+# Development Center.
+# -------------------------------------------------------------------------------------------------
 
 
-from io import StringIO
+from collections import defaultdict
 import microhapdb
-from microhapdb.marker import standardize_ids
-import pandas
+from microhapdb import Marker, Locus
 import pytest
 
 
 def test_standardize_ids():
-    assert list(standardize_ids(['FakeIdentifier']).values) == []
-    assert list(standardize_ids(['mh11KK-089']).values) == ['mh11KK-089']
-    assert list(standardize_ids(['SI664625D']).values) == ['mh17KK-110']
-    assert list(standardize_ids(['MHDBM-19b49670']).values) == ['mh11KK-187']
-    assert list(standardize_ids(['MHDBM-07c8d144']).values) == ['mh04KK-010', 'mh04AT-10']
-    assert list(standardize_ids(['rs9925859']).values) == ['mh16PK-83544']
-    assert list(standardize_ids(['rs1533623']).values) == ['mh01KKCS-205', 'mh01KK-205', 'mh01AT-02']
-    assert list(standardize_ids(['rs4697751', 'SI664918I', 'MHDBM-22a6ab26']).values) == ['mh04CP-007', 'mh05KK-123', 'mh11KK-092']
+    assert Marker.standardize_ids(["FakeIdentifier"]) == []
+    assert Marker.standardize_ids(["mh11KK-089"]) == ["mh11KK-089"]
+    assert Marker.standardize_ids(["rs9925859"]) == ["mh16PK-83544"]
+    assert Marker.standardize_ids(["rs1533623"]) == [
+        "mh01KK-205.v1",
+        "mh01KK-205.v2",
+        "mh01KK-205.v3",
+        "mh01KK-205.v4",
+        "mh01KK-205.v5",
+    ]
+    assert Marker.standardize_ids(["mh05KK-123", "rs4697751"]) == [
+        "mh04CP-007",
+        "mh05KK-123",
+    ]
 
 
 def test_assumptions():
-    assert len(microhapdb.markers) == 198 + 15 + 40 + 26 + (11 - 1) + 10 + 118 + 90
+    total_markers_per_source = [
+        11,  # Chen2019
+        22,  # Fan2022
+        90,  # Gandotra2020
+        26,  # Hiroaki2015
+        23,  # Jin2020
+        198,  # Kidd2018
+        20,  # Kureshi2020
+        90,  # Pakstis2021
+        45,  # Staadig2021
+        36,  # Sun2020
+        89,  # Turchi2019
+        10,  # Voskoboinik2018
+        59,  # Wu2021
+        703,  # Yu2022G1,
+        301,  # Yu2022G2,
+        337,  # Yu2022G3,
+        190,  # Yu2022G4,
+        21,  # Zou2022
+        118,  # delaPuente2020
+        15,  # vanderGaag2018
+        988,  # Zhu2023
+    ]
+    redundant_markers_per_source = [
+        1,  # Chen2019
+        2,  # Gandotra2020
+        5,  # Kureshi202
+        13,  # Pakstis2021
+        9,  # Staadig2021
+        6,  # Sun2020
+        84,  # Turchi2019
+        3,  # Yu2022G1
+        296,  # Yu2022G2
+        85,  # Yu2022G3
+        64,  # Yu2022G4
+        20,  # Zhu2023
+    ]
+    expected_markers = sum(total_markers_per_source) - sum(redundant_markers_per_source)
+    observed_markers = len(microhapdb.markers)
+    assert observed_markers == expected_markers
 
 
 def test_markers():
     """
-    >>> import microhapdb
-    >>> m = microhapdb.markers
-    >>> m[m.Name == 'mh18CP-005']
-               Name          PermID Reference  Chrom                          Offsets      Ae      In     Fst  Source
-    425  mh18CP-005  MHDBM-a85754d3    GRCh38  chr18  8892864,8892893,8892896,8892907  3.6722  0.0904  0.0059  ALFRED
-    >>> m[m.Name == 'mh01KK-117']
-              Name          PermID Reference Chrom                                  Offsets      Ae      In     Fst  Source
-    30  mh01KK-117  MHDBM-39dc025f    GRCh38  chr1  204664211,204664268,204664371,204664397  4.4565  0.1933  0.0472  ALFRED
-    >>> m[m.Name == 'mh11PK-63643']
-                 Name          PermID Reference  Chrom                                            Offsets  Ae  In  Fst                        Source
-    272  mh11PK-63643  MHDBM-c5ce121f    GRCh38  chr11  34415814,34415816,34415818,34415835,34415836,3... NaN NaN  NaN  10.1016/j.fsigen.2018.05.008
-    >>> m[m.Name == 'mh02AT-05']
-             Name          PermID Reference Chrom                        Offsets      Ae   In    Fst         Source
-    67  mh02AT-05  MHDBM-c3feaba8    GRCh38  chr2  160222899,160222923,160222938  4.5544  0.2  0.152  ISFG2019:P597
+    >>> from microhapdb import Marker
+    >>> marker = Marker.from_id("mh18CP-005")
+    >>> print(marker)
+    mh18CP-005 (chr18:8892865-8892908)
+    >>> marker.offsets
+    [8892864, 8892893, 8892896, 8892907]
+    >>> print(marker.fasta)
+    >mh18CP-005 GRCh38:chr18:8892846-8892926 variants=18,47,50,61
+    GCAGATGTCCTTATACGCAGTGGTGTTAGTTTTAGAAACTGATTCTACGGGTATGCTTGCTCGTGTGTAAAATTATTCAT
+    >>> for marker in Marker.from_query("Source.str.contains('vanderGaag2018')"):
+    ...   print(marker)
+    mh06PK-24844 (chr6:13861393-13861447)
+    mh06PK-25713 (chr6:31196950-31197002)
+    mh07PK-38311 (chr7:52677451-52677509)
+    mh08PK-46625 (chr8:1194353-1194372)
+    mh10PK-62104 (chr10:127392566-127392633)
+    mh11PK-62906 (chr11:247980-248036)
+    mh11PK-63643.v1 (chr11:34415815-34415851)
+    mh14PK-72639 (chr14:32203274-32203324)
+    mh15PK-75170 (chr15:24802314-24802380)
+    mh16PK-83362 (chr16:77999243-77999292)
+    mh16PK-83483 (chr16:84516829-84516899)
+    mh16PK-83544 (chr16:85934075-85934138)
+    mh18PK-87558 (chr18:1960543-1960589)
+    mh21PK-MX1s (chr21:41464745-41464824)
+    mh22PK-104638 (chr22:44857883-44857955)
     """
-    m = microhapdb.markers
-    vm = microhapdb.variantmap
-    assert m.shape == (507, 9)
-    result = m[m.Chrom == 'chr19']
-    assert len(result) == 13
-    varids = vm[vm.Marker.isin(result.Name)].Variant.unique()
-    assert len(varids) == 42
-
-
-def test_marker_table(capsys):
-    marker = microhapdb.markers[microhapdb.markers.Name == 'mh04CP-003']
-    microhapdb.marker.print_table(marker)
-    testout = '''
-      Name         PermID Reference Chrom                 Offsets     Ae     In    Fst Source
-mh04CP-003 MHDBM-2be52d8b    GRCh38  chr4 4324722,4324735,4324749 2.9151 0.1668 0.0321 ALFRED
-'''
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert terminal.out.strip() == testout.strip()
-
-
-def test_marker_table_multi(capsys):
-    markers = microhapdb.markers.query('Name.str.contains("PK")', engine='python').head(n=5)
-    microhapdb.marker.print_table(markers)
-    testout = '''
-         Name          PermID Reference  Chrom                                            Offsets      Ae      In     Fst                        Source
- mh06PK-24844  MHDBM-aa39cbba    GRCh38   chr6  13861392,13861399,13861414,13861421,13861430,1...     NaN     NaN     NaN  10.1016/j.fsigen.2018.05.008
- mh06PK-25713  MHDBM-7d00efdc    GRCh38   chr6  31196949,31196961,31196972,31196985,31196992,3...  2.9544  0.0898  0.0681  10.1016/j.fsigen.2018.05.008
- mh07PK-38311  MHDBM-3ae6dc1b    GRCh38   chr7                52677450,52677456,52677462,52677508  3.2638  0.1000  0.1927  10.1016/j.fsigen.2018.05.008
- mh08PK-46625  MHDBM-840756f3    GRCh38   chr8                    1194352,1194356,1194364,1194371  2.3775  0.1132  0.1395  10.1016/j.fsigen.2018.05.008
- mh10PK-62104  MHDBM-5f9c6cab    GRCh38  chr10  127392565,127392577,127392596,127392610,127392...  2.0068  0.0482  0.1032  10.1016/j.fsigen.2018.05.008
-'''
-    testoutlong = '''
-        Name         PermID Reference Chrom                                                                                   Offsets     Ae     In    Fst                       Source
-mh06PK-24844 MHDBM-aa39cbba    GRCh38  chr6 13861392,13861399,13861414,13861421,13861430,13861434,13861438,13861439,13861440,13861446    NaN    NaN    NaN 10.1016/j.fsigen.2018.05.008
-mh06PK-25713 MHDBM-7d00efdc    GRCh38  chr6                                     31196949,31196961,31196972,31196985,31196992,31197001 2.9544 0.0898 0.0681 10.1016/j.fsigen.2018.05.008
-mh07PK-38311 MHDBM-3ae6dc1b    GRCh38  chr7                                                       52677450,52677456,52677462,52677508 3.2638 0.1000 0.1927 10.1016/j.fsigen.2018.05.008
-mh08PK-46625 MHDBM-840756f3    GRCh38  chr8                                                           1194352,1194356,1194364,1194371 2.3775 0.1132 0.1395 10.1016/j.fsigen.2018.05.008
-mh10PK-62104 MHDBM-5f9c6cab    GRCh38 chr10                     127392565,127392577,127392596,127392610,127392611,127392620,127392632 2.0068 0.0482 0.1032 10.1016/j.fsigen.2018.05.008
-'''
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert terminal.out.strip() == testout.strip() or terminal.out.strip() == testoutlong.strip()
-
-
-def test_marker_table_multi_notrunc(capsys):
-    markers = microhapdb.markers.query('Name.str.contains("PK")', engine='python').head(n=5)
-    microhapdb.marker.print_table(markers, trunc=False)
-    testoutlong = '''
-        Name         PermID Reference Chrom                                                                                   Offsets     Ae     In    Fst                       Source
-mh06PK-24844 MHDBM-aa39cbba    GRCh38  chr6 13861392,13861399,13861414,13861421,13861430,13861434,13861438,13861439,13861440,13861446    NaN    NaN    NaN 10.1016/j.fsigen.2018.05.008
-mh06PK-25713 MHDBM-7d00efdc    GRCh38  chr6                                     31196949,31196961,31196972,31196985,31196992,31197001 2.9544 0.0898 0.0681 10.1016/j.fsigen.2018.05.008
-mh07PK-38311 MHDBM-3ae6dc1b    GRCh38  chr7                                                       52677450,52677456,52677462,52677508 3.2638 0.1000 0.1927 10.1016/j.fsigen.2018.05.008
-mh08PK-46625 MHDBM-840756f3    GRCh38  chr8                                                           1194352,1194356,1194364,1194371 2.3775 0.1132 0.1395 10.1016/j.fsigen.2018.05.008
-mh10PK-62104 MHDBM-5f9c6cab    GRCh38 chr10                     127392565,127392577,127392596,127392610,127392611,127392620,127392632 2.0068 0.0482 0.1032 10.1016/j.fsigen.2018.05.008
-'''
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert terminal.out.strip() == testoutlong.strip()
-
-
-def test_marker_detail(capsys):
-    marker = microhapdb.markers[microhapdb.markers.Name == 'mh09AT-17']
-    microhapdb.marker.print_detail(marker, delta=10, minlen=90)
-    testout = '''
+    assert microhapdb.markers.shape == (2804, 11)
+    result = microhapdb.markers[microhapdb.markers.Chrom == "chr19"]
+    assert len(result) == 71
+    varids = microhapdb.variantmap[microhapdb.variantmap.Marker.isin(result.Name)].Variant.unique()
+    assert len(varids) == 148
+
+
+def test_marker_detail():
+    marker = Marker.from_id("mh09KK-157.v3")
+    observed = marker.detail
+    expected = """
 --------------------------------------------------------------[ MicroHapDB ]----
-mh09AT-17    a.k.a MHDBM-b34d6dc3
+mh09KK-157.v3
 
-Marker Definition (GRCh38)
+Marker Definition
     Marker extent
-        - chr9:132987175-132987245 (70 bp)
-    Target amplicon
+        - chr9:132987176-132987245 (70 bp)
+    Target locus
         - chr9:132987165-132987255 (90 bp)
     Constituent variants
-        - chromosome offsets: 132987175,132987204,132987244
-        - marker offsets: 0,29,69
-        - amplicon offsets: 10,39,79
-        - cross-references: rs2073578, rs56256724, rs633153
+        - chromosome offsets (GRCh37): 135862562, 135862591, 135862631
+        - chromosome offsets (GRCh38): 132987175, 132987204, 132987244
+        - marker offsets: 0, 29, 69
+        - target offsets: 10, 39, 79
+        - cross-references: rs56256724, rs2073578, rs633153
     Observed haplotypes
-        - C,A,C
-        - C,A,T
-        - C,C,C
-        - C,C,T
-        - T,A,C
-        - T,A,T
-        - T,C,T
+        - C|A|C
+        - C|A|T
+        - C|C|C
+        - C|C|T
+        - T|A|T
+        - T|C|T
 
 
 --[ Core Marker Sequence ]--
->mh09AT-17
+>mh09KK-157.v3
 CTGTCTCTCTGGGCCTCCTCCTCCTAGGAAGGGCGTGCCCTCCTTGCTCCCTCTGGGCTTCCCAGAAACC
 
 
---[ Target Amplicon Sequence with Haplotypes ]--
+--[ Marker Target Sequence with MH alleles (haplotypes) ]--
           *                            *                                       *
 CGGCACGTGGCTGTCTCTCTGGGCCTCCTCCTCCTAGGAAGGGCGTGCCCTCCTTGCTCCCTCTGGGCTTCCCAGAAACCGTGGCTATTG
 ..........C............................A.......................................C..........
 ..........C............................A.......................................T..........
 ..........C............................C.......................................C..........
 ..........C............................C.......................................T..........
-..........T............................A.......................................C..........
 ..........T............................A.......................................T..........
 ..........T............................C.......................................T..........
 --------------------------------------------------------------------------------
-'''
-    terminal = capsys.readouterr()
-    assert terminal.out.strip() == testout.strip()
+"""
+    assert observed.strip() == expected.strip()
 
 
-def test_marker_detail_long(capsys):
-    marker = microhapdb.markers[microhapdb.markers.Name == 'mh05KK-170']
-    microhapdb.marker.print_detail(marker, delta=20, minlen=125)
-    testout = '''
+def test_marker_detail_long():
+    marker = Marker.from_id("mh05KK-170.v1", delta=20, minlen=200, extendmode=-1)
+    observed = marker.detail
+    expected = """
 --------------------------------------------------------------[ MicroHapDB ]----
-mh05KK-170    a.k.a MHDBM-22ddbb7d, SI664573F
+mh05KK-170.v1
 
-Marker Definition (GRCh38)
+Marker Definition
     Marker extent
-        - chr5:2447909-2448046 (137 bp)
-    Target amplicon
-        - chr5:2447889-2448066 (177 bp)
+        - chr5:2447910-2448046 (137 bp)
+    Target locus
+        - chr5:2447866-2448066 (200 bp)
     Constituent variants
-        - chromosome offsets: 2447909,2447937,2448031,2448045
-        - marker offsets: 0,28,122,136
-        - amplicon offsets: 20,48,142,156
-        - cross-references: rs370672, rs438055, rs6555108, rs74865590
+        - chromosome offsets (GRCh37): 2448023, 2448051, 2448145, 2448159
+        - chromosome offsets (GRCh38): 2447909, 2447937, 2448031, 2448045
+        - marker offsets: 0, 28, 122, 136
+        - target offsets: 43, 71, 165, 179
+        - cross-references: rs74865590, rs438055, rs370672, rs6555108
     Observed haplotypes
-        - C,A,A,A
-        - C,A,A,G
-        - C,A,G,A
-        - C,A,G,G
-        - C,G,A,A
-        - C,G,A,G
-        - C,G,G,A
-        - C,G,G,G
-        - T,A,A,A
-        - T,A,A,G
-        - T,A,G,A
-        - T,A,G,G
-        - T,G,A,A
-        - T,G,A,G
-        - T,G,G,G
+        - C|A|A|A
+        - C|A|A|G
+        - C|A|G|A
+        - C|A|G|G
+        - C|G|A|A
+        - C|G|A|G
+        - C|G|G|A
+        - C|G|G|G
+        - T|A|A|A
+        - T|A|A|G
+        - T|A|G|A
+        - T|A|G|G
+        - T|G|A|A
+        - T|G|A|G
+        - T|G|G|G
 
 
 --[ Core Marker Sequence ]--
->mh05KK-170
+>mh05KK-170.v1
 CCACAGTTGAAGAGAGAGAGCATGAGACAGCTTGATCGAAATGGTGAAGCTTTGGAGAGATTTTGCGGGGAATGCACTGG
 AGAACCATGAAGATGTGGAAACAAACAAACAAACAAAAAACCGCTTTTGCATCTTCA
 
 
---[ Target Amplicon Sequence with Haplotypes ]--
-                    *                           *                                                                                             *             *
-TTTCTTAACAAAACTGAAGGCCACAGTTGAAGAGAGAGAGCATGAGACAGCTTGATCGAAATGGTGAAGCTTTGGAGAGATTTTGCGGGGAATGCACTGGAGAACCATGAAGATGTGGAAACAAACAAACAAACAAAAAACCGCTTTTGCATCTTCAGACATCTCACTTGTCATCAC
-....................C...........................A.............................................................................................A.............A....................
-....................C...........................A.............................................................................................A.............G....................
-....................C...........................A.............................................................................................G.............A....................
-....................C...........................A.............................................................................................G.............G....................
-....................C...........................G.............................................................................................A.............A....................
-....................C...........................G.............................................................................................A.............G....................
-....................C...........................G.............................................................................................G.............A....................
-....................C...........................G.............................................................................................G.............G....................
-....................T...........................A.............................................................................................A.............A....................
-....................T...........................A.............................................................................................A.............G....................
-....................T...........................A.............................................................................................G.............A....................
-....................T...........................A.............................................................................................G.............G....................
-....................T...........................G.............................................................................................A.............A....................
-....................T...........................G.............................................................................................A.............G....................
-....................T...........................G.............................................................................................G.............G....................
+--[ Marker Target Sequence with MH alleles (haplotypes) ]--
+                                           *                           *                                                                                             *             *
+TGGAGGACAAAAGTGAACTTGATTTTCTTAACAAAACTGAAGGCCACAGTTGAAGAGAGAGAGCATGAGACAGCTTGATCGAAATGGTGAAGCTTTGGAGAGATTTTGCGGGGAATGCACTGGAGAACCATGAAGATGTGGAAACAAACAAACAAACAAAAAACCGCTTTTGCATCTTCAGACATCTCACTTGTCATCAC
+...........................................C...........................A.............................................................................................A.............A....................
+...........................................C...........................A.............................................................................................A.............G....................
+...........................................C...........................A.............................................................................................G.............A....................
+...........................................C...........................A.............................................................................................G.............G....................
+...........................................C...........................G.............................................................................................A.............A....................
+...........................................C...........................G.............................................................................................A.............G....................
+...........................................C...........................G.............................................................................................G.............A....................
+...........................................C...........................G.............................................................................................G.............G....................
+...........................................T...........................A.............................................................................................A.............A....................
+...........................................T...........................A.............................................................................................A.............G....................
+...........................................T...........................A.............................................................................................G.............A....................
+...........................................T...........................A.............................................................................................G.............G....................
+...........................................T...........................G.............................................................................................A.............A....................
+...........................................T...........................G.............................................................................................A.............G....................
+...........................................T...........................G.............................................................................................G.............G....................
 --------------------------------------------------------------------------------
-'''
-    terminal = capsys.readouterr()
-    assert terminal.out.strip() == testout.strip()
+"""
+    assert observed.strip() == expected.strip()
 
 
-def test_marker_detail_short(capsys):
-    marker = microhapdb.markers[microhapdb.markers.Name == 'mh16PK-83544']
-    microhapdb.marker.print_detail(marker, delta=0, minlen=0)
-    testout = '''
+def test_marker_detail_short():
+    marker = Marker.from_id("mh16PK-83544", delta=0, minlen=0)
+    observed = marker.detail
+    expected = """
 --------------------------------------------------------------[ MicroHapDB ]----
-mh16PK-83544    a.k.a MHDBM-c80956b4
+mh16PK-83544
 
-Marker Definition (GRCh38)
+Marker Definition
     Marker extent
-        - chr16:85934074-85934138 (64 bp)
-    Target amplicon
+        - chr16:85934075-85934138 (64 bp)
+    Target locus
         - chr16:85934074-85934138 (64 bp)
     Constituent variants
-        - chromosome offsets: 85934074,85934082,85934105,85934115,85934128,85934137
-        - marker offsets: 0,8,31,41,54,63
-        - amplicon offsets: 0,8,31,41,54,63
-        - cross-references: rs528179479, rs66509440, rs66804793, rs74032085, rs9925859, rs9929895
+        - chromosome offsets (GRCh37): 85967680, 85967688, 85967711, 85967721, 85967734, 85967743
+        - chromosome offsets (GRCh38): 85934074, 85934082, 85934105, 85934115, 85934128, 85934137
+        - marker offsets: 0, 8, 31, 41, 54, 63
+        - target offsets: 0, 8, 31, 41, 54, 63
+        - cross-references: rs66509440, rs66804793, rs528179479, rs9925859, rs9929895, rs74032085
     Observed haplotypes
-        - C,G,G,C,A,T
-        - C,G,G,G,A,T
-        - C,G,G,G,G,T
-        - T,A,C,G,T,C
-        - T,A,G,G,A,T
-        - T,A,G,G,T,C
+        - C|G|G|C|A|T
+        - C|G|G|G|A|T
+        - C|G|G|G|G|T
+        - T|A|C|G|T|C
+        - T|A|G|G|A|T
+        - T|A|G|G|T|C
 
 
 --[ Core Marker Sequence ]--
 >mh16PK-83544
 CGGGCGGTGTGTGGCTGAAGGGCAAGAGAAAGGAGAGACTGCGGCTGGGAACCCATATGGGAAT
 
 
---[ Target Amplicon Sequence with Haplotypes ]--
+--[ Marker Target Sequence with MH alleles (haplotypes) ]--
 *       *                      *         *            *        *
 CGGGCGGTGTGTGGCTGAAGGGCAAGAGAAAGGAGAGACTGCGGCTGGGAACCCATATGGGAAT
 C.......G......................G.........C............A........T
 C.......G......................G.........G............A........T
 C.......G......................G.........G............G........T
 T.......A......................C.........G............T........C
 T.......A......................G.........G............A........T
 T.......A......................G.........G............T........C
 --------------------------------------------------------------------------------
-
-
-'''
-    terminal = capsys.readouterr()
-    assert terminal.out.strip() == testout.strip()
+"""
+    assert observed.strip() == expected.strip()
 
 
 def test_marker_detail_multi(capsys):
-    markerids = ['mh22PK-104638', 'mh18PK-87558', 'mh06PK-24844']
-    markers = microhapdb.markers[microhapdb.markers.Name.isin(markerids)]
-    microhapdb.marker.print_detail(markers, delta=10, minlen=80)
-    testout = '''
+    for marker in Marker.from_ids(["mh22PK-104638", "mh18PK-87558", "mh06PK-24844"]):
+        print(marker.detail)
+    observed = capsys.readouterr().out
+    expected = """
 --------------------------------------------------------------[ MicroHapDB ]----
-mh06PK-24844    a.k.a MHDBM-aa39cbba
+mh06PK-24844
 
-Marker Definition (GRCh38)
+Marker Definition
     Marker extent
-        - chr6:13861392-13861447 (55 bp)
-    Target amplicon
+        - chr6:13861393-13861447 (55 bp)
+    Target locus
         - chr6:13861379-13861460 (81 bp)
     Constituent variants
-        - chromosome offsets: 13861392,13861399,13861414,13861421,13861430,13861434,13861438,13861439,13861440,13861446
-        - marker offsets: 0,7,22,29,38,42,46,47,48,54
-        - amplicon offsets: 13,20,35,42,51,55,59,60,61,67
-        - cross-references: rs1196416099, rs1204206, rs1204207, rs1204208, rs34901968, rs35198802, rs376614501, rs545720382, rs546942508, rs553417439
+        - chromosome offsets (GRCh37): 13861623, 13861630, 13861645, 13861652, 13861661, 13861665, 13861669, 13861670, 13861671, 13861677
+        - chromosome offsets (GRCh38): 13861392, 13861399, 13861414, 13861421, 13861430, 13861434, 13861438, 13861439, 13861440, 13861446
+        - marker offsets: 0, 7, 22, 29, 38, 42, 46, 47, 48, 54
+        - target offsets: 13, 20, 35, 42, 51, 55, 59, 60, 61, 67
+        - cross-references: rs1204206, rs376614501, rs1196416099, rs35198802, rs553417439, rs1204207, rs545720382, rs34901968, rs546942508, rs1204208
     Observed haplotypes
-        - C,C,G,C,C,C,A,A,A,A
-        - C,C,G,C,C,C,A,A,G,A
-        - G,C,G,T,C,C,A,G,G,A
-        - G,C,G,T,G,C,A,G,G,A
-        - G,CT,G,C,C,C,A,G,G,A
-        - T,C,G,C,C,C,A,A,G,A
-        - T,C,G,C,C,T,A,A,G,G
-        - T,C,G,C,C,T,T,A,G,G
-        - T,C,GA,C,C,T,A,A,G,G
+        - C|C|G|C|C|C|A|A|A|A
+        - C|C|G|C|C|C|A|A|G|A
+        - G|CT|G|C|C|C|A|G|G|A
+        - G|C|G|C|C|C|A|G|G|A
+        - G|C|G|T|C|C|A|G|G|A
+        - G|C|G|T|C|T|A|G|G|A
+        - G|C|G|T|G|C|A|G|G|A
+        - T|C|GA|C|C|T|A|A|G|G
+        - T|C|G|C|C|C|A|A|A|A
+        - T|C|G|C|C|C|A|A|G|A
+        - T|C|G|C|C|C|T|A|G|A
+        - T|C|G|C|C|T|A|A|G|G
+        - T|C|G|C|C|T|T|A|G|G
+        - T|C|G|T|C|C|A|A|G|A
+        - T|C|G|T|C|C|A|G|G|A
 
 
 --[ Core Marker Sequence ]--
 >mh06PK-24844
 TTACATCCAAACGTGAGCAGGAGGAAACTCGGAACATACTGTTTTTAAGAACTAG
 
 
---[ Target Amplicon Sequence with Haplotypes ]--
+--[ Marker Target Sequence with MH alleles (haplotypes) ]--
              *      **              **      *        *   *   ***     *
 AGGAAGAAAGTGATTACATCC-AAACGTGAGCAGGAG-GAAACTCGGAACATACTGTTTTTAAGAACTAGTATCACTAGAGTT
 .............C......C-..............G-......C........C...C...AAA.....A.............
 .............C......C-..............G-......C........C...C...AAG.....A.............
+.............G......CT..............G-......C........C...C...AGG.....A.............
+.............G......C-..............G-......C........C...C...AGG.....A.............
 .............G......C-..............G-......T........C...C...AGG.....A.............
+.............G......C-..............G-......T........C...T...AGG.....A.............
 .............G......C-..............G-......T........G...C...AGG.....A.............
-.............G......CT..............G-......C........C...C...AGG.....A.............
+.............T......C-..............GA......C........C...T...AAG.....G.............
+.............T......C-..............G-......C........C...C...AAA.....A.............
 .............T......C-..............G-......C........C...C...AAG.....A.............
+.............T......C-..............G-......C........C...C...TAG.....A.............
 .............T......C-..............G-......C........C...T...AAG.....G.............
 .............T......C-..............G-......C........C...T...TAG.....G.............
-.............T......C-..............GA......C........C...T...AAG.....G.............
+.............T......C-..............G-......T........C...C...AAG.....A.............
+.............T......C-..............G-......T........C...C...AGG.....A.............
 --------------------------------------------------------------------------------
 
 --------------------------------------------------------------[ MicroHapDB ]----
-mh18PK-87558    a.k.a MHDBM-1e5374f1
+mh18PK-87558
 
-Marker Definition (GRCh38)
+Marker Definition
     Marker extent
-        - chr18:1960542-1960589 (47 bp)
-    Target amplicon
+        - chr18:1960543-1960589 (47 bp)
+    Target locus
         - chr18:1960525-1960606 (81 bp)
     Constituent variants
-        - chromosome offsets: 1960542,1960557,1960561,1960566,1960582,1960588
-        - marker offsets: 0,15,19,24,40,46
-        - amplicon offsets: 17,32,36,41,57,63
-        - cross-references: rs28612163, rs28695806, rs62081065, rs62081066, rs9947384, rs9962474
+        - chromosome offsets (GRCh37): 1960543, 1960558, 1960562, 1960567, 1960583, 1960589
+        - chromosome offsets (GRCh38): 1960542, 1960557, 1960561, 1960566, 1960582, 1960588
+        - marker offsets: 0, 15, 19, 24, 40, 46
+        - target offsets: 17, 32, 36, 41, 57, 63
+        - cross-references: rs9962474, rs9947384, rs62081065, rs28612163, rs62081066, rs28695806
     Observed haplotypes
-        - C,A,A,G,A,T
-        - C,A,G,C,A,C
-        - C,A,G,C,A,T
-        - C,A,G,C,T,C
-        - C,G,A,G,A,T
-        - T,A,G,C,T,C
-        - T,G,A,G,A,T
+        - C|A|A|G|A|T
+        - C|A|G|C|A|C
+        - C|A|G|C|T|C
+        - T|G|A|G|A|T
 
 
 --[ Core Marker Sequence ]--
 >mh18PK-87558
 TCAGGTGTTAGCAACGAGGATTTAGAAAAAACAGGTACAAATTATTT
 
 
---[ Target Amplicon Sequence with Haplotypes ]--
+--[ Marker Target Sequence with MH alleles (haplotypes) ]--
                  *              *   *    *               *     *
 AGCCTAGCCAAGAGCTGTCAGGTGTTAGCAACGAGGATTTAGAAAAAACAGGTACAAATTATTTCATCACCCAGGTAGTGA
 .................C..............A...A....G...............A.....T.................
 .................C..............A...G....C...............A.....C.................
-.................C..............A...G....C...............A.....T.................
 .................C..............A...G....C...............T.....C.................
-.................C..............G...A....G...............A.....T.................
-.................T..............A...G....C...............T.....C.................
 .................T..............G...A....G...............A.....T.................
 --------------------------------------------------------------------------------
 
 --------------------------------------------------------------[ MicroHapDB ]----
-mh22PK-104638    a.k.a MHDBM-eb63e78f
+mh22PK-104638
 
-Marker Definition (GRCh38)
+Marker Definition
     Marker extent
-        - chr22:44857882-44857955 (73 bp)
-    Target amplicon
+        - chr22:44857883-44857955 (73 bp)
+    Target locus
         - chr22:44857872-44857965 (93 bp)
     Constituent variants
-        - chromosome offsets: 44857882,44857883,44857884,44857891,44857892,44857893,44857907,44857930,44857946,44857949,44857950,44857954
-        - marker offsets: 0,1,2,9,10,11,25,48,64,67,68,72
-        - amplicon offsets: 10,11,12,19,20,21,35,58,74,77,78,82
-        - cross-references: rs10685889, rs10685890, rs113141650, rs117862404, rs62232223, rs62232224, rs62232225, rs62232226, rs71328677, rs7291353
+        - chromosome offsets (GRCh37): 45253762, 45253763, 45253764, 45253771, 45253772, 45253773, 45253787, 45253810, 45253826, 45253829, 45253830, 45253834
+        - chromosome offsets (GRCh38): 44857882, 44857883, 44857884, 44857891, 44857892, 44857893, 44857907, 44857930, 44857946, 44857949, 44857950, 44857954
+        - marker offsets: 0, 1, 2, 9, 10, 11, 25, 48, 64, 67, 68, 72
+        - target offsets: 10, 11, 12, 19, 20, 21, 35, 58, 74, 77, 78, 82
+        - cross-references: rs117862404, rs62232223, rs7291353, rs71328677, rs62232224, rs10685889, rs10685890, rs113141650, rs62232225, rs62232226
     Observed haplotypes
-        - C,A,G,C,G,C,CCTGCC,TTCTT,GTGAG,C,T,G
-        - C,A,G,C,G,T,CCTGCC,TTCTT,GTGAG,C,C,T
-        - C,G,C,C,G,C,CCTGCC,T,GTGAG,C,T,G
-        - C,G,G,C,A,C,CCTGCC,T,G,C,T,G
-        - C,G,G,C,G,C,CCTGCC,T,G,C,T,G
-        - C,G,G,C,G,C,CCTGCC,T,GTGAG,C,T,G
-        - C,G,G,C,G,C,CCTGCC,T,GTGAG,G,T,G
-        - C,G,G,C,G,T,C,TTCTT,GTGAG,C,C,T
-        - C,G,G,C,G,T,CCTGCC,TTCTT,GTGAG,C,C,T
-        - C,G,G,T,G,C,CCTGCC,TTCTT,GTGAG,C,T,G
-        - T,G,G,C,G,C,CCTGCC,TTCTT,GTGAG,C,T,G
+        - C|A|G|C|G|C|CCTGCC|TTCTT|GTGAG|C|T|G
+        - C|A|G|C|G|C|C|T|G|C|T|G
+        - C|A|G|C|G|T|CCTGCC|TTCTT|GTGAG|C|C|T
+        - C|A|G|C|G|T|C|T|G|C|C|T
+        - C|G|C|C|G|C|CCTGCC|T|GTGAG|C|T|G
+        - C|G|G|C|A|C|CCTGCC|T|G|C|T|G
+        - C|G|G|C|A|C|C|T|G|C|T|G
+        - C|G|G|C|G|C|CCTGCC|T|GTGAG|C|T|G
+        - C|G|G|C|G|C|CCTGCC|T|GTGAG|G|T|G
+        - C|G|G|C|G|C|CCTGCC|T|G|C|T|G
+        - C|G|G|C|G|C|C|T|G|C|T|G
+        - C|G|G|C|G|C|C|T|G|G|T|G
+        - C|G|G|C|G|T|CCTGCC|TTCTT|GTGAG|C|C|T
+        - C|G|G|C|G|T|C|TTCTT|GTGAG|C|C|T
+        - C|G|G|C|G|T|C|T|G|C|C|T
+        - C|G|G|T|G|C|CCTGCC|TTCTT|GTGAG|C|T|G
+        - C|G|G|T|G|C|C|T|G|C|T|G
+        - T|G|G|C|A|C|C|T|G|C|T|G
+        - T|G|G|C|G|C|CCTGCC|TTCTT|GTGAG|C|T|G
+        - T|G|G|C|G|C|C|T|G|C|T|G
 
 
 --[ Core Marker Sequence ]--
 >mh22PK-104638
 CGGTTGTGACGCTCAGCTCACCAGTCCTGCCTACTTGCCAGCAGGTATTCTCAGAGGGACCACAGAGCTGAGG
 
 
---[ Target Amplicon Sequence with Haplotypes ]--
+--[ Marker Target Sequence with MH alleles (haplotypes) ]--
           ***      ***             ******                 *****               *****  **   *
 GTGACATTGGCGGTTGTGACGCTCAGCTCACCAGTCCTGCCTACTTGCCAGCAGGTATT----CTCAGAGGGACCACAG----AGCTGAGGGTGACCTGCA
 ..........CAG......CGC.............CCTGCC.................TTCTT...............GTGAG..CT...G..........
+..........CAG......CGC.............C-----.................T----...............G----..CT...G..........
 ..........CAG......CGT.............CCTGCC.................TTCTT...............GTGAG..CC...T..........
+..........CAG......CGT.............C-----.................T----...............G----..CC...T..........
 ..........CGC......CGC.............CCTGCC.................T----...............GTGAG..CT...G..........
 ..........CGG......CAC.............CCTGCC.................T----...............G----..CT...G..........
-..........CGG......CGC.............CCTGCC.................T----...............G----..CT...G..........
+..........CGG......CAC.............C-----.................T----...............G----..CT...G..........
 ..........CGG......CGC.............CCTGCC.................T----...............GTGAG..CT...G..........
 ..........CGG......CGC.............CCTGCC.................T----...............GTGAG..GT...G..........
-..........CGG......CGT.............C-----.................TTCTT...............GTGAG..CC...T..........
+..........CGG......CGC.............CCTGCC.................T----...............G----..CT...G..........
+..........CGG......CGC.............C-----.................T----...............G----..CT...G..........
+..........CGG......CGC.............C-----.................T----...............G----..GT...G..........
 ..........CGG......CGT.............CCTGCC.................TTCTT...............GTGAG..CC...T..........
+..........CGG......CGT.............C-----.................TTCTT...............GTGAG..CC...T..........
+..........CGG......CGT.............C-----.................T----...............G----..CC...T..........
 ..........CGG......TGC.............CCTGCC.................TTCTT...............GTGAG..CT...G..........
+..........CGG......TGC.............C-----.................T----...............G----..CT...G..........
+..........TGG......CAC.............C-----.................T----...............G----..CT...G..........
 ..........TGG......CGC.............CCTGCC.................TTCTT...............GTGAG..CT...G..........
+..........TGG......CGC.............C-----.................T----...............G----..CT...G..........
 --------------------------------------------------------------------------------
-'''
-    terminal = capsys.readouterr()
-    assert terminal.out.strip() == testout.strip()
+"""
+    assert observed.strip() == expected.strip()
 
 
-def test_marker_fasta(capsys):
-    markers = microhapdb.markers[microhapdb.markers.Name == 'mh14PK-72639']
-    microhapdb.marker.print_fasta(markers, delta=10, minlen=70)
-    testout = '''
->mh14PK-72639 PermID=MHDBM-5548fd05 GRCh38:chr14:32203273-32203323 variants=10,11,14,15,28,39,46,57,60
+def test_marker_fasta():
+    marker = Marker.from_id("mh14PK-72639", minlen=70)
+    observed = marker.fasta
+    expected = """
+>mh14PK-72639 GRCh38:chr14:32203263-32203334 variants=10,11,14,15,28,39,46,57,60
 GAGCACGTTGAGAAGAAGTCACCCACAGGCCTTATAAGGCACGGGAGTCTTTCACCTATTCTACTTACGGT
-'''
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert terminal.out.strip() == testout.strip()
+"""
+    assert observed.strip() == expected.strip()
 
 
 def test_marker_fasta_multi(capsys):
-    markerids = ['mh05CP-010', 'mh13KK-223', 'mh14PK-72639']
-    markers = microhapdb.markers[microhapdb.markers.Name.isin(markerids)]
-    microhapdb.marker.print_fasta(markers, delta=15, minlen=150)
-    testout = '''
->mh05CP-010 PermID=MHDBM-df4e5f79 GRCh38:chr5:17903164-17903213 variants=50,69,94,99 Xref=SI664883J
+    markerids = ["mh05CP-010", "mh13KK-223.v1", "mh14PK-72639"]
+    for marker in Marker.from_ids(markerids, delta=15, minlen=150):
+        print(marker.fasta)
+    observed = capsys.readouterr().out
+    expected = """
+>mh05CP-010 GRCh38:chr5:17903114-17903264 variants=50,69,94,99
 CTGCTCAGAGTTTACATCAGAGTACTTGATGTAAATTACATCAGAGTACGCTGATGTAAATTACATCAGCGTACGCTGAT
 GTAAATTACATCAGCGTACTCTGATGTAAATTACATCAGCGTACTCTGATGTAATTTCAGTTTTCTTAAA
->mh13KK-223 PermID=MHDBM-4088f2e4 GRCh38:chr13:110154351-110154504 variants=15,58,75,168 Xref=SI664608E
+>mh13KK-223.v1 GRCh38:chr13:110154336-110154520 variants=15,58,75,168
 TTCAGTTGGCTTTTGTGGGAAAGGGAAGCCCTGGGGCTAGGAGAGCAGTCCTTGCCCTCTGGGAAGGGTCCCAGGCGGCA
 CTGCCCCAGGAGGGCCTTCGTGGAGGCCACGGCCAGCCCTCGGGTGTTCTCTCCCTAACTCAAGCTTCTGCTTTCAAGCT
 CGTGCATGTTGTAGTAGAATGTGT
->mh14PK-72639 PermID=MHDBM-5548fd05 GRCh38:chr14:32203273-32203323 variants=50,51,54,55,68,79,86,97,100
+>mh14PK-72639 GRCh38:chr14:32203223-32203374 variants=50,51,54,55,68,79,86,97,100
 CTCTGTATCGTTCCAATTTTAGTATATGTGCTGCCGAAGCGAGCACGTTGAGAAGAAGTCACCCACAGGCCTTATAAGGC
 ACGGGAGTCTTTCACCTATTCTACTTACGGTGACCGAACCGCGCCCTTTCCTGTCCATCTTGGAGCCTTTG
-'''
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert terminal.out.strip() == testout.strip()
+"""
+    assert observed.strip() == expected.strip()
 
 
-def test_amplicon_object(capsys):
-    amp = microhapdb.marker.TargetAmplicon('mh11KK-090', delta=10, minlen=60)
-    assert amp.local_to_global(10) == 113425537
-    assert amp.global_to_local(113425559) == 32
-    assert amp.local_to_global(65) is None
-    assert amp.global_to_local(113425599) is None
-    print(amp)
-    testout = '''
---------------------------------------------------------------[ MicroHapDB ]----
-mh11KK-090    a.k.a MHDBM-f67cb0d4, SI664596K
-
-Marker Definition (GRCh38)
-    Marker extent
-        - chr11:113425551-113425564 (13 bp)
-    Target amplicon
-        - chr11:113425527-113425588 (61 bp)
-    Constituent variants
-        - chromosome offsets: 113425551,113425563
-        - marker offsets: 0,12
-        - amplicon offsets: 24,36
-        - cross-references: rs1079597, rs1079598
-    Observed haplotypes
-        - A,C
-        - A,T
-        - G,C
-        - G,T
+def test_marker_object(capsys):
+    marker = Marker.from_id("mh11KK-090", delta=10, minlen=60)
+    assert marker.local_to_global(10) == 113425537
+    assert marker.global_to_local(113425559) == 32
+    assert marker.local_to_global(65) is None
+    assert marker.global_to_local(113425599) is None
+    assert marker.slug == "chr11:113425552-113425564"
+
+
+@pytest.mark.parametrize(
+    "markername,slug,length,source",
+    [
+        ("mh16KK-062", "chr16:87468089-87468386", 298, "Kidd2018"),
+        ("mh01CP-010", "chr1:85240118-85240140", 23, "Chen2019"),
+        ("mh09KK-153.v2", "chr9:101207360-101207606", 247, "Gandotra2020"),
+        ("mh10NH-14", "chr10:11288562-11288613", 52, "Hiroaki2015"),
+        ("mh02ZBF-001", "chr2:99401808-99401896", 89, "Jin2020"),
+        ("mh17ZHA-001", "chr17:390130-390249", 120, "Kureshi2020"),
+        ("mh16USC-16pB", "chr16:24314927-24314937", 11, "delaPuente2020"),
+        ("mh13KK-213.v3", "chr13:23191462-23191496", 35, "Staadig2021"),
+        ("mh08ZHA-003", "chr8:2914706-2915053", 348, "Sun2020"),
+        ("mh15PK-75170", "chr15:24802314-24802380", 67, "vanderGaag2018"),
+        ("mh03LV-06.v1", "chr3:11914401-11914598", 198, "Voskoboinik2018"),
+        ("mh15SHY-003", "chr15:92605653-92605846", 194, "Wu2021"),
+        ("mh01FHL-009.v2", "chr1:231954505-231954667", 163, "Fan2022"),
+        ("mh02KK-004.v2", "chr2:118984970-118985128", 159, "Turchi2019"),
+        ("mh20HYP-42", "chr20:59132558-59132664", 107, "Zou2022"),
+        ("mh13WL-032", "chr13:113079836-113079970", 135, "Yu2022G1"),
+    ],
+)
+def test_all_sources(markername, slug, length, source):
+    marker = Marker.from_id(markername)
+    assert marker.slug == slug
+    assert len(marker) == length
+    assert marker.data.Source == source
+
+
+@pytest.mark.parametrize(
+    "markername,attr,offsets",
+    [
+        ("mh01KK-117.v2", "offsets37", [204633339, 204633396, 204633461, 204633499, 204633525]),
+        ("mh06KK-104", "offsets", [165385361, 165385404, 165385450, 165385473, 165385548]),
+        ("mh12KK-199.v1", "offsets37", [12229785, 12229848, 12229849, 12229885, 12229951]),
+        ("mh12KK-199.v1", "offsets", [12076851, 12076914, 12076915, 12076951, 12077017]),
+    ],
+)
+def test_gandotra_offsets(markername, attr, offsets):
+    marker = Marker.from_id(markername)
+    observed = getattr(marker, attr)
+    expected = offsets
+    assert observed == expected
 
 
---[ Core Marker Sequence ]--
->mh11KK-090
-AGATTCGCCTTTC
+@pytest.mark.parametrize(
+    "marker,mode,offsets",
+    [
+        ("mh01USC-1pD", 0, "variants=70,92,104"),
+        ("mh01USC-1pD", -1, "variants=120,142,154"),
+        ("mh01USC-1pD", 1, "variants=20,42,54"),
+        ("mh22NH-27", 0, "variants=47,82,128"),
+        ("mh22NH-27", -1, "variants=73,108,154"),
+        ("mh22NH-27", 1, "variants=20,55,101"),
+    ],
+)
+def test_marker_extendmode(marker, mode, offsets):
+    marker = Marker.from_id(marker, delta=20, minlen=175, extendmode=mode)
+    assert offsets in marker.defline
 
 
---[ Target Amplicon Sequence with Haplotypes ]--
-                        *           *
-AAGGGCAGCAGGAACCACATGATCAGATTCGCCTTTCGAATAGGTGATTCTGACAGCACTG
-........................A...........C........................
-........................A...........T........................
-........................G...........C........................
-........................G...........T........................
---------------------------------------------------------------------------------
-'''
-    terminal = capsys.readouterr()
-    assert terminal.out.strip() == testout.strip()
-
-
-@pytest.mark.parametrize('name,data', [
-    ('mh04KK-010', 'mh04KK-010 MHDBM-07c8d144    GRCh38  chr4 1985210,1985244 2.9226 0.1306 0.0406 ALFRED'),
-    ('mh08PK-46625', 'mh08PK-46625 MHDBM-840756f3    GRCh38  chr8 1194352,1194356,1194364,1194371 2.3775 0.1132 0.1395 10.1016/j.fsigen.2018.05.008'),
-    ('mh04AT-10', 'mh04AT-10 MHDBM-07c8d144    GRCh38  chr4 1985210,1985244 2.9226 0.1306 0.0406 ISFG2019:P597'),
-    ('mh01NH-03', 'mh01NH-03 MHDBM-e7a95c5e    GRCh38  chr1 184807944,184807966,184808042 1.9086 0.1987 0.1725 10.1016/j.legalmed.2015.06.003'),
-    ('mh04CP-004', 'mh04CP-004 MHDBM-8408d717    GRCh38  chr4 7402842,7402854,7402870 2.6744 0.0477 0.061 10.1016/j.fsigen.2019.02.018'),
-    ('mh03LV-07', 'mh03LV-07 MHDBM-5f7e29b6    GRCh38  chr3 5783508,5783509,5783518,5783523,5783525,5783531,5783541,5783542,5783543,5783544,5783552,5783562,5783564,5783571,5783577,5783607,5783608,5783611,5783612,5783617,5783618,5783619,5783623,5783626,5783635,5783648,5783652,5783653,5783663,5783664,5783671,5783672,5783673,5783676,5783677,5783678,5783681,5783684,5783687,5783695,5783704,5783705 14.0275 1.081 0.057 10.1016/j.fsigen.2018.05.001'),
-    ('mh09USC-9pB', 'mh09USC-9pB MHDBM-7da7af40    GRCh38  chr9 31196676,31196714,31196731,31196744 3.0919 0.1616 0.0574 10.1016/j.fsigen.2019.102213'),
-    ('mh13KKCS-223', 'mh13KKCS-223 MHDBM-3ca7e2fc    GRCh38 chr13 110154341,110154351,110154394,110154411,110154438,110154441,110154485,110154504 NaN NaN  NaN 10.1016/j.fsigen.2020.102275')
-])
-def test_all_sources(name, data, capsys):
-    marker = microhapdb.markers[microhapdb.markers.Name == name]
-    microhapdb.marker.print_table(marker, trunc=False)
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert data in terminal.out
-
-
-def test_set_reference():
-    coords37 = [
-        '22137318,22137395,22137411,22137453',
-        '22137395,22137411,22137453',
-        '23068395,23068425,23068433',
-    ]
-    coords38 = [
-        '24557354,24557431,24557447,24557489',
-        '24557431,24557447,24557489',
+def test_marker_extendmode_bad():
+    with pytest.raises(ValueError, match=r"invalid literal for int"):
+        markers = Marker.from_ids(["mh01USC-1pD", "mh22NH-27"], minlen=175, extendmode="NotAnInt")
+        for marker in markers:
+            pass
+    with pytest.raises(TypeError, match=r"argument must be a string"):
+        markers = Marker.from_ids(["mh01USC-1pD", "mh22NH-27"], minlen=175, extendmode=None)
+        for marker in markers:
+            pass
+
+
+def test_marker_definition_single():
+    marker = Marker.from_id("mh07SHY-002")
+    definition = marker.definition
+    assert definition.shape == (9, 4)
+    assert definition.Offset.tolist() == [10, 36, 45, 67, 68, 90, 116, 121, 122]
+
+
+def test_marker_definition_multi():
+    ids = ["mh03KK-150.v2", "mh11KK-180.v1", "mh13KK-217.v1", "mh07USC-7qC"]
+    definition = Marker.definitions_from_ids(ids, delta=25, minlen=200)
+    assert definition.shape == (15, 4)
+    observed = definition.Offset.tolist()
+    expected = [85, 114, 66, 95, 122, 123, 134, 25, 145, 203, 218, 25, 65, 179, 217]
+    assert observed == expected
+    observed = definition.ChromOffset.tolist()
+    expected = [
+        131927127,
+        131927156,
+        151821663,
+        151821692,
+        151821719,
+        151821720,
+        151821731,
+        1669560,
+        1669680,
+        1669738,
+        1669753,
+        46291794,
+        46291834,
+        46291948,
+        46291986,
     ]
-    # Make sure they can be swapped in & out multiple times without issues
-    for _ in range(4):
-        microhapdb.set_reference(37)
-        result = microhapdb.retrieve.by_region('chr18:20000000-25000000')
-        assert result.Offsets.tolist() == coords37
-        microhapdb.set_reference(38)
-        result = microhapdb.retrieve.by_region('chr18:20000000-25000000')
-        assert result.Offsets.tolist() == coords38
-
-
-@pytest.mark.parametrize('markername,refr,offsets', [
-    (
-        'mh11KKCS-180', 37,
-        '1690724,1690769,1690790,1690824,1690886,1690910,1690949,1690961,1690968,1690983'
-    ),
-    (
-        'mh11KKCS-180', 38,
-        '1669494,1669539,1669560,1669594,1669656,1669680,1669719,1669731,1669738,1669753'
-    ),
-    (
-        'mh12KKCS-199', 37,
-        '12229785,12229848,12229849,12229885,12229951'
-    ),
-    (
-        'mh12KKCS-199', 38,
-        '12076851,12076914,12076915,12076951,12077017'
-    ),
-])
-def test_gandotra_offsets(markername, refr, offsets, capsys):
-    microhapdb.set_reference(refr)
-    marker = microhapdb.markers[microhapdb.markers.Name == markername]
-    microhapdb.marker.print_detail(marker)
-    terminal = capsys.readouterr()
-    microhapdb.set_reference(38)
-    assert offsets in terminal.out
-
-
-@pytest.mark.parametrize('markername', ['mh0XUSC-XqD'])
-def test_marker_no_freq(markername, capsys):
-    marker = microhapdb.markers[microhapdb.markers.Name == markername]
-    microhapdb.marker.print_detail(marker)
-    terminal = capsys.readouterr()
-    message = 'Unable to display a full detail view for markers without frequency information'
-    assert message in terminal.err
-
-
-@pytest.mark.parametrize('mode,offsets1,offsets2', [
-    (0, 'variants=70,92,104', 'variants=47,82,128'),
-    (-1, 'variants=120,142,154', 'variants=73,108,154'),
-    (1, 'variants=20,42,54', 'variants=20,55,101'),
-])
-def test_marker_extendmode(mode, offsets1, offsets2, capsys):
-    markers = microhapdb.markers[microhapdb.markers.Name.isin(['mh01USC-1pD', 'mh22NH-27'])]
-    microhapdb.marker.print_fasta(markers, delta=20, minlen=175, extendmode=mode)
-    terminal = capsys.readouterr()
-    assert offsets1 in terminal.out
-    assert offsets2 in terminal.out
+    assert observed == expected
 
 
-def test_marker_extendmode_bad():
-    markers = microhapdb.markers[microhapdb.markers.Name.isin(['mh01USC-1pD', 'mh22NH-27'])]
-    with pytest.raises(ValueError, match=r'invalid literal for int'):
-        microhapdb.marker.print_fasta(markers, delta=20, minlen=175, extendmode="NotAnInt")
-    with pytest.raises(TypeError, match=r'argument must be a string'):
-        microhapdb.marker.print_fasta(markers, delta=20, minlen=175, extendmode=None)
+def test_from_region():
+    with pytest.raises(ValueError, match='cannot parse region "chr7:123-456-789"'):
+        Marker.parse_regionstr("chr7:123-456-789")
+    assert len(Marker.table_from_region("chrX")) == 11
+    assert len(Marker.table_from_region("chrY")) == 0
+    markers = list(Marker.from_region("chr12:100000000-200000000"))
+    assert len(markers) == 41
+    observed = sorted([marker.name for marker in markers])
+    print(observed)
+    expected = sorted(
+        [
+            "mh12CP-003",
+            "mh12KK-042",
+            "mh12KK-045",
+            "mh12KK-046.v1",
+            "mh12KK-046.v2",
+            "mh12KK-046.v3",
+            "mh12KK-093",
+            "mh12KK-209",
+            "mh12SCUZJ-0326486.v1",
+            "mh12SCUZJ-0326486.v2",
+            "mh12SCUZJ-0331644",
+            "mh12SCUZJ-0345285",
+            "mh12SCUZJ-0347622",
+            "mh12SCUZJ-0363998",
+            "mh12SCUZJ-0364164",
+            "mh12SCUZJ-0374276",
+            "mh12SCUZJ-0382800",
+            "mh12SCUZJ-0392651",
+            "mh12SCUZJ-0396248",
+            "mh12SCUZJ-0420557",
+            "mh12SCUZJ-0423152",
+            "mh12SCUZJ-0429356.v1",
+            "mh12SCUZJ-0429356.v2",
+            "mh12WL-001.v1",
+            "mh12WL-001.v2",
+            "mh12WL-003",
+            "mh12WL-004",
+            "mh12WL-009",
+            "mh12WL-013.v1",
+            "mh12WL-013.v2",
+            "mh12WL-013.v3",
+            "mh12WL-024",
+            "mh12WL-033",
+            "mh12WL-046",
+            "mh12WL-047",
+            "mh12WL-048.v1",
+            "mh12WL-048.v2",
+            "mh12WL-049",
+            "mh12WL-050",
+            "mh12WL-054",
+            "mh12WL-059",
+        ]
+    )
+    assert observed == expected
 
 
-def test_marker_offsets(capsys):
-    ids = ['mh03AT-09', 'mh11KK-180', 'mh13KK-217', 'mh07USC-7qC']
-    markers = microhapdb.markers[microhapdb.markers.Name.isin(ids)]
-    microhapdb.marker.print_offsets(markers, delta=25, minlen=200)
-    terminal = capsys.readouterr()
-    result = pandas.read_csv(StringIO(terminal.out), sep='\t')
-    assert result.shape == (15, 2)
-    observed = list(result.Offset)
-    expected = [85, 114, 66, 95, 122, 123, 134, 25, 145, 203, 218, 25, 65, 179, 217]
-    assert observed == expected
+def test_from_id_no_such_marker():
+    with pytest.raises(ValueError, match=r"no such marker 'BoGUSid'"):
+        Marker.from_id("BoGUSid")
+
+
+def test_from_id_no_such_marker():
+    with pytest.raises(ValueError, match=r"no such marker 'BoGUSid'"):
+        Marker.from_id("BoGUSid")
+
+
+@pytest.mark.parametrize(
+    "query,result",
+    [
+        (
+            ["mh02FHL-006", "mh10FHL-007", "mh21WL-004"],
+            [
+                "mh02ZHA-013.v1",
+                "mh02ZHA-013.v2",
+                "mh10FHL-007",
+                "mh21FHL-002.v1",
+                "mh21FHL-002.v2",
+                "mh21FHL-002.v3",
+                "mh21FHL-002.v4",
+                "mh21FHL-002.v5",
+            ],
+        ),
+        (["mh11USC-11pB"], ["mh11PK-63643.v1", "mh11PK-63643.v2"]),
+        (["mh05KK-020"], ["mh05KK-023.v1", "mh05KK-023.v2", "mh05KK-023.v3", "mh05KK-023.v4"]),
+    ],
+)
+def test_standardize_merged_designators(query, result):
+    print(Marker.standardize_ids(query))
+    assert Marker.standardize_ids(query) == result
+
+
+@pytest.mark.parametrize(
+    "locus,num_markers",
+    [
+        ("mh01KK-001", 5),
+        ("mh13KK-225", 4),
+        ("mh06KK-008", 3),
+        ("mh02KK-031", 2),
+        ("mh10KK-088", 1),
+    ],
+)
+def test_standardize_locus_names(locus, num_markers):
+    marker_names = Marker.standardize_ids([locus])
+    assert len(marker_names) == num_markers
+
+
+def test_standardize_ids_incomplete_prefixes():
+    assert Marker.standardize_ids(["mh01"]) == []
+
+
+def test_locus_length():
+    loci = defaultdict(Locus)
+    for marker in Marker.objectify(microhapdb.markers, delta=0, minlen=0):
+        loci[marker.locus].markers.append(marker)
+    for locus in loci.values():
+        assert len(locus.target_seq) <= 610, locus.name
```

### Comparing `microhapdb-0.7rc1/microhapdb/tests/test_population.py` & `microhapdb-0.9/microhapdb/tests/test_population.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,104 @@
-# -----------------------------------------------------------------------------
-# Copyright (c) 2019, Battelle National Biodefense Institute.
+# -------------------------------------------------------------------------------------------------
+# Copyright (c) 2019, DHS.
 #
-# This file is part of MicroHapDB (http://github.com/bioforensics/microhapdb)
-# and is licensed under the BSD license: see LICENSE.txt.
-# -----------------------------------------------------------------------------
+# This file is part of MicroHapDB (http://github.com/bioforensics/MicroHapDB) and is licensed under
+# the BSD license: see LICENSE.txt.
+#
+# This software was prepared for the Department of Homeland Security (DHS) by the Battelle National
+# Biodefense Institute, LLC (BNBI) as part of contract HSHQDC-15-C-00064 to manage and operate the
+# National Biodefense Analysis and Countermeasures Center (NBACC), a Federally Funded Research and
+# Development Center.
+# -------------------------------------------------------------------------------------------------
 
 
 import microhapdb
-from microhapdb.population import standardize_ids
+from microhapdb import Population
 import pytest
 
 
 def test_standardize_ids():
-    assert list(standardize_ids(['SA004057Q']).values) == ['TSI']
-    assert list(standardize_ids(['MSL']).values) == ['MSL']
-    assert list(standardize_ids(['Maya, Yucatan', 'SA000055K', 'Greeks']).values) == ['SA002767W', 'SA000055K', 'SA000013E']
-    print(list(standardize_ids(['Han']).values))
-    assert list(standardize_ids(['Han']).values) == ['MHDBP-48c2cfb2aa', 'SA000001B', 'SA000009J']
+    assert Population.standardize_ids(["SA002766V"]) == ["SA002766V"]
+    assert Population.standardize_ids(["Samoans"]) == ["SA000072J"]
+    assert Population.standardize_ids(["Han"]) == ["MHDBP-48c2cfb2aa", "SA000001B", "SA000009J"]
+    assert Population.standardize_ids(["Maya, Yucatan", "SA000055K", "Greeks"]) == [
+        "SA000013E",
+        "SA000055K",
+        "SA002767W",
+    ]
 
 
 def test_assumptions():
-    assert len(microhapdb.populations) == 96 + 3 + 1 + 1 + 1 + 7
+    num_populations_per_source = [
+        31,  # Byrska-Bishop2022
+        1,  # Chen2019
+        7,  # Gandotra2020
+        1,  # Hiroaki2015
+        70,  # Kidd2018
+        1,  # Staadig2021
+        1,  # Turchi2019
+        10,  # Zou2022
+        3,  # vanderGaag2018
+    ]
+    assert len(microhapdb.populations) == sum(num_populations_per_source)
 
 
 def test_populations():
     """
-    >>> import microhapdb
-    >>> p = microhapdb.populations
-    >>> p[p.ID == 'SA000040E']
-               ID     Name  Source
-    52  SA000040E  Kachari  ALFRED
-    >>> p[p.ID == 'SA000936S']
-               ID     Name  Source
-    58  SA000936S  Koreans  ALFRED
-    >>> p[p.Name == 'Japanese']
-                      ID      Name                          Source
-    45  MHDBP-63967b883e  Japanese  10.1016/j.legalmed.2015.06.003
-    46         SA000010B  Japanese                          ALFRED
-    >>> p[p.Name.str.contains('Han')]
-                      ID                           Name                        Source
-    33  MHDBP-48c2cfb2aa                            Han  10.1016/j.fsigen.2019.02.018
-    34         SA000001B                            Han                        ALFRED
-    35         SA000009J                            Han                        ALFRED
-    36               CHB  Han Chinese in Beijing, China                          1KGP
-    93               CHS           Southern Han Chinese                          1KGP
-    >>> p.query('Name.str.contains("Afr")', engine='python')
-                     ID                                     Name                        Source
-    2  MHDBP-3dab7bdd14                                   Africa  10.1016/j.fsigen.2018.05.008
-    3         SA000101C                        African Americans                        ALFRED
-    4               ACB           African Caribbeans in Barbados                          1KGP
-    5               ASW  Americans of African Ancestry in SW USA                          1KGP
+    >>> pop = Population.from_id("SA000040E")
+    >>> print(pop.popid, pop.name, pop.source)
+    SA000040E Kachari Kidd2018
+    >>> Population.table_from_ids(["EAS", "SAS"])
+          ID        Name             Source
+    27   EAS   East Asia  Byrska-Bishop2022
+    104  SAS  South Asia  Byrska-Bishop2022
+    >>> for pop in Population.from_query("Name.str.contains('Han')"):
+    ...   print(pop.popid, pop.name, pop.source)
+    ChengduHan Chengdu Han Zou2022
+    HainanHan Hainan Han Zou2022
+    MHDBP-48c2cfb2aa Han Chen2019
+    SA000001B Han Kidd2018
+    SA000009J Han Kidd2018
+    CHB Han Chinese in Beijing, China Byrska-Bishop2022
+    CHS Southern Han Chinese Byrska-Bishop2022
+    >>> Population.table_from_query("Name.str.contains('Afr')")
+                     ID                                     Name             Source
+    3               AFR                                   Africa  Byrska-Bishop2022
+    4  MHDBP-3dab7bdd14                                   Africa     vanderGaag2018
+    5         SA000101C                        African Americans           Kidd2018
+    6               ACB           African Caribbeans in Barbados  Byrska-Bishop2022
+    7               ASW  Americans of African Ancestry in SW USA  Byrska-Bishop2022
     """
     pop = microhapdb.populations
-    assert pop.shape == (109, 3)
-    assert pop[pop.ID == 'FIN'].Name.values == ['Finnish in Finland']
-    assert pop[pop.ID == 'SA000028K'].Name.values == ['Karitiana']
-    result = pop[pop.Name.str.contains('Jews')].ID.values
-    assert list(result) == ['SA000490N', 'SA000015G', 'SA000096P', 'SA000016H']
-
-
-def test_pop_table(capsys):
-    masai = microhapdb.populations[microhapdb.populations.Name == 'Masai']
-    microhapdb.population.print_table(masai)
-    testout = '''
-       ID  Name Source
-SA000854R Masai ALFRED
-'''
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert terminal.out.strip() == testout.strip()
-
-
-def test_pop_table_multi(capsys):
-    hanchinese = microhapdb.populations[microhapdb.populations.Name == 'Han']
-    microhapdb.population.print_table(hanchinese)
-    testout = '''
-              ID Name                       Source
-MHDBP-48c2cfb2aa  Han 10.1016/j.fsigen.2019.02.018
-       SA000001B  Han                       ALFRED
-       SA000009J  Han                       ALFRED
-'''
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert terminal.out.strip() == testout.strip()
-
-
-def test_pop_detail(capsys):
-    hausa = microhapdb.populations[microhapdb.populations.Name == 'Hausa']
-    microhapdb.population.print_detail(hausa)
-    testout = '''
+    assert pop.shape == (125, 3)
+    assert Population.from_id("MHDBP-7c055e7ee8").name == "Swedish"
+    assert Population.from_id("SA000028K").name == "Karitiana"
+    result = Population.table_from_query("Name.str.contains('Jews')")
+    assert result.ID.tolist() == ["SA000490N", "SA000015G", "SA000096P", "SA000016H"]
+
+
+def test_pop_table():
+    result = Population.table_from_ids(["Masai"])
+    assert len(result) == 1
+    assert result.ID.iloc[0] == "SA000854R"
+    assert result.Source.iloc[0] == "Kidd2018"
+
+
+def test_pop_table_multi():
+    result = Population.table_from_query("Name == 'Han'")
+    assert len(result) == 3
+    assert sorted(result.ID.tolist()) == ["MHDBP-48c2cfb2aa", "SA000001B", "SA000009J"]
+
+
+def test_pop_detail():
+    pop = Population.from_id("Hausa")
+    observed = pop.detail
+    expected = """
 --------------------------------------------------------------[ MicroHapDB ]----
-Hausa    (SA000100B; source=ALFRED)
+Hausa    (SA000100B; source=Kidd2018)
 
 - 878 total allele frequencies available
   for 165 markers
 
 # Alleles | # Markers
 ---------------------
         19|*
@@ -108,38 +112,38 @@
          8|************
          7|****
          6|************
          5|*********************
          4|**************************************************************************************************
          2|****
 --------------------------------------------------------------------------------
-'''
-    terminal = capsys.readouterr()
-    assert terminal.out.strip() == testout.strip()
+"""
+    assert observed.strip() == expected.strip()
 
 
 def test_pop_detail_multi(capsys):
-    japanese = microhapdb.populations[microhapdb.populations.Name == 'Japanese']
-    microhapdb.population.print_detail(japanese)
-    testout = '''
+    for pop in Population.from_query("Name == 'Japanese'"):
+        print(pop.detail)
+    observed = capsys.readouterr().out
+    expected = """
 --------------------------------------------------------------[ MicroHapDB ]----
-Japanese    (MHDBP-63967b883e; source=10.1016/j.legalmed.2015.06.003)
+Japanese    (MHDBP-63967b883e; source=Hiroaki2015)
 
 - 33 total allele frequencies available
   for 7 markers
 
 # Alleles | # Markers
 ---------------------
          7|*
          6|*
          4|*****
 --------------------------------------------------------------------------------
 
 --------------------------------------------------------------[ MicroHapDB ]----
-Japanese    (SA000010B; source=ALFRED)
+Japanese    (SA000010B; source=Kidd2018)
 
 - 878 total allele frequencies available
   for 165 markers
 
 # Alleles | # Markers
 ---------------------
         19|*
@@ -153,25 +157,33 @@
          8|************
          7|****
          6|************
          5|*********************
          4|**************************************************************************************************
          2|****
 --------------------------------------------------------------------------------
-'''
-    terminal = capsys.readouterr()
-    assert terminal.out.strip() == testout.strip()
-
-
-@pytest.mark.parametrize('ident,data', [
-    ('SA000019K', 'SA000019K Russians ALFRED'),
-    ('MHDBP-936bc36f79', 'MHDBP-936bc36f79 Asia 10.1016/j.fsigen.2018.05.008'),
-    ('MHDBP-7c055e7ee8', 'MHDBP-7c055e7ee8 Swedish ISFG2019:P597'),
-    ('MHDBP-63967b883e', 'MHDBP-63967b883e Japanese 10.1016/j.legalmed.2015.06.003'),
-    ('MHDBP-48c2cfb2aa', 'MHDBP-48c2cfb2aa  Han 10.1016/j.fsigen.2019.02.018'),
-])
-def test_all_sources(ident, data, capsys):
-    pop = microhapdb.populations[microhapdb.populations.ID == ident]
-    microhapdb.population.print_table(pop)
-    terminal = capsys.readouterr()
-    print(terminal.out)
-    assert data in terminal.out
+"""
+    assert observed.strip() == expected.strip()
+
+
+@pytest.mark.parametrize(
+    "popid,name,source",
+    [
+        ("SAS", "South Asia", "Byrska-Bishop2022"),
+        ("SA000019K", "Russians", "Kidd2018"),
+        ("MHDBP-48c2cfb2aa", "Han", "Chen2019"),
+        ("mMHseq-Zaramo", "Zaramo", "Gandotra2020"),
+        ("MHDBP-63967b883e", "Japanese", "Hiroaki2015"),
+        ("MHDBP-7c055e7ee8", "Swedish", "Staadig2021"),
+        ("MHDBP-936bc36f79", "Asia", "vanderGaag2018"),
+    ],
+)
+def test_all_sources(popid, name, source):
+    pop = Population.from_id(popid)
+    assert pop.popid == popid
+    assert pop.name == name
+    assert pop.source == source
+
+
+def test_from_id_pop_not_found():
+    with pytest.raises(ValueError, match=r"population 'Romulans' not found"):
+        Population.from_id("Romulans")
```

### Comparing `microhapdb-0.7rc1/microhapdb.egg-info/SOURCES.txt` & `microhapdb-0.9/microhapdb.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,39 +4,38 @@
 setup.cfg
 setup.py
 versioneer.py
 microhapdb/__init__.py
 microhapdb/_version.py
 microhapdb/conftest.py
 microhapdb/marker.py
+microhapdb/nomenclature.py
 microhapdb/panel.py
 microhapdb/population.py
-microhapdb/retrieve.py
-microhapdb/util.py
+microhapdb/tables.py
 microhapdb.egg-info/PKG-INFO
 microhapdb.egg-info/SOURCES.txt
 microhapdb.egg-info/dependency_links.txt
 microhapdb.egg-info/entry_points.txt
 microhapdb.egg-info/requires.txt
 microhapdb.egg-info/top_level.txt
 microhapdb.egg-info/zip-safe
 microhapdb/cli/__init__.py
 microhapdb/cli/frequency.py
 microhapdb/cli/lookup.py
 microhapdb/cli/marker.py
 microhapdb/cli/population.py
-microhapdb/data/frequency.tsv
-microhapdb/data/idmap.tsv
-microhapdb/data/indels.tsv
-microhapdb/data/marker-aes.tsv
-microhapdb/data/marker-offsets-GRCh37.tsv
-microhapdb/data/marker.tsv
-microhapdb/data/population.tsv
-microhapdb/data/sequences.tsv
-microhapdb/data/variantmap.tsv
-microhapdb/data/tests/panel-alpha.fasta
-microhapdb/data/tests/panel-beta.fasta
+microhapdb/cli/summarize.py
+microhapdb/data/frequency.csv.gz
+microhapdb/data/indels.csv
+microhapdb/data/marker-aes.csv
+microhapdb/data/marker.csv
+microhapdb/data/merged.csv
+microhapdb/data/population.csv
 microhapdb/tests/test_cli.py
 microhapdb/tests/test_frequency.py
 microhapdb/tests/test_marker.py
+microhapdb/tests/test_nomenclature.py
 microhapdb/tests/test_population.py
-microhapdb/tests/test_retrieve.py
+microhapdb/tests/test_retrieve.py
+microhapdb/tests/data/panel-alpha.fasta
+microhapdb/tests/data/panel-beta.fasta
```

### Comparing `microhapdb-0.7rc1/setup.py` & `microhapdb-0.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-#!/usr/bin/env python3
+# -------------------------------------------------------------------------------------------------
+# Copyright (c) 2018, DHS.
 #
-# -----------------------------------------------------------------------------
-# Copyright (c) 2018, Battelle National Biodefense Institute.
+# This file is part of MicroHapDB (http://github.com/bioforensics/MicroHapDB) and is licensed under
+# the BSD license: see LICENSE.txt.
 #
-# This file is part of MicroHapDB (http://github.com/bioforensics/microhapdb)
-# and is licensed under the BSD license: see LICENSE.txt.
-# -----------------------------------------------------------------------------
+# This software was prepared for the Department of Homeland Security (DHS) by the Battelle National
+# Biodefense Institute, LLC (BNBI) as part of contract HSHQDC-15-C-00064 to manage and operate the
+# National Biodefense Analysis and Countermeasures Center (NBACC), a Federally Funded Research and
+# Development Center.
+# -------------------------------------------------------------------------------------------------
 
 from setuptools import setup
 import versioneer
 
 
-desc = (
-    'Portable database of microhaplotype marker and allele frequency data'
-)
-with open('README.md', 'r') as infile:
+desc = "Portable database of microhaplotype marker and allele frequency data"
+with open("README.md", "r") as infile:
     longdesc = infile.read()
 
 setup(
-    name='microhapdb',
+    name="microhapdb",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description=desc,
     long_description=longdesc,
-    long_description_content_type='text/markdown',
-    url='https://github.com/bioforensics/MicroHapDB',
-    author='Daniel Standage',
-    author_email='daniel.standage@nbacc.dhs.gov',
-    packages=['microhapdb', 'microhapdb.cli', 'microhapdb.tests'],
-    package_data={
-        'microhapdb': ['microhapdb/data/*', 'microhapdb/data/tests/*']
-    },
+    long_description_content_type="text/markdown",
+    url="https://github.com/bioforensics/MicroHapDB",
+    author="Daniel Standage",
+    author_email="daniel.standage@nbacc.dhs.gov",
+    packages=["microhapdb", "microhapdb.cli", "microhapdb.tests"],
+    package_data={"microhapdb": ["microhapdb/data/*", "microhapdb/data/tests/*"]},
     include_package_data=True,
-    install_requires=['pandas>=1.2'],
-    entry_points={
-        'console_scripts': ['microhapdb = microhapdb.cli:main']
-    },
+    install_requires=["pandas>=1.2", "pyfaidx>=0.7"],
+    entry_points={"console_scripts": ["microhapdb = microhapdb.cli:main"]},
     classifiers=[
-        'Environment :: Console',
-        'Framework :: IPython',
-        'Framework :: Jupyter',
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Legal Industry',
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python :: 3',
-        'Topic :: Scientific/Engineering :: Bio-Informatics',
+        "Environment :: Console",
+        "Framework :: IPython",
+        "Framework :: Jupyter",
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Legal Industry",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python :: 3",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     zip_safe=True,
 )
```

### Comparing `microhapdb-0.7rc1/versioneer.py` & `microhapdb-0.9/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -273,14 +272,15 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
+
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,33 +304,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(me), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -344,14 +348,15 @@
         parser.readfp(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
+
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -368,36 +373,40 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            p = subprocess.Popen(
+                [c] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+            )
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -414,15 +423,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY[
+    "git"
+] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -989,71 +1000,78 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = set([r for r in refs if re.search(r"\d", r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = run_command(
+        GITS,
+        ["describe", "--tags", "--dirty", "--always", "--long", "--match", "%s*" % tag_prefix],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1068,54 +1086,50 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (full_tag, tag_prefix)
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1163,24 +1177,30 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1201,29 +1221,26 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1247,16 +1264,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1362,19 +1378,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1386,17 +1404,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1411,16 +1433,15 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1466,17 +1487,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1517,14 +1542,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1549,22 +1575,23 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1577,25 +1604,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1606,21 +1637,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1639,16 +1674,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(target_versionfile, self._versioneer_generated_versions)
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1695,36 +1730,37 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (EnvironmentError, configparser.NoSectionError, configparser.NoOptionError) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1758,16 +1794,15 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
+        print(" appending versionfile_source ('%s') to MANIFEST.in" % cfg.versionfile_source)
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

