# Comparing `tmp/trimnami-0.0.2.tar.gz` & `tmp/trimnami-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimnami-0.0.2.tar", last modified: Fri Jun 30 07:19:55 2023, max compression
+gzip compressed data, was "trimnami-0.0.3.tar", last modified: Thu Jul  6 06:25:59 2023, max compression
```

## Comparing `trimnami-0.0.2.tar` & `trimnami-0.0.3.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.602539 trimnami-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-30 07:19:46.000000 trimnami-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-30 07:19:55.602539 trimnami-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-30 07:19:46.000000 trimnami-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 07:19:55.602539 trimnami-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-30 07:19:46.000000 trimnami-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.586539 trimnami-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 07:19:46.000000 trimnami-0.0.2/tests/test_skipHostRm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-30 07:19:46.000000 trimnami-0.0.2/tests/test_trimnami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.586539 trimnami-0.0.2/trimnami/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.590539 trimnami-0.0.2/trimnami/config/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/config/system_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.590539 trimnami-0.0.2/trimnami/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/scripts/skipHostRm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.594539 trimnami-0.0.2/trimnami/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.598539 trimnami-0.0.2/trimnami/test_data/nanopore/
--rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/nanopore/SRR7947171.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/nanopore/SRR7947176.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/test_data/ref.fna
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/trimnami.CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/trimnami.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/trimnami.VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.598539 trimnami-0.0.2/trimnami/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.598539 trimnami-0.0.2/trimnami/workflow/databases/
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/databases/nebnext_adapters.fa
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/databases/primerB.fa
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/databases/rc_primerB_ad6.fa
--rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/databases/vector_contaminants.fa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.598539 trimnami-0.0.2/trimnami/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/bbmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/fastp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/filtlong.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/minimap2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/pigz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/prinseq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/envs/rasusa.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.602539 trimnami-0.0.2/trimnami/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/fastp.smk
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/hostRemoval.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/nanopore.smk
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/notrim.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/preflight.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/prinseq.smk
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/reports.smk
--rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-06-30 07:19:46.000000 trimnami-0.0.2/trimnami/workflow/rules/roundAB.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:19:55.590539 trimnami-0.0.2/trimnami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 07:19:55.000000 trimnami-0.0.2/trimnami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.980682 trimnami-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 06:25:50.000000 trimnami-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-06 06:25:59.980682 trimnami-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-06 06:25:50.000000 trimnami-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:25:59.980682 trimnami-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-06 06:25:50.000000 trimnami-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-06 06:25:50.000000 trimnami-0.0.3/tests/test_skipHostRm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 06:25:50.000000 trimnami-0.0.3/tests/test_trimnami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/trimnami/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/trimnami/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/config/system_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/trimnami/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/scripts/skipHostRm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.972682 trimnami-0.0.3/trimnami/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.976682 trimnami-0.0.3/trimnami/test_data/nanopore/
+-rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/nanopore/SRR7947171.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/nanopore/SRR7947176.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/test_data/ref.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/trimnami.CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/trimnami.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/trimnami.VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.976682 trimnami-0.0.3/trimnami/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.976682 trimnami-0.0.3/trimnami/workflow/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/databases/nebnext_adapters.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/databases/primerB.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/databases/rc_primerB_ad6.fa
+-rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/databases/vector_contaminants.fa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.980682 trimnami-0.0.3/trimnami/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/bbmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/fastp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/fastqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/filtlong.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/minimap2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/multiqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/pigz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/prinseq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/envs/rasusa.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.980682 trimnami-0.0.3/trimnami/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/fastp.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/fastqc.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/hostRemoval.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/nanopore.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/notrim.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/preflight.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/prinseq.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/reports.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-07-06 06:25:50.000000 trimnami-0.0.3/trimnami/workflow/rules/roundAB.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:25:59.968682 trimnami-0.0.3/trimnami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 06:25:59.000000 trimnami-0.0.3/trimnami.egg-info/top_level.txt
```

### Comparing `trimnami-0.0.2/PKG-INFO` & `trimnami-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,13 @@
-Metadata-Version: 2.1
-Name: trimnami
-Version: 0.0.2
-Summary: Trim lots of metagenomics samples all at once.
-Home-page: https://github.com/beardymcjohnface/Trimnami
-Author: Michael Roach
-Author-email: beardymcjohnface@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 ![](trimnami.png)
 
 [![](https://img.shields.io/static/v1?label=CLI&message=Snaketool&color=blueviolet)](https://github.com/beardymcjohnface/Snaketool)
 [![](https://img.shields.io/static/v1?label=Licence&message=MIT&color=black)](https://opensource.org/license/mit/)
 [![](https://img.shields.io/static/v1?label=Install%20with&message=PIP&color=success)](https://pypi.org/project/trimnami/)
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/beardymcjohnface/Trimnami/main)
 [![Unit tests](https://github.com/beardymcjohnface/Trimnami/actions/workflows/python-app.yml/badge.svg)](https://github.com/beardymcjohnface/Trimnami/actions/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/beardymcjohnface/Trimnami/branch/main/graph/badge.svg?token=E0w8zHLLDq)](https://codecov.io/gh/beardymcjohnface/Trimnami)
 
 
 ---
 
 Trim lots of metagenomics samples all at once.
```

### Comparing `trimnami-0.0.2/README.md` & `trimnami-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+Metadata-Version: 2.1
+Name: trimnami
+Version: 0.0.3
+Summary: Trim lots of metagenomics samples all at once.
+Home-page: https://github.com/beardymcjohnface/Trimnami
+Author: Michael Roach
+Author-email: beardymcjohnface@gmail.com
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 ![](trimnami.png)
 
 [![](https://img.shields.io/static/v1?label=CLI&message=Snaketool&color=blueviolet)](https://github.com/beardymcjohnface/Snaketool)
 [![](https://img.shields.io/static/v1?label=Licence&message=MIT&color=black)](https://opensource.org/license/mit/)
 [![](https://img.shields.io/static/v1?label=Install%20with&message=PIP&color=success)](https://pypi.org/project/trimnami/)
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/beardymcjohnface/Trimnami/main)
 [![Unit tests](https://github.com/beardymcjohnface/Trimnami/actions/workflows/python-app.yml/badge.svg)](https://github.com/beardymcjohnface/Trimnami/actions/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/beardymcjohnface/Trimnami/branch/main/graph/badge.svg?token=E0w8zHLLDq)](https://codecov.io/gh/beardymcjohnface/Trimnami)
 
 
 ---
 
 Trim lots of metagenomics samples all at once.
```

### Comparing `trimnami-0.0.2/setup.py` & `trimnami-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/tests/test_skipHostRm.py` & `trimnami-0.0.3/tests/test_skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/tests/test_trimnami.py` & `trimnami-0.0.3/tests/test_trimnami.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     exec_command("trimnami -v")
     exec_command("trimnami -h")
     exec_command("trimnami run -h")
     exec_command("trimnami config -h")
 
 
 def test_trimnami_commands(tmp_dir):
-    exec_command("trimnami test --threads 1 -n prinseq fastp roundAB nanopore notrim")
+    exec_command("trimnami test --threads 1 --fastqc -n prinseq fastp roundAB nanopore notrim")
     exec_command("trimnami config")
     exec_command("trimnami citation")
```

### Comparing `trimnami-0.0.2/trimnami/__main__.py` & `trimnami-0.0.3/trimnami/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,20 @@
             callback=default_to_output,
             help="Custom config file [default: (outputDir)/trimnami.config.yaml]",
         ),
         click.option(
             "--threads", help="Number of threads to use", default=8, show_default=True
         ),
         click.option(
+            "--fastqc/--no-fastqc",
+            default=False,
+            help="Run fastqc on trimmed and untrimmed reads",
+            show_default=True,
+        ),
+        click.option(
             "--use-conda/--no-use-conda",
             default=True,
             help="Use conda for Snakemake rules",
             show_default=True,
         ),
         click.option(
             "--conda-prefix",
@@ -107,16 +113,15 @@
     \b
     For more options, run:
     trimnami command --help"""
     pass
 
 
 def print_splash():
-    click.echo("""
-\b
+    click.echo("""\b
 ████████╗██████╗ ██╗███╗   ███╗███╗   ██╗ █████╗ ███╗   ███╗██╗
 ╚══██╔══╝██╔══██╗██║████╗ ████║████╗  ██║██╔══██╗████╗ ████║██║
    ██║   ██████╔╝██║██╔████╔██║██╔██╗ ██║███████║██╔████╔██║██║
    ██║   ██╔══██╗██║██║╚██╔╝██║██║╚██╗██║██╔══██║██║╚██╔╝██║██║
    ██║   ██║  ██║██║██║ ╚═╝ ██║██║ ╚████║██║  ██║██║ ╚═╝ ██║██║
    ╚═╝   ╚═╝  ╚═╝╚═╝╚═╝     ╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝╚═╝     ╚═╝╚═╝
 """)
@@ -137,14 +142,15 @@
 Add Snakemake args: trimnami run ... --dry-run --keep-going --touch
 Specify targets:    trimnami run ... all print_targets
 Available targets:
     fastp           Trim reads with fastp (default)
     prinseq         Trim reads with prinseq++
     roundAB         Trim round A/B viral metagenome reads
     nanopore        Trim nanopore reads
+    notrim          Skip read trimming
     print_targets   List available targets
 """
 
 
 @click.command(
     epilog=help_msg_extra,
     context_settings=dict(
@@ -156,20 +162,23 @@
 @click.option("--minimap", help="Minimap preset", default="sr", show_default=True,
               type=click.Choice(["map-pb", "map-ont", "map-hifi", "sr"]))
 @common_options
 def run(**kwargs):
     """Run Trimnami"""
     # Config to add or update in configfile
     merge_config = {
-        "args": {
-            "reads": kwargs["reads"],
-            "output": kwargs["output"],
-            "host": kwargs["host"],
-            "minimap": kwargs["minimap"],
-            "log": kwargs["log"]
+        "trimnami": {
+            "args": {
+                "reads": kwargs["reads"],
+                "output": kwargs["output"],
+                "host": kwargs["host"],
+                "fastqc": kwargs["fastqc"],
+                "minimap": kwargs["minimap"],
+                "log": kwargs["log"]
+            }
         }
     }
 
     # run!
     run_snakemake(
         # Full path to Snakefile
         snakefile_path=snake_base(os.path.join("workflow", "Snakefile")),
@@ -186,20 +195,23 @@
     ),
 )
 @common_options
 def test(**kwargs):
     """Run Trimnami with the test dataset"""
     # Config to add or update in configfile
     merge_config = {
-        "args": {
-            "reads": snake_base(os.path.join("test_data")),
-            "host": None,
-            "output": kwargs["output"],
-            "minimap": "sr",
-            "log": kwargs["log"]
+        "trimnami": {
+            "args": {
+                "reads": snake_base(os.path.join("test_data")),
+                "host": None,
+                "fastqc": kwargs["fastqc"],
+                "output": kwargs["output"],
+                "minimap": "sr",
+                "log": kwargs["log"]
+            }
         }
     }
 
     # run!
     run_snakemake(
         # Full path to Snakefile
         snakefile_path=snake_base(os.path.join("workflow", "Snakefile")),
@@ -216,20 +228,23 @@
     ),
 )
 @common_options
 def testhost(**kwargs):
     """Run Trimnami with the test dataset and test host"""
     # Config to add or update in configfile
     merge_config = {
-        "args": {
-            "reads": snake_base(os.path.join("test_data")),
-            "host": snake_base(os.path.join("test_data", "ref.fna")),
-            "output": kwargs["output"],
-            "minimap": "sr",
-            "log": kwargs["log"]
+        "trimnami": {
+            "args": {
+                "reads": snake_base(os.path.join("test_data")),
+                "host": snake_base(os.path.join("test_data", "ref.fna")),
+                "output": kwargs["output"],
+                "fastqc": kwargs["fastqc"],
+                "minimap": "sr",
+                "log": kwargs["log"]
+            }
         }
     }
 
     # run!
     run_snakemake(
         # Full path to Snakefile
         snakefile_path=snake_base(os.path.join("workflow", "Snakefile")),
@@ -246,20 +261,23 @@
     ),
 )
 @common_options
 def testnp(**kwargs):
     """Run Trimnami with the test dataset and test host"""
     # Config to add or update in configfile
     merge_config = {
-        "args": {
-            "reads": snake_base(os.path.join("test_data", "nanopore")),
-            "host": snake_base(os.path.join("test_data", "ref.fna")),
-            "output": kwargs["output"],
-            "minimap": "map-ont",
-            "log": kwargs["log"]
+        "trimnami": {
+            "args": {
+                "reads": snake_base(os.path.join("test_data", "nanopore")),
+                "host": snake_base(os.path.join("test_data", "ref.fna")),
+                "output": kwargs["output"],
+                "fastqc": kwargs["fastqc"],
+                "minimap": "map-ont",
+                "log": kwargs["log"]
+            }
         }
     }
 
     kwargs["snake_args"] = ["nanopore"]
 
     # run!
     run_snakemake(
```

### Comparing `trimnami-0.0.2/trimnami/config/config.yaml` & `trimnami-0.0.3/trimnami/config/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-resources:
-  job:
-    cpu: 8
-    mem: 16000
-    time: 480
-
-qc:
-    compression: 1
-    minimapIndex:
-        -I 8G
-    fastp:
-        --qualified_quality_phred 15
-        --length_required 90
-        --cut_tail 
-        --cut_tail_window_size 25
-        --cut_tail_mean_quality 15
-        --dedup
-        --dup_calc_accuracy 4
-        --trim_poly_x
-        --detect_adapter_for_pe
-    prinseq:
-        -min_len 60 
-        -min_qual_mean 25 
-        -ns_max_n 1 
-        -derep 1
-        -out_format 0 
-        -trim_tail_left 5 
-        -trim_tail_right 5
-        -ns_max_n 5  
-        -trim_qual_type min 
-        -trim_qual_left 30
-        -trim_qual_right 30 
-        -trim_qual_window 10
-    nanopore:
-        filtlong:
-            --min_length 1000
-            --keep_percent 95
-        rasusa:
-            --bases 10000000
+trimnami:
+    resources:
+        job:
+            cpu: 8
+            mem: 16000
+            time: 480
+    qc:
+        compression:
+            1
+        minimapIndex:
+            -I 8G
+        fastp:
+            --qualified_quality_phred 15
+            --length_required 90
+            --cut_tail 
+            --cut_tail_window_size 25
+            --cut_tail_mean_quality 15
+            --dedup
+            --dup_calc_accuracy 4
+            --trim_poly_x
+            --detect_adapter_for_pe
+        prinseq:
+            -min_len 60 
+            -min_qual_mean 25 
+            -ns_max_n 1 
+            -derep 1
+            -out_format 0 
+            -trim_tail_left 5 
+            -trim_tail_right 5
+            -ns_max_n 5  
+            -trim_qual_type min 
+            -trim_qual_left 30
+            -trim_qual_right 30 
+            -trim_qual_window 10
+        nanopore:
+            filtlong:
+                --min_length 1000
+                --keep_percent 95
+            rasusa:
+                --bases 10000000
```

### Comparing `trimnami-0.0.2/trimnami/scripts/skipHostRm.py` & `trimnami-0.0.3/trimnami/scripts/skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz` & `trimnami-0.0.3/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz` & `trimnami-0.0.3/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz` & `trimnami-0.0.3/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz` & `trimnami-0.0.3/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/test_data/A13-135-177-06_AGTTCC.fastq` & `trimnami-0.0.3/trimnami/test_data/A13-135-177-06_AGTTCC.fastq`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/test_data/nanopore/SRR7947171.fastq.gz` & `trimnami-0.0.3/trimnami/test_data/nanopore/SRR7947171.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/test_data/nanopore/SRR7947176.fastq.gz` & `trimnami-0.0.3/trimnami/test_data/nanopore/SRR7947176.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/test_data/ref.fna` & `trimnami-0.0.3/trimnami/test_data/ref.fna`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/trimnami.LICENSE` & `trimnami-0.0.3/trimnami/trimnami.LICENSE`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/Snakefile` & `trimnami-0.0.3/trimnami/workflow/Snakefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import attrmap as ap
 import attrmap.utils as au
 
 
 configfile: os.path.join(workflow.basedir, '../', 'config', 'config.yaml')
 configfile: os.path.join(workflow.basedir, '../', 'config', 'system_config.yaml')
-config = ap.AttrMap(config)
+config = ap.AttrMap(config["trimnami"])
 
 
 def copy_log_file():
     """Concatenate Snakemake's own logfile with the CLI logfile"""
     files = glob.glob(os.path.join(".snakemake", "log", "*.snakemake.log"))
     if files:
         current_log = max(files, key=os.path.getmtime)
@@ -21,14 +21,15 @@
 onerror:
     copy_log_file()
 
 
 # Import rules
 include: os.path.join("rules", "preflight.smk")
 include: os.path.join("rules", "hostRemoval.smk")
+include: os.path.join("rules", "fastqc.smk")
 include: os.path.join("rules", "fastp.smk")
 include: os.path.join("rules", "prinseq.smk")
 include: os.path.join("rules", "roundAB.smk")
 include: os.path.join("rules", "nanopore.smk")
 include: os.path.join("rules", "notrim.smk")
 include: os.path.join("rules", "reports.smk")
```

### Comparing `trimnami-0.0.2/trimnami/workflow/databases/nebnext_adapters.fa` & `trimnami-0.0.3/trimnami/workflow/databases/nebnext_adapters.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/databases/primerB.fa` & `trimnami-0.0.3/trimnami/workflow/databases/primerB.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/databases/rc_primerB_ad6.fa` & `trimnami-0.0.3/trimnami/workflow/databases/rc_primerB_ad6.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/databases/vector_contaminants.fa` & `trimnami-0.0.3/trimnami/workflow/databases/vector_contaminants.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/rules/fastp.smk` & `trimnami-0.0.3/trimnami/workflow/rules/fastp.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/rules/hostRemoval.smk` & `trimnami-0.0.3/trimnami/workflow/rules/hostRemoval.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/rules/nanopore.smk` & `trimnami-0.0.3/trimnami/workflow/rules/nanopore.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/rules/notrim.smk` & `trimnami-0.0.3/trimnami/workflow/rules/notrim.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/rules/prinseq.smk` & `trimnami-0.0.3/trimnami/workflow/rules/prinseq.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami/workflow/rules/roundAB.smk` & `trimnami-0.0.3/trimnami/workflow/rules/roundAB.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.2/trimnami.egg-info/PKG-INFO` & `trimnami-0.0.3/trimnami.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![](trimnami.png)
 
 [![](https://img.shields.io/static/v1?label=CLI&message=Snaketool&color=blueviolet)](https://github.com/beardymcjohnface/Snaketool)
 [![](https://img.shields.io/static/v1?label=Licence&message=MIT&color=black)](https://opensource.org/license/mit/)
 [![](https://img.shields.io/static/v1?label=Install%20with&message=PIP&color=success)](https://pypi.org/project/trimnami/)
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/beardymcjohnface/Trimnami/main)
 [![Unit tests](https://github.com/beardymcjohnface/Trimnami/actions/workflows/python-app.yml/badge.svg)](https://github.com/beardymcjohnface/Trimnami/actions/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/beardymcjohnface/Trimnami/branch/main/graph/badge.svg?token=E0w8zHLLDq)](https://codecov.io/gh/beardymcjohnface/Trimnami)
 
 
 ---
 
 Trim lots of metagenomics samples all at once.
```

### Comparing `trimnami-0.0.2/trimnami.egg-info/SOURCES.txt` & `trimnami-0.0.3/trimnami.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,20 +29,23 @@
 trimnami/workflow/Snakefile
 trimnami/workflow/databases/nebnext_adapters.fa
 trimnami/workflow/databases/primerB.fa
 trimnami/workflow/databases/rc_primerB_ad6.fa
 trimnami/workflow/databases/vector_contaminants.fa
 trimnami/workflow/envs/bbmap.yaml
 trimnami/workflow/envs/fastp.yaml
+trimnami/workflow/envs/fastqc.yaml
 trimnami/workflow/envs/filtlong.yaml
 trimnami/workflow/envs/minimap2.yaml
+trimnami/workflow/envs/multiqc.yaml
 trimnami/workflow/envs/pigz.yaml
 trimnami/workflow/envs/prinseq.yaml
 trimnami/workflow/envs/rasusa.yaml
 trimnami/workflow/rules/fastp.smk
+trimnami/workflow/rules/fastqc.smk
 trimnami/workflow/rules/hostRemoval.smk
 trimnami/workflow/rules/nanopore.smk
 trimnami/workflow/rules/notrim.smk
 trimnami/workflow/rules/preflight.smk
 trimnami/workflow/rules/prinseq.smk
 trimnami/workflow/rules/reports.smk
 trimnami/workflow/rules/roundAB.smk
```

