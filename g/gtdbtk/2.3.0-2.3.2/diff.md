# Comparing `tmp/gtdbtk-2.3.0.tar.gz` & `tmp/gtdbtk-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtdbtk-2.3.0.tar", last modified: Tue May  9 00:11:54 2023, max compression
+gzip compressed data, was "gtdbtk-2.3.2.tar", last modified: Wed Jul  5 22:39:36 2023, max compression
```

## Comparing `gtdbtk-2.3.0.tar` & `gtdbtk-2.3.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.405002 gtdbtk-2.3.0/gtdbtk/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/ani_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/ani_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.405002 gtdbtk-2.3.0/gtdbtk/biolib_lite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/custom_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/newick.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/prodigal_biolib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/seq_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    30846 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)   117674 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    24439 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/config/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/decorate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/fastani.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/fasttree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/hmm_aligner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/mash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pfam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pplacer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/prodigal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/external/pypfam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMMatch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4876 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMResults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21015 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMResultsIO.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMSequence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMUnit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/external/pypfam/Scan/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22327 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/Scan/PfamScan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/Scan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/tigrfam_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/batchfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/classify_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/gtdb_radii.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/files/marker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/marker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/marker/copy_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/marker/tophit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/marker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/missing_genomes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/pplacer_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.413002 gtdbtk-2.3.0/gtdbtk/files/prodigal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/prodigal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/prodigal/tln_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/prodigal/tln_table_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/red_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/stage_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/tree_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/infer_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)    54256 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    34860 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.413002 gtdbtk-2.3.0/gtdbtk/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/model/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.413002 gtdbtk-2.3.0/gtdbtk/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/pipeline/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/pipeline/export_msa.py
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/relative_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/reroot_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.401002 gtdbtk-2.3.0/gtdbtk/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.401002 gtdbtk-2.3.0/gtdbtk/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.417002 gtdbtk-2.3.0/gtdbtk/tests/data/genomes/
--rw-r--r--   0 runner    (1001) docker     (123)  2973983 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_1.fna
--rw-r--r--   0 runner    (1001) docker     (123)  1292421 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_2.fna
--rw-r--r--   0 runner    (1001) docker     (123)  1210030 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_3.fna
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12742 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/trim_msa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.405002 gtdbtk-2.3.0/gtdbtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.417002 gtdbtk-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.417002 gtdbtk-2.3.0/tests/test_gtdbtk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_newick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_external/test_fastani.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_external/test_fasttree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/test_tophit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_prodigal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_prodigal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_trim_msa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.252113 gtdbtk-2.3.2/gtdbtk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/ani_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/ani_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.260113 gtdbtk-2.3.2/gtdbtk/biolib_lite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/custom_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/newick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/prodigal_biolib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/seq_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30846 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/biolib_lite/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117674 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24439 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.264113 gtdbtk-2.3.2/gtdbtk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/config/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/decorate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.268113 gtdbtk-2.3.2/gtdbtk/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/fastani.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/fasttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/hmm_aligner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/mash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pfam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pplacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/prodigal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.268113 gtdbtk-2.3.2/gtdbtk/external/pypfam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.268113 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMMatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4876 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMResults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21015 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMResultsIO.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMSequence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMUnit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.272113 gtdbtk-2.3.2/gtdbtk/external/pypfam/Scan/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22327 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/Scan/PfamScan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/Scan/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/pypfam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/external/tigrfam_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.276113 gtdbtk-2.3.2/gtdbtk/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/batchfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/classify_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/gtdb_radii.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.276113 gtdbtk-2.3.2/gtdbtk/files/marker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/marker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/marker/copy_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/marker/tophit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/marker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/missing_genomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/pplacer_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.280113 gtdbtk-2.3.2/gtdbtk/files/prodigal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/prodigal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/prodigal/tln_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/prodigal/tln_table_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/red_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/stage_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/files/tree_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/infer_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54256 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34860 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.284113 gtdbtk-2.3.2/gtdbtk/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/model/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.284113 gtdbtk-2.3.2/gtdbtk/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/pipeline/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/pipeline/export_msa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/relative_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/reroot_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.240113 gtdbtk-2.3.2/gtdbtk/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.244113 gtdbtk-2.3.2/gtdbtk/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.292113 gtdbtk-2.3.2/gtdbtk/tests/data/genomes/
+-rw-r--r--   0 runner    (1001) docker     (123)  2973983 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_1.fna
+-rw-r--r--   0 runner    (1001) docker     (123)  1292421 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_2.fna
+-rw-r--r--   0 runner    (1001) docker     (123)  1210030 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_3.fna
+-rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12742 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/gtdbtk/trim_msa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.256113 gtdbtk-2.3.2/gtdbtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 22:39:36.000000 gtdbtk-2.3.2/gtdbtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/test_gtdbtk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_newick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/test_gtdbtk/test_external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_external/test_fastani.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_external/test_fasttree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.296113 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/test_tophit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:36.300113 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_prodigal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_prodigal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-05 22:39:23.000000 gtdbtk-2.3.2/tests/test_gtdbtk/test_trim_msa.py
```

### Comparing `gtdbtk-2.3.0/LICENSE` & `gtdbtk-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/PKG-INFO` & `gtdbtk-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtdbtk
-Version: 2.3.0
+Version: 2.3.2
 Summary: A toolkit for assigning objective taxonomic classifications to bacterial and archaeal genomes.
 Home-page: https://github.com/Ecogenomics/GTDBTk
 Author: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Author-email: p.chaumeil@uq.edu.au
 Maintainer: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Maintainer-email: donovan.parks@gmail.com
 License: GPL3
```

### Comparing `gtdbtk-2.3.0/README.md` & `gtdbtk-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/__init__.py` & `gtdbtk-2.3.2/gtdbtk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 __maintainer__ = 'Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks'
 __maintainer_email__ = 'donovan.parks@gmail.com'
 __name__ = 'gtdbtk'
 __python_requires__ = '>=3.6'
 __status__ = 'Production'
 __title__ = 'GTDB-Tk'
 __url__ = 'https://github.com/Ecogenomics/GTDBTk'
-__version__ = '2.3.0'
+__version__ = '2.3.2'
```

### Comparing `gtdbtk-2.3.0/gtdbtk/__main__.py` & `gtdbtk-2.3.2/gtdbtk/__main__.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/ani_rep.py` & `gtdbtk-2.3.2/gtdbtk/ani_rep.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/ani_screen.py` & `gtdbtk-2.3.2/gtdbtk/ani_screen.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/common.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/custom_help_formatter.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/custom_help_formatter.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/exceptions.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/exceptions.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/execute.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/execute.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/logger.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/logger.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/newick.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/newick.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/parallel.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/parallel.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/prodigal_biolib.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/prodigal_biolib.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/seq_io.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/seq_io.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/biolib_lite/taxonomy.py` & `gtdbtk-2.3.2/gtdbtk/biolib_lite/taxonomy.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/classify.py` & `gtdbtk-2.3.2/gtdbtk/classify.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/cli.py` & `gtdbtk-2.3.2/gtdbtk/cli.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/config/common.py` & `gtdbtk-2.3.2/gtdbtk/config/common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/config/output.py` & `gtdbtk-2.3.2/gtdbtk/config/output.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/decorate.py` & `gtdbtk-2.3.2/gtdbtk/decorate.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/exceptions.py` & `gtdbtk-2.3.2/gtdbtk/exceptions.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/fastani.py` & `gtdbtk-2.3.2/gtdbtk/external/fastani.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/fasttree.py` & `gtdbtk-2.3.2/gtdbtk/external/fasttree.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/hmm_aligner.py` & `gtdbtk-2.3.2/gtdbtk/external/hmm_aligner.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/mash.py` & `gtdbtk-2.3.2/gtdbtk/external/mash.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,22 +230,25 @@
                     fh.write(f'{path}\n')
 
             args = ['mash', 'sketch', '-l', '-p', self.cpus, path_genomes, '-o',
                     self.path, '-k', self.k, '-s', self.s]
             args = list(map(str, args))
             proc = subprocess.Popen(args, stdout=subprocess.PIPE,
                                     stderr=subprocess.PIPE, encoding='utf-8')
+            stderr_lines = []
             with tqdm_log(total=len(self.genomes), unit='genome') as p_bar:
                 for line in iter(proc.stderr.readline, ''):
+                    stderr_lines.append(line)
                     if line.startswith('Sketching'):
                         p_bar.update()
             proc.wait()
 
             if proc.returncode != 0 or not os.path.isfile(self.path):
-                raise GTDBTkExit(f'Error generating Mash sketch: {proc.stderr.read()}')
+                raise GTDBTkExit(f'Error generating Mash sketch:\n'
+                                 f'{"".join(stderr_lines)}')
 
 
 class QrySketchFile(SketchFile):
     name = 'user_query_sketch.msh'
 
     def __init__(self, genomes, root, prefix, cpus, k, s):
         """Create a query file for a given set of genomes.
```

### Comparing `gtdbtk-2.3.0/gtdbtk/external/pfam_search.py` & `gtdbtk-2.3.2/gtdbtk/external/pfam_search.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/pplacer.py` & `gtdbtk-2.3.2/gtdbtk/external/pplacer.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/prodigal.py` & `gtdbtk-2.3.2/gtdbtk/external/prodigal.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMMatch.py` & `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMMatch.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMResults.py` & `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMResults.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMResultsIO.py` & `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMResultsIO.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMSequence.py` & `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMSequence.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMUnit.py` & `gtdbtk-2.3.2/gtdbtk/external/pypfam/HMM/HMMUnit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/pypfam/Scan/PfamScan.py` & `gtdbtk-2.3.2/gtdbtk/external/pypfam/Scan/PfamScan.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/external/tigrfam_search.py` & `gtdbtk-2.3.2/gtdbtk/external/tigrfam_search.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/batchfile.py` & `gtdbtk-2.3.2/gtdbtk/files/batchfile.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/classify_summary.py` & `gtdbtk-2.3.2/gtdbtk/files/classify_summary.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/gtdb_radii.py` & `gtdbtk-2.3.2/gtdbtk/files/gtdb_radii.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/marker/copy_number.py` & `gtdbtk-2.3.2/gtdbtk/files/marker/copy_number.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/marker/tophit.py` & `gtdbtk-2.3.2/gtdbtk/files/marker/tophit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/marker_info.py` & `gtdbtk-2.3.2/gtdbtk/files/marker_info.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/missing_genomes.py` & `gtdbtk-2.3.2/gtdbtk/files/missing_genomes.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/pplacer_classification.py` & `gtdbtk-2.3.2/gtdbtk/files/pplacer_classification.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/prodigal/tln_table.py` & `gtdbtk-2.3.2/gtdbtk/files/prodigal/tln_table.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/prodigal/tln_table_summary.py` & `gtdbtk-2.3.2/gtdbtk/files/prodigal/tln_table_summary.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/red_dict.py` & `gtdbtk-2.3.2/gtdbtk/files/red_dict.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/stage_logger.py` & `gtdbtk-2.3.2/gtdbtk/files/stage_logger.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/files/tree_mapping.py` & `gtdbtk-2.3.2/gtdbtk/files/tree_mapping.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/infer_ranks.py` & `gtdbtk-2.3.2/gtdbtk/infer_ranks.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/main.py` & `gtdbtk-2.3.2/gtdbtk/main.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/markers.py` & `gtdbtk-2.3.2/gtdbtk/markers.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/misc.py` & `gtdbtk-2.3.2/gtdbtk/misc.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/pipeline/align.py` & `gtdbtk-2.3.2/gtdbtk/pipeline/align.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/pipeline/export_msa.py` & `gtdbtk-2.3.2/gtdbtk/pipeline/export_msa.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/relative_distance.py` & `gtdbtk-2.3.2/gtdbtk/relative_distance.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/reroot_tree.py` & `gtdbtk-2.3.2/gtdbtk/reroot_tree.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/split.py` & `gtdbtk-2.3.2/gtdbtk/split.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_1.fna` & `gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_1.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_2.fna` & `gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_2.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_3.fna` & `gtdbtk-2.3.2/gtdbtk/tests/data/genomes/genome_3.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/tools.py` & `gtdbtk-2.3.2/gtdbtk/tools.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk/trim_msa.py` & `gtdbtk-2.3.2/gtdbtk/trim_msa.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/gtdbtk.egg-info/PKG-INFO` & `gtdbtk-2.3.2/gtdbtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtdbtk
-Version: 2.3.0
+Version: 2.3.2
 Summary: A toolkit for assigning objective taxonomic classifications to bacterial and archaeal genomes.
 Home-page: https://github.com/Ecogenomics/GTDBTk
 Author: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Author-email: p.chaumeil@uq.edu.au
 Maintainer: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Maintainer-email: donovan.parks@gmail.com
 License: GPL3
```

### Comparing `gtdbtk-2.3.0/gtdbtk.egg-info/SOURCES.txt` & `gtdbtk-2.3.2/gtdbtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/setup.py` & `gtdbtk-2.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     data_files=[("", ["LICENSE"])],
     description=meta['description'],
     entry_points={
         'console_scripts': [
             'gtdbtk = gtdbtk.__main__:main'
         ]
     },
-    install_requires=["dendropy>=4.1.0", 'numpy>=1.9.0', 'tqdm>=4.35.0', 'pydantic'],
+    install_requires=["dendropy>=4.1.0", 'numpy>=1.9.0', 'tqdm>=4.35.0', 'pydantic>=1.9.2,<2.0a1'],
     license=meta['license'],
     long_description=readme(),
     long_description_content_type='text/markdown',
     maintainer=meta['maintainer'],
     maintainer_email=meta['maintainer_email'],
     name=meta['name'],
     packages=find_packages(),
```

### Comparing `gtdbtk-2.3.0/tests/common.py` & `gtdbtk-2.3.2/tests/common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_classify.py` & `gtdbtk-2.3.2/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_cli.py` & `gtdbtk-2.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test__main__.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test__main__.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_common.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_newick.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_newick.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_external/test_fastani.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_external/test_fastani.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_external/test_fasttree.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_external/test_fasttree.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/test_tophit.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_marker/test_tophit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_main.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_main.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_markers.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_markers.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_tools.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_tools.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.3.0/tests/test_gtdbtk/test_trim_msa.py` & `gtdbtk-2.3.2/tests/test_gtdbtk/test_trim_msa.py`

 * *Files identical despite different names*

