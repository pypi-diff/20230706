# Comparing `tmp/microcat-0.1.6.tar.gz` & `tmp/microcat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.1.6.tar", last modified: Sat Jun 17 14:38:34 2023, max compression
+gzip compressed data, was "microcat-0.1.7.tar", last modified: Thu Jul  6 06:50:49 2023, max compression
```

## Comparing `microcat-0.1.6.tar` & `microcat-0.1.7.tar`

### file list

```diff
@@ -1,66 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.903153 microcat-0.1.6/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-17 14:38:34.903153 microcat-0.1.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.895153 microcat-0.1.6/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-17 14:38:32.000000 microcat-0.1.6/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      913 2023-06-17 14:38:27.000000 microcat-0.1.6/microcat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/config/
--rw-r--r--   0 root         (0) root         (0)     2840 2023-06-17 11:49:35.000000 microcat-0.1.6/microcat/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.6/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    36419 2023-06-17 14:26:11.000000 microcat-0.1.6/microcat/corer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/envs/
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-17 10:22:04.000000 microcat-0.1.6/microcat/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 02:38:08.000000 microcat-0.1.6/microcat/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.1.6/microcat/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.6/microcat/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 06:24:12.000000 microcat-0.1.6/microcat/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.6/microcat/envs/trimming.yaml
--rwxr-xr-x   0 root         (0) root         (0)     4320 2023-06-17 14:16:31.000000 microcat-0.1.6/microcat/prepare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.895153 microcat-0.1.6/microcat/profiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/profiles/lsf/
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-14 02:37:56.000000 microcat-0.1.6/microcat/profiles/lsf/CookieCutter.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/OSLayer.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_cancel.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_config.py
--rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_jobscript.sh
--rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_status.py
--rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/lsf_submit.py
--rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/profiles/lsf/memory_units.py
--rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.1.6/microcat/rich_agrpase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.6/microcat/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.1.6/microcat/rules/build.smk
--rw-r--r--   0 root         (0) root         (0)    40814 2023-06-09 02:28:56.000000 microcat-0.1.6/microcat/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.6/microcat/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    42505 2023-06-17 11:13:48.000000 microcat-0.1.6/microcat/rules/host.smk
--rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.6/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat/scripts/
--rw-r--r--   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.6/microcat/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.6/microcat/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3849 2023-06-07 07:14:23.000000 microcat-0.1.6/microcat/scripts/extract_microbiome_output.R
--rwxr-xr-x   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/scripts/get_ncbi_domains.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-07 07:15:11.000000 microcat-0.1.6/microcat/scripts/krak2_output_denosing.R
--rwxr-xr-x   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.6/microcat/scripts/kraken2mpa.py
--rwxr-xr-x   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.6/microcat/scripts/kraken2sc.py
--rw-r--r--   0 root         (0) root         (0)     4698 2023-06-07 07:14:59.000000 microcat-0.1.6/microcat/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15665 2023-06-07 07:13:48.000000 microcat-0.1.6/microcat/scripts/sckmer_unpaired.R
--rwxr-xr-x   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.6/microcat/scripts/spilt_bam_by_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.903153 microcat-0.1.6/microcat/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.6/microcat/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)     1832 2023-06-09 04:28:17.000000 microcat-0.1.6/microcat/snakefiles/scRNA_wf.smk
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.6/microcat/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:38:34.899153 microcat-0.1.6/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1564 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-17 14:38:34.000000 microcat-0.1.6/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 14:38:34.903153 microcat-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.471418 microcat-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-06 06:50:49.471418 microcat-0.1.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.127422 microcat-0.1.7/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-06 06:48:34.000000 microcat-0.1.7/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      913 2023-06-17 14:38:27.000000 microcat-0.1.7/microcat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.127422 microcat-0.1.7/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-06-19 01:50:35.000000 microcat-0.1.7/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.7/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    34571 2023-07-06 06:37:50.000000 microcat-0.1.7/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.239421 microcat-0.1.7/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-17 10:22:04.000000 microcat-0.1.7/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 02:38:08.000000 microcat-0.1.7/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.1.7/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.7/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.1.7/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.1.7/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.7/microcat/envs/trimming.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     5102 2023-07-06 06:34:24.000000 microcat-0.1.7/microcat/prepare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.079423 microcat-0.1.7/microcat/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.263421 microcat-0.1.7/microcat/profiles/lsf/
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-14 02:37:56.000000 microcat-0.1.7/microcat/profiles/lsf/CookieCutter.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/profiles/lsf/OSLayer.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/profiles/lsf/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/profiles/lsf/lsf_cancel.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/profiles/lsf/lsf_config.py
+-rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/profiles/lsf/lsf_jobscript.sh
+-rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/profiles/lsf/lsf_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/profiles/lsf/lsf_submit.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/profiles/lsf/memory_units.py
+-rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.1.7/microcat/rich_agrpase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.299420 microcat-0.1.7/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.7/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.1.7/microcat/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    40959 2023-06-25 01:22:49.000000 microcat-0.1.7/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.7/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    74506 2023-07-06 06:41:05.000000 microcat-0.1.7/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.7/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.459418 microcat-0.1.7/microcat/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.7/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.1.7/microcat/scripts/add_tags_to_PathSeq_bam.py
+-rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.1.7/microcat/scripts/create_hdf5.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.7/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3850 2023-06-26 01:17:41.000000 microcat-0.1.7/microcat/scripts/extract_microbiome_output.R
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-06-23 14:00:52.000000 microcat-0.1.7/microcat/scripts/generate_PE_manifest_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/scripts/get_ncbi_domains.py
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-26 01:14:49.000000 microcat-0.1.7/microcat/scripts/krak2_output_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.7/microcat/scripts/kraken2mpa.py
+-rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.7/microcat/scripts/kraken2sc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.1.7/microcat/scripts/microcat_bam_handle.Rmd
+-rwxrwxrwx   0 root         (0) root         (0)     4698 2023-06-26 01:13:57.000000 microcat-0.1.7/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15666 2023-06-26 01:14:02.000000 microcat-0.1.7/microcat/scripts/sckmer_unpaired.R
+-rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.7/microcat/scripts/spilt_bam_by_tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     1973 2023-06-24 01:45:21.000000 microcat-0.1.7/microcat/scripts/split_Starsolo_BAM_by_RG.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.471418 microcat-0.1.7/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.7/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-06-24 02:40:05.000000 microcat-0.1.7/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     8723 2023-07-02 16:16:54.000000 microcat-0.1.7/microcat/snakefiles/scRNA_wf_test.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.7/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:50:49.127422 microcat-0.1.7/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-06 06:50:48.000000 microcat-0.1.7/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-07-06 06:50:48.000000 microcat-0.1.7/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 06:50:48.000000 microcat-0.1.7/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-06 06:50:48.000000 microcat-0.1.7/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-06 06:50:48.000000 microcat-0.1.7/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 06:50:48.000000 microcat-0.1.7/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 06:50:49.471418 microcat-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.7/setup.py
```

### Comparing `microcat-0.1.6/LICENSE` & `microcat-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/PKG-INFO` & `microcat-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.6
+Version: 0.1.7
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.6/microcat/__init__.py` & `microcat-0.1.7/microcat/__init__.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/config/config.yaml` & `microcat-0.1.7/microcat/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/configer.py` & `microcat-0.1.7/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/corer.py` & `microcat-0.1.7/microcat/corer.py`

 * *Files 7% similar despite different names*

```diff
@@ -629,38 +629,20 @@
         print(f"Error: Failed to run prepare.py ({e})")
 
 
 def main():
 
     # Banner text and program information
     banner = '''
-            ███╗   ███╗██╗ ██████╗██████╗  ██████╗  ██████╗ █████╗ ████████╗
-            ████╗ ████║██║██╔════╝██╔══██╗██╔═══██╗██╔════╝██╔══██╗╚══██╔══╝
-            ██╔████╔██║██║██║     ██████╔╝██║   ██║██║     ███████║   ██║   
-            ██║╚██╔╝██║██║██║     ██╔══██╗██║   ██║██║     ██╔══██║   ██║   
-            ██║ ╚═╝ ██║██║╚██████╗██║  ██║╚██████╔╝╚██████╗██║  ██║   ██║   
-            ╚═╝     ╚═╝╚═╝ ╚═════╝╚═╝  ╚═╝ ╚═════╝  ╚═════╝╚═╝  ╚═╝   ╚═╝   
-              *         *     *        *   *     _      *      *      *
-                   *         *                  / )        *     *
-              *            *     (\__/) *       ( (  *       *      *
-                         ,-.,-.,)     (.,-.,-.,-.) ).,-.,-.
-                |  |  |  | @|  ={      }= | @|  / / | @|o |
-    j__j__j__j__j__j__j__j__j__j_)     `-------/ /__j__j__j__j__j__j__j__j_
-    ____________________________(               /__________________________
-                   |    |  | @| \              || o|O | @|
-                   |    |o |  |,'\       ,   ,'"|  |  |  |  hjw
-                   |vV\ vV\|/vV|`-'\  ,---\   | \Vv\hjwVv\//v
-                                  _) )  `. \ /
-                                 (__/      ) )
-                                          (_/
-
     Microbiome Identification in Cell Resolution from Omics-Computational Analysis Toolbox
     
     Version: dev
+
     Manual: https://github.com/ChangxingSu/microcat/wiki
+    
     Source code: https://github.com/ChangxingSu/microcat
     '''
 
     # Create the main parser object with a banner and program name
     parser = argparse.ArgumentParser(
         formatter_class=RichHelpFormatter,
         description=textwrap.dedent(banner),
@@ -869,15 +851,15 @@
         choices=["starsolo","cellranger"],
         help="Which rmhoster used",
     )
     parser_init.add_argument(
         "--assay",
         type=str,
         default=None,
-        choices=["Smartseq", "Smartseq2", "tenX_v3", "tenX_v2", "tenX_v1"],
+        choices=["Smartseq", "Smartseq2", "tenX_v3", "tenX_v2", "tenX_v1","Seq-well","tenX_auto"],
         help="Sequencing assay option, required when host is starsolo",
     )
     
     parser_init.add_argument(
         "--classifier",
         nargs="+",
         required=False,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `microcat-0.1.6/microcat/prepare.py` & `microcat-0.1.7/microcat/prepare.py`

 * *Files 14% similar despite different names*

```diff
@@ -108,9 +108,24 @@
     tenX_v3_barcode_gz_save_path = tenX_v3_barcode_save_path + '.gz'
     print(f"Downloading {tenX_v3_barcode_filename}.gz")
     download_file(tenX_v3_barcode_url, tenX_v3_barcode_gz_save_path)
     print(f"Extracting {tenX_v3_barcode_filename}.gz")
     extract_gzip_file(tenX_v3_barcode_gz_save_path, tenX_v3_barcode_save_path)
     os.remove(tenX_v3_barcode_gz_save_path)
 
+
+tenX_multiome_barcode_url = 'https://github.com/nanoporetech/sockeye/blob/master/data/737K-arc-v1.txt.gz'
+tenX_multiome_barcode_filename = '737K-arc-v1.txt'
+tenX_multiome_barcode_save_path = os.path.join(data_save_path, tenX_multiome_barcode_filename)
+
+
+# Download the file if it doesn't exist
+if not os.path.exists(tenX_multiome_barcode_save_path):
+    tenX_multiome_barcode_gz_save_path = tenX_multiome_barcode_save_path + '.gz'
+    print(f"Downloading {tenX_multiome_barcode_filename}.gz")
+    download_file(tenX_multiome_barcode_url, tenX_multiome_barcode_gz_save_path)
+    print(f"Extracting {tenX_multiome_barcode_filename}.gz")
+    extract_gzip_file(tenX_multiome_barcode_gz_save_path, tenX_multiome_barcode_save_path)
+    os.remove(tenX_multiome_barcode_gz_save_path)
+    
 # Update the config.yaml file
 update_config_file(data_save_path)
```

### Comparing `microcat-0.1.6/microcat/profiles/lsf/CookieCutter.py` & `microcat-0.1.7/microcat/profiles/lsf/CookieCutter.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/profiles/lsf/OSLayer.py` & `microcat-0.1.7/microcat/profiles/lsf/OSLayer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/profiles/lsf/lsf_cancel.py` & `microcat-0.1.7/microcat/profiles/lsf/lsf_cancel.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/profiles/lsf/lsf_config.py` & `microcat-0.1.7/microcat/profiles/lsf/lsf_config.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/profiles/lsf/lsf_status.py` & `microcat-0.1.7/microcat/profiles/lsf/lsf_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/profiles/lsf/lsf_submit.py` & `microcat-0.1.7/microcat/profiles/lsf/lsf_submit.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/profiles/lsf/memory_units.py` & `microcat-0.1.7/microcat/profiles/lsf/memory_units.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/rich_agrpase.py` & `microcat-0.1.7/microcat/rich_agrpase.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/rules/ERCC.smk` & `microcat-0.1.7/microcat/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/rules/build.smk` & `microcat-0.1.7/microcat/rules/build.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/rules/classfier.smk` & `microcat-0.1.7/microcat/rules/classfier.smk`

 * *Files 2% similar despite different names*

```diff
@@ -417,16 +417,16 @@
         log:
             os.path.join(config["logs"]["classifier"],
                         "rmhost_krakenuniq/{sample}_krakenuniq_classifier.log")
         resources:
             mem_mb=config["params"]["classifier"]["krakenuniq"]["mem_mb"]
         conda:
             config["envs"]["krakenuniq"]
-        message:
-            "Classifier: Performing Taxonomic Classifcation of Sample {sample} with krakenuniq."
+        # message:
+        #     "Classifier: Performing Taxonomic Classifcation of Sample {sample} with krakenuniq."
         shell:
             '''
             krakenuniq --db {params.database} \
             --threads {params.threads} \
             --hll-precision {params.estimate_precision} \
             --classified-out {output.krakenuniq_classified_output}\
             --unclassified-out {output.krakenuniq_unclassified_output}\
@@ -649,116 +649,116 @@
             --taxonomy-file {params.taxonomy_db} \
             --scores-output {output.pathseq_classified_score_output} \
             --java-options "-Xmx15g -Xms15G" \
             --conf spark.port.maxRetries=64 \
             {params.pathseqscore_other_params}\
             2>&1 | tee {log}; \
             '''
-    rule pathseq_INVADESEQ:
-        input:
-            unmapped_bam_sorted_file =os.path.join(
-                config["output"]["host"],
-                "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"),
-            features_file = os.path.join(
-                config["output"]["host"],
-                "cellranger_count/{sample}/{sample}_features.tsv"),
-            pathseq_classified_bam_file = os.path.join(
-                            config["output"]["classifier"],
-                            "pathseq_classified_output/{sample}/{sample}_pathseq_classified.bam"),
-            pathseq_output = os.path.join(
+    # rule pathseq_INVADESEQ:
+    #     input:
+    #         unmapped_bam_sorted_file =os.path.join(
+    #             config["output"]["host"],
+    #             "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"),
+    #         features_file = os.path.join(
+    #             config["output"]["host"],
+    #             "cellranger_count/{sample}/{sample}_features.tsv"),
+    #         pathseq_classified_bam_file = os.path.join(
+    #                         config["output"]["classifier"],
+    #                         "pathseq_classified_output/{sample}/{sample}_pathseq_classified.bam"),
+    #         pathseq_output = os.path.join(
+    #             config["output"]["classifier"],
+    #             "pathseq_classified_output/{sample}/{sample}_pathseq_classified.txt")
+    #     output:
+    #         filtered_matrix_readname = os.path.join(
+    #             config["output"]["classifier"],
+    #             "pathseq_final_output/{sample}/{sample}_filtered_matrix_readname.txt"),
+    #         unmap_cbub_bam = os.path.join(
+    #             config["output"]["classifier"],
+    #             "pathseq_final_output/{sample}/{sample}_pathseq_unmap_cbub.bam"),
+    #         unmap_cbub_fasta = os.path.join(
+    #             config["output"]["classifier"],
+    #             "pathseq_final_output/{sample}/{sample}_pathseq_unmap_cbub.fasta"),
+    #         filtered_matrix_list= os.path.join(
+    #             config["output"]["classifier"],
+    #             "pathseq_final_output/{sample}/{sample}_pathseq_filtered_matrix_list.txt"),
+    #         matrix_readnamepath = os.path.join(
+    #                 config["output"]["classifier"],
+    #                 "pathseq_final_output/{sample}/{sample}_filtered_matrix.readnamepath"),
+    #         genus_cell = os.path.join(
+    #                 config["output"]["classifier"],
+    #                 "pathseq_final_output/{sample}/{sample}_genus_cell.txt"),
+    #         filtered_matrix_genus_csv = os.path.join(
+    #                 config["output"]["classifier"],
+    #                 "pathseq_final_output/{sample}/{sample}_filtered_matrix_genus.csv"),
+    #         filtered_matrix_validate = os.path.join(
+    #                 config["output"]["classifier"],
+    #                 "pathseq_final_output/{sample}/{sample}_filtered_matrix.validate.csv")
+    #     conda:
+    #         config["envs"]["kmer_python"]
+    #     params:
+    #         SampleID="{sample}",
+    #         INVADEseq_script = config["scripts"]["INVADEseq"]
+    #     shell:
+    #         '''
+    #         python {params.INVADEseq_script} \
+    #         {input.unmapped_bam_sorted_file} \
+    #         {params.SampleID} \
+    #         {input.features_file} \
+    #         {input.pathseq_classified_bam_file}\
+    #         {input.pathseq_output} \
+    #         {output.filtered_matrix_readname} \
+    #         {output.unmap_cbub_bam} \
+    #         {output.unmap_cbub_fasta} \
+    #         {output.filtered_matrix_list} \
+    #         {output.matrix_readnamepath} \
+    #         {output.genus_cell} \
+    #         {output.filtered_matrix_genus_csv} \
+    #         {output.filtered_matrix_validate}
+    #         '''
+    rule pathseq_classified_all:
+        input:   
+            expand(os.path.join(
                 config["output"]["classifier"],
-                "pathseq_classified_output/{sample}/{sample}_pathseq_classified.txt")
-        output:
-            filtered_matrix_readname = os.path.join(
+                "pathseq_classified_output/{sample}/{sample}_pathseq_classified.bam"),sample=SAMPLES_ID_LIST),
+            expand(os.path.join(
+                config["output"]["classifier"],
+                "pathseq_classified_output/{sample}/{sample}_pathseq_classified.txt"),sample=SAMPLES_ID_LIST),
+            expand(os.path.join(
                 config["output"]["classifier"],
-                "pathseq_final_output/{sample}/{sample}_filtered_matrix_readname.txt"),
-            unmap_cbub_bam = os.path.join(
+                "pathseq_classified_output/{sample}/{sample}_pathseq_filter_metrics.txt"),sample=SAMPLES_ID_LIST),
+            expand(os.path.join(
                 config["output"]["classifier"],
-                "pathseq_final_output/{sample}/{sample}_pathseq_unmap_cbub.bam"),
-            unmap_cbub_fasta = os.path.join(
+                "pathseq_classified_output/{sample}/{sample}_pathseq_score_metrics.txt"),sample=SAMPLES_ID_LIST),
+            expand(os.path.join(
                 config["output"]["classifier"],
-                "pathseq_final_output/{sample}/{sample}_pathseq_unmap_cbub.fasta"),
-            filtered_matrix_list= os.path.join(
-                config["output"]["classifier"],
-                "pathseq_final_output/{sample}/{sample}_pathseq_filtered_matrix_list.txt"),
-            matrix_readnamepath = os.path.join(
-                    config["output"]["classifier"],
-                    "pathseq_final_output/{sample}/{sample}_filtered_matrix.readnamepath"),
-            genus_cell = os.path.join(
-                    config["output"]["classifier"],
-                    "pathseq_final_output/{sample}/{sample}_genus_cell.txt"),
-            filtered_matrix_genus_csv = os.path.join(
-                    config["output"]["classifier"],
-                    "pathseq_final_output/{sample}/{sample}_filtered_matrix_genus.csv"),
-            filtered_matrix_validate = os.path.join(
-                    config["output"]["classifier"],
-                    "pathseq_final_output/{sample}/{sample}_filtered_matrix.validate.csv")
-        conda:
-            config["envs"]["kmer_python"]
-        params:
-            SampleID="{sample}",
-            INVADEseq_script = config["scripts"]["INVADEseq"]
-        shell:
-            '''
-            python {params.INVADEseq_script} \
-            {input.unmapped_bam_sorted_file} \
-            {params.SampleID} \
-            {input.features_file} \
-            {input.pathseq_classified_bam_file}\
-            {input.pathseq_output} \
-            {output.filtered_matrix_readname} \
-            {output.unmap_cbub_bam} \
-            {output.unmap_cbub_fasta} \
-            {output.filtered_matrix_list} \
-            {output.matrix_readnamepath} \
-            {output.genus_cell} \
-            {output.filtered_matrix_genus_csv} \
-            {output.filtered_matrix_validate}
-            '''
-    rule pathseq_classified_all:
-        input:   
+                "pathseq_classified_output/{sample}/{sample}_pathseq_output.txt"),sample=SAMPLES_ID_LIST)
             # expand(os.path.join(
             #     config["output"]["classifier"],
-            #     "pathseq_classified_output/{sample}/{sample}_pathseq_classified.bam"),sample=SAMPLES_ID_LIST),
+            #     "pathseq_final_output/{sample}/{sample}_filtered_matrix_readname.txt"),sample=SAMPLES_ID_LIST),
             # expand(os.path.join(
             #     config["output"]["classifier"],
-            #     "pathseq_classified_output/{sample}/{sample}_pathseq_classified.txt"),sample=SAMPLES_ID_LIST),
+            #     "pathseq_final_output/{sample}/{sample}_pathseq_unmap_cbub.bam"),sample=SAMPLES_ID_LIST),
             # expand(os.path.join(
             #     config["output"]["classifier"],
-            #     "pathseq_classified_output/{sample}/{sample}_pathseq_filter_metrics.txt"),sample=SAMPLES_ID_LIST),
+            #     "pathseq_final_output/{sample}/{sample}_pathseq_unmap_cbub.fasta"),sample=SAMPLES_ID_LIST),
             # expand(os.path.join(
             #     config["output"]["classifier"],
-            #     "pathseq_classified_output/{sample}/{sample}_pathseq_score_metrics.txt"),sample=SAMPLES_ID_LIST)
+            #     "pathseq_final_output/{sample}/{sample}_pathseq_filtered_matrix_list.txt"),sample=SAMPLES_ID_LIST),
             # expand(os.path.join(
-            #     config["output"]["classifier"],
-            #     "pathseq_classified_output/{sample}/{sample}_pathseq_output.txt"),sample=SAMPLES_ID_LIST)
-            expand(os.path.join(
-                config["output"]["classifier"],
-                "pathseq_final_output/{sample}/{sample}_filtered_matrix_readname.txt"),sample=SAMPLES_ID_LIST),
-            expand(os.path.join(
-                config["output"]["classifier"],
-                "pathseq_final_output/{sample}/{sample}_pathseq_unmap_cbub.bam"),sample=SAMPLES_ID_LIST),
-            expand(os.path.join(
-                config["output"]["classifier"],
-                "pathseq_final_output/{sample}/{sample}_pathseq_unmap_cbub.fasta"),sample=SAMPLES_ID_LIST),
-            expand(os.path.join(
-                config["output"]["classifier"],
-                "pathseq_final_output/{sample}/{sample}_pathseq_filtered_matrix_list.txt"),sample=SAMPLES_ID_LIST),
-            expand(os.path.join(
-                    config["output"]["classifier"],
-                    "pathseq_final_output/{sample}/{sample}_filtered_matrix.readnamepath"),sample=SAMPLES_ID_LIST),
-            expand(os.path.join(
-                    config["output"]["classifier"],
-                    "pathseq_final_output/{sample}/{sample}_genus_cell.txt"),sample=SAMPLES_ID_LIST),
-            expand(os.path.join(
-                    config["output"]["classifier"],
-                    "pathseq_final_output/{sample}/{sample}_filtered_matrix_genus.csv"),sample=SAMPLES_ID_LIST),
-            expand(os.path.join(
-                    config["output"]["classifier"],
-                    "pathseq_final_output/{sample}/{sample}_filtered_matrix.validate.csv"),sample=SAMPLES_ID_LIST)
+            #         config["output"]["classifier"],
+            #         "pathseq_final_output/{sample}/{sample}_filtered_matrix.readnamepath"),sample=SAMPLES_ID_LIST),
+            # expand(os.path.join(
+            #         config["output"]["classifier"],
+            #         "pathseq_final_output/{sample}/{sample}_genus_cell.txt"),sample=SAMPLES_ID_LIST),
+            # expand(os.path.join(
+            #         config["output"]["classifier"],
+            #         "pathseq_final_output/{sample}/{sample}_filtered_matrix_genus.csv"),sample=SAMPLES_ID_LIST),
+            # expand(os.path.join(
+            #         config["output"]["classifier"],
+            #         "pathseq_final_output/{sample}/{sample}_filtered_matrix.validate.csv"),sample=SAMPLES_ID_LIST)
 else:
     rule pathseq_classified_all:
         input:    
 
 if config["params"]["classifier"]["metaphlan"]["do"]:
     rule metaphlan_classified:
         input:
```

### Comparing `microcat-0.1.6/microcat/rules/database.smk` & `microcat-0.1.7/microcat/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/sample.py` & `microcat-0.1.7/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/scripts/INVADEseq.py` & `microcat-0.1.7/microcat/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/scripts/extract_kraken_reads.py` & `microcat-0.1.7/microcat/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/scripts/extract_microbiome_output.R` & `microcat-0.1.7/microcat/scripts/extract_microbiome_output.R`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
   make_option(c("--cores"), action="store", default = 8, help = "number of cores at a time")
 )
 
 ## ntaxid: There is a certain limit on the length of command line in Linux system. The maximum length of the command line is determined by the system kernel parameter `ARG_MAX`, 
 ## which is usually several thousand or tens of thousands of characters. If you enter more characters than this limit on the command line, the system will not be able 
 ## to handle the command properly. Therefore, when searching for a large number of tax IDs, it is important to avoid exceeding the limit of command line length for 
 ## successful execution of the command.
-setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Saliba2016")
 
+setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Galeano2022")
 opt = parse_args(OptionParser(option_list = option_list))
 
 kr = read.delim(opt$kraken_report, header = F)
 # removing root and unclassified taxa
 kr = kr[-c(1:2), ]
 mpa = read.delim(opt$mpa_report, header = F)
```

### Comparing `microcat-0.1.6/microcat/scripts/get_ncbi_domains.py` & `microcat-0.1.7/microcat/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/scripts/krak2_output_denosing.R` & `microcat-0.1.7/microcat/scripts/krak2_output_denosing.R`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   make_option(c("--output_file"), action="store", help = "path to kraken output file"),
   make_option(c("--taxa"),type = "character", help = "tsv containing taxa to extract"),
   make_option(c("--out_krak2_denosing"), action="store", help = "output path to save files")
 )
 
 opt = parse_args(OptionParser(option_list = option_list))
 
-setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Saliba2016")
+setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Galeano2022")
 
 krak2_output_file = read.delim(opt$output_file, header = F)
 
 krak2_output_file_taxid = krak2_output_file %>% 
   select(-V1) %>% 
   separate(V3, into = c('name', 'taxid'), sep = '\\(taxid') %>% 
   mutate(taxid = str_remove(taxid, '\\)') %>% trimws(),
```

### Comparing `microcat-0.1.6/microcat/scripts/kraken2mpa.py` & `microcat-0.1.7/microcat/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/scripts/kraken2sc.py` & `microcat-0.1.7/microcat/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/scripts/sample_denosing.R` & `microcat-0.1.7/microcat/scripts/sample_denosing.R`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
               help = "Minimum number of reads per taxon"),
   make_option(c("-u", "--min_uniq"), type = "integer", default = 2,
               help = "Minimum number of unique sequences per taxon")           
 )
 opt_parser <- OptionParser(option_list = option_list)
 opt <- parse_args(opt_parser)
 
-setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Saliba2016/")
+setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Galeano2022")
 
 files <- list.files(opt$path,recursive = TRUE)
 stopifnot(length(files) > 0) # make sure the input dir path is set correctly
 min_reads <- opt$min_reads
 min_uniq <- opt$min_uniq
 
 kraken_report_sample <- read_kraken_reports(files = files,
```

### Comparing `microcat-0.1.6/microcat/scripts/sckmer_unpaired.R` & `microcat-0.1.7/microcat/scripts/sckmer_unpaired.R`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   make_option(c("--kmer_len"), action="store", default = 35, help = "Kraken kmer length"),
   make_option(c("--nsample"), action="store", default = 1000, help = "Max number of barcodes to sample per taxa"),
   make_option(c("--kmer_test_file"), action="store", help = "kmer test output filename"),
   make_option(c("--kmer_file"), action="store", help = "output kmer filename")
 )
 
 opt = parse_args(OptionParser(option_list = option_list))
-setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Saliba2016")
+setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Galeano2022")
 # opt = list(fa1 = '/data/scRNA/EarlyGastricCancer-EGC/results/03.classifier/rmhost_extracted_classified_output/SRR9713114/SRR9713114_kraken2_extracted_classified.fq',
 #            microbiome_output_file = '/data/scRNA/EarlyGastricCancer-EGC/results/03.classifier/rmhost_extracted_classified_output/SRR9713114/SRR9713114_kraken2_extracted_classified_output.txt',
 #            cb_len = 16,
 #            umi_len = 10,
 #            kraken_report = '/data/scRNA/EarlyGastricCancer-EGC/results/03.classifier/rmhost_kraken2_report/custom/SRR9713114/SRR9713114_kraken2_report.txt',
 #            mpa_report = '/data/scRNA/EarlyGastricCancer-EGC/results/03.classifier/rmhost_kraken2_report/mpa/SRR9713114/SRR9713114_kraken2_mpa_report.txt',
 #            ranks = c('G', 'S'),
```

### Comparing `microcat-0.1.6/microcat/scripts/spilt_bam_by_tag.py` & `microcat-0.1.7/microcat/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.6/microcat/snakefiles/scRNA_wf.smk` & `microcat-0.1.7/microcat/snakefiles/scRNA_wf.smk`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 PLATFORM = None
 
 if config["params"]["host"]["starsolo"]["do"]:
     if "tenX" in config["params"]["host"]["starsolo"]["assay"]:
         PLATFORM = "tenX"
     elif "Smartseq" in config["params"]["host"]["starsolo"]["assay"]:
         PLATFORM = "smartseq"
+    elif "Seq-well" in config["params"]["host"]["starsolo"]["assay"]:
+        PLATFORM = "tenX"
     else:
         raise ValueError("Platform must be either 'tenX' or 'smartseq'")
 elif config["params"]["host"]["cellranger"]["do"]:
     PLATFORM = "tenX"
 else:
     raise ValueError("Platform must be either 'tenX' or 'smartseq'")
```

### Comparing `microcat-0.1.6/microcat.egg-info/PKG-INFO` & `microcat-0.1.7/microcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.6
+Version: 0.1.7
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.6/microcat.egg-info/SOURCES.txt` & `microcat-0.1.7/microcat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -36,19 +36,25 @@
 microcat/profiles/lsf/memory_units.py
 microcat/rules/ERCC.smk
 microcat/rules/build.smk
 microcat/rules/classfier.smk
 microcat/rules/database.smk
 microcat/rules/host.smk
 microcat/scripts/INVADEseq.py
+microcat/scripts/add_tags_to_PathSeq_bam.py
+microcat/scripts/create_hdf5.py
 microcat/scripts/extract_kraken_reads.py
 microcat/scripts/extract_microbiome_output.R
+microcat/scripts/generate_PE_manifest_file.py
 microcat/scripts/get_ncbi_domains.py
 microcat/scripts/krak2_output_denosing.R
 microcat/scripts/kraken2mpa.py
 microcat/scripts/kraken2sc.py
+microcat/scripts/microcat_bam_handle.Rmd
 microcat/scripts/sample_denosing.R
 microcat/scripts/sckmer_unpaired.R
 microcat/scripts/spilt_bam_by_tag.py
+microcat/scripts/split_Starsolo_BAM_by_RG.py
 microcat/snakefiles/bulk_wf.smk
 microcat/snakefiles/scRNA_wf.smk
+microcat/snakefiles/scRNA_wf_test.smk
 microcat/snakefiles/spatial_wf.smk
```

### Comparing `microcat-0.1.6/setup.py` & `microcat-0.1.7/setup.py`

 * *Files identical despite different names*

