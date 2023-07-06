# Comparing `tmp/seismic-rna-0.1.0.tar.gz` & `tmp/seismic-rna-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-rna-0.1.0.tar", last modified: Fri Jun 30 05:00:11 2023, max compression
+gzip compressed data, was "seismic-rna-0.1.1.tar", last modified: Thu Jul  6 01:29:40 2023, max compression
```

## Comparing `seismic-rna-0.1.0.tar` & `seismic-rna-0.1.1.tar`

### file list

```diff
@@ -1,112 +1,116 @@
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.732189 seismic-rna-0.1.0/
--rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.1.0/LICENSE
--rw-r--r--   0 mfa        (503) staff       (20)     1822 2023-06-30 05:00:11.731816 seismic-rna-0.1.0/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     1259 2023-06-29 04:20:57.000000 seismic-rna-0.1.0/README.md
--rw-r--r--   0 mfa        (503) staff       (20)      998 2023-06-30 04:29:15.000000 seismic-rna-0.1.0/pyproject.toml
--rw-r--r--   0 mfa        (503) staff       (20)       38 2023-06-30 05:00:11.732298 seismic-rna-0.1.0/setup.cfg
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.088842 seismic-rna-0.1.0/src/
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.132838 seismic-rna-0.1.0/src/seismic_rna.egg-info/
--rw-r--r--   0 mfa        (503) staff       (20)     1822 2023-06-30 05:00:11.000000 seismic-rna-0.1.0/src/seismic_rna.egg-info/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     2881 2023-06-30 05:00:11.000000 seismic-rna-0.1.0/src/seismic_rna.egg-info/SOURCES.txt
--rw-r--r--   0 mfa        (503) staff       (20)        1 2023-06-30 05:00:11.000000 seismic-rna-0.1.0/src/seismic_rna.egg-info/dependency_links.txt
--rw-r--r--   0 mfa        (503) staff       (20)       50 2023-06-30 05:00:11.000000 seismic-rna-0.1.0/src/seismic_rna.egg-info/entry_points.txt
--rw-r--r--   0 mfa        (503) staff       (20)      153 2023-06-30 05:00:11.000000 seismic-rna-0.1.0/src/seismic_rna.egg-info/requires.txt
--rw-r--r--   0 mfa        (503) staff       (20)       11 2023-06-30 05:00:11.000000 seismic-rna-0.1.0/src/seismic_rna.egg-info/top_level.txt
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.159678 seismic-rna-0.1.0/src/seismicrna/
--rw-r--r--   0 mfa        (503) staff       (20)      201 2023-06-29 18:12:04.000000 seismic-rna-0.1.0/src/seismicrna/__init__.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.194555 seismic-rna-0.1.0/src/seismicrna/align/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/align/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    22639 2023-06-30 02:20:07.000000 seismic-rna-0.1.0/src/seismicrna/align/fq2bam.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/align/fqutil.py
--rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-06-29 21:22:27.000000 seismic-rna-0.1.0/src/seismicrna/align/main.py
--rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/align/strandedness.py
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/align/test.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.257276 seismic-rna-0.1.0/src/seismicrna/cluster/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     9128 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/compare.py
--rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/em.py
--rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/krun.py
--rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1874 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/main.py
--rw-r--r--   0 mfa        (503) staff       (20)      384 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/names.py
--rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/cluster/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.432216 seismic-rna-0.1.0/src/seismicrna/core/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.1.0/src/seismicrna/core/bitcall.py
--rw-r--r--   0 mfa        (503) staff       (20)    17933 2023-06-29 19:57:56.000000 seismic-rna-0.1.0/src/seismicrna/core/bitvect.py
--rw-r--r--   0 mfa        (503) staff       (20)    24198 2023-06-30 00:55:13.000000 seismic-rna-0.1.0/src/seismicrna/core/cli.py
--rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.1.0/src/seismicrna/core/depend.py
--rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/docdef.py
--rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/docstring.py
--rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/dump.py
--rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/files.py
--rw-r--r--   0 mfa        (503) staff       (20)    14191 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/files_sanity.py
--rw-r--r--   0 mfa        (503) staff       (20)     7851 2023-06-29 19:57:01.000000 seismic-rna-0.1.0/src/seismicrna/core/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2867 2023-06-29 17:37:52.000000 seismic-rna-0.1.0/src/seismicrna/core/logs.py
--rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/mu.py
--rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-06-29 19:37:32.000000 seismic-rna-0.1.0/src/seismicrna/core/parallel.py
--rw-r--r--   0 mfa        (503) staff       (20)    23506 2023-06-29 20:01:50.000000 seismic-rna-0.1.0/src/seismicrna/core/path.py
--rw-r--r--   0 mfa        (503) staff       (20)    29386 2023-06-29 17:35:09.000000 seismic-rna-0.1.0/src/seismicrna/core/rel.py
--rw-r--r--   0 mfa        (503) staff       (20)    29463 2023-06-29 19:57:29.000000 seismic-rna-0.1.0/src/seismicrna/core/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/rna.py
--rw-r--r--   0 mfa        (503) staff       (20)    26188 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/sect.py
--rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.1.0/src/seismicrna/core/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.1.0/src/seismicrna/core/shell.py
--rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.1.0/src/seismicrna/core/sim.py
--rw-r--r--   0 mfa        (503) staff       (20)    71099 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/test.py
--rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/core/types.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.1.0/src/seismicrna/core/xam.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.452439 seismic-rna-0.1.0/src/seismicrna/demult/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/demult/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    42588 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/demult/demultiplex.py
--rw-r--r--   0 mfa        (503) staff       (20)     2073 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/demult/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.505870 seismic-rna-0.1.0/src/seismicrna/draw/
--rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.1.0/src/seismicrna/draw/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/draw/load_dataset.py
--rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/draw/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/draw/manipulator.py
--rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.1.0/src/seismicrna/draw/plotter.py
--rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/draw/study.py
--rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/draw/util.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.553900 seismic-rna-0.1.0/src/seismicrna/graph/
--rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/graph/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     8667 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/graph/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     3249 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/graph/color.py
--rw-r--r--   0 mfa        (503) staff       (20)     2700 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/graph/default.py
--rw-r--r--   0 mfa        (503) staff       (20)     7441 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/graph/hist.py
--rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/graph/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     8608 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/graph/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     9744 2023-06-30 04:08:02.000000 seismic-rna-0.1.0/src/seismicrna/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.588904 seismic-rna-0.1.0/src/seismicrna/mask/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/mask/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     4083 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/mask/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     4321 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/mask/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/mask/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    13982 2023-06-29 19:40:06.000000 seismic-rna-0.1.0/src/seismicrna/mask/write.py
--rw-r--r--   0 mfa        (503) staff       (20)       48 2023-06-30 04:29:48.000000 seismic-rna-0.1.0/src/seismicrna/meta.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.657421 seismic-rna-0.1.0/src/seismicrna/relate/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/relate/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/relate/export.py
--rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/relate/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     3175 2023-06-30 04:06:44.000000 seismic-rna-0.1.0/src/seismicrna/relate/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/relate/relate.py
--rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/relate/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.1.0/src/seismicrna/relate/sam.py
--rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/relate/seqpos.py
--rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/relate/test.py
--rw-r--r--   0 mfa        (503) staff       (20)    15021 2023-06-30 04:03:22.000000 seismic-rna-0.1.0/src/seismicrna/relate/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.678138 seismic-rna-0.1.0/src/seismicrna/struct/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/struct/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3905 2023-06-29 20:47:08.000000 seismic-rna-0.1.0/src/seismicrna/struct/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1862 2023-06-29 20:23:36.000000 seismic-rna-0.1.0/src/seismicrna/struct/rnastructure.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.719011 seismic-rna-0.1.0/src/seismicrna/table/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/table/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     7405 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/table/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     5929 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/table/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1520 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/table/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    14642 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/table/tabulate.py
--rw-r--r--   0 mfa        (503) staff       (20)     4841 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/table/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-06-30 05:00:11.731281 seismic-rna-0.1.0/src/seismicrna/test/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.0/src/seismicrna/test/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      914 2023-06-29 19:51:19.000000 seismic-rna-0.1.0/src/seismicrna/test/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.569640 seismic-rna-0.1.1/
+-rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.1.1/LICENSE
+-rw-r--r--   0 mfa        (503) staff       (20)     1831 2023-07-06 01:29:40.568861 seismic-rna-0.1.1/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     1268 2023-07-06 00:54:05.000000 seismic-rna-0.1.1/README.md
+-rw-r--r--   0 mfa        (503) staff       (20)      997 2023-07-06 00:52:32.000000 seismic-rna-0.1.1/pyproject.toml
+-rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-06 01:29:40.569757 seismic-rna-0.1.1/setup.cfg
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.469309 seismic-rna-0.1.1/src/
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.482473 seismic-rna-0.1.1/src/seismic_rna.egg-info/
+-rw-r--r--   0 mfa        (503) staff       (20)     1831 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     3013 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/SOURCES.txt
+-rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/dependency_links.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/entry_points.txt
+-rw-r--r--   0 mfa        (503) staff       (20)      153 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/requires.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/top_level.txt
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.484731 seismic-rna-0.1.1/src/seismicrna/
+-rw-r--r--   0 mfa        (503) staff       (20)      201 2023-06-29 18:12:04.000000 seismic-rna-0.1.1/src/seismicrna/__init__.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.489835 seismic-rna-0.1.1/src/seismicrna/align/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/align/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.1.1/src/seismicrna/align/fq2bam.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/align/fqutil.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-06-29 21:22:27.000000 seismic-rna-0.1.1/src/seismicrna/align/main.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/align/strandedness.py
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/align/test.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.495106 seismic-rna-0.1.1/src/seismicrna/cluster/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9128 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/compare.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/em.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/krun.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1874 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)      384 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/names.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.525226 seismic-rna-0.1.1/src/seismicrna/core/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.1.1/src/seismicrna/core/bitcall.py
+-rw-r--r--   0 mfa        (503) staff       (20)    17933 2023-06-29 19:57:56.000000 seismic-rna-0.1.1/src/seismicrna/core/bitvect.py
+-rw-r--r--   0 mfa        (503) staff       (20)    24046 2023-07-05 20:58:22.000000 seismic-rna-0.1.1/src/seismicrna/core/cli.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.1.1/src/seismicrna/core/depend.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/docdef.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/docstring.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/dump.py
+-rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/files.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14191 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/files_sanity.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7851 2023-06-29 19:57:01.000000 seismic-rna-0.1.1/src/seismicrna/core/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2867 2023-06-29 17:37:52.000000 seismic-rna-0.1.1/src/seismicrna/core/logs.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/mu.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.1.1/src/seismicrna/core/mu_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-06-29 19:37:32.000000 seismic-rna-0.1.1/src/seismicrna/core/parallel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    23506 2023-06-29 20:01:50.000000 seismic-rna-0.1.1/src/seismicrna/core/path.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29386 2023-06-29 17:35:09.000000 seismic-rna-0.1.1/src/seismicrna/core/rel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.1.1/src/seismicrna/core/rel_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29463 2023-06-29 19:57:29.000000 seismic-rna-0.1.1/src/seismicrna/core/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/rna.py
+-rw-r--r--   0 mfa        (503) staff       (20)    26188 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/sect.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.1.1/src/seismicrna/core/sect_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.1.1/src/seismicrna/core/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.1.1/src/seismicrna/core/seq_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.1.1/src/seismicrna/core/shell.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.1.1/src/seismicrna/core/sim.py
+-rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.1.1/src/seismicrna/core/sim_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/types.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.1.1/src/seismicrna/core/xam.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.528536 seismic-rna-0.1.1/src/seismicrna/demult/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/demult/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    42588 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/demult/demultiplex.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2073 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/demult/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.537203 seismic-rna-0.1.1/src/seismicrna/draw/
+-rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.1.1/src/seismicrna/draw/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/load_dataset.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/manipulator.py
+-rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.1.1/src/seismicrna/draw/plotter.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/study.py
+-rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/util.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.543180 seismic-rna-0.1.1/src/seismicrna/graph/
+-rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8667 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3249 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/color.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2700 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/default.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7441 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/hist.py
+-rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8608 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9744 2023-06-30 04:08:02.000000 seismic-rna-0.1.1/src/seismicrna/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.547460 seismic-rna-0.1.1/src/seismicrna/mask/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/mask/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4083 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/mask/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4321 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/mask/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/mask/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    13982 2023-06-29 19:40:06.000000 seismic-rna-0.1.1/src/seismicrna/mask/write.py
+-rw-r--r--   0 mfa        (503) staff       (20)       47 2023-07-06 00:52:00.000000 seismic-rna-0.1.1/src/seismicrna/meta.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.555786 seismic-rna-0.1.1/src/seismicrna/relate/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/export.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3175 2023-06-30 04:06:44.000000 seismic-rna-0.1.1/src/seismicrna/relate/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/relate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.1.1/src/seismicrna/relate/sam.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/seqpos.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15021 2023-06-30 04:03:22.000000 seismic-rna-0.1.1/src/seismicrna/relate/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.558176 seismic-rna-0.1.1/src/seismicrna/struct/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/struct/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3905 2023-06-29 20:47:08.000000 seismic-rna-0.1.1/src/seismicrna/struct/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1862 2023-06-29 20:23:36.000000 seismic-rna-0.1.1/src/seismicrna/struct/rnastructure.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.565120 seismic-rna-0.1.1/src/seismicrna/table/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7405 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     5929 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1520 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14642 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/tabulate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4841 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.568019 seismic-rna-0.1.1/src/seismicrna/test/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/test/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.1.1/src/seismicrna/test/main.py
```

### Comparing `seismic-rna-0.1.0/LICENSE` & `seismic-rna-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/PKG-INFO` & `seismic-rna-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.1.0
+Version: 0.1.1
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 
 
 ### Contributors
 
 SEISMIC RNA has been developed in [Silvi Rouskin's lab](https://rouskinlab.com)
 at Harvard Medical School by the following individuals:
 
-- [Matty Allan](https://github.com/matthewfallan)
+- [Matthew "Matty" Allan](https://github.com/matthewfallan)
 - [Yves Martin](https://github.com/yvesmartindestaillades)
 - [Scott Grote](https://github.com/heWhosShouldersBlockTheSun)
 - [Albéric de Lajarte](https://github.com/AlbericDeLajarte)
 
 
 ## Installation
 
@@ -56,8 +56,7 @@
 
 
 ## Issues
 
 The [issue page](https://github.com/rouskinlab/seismic-rna/issues) of the GitHub
 repository is the official location for reporting bugs and other issues. Before
 opening a new issue, please check if a similar issue already exists.
-
```

### Comparing `seismic-rna-0.1.0/README.md` & `seismic-rna-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 ### Contributors
 
 SEISMIC RNA has been developed in [Silvi Rouskin's lab](https://rouskinlab.com)
 at Harvard Medical School by the following individuals:
 
-- [Matty Allan](https://github.com/matthewfallan)
+- [Matthew "Matty" Allan](https://github.com/matthewfallan)
 - [Yves Martin](https://github.com/yvesmartindestaillades)
 - [Scott Grote](https://github.com/heWhosShouldersBlockTheSun)
 - [Albéric de Lajarte](https://github.com/AlbericDeLajarte)
 
 
 ## Installation
 
@@ -42,8 +42,7 @@
 
 
 ## Issues
 
 The [issue page](https://github.com/rouskinlab/seismic-rna/issues) of the GitHub
 repository is the official location for reporting bugs and other issues. Before
 opening a new issue, please check if a similar issue already exists.
-
```

### Comparing `seismic-rna-0.1.0/pyproject.toml` & `seismic-rna-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seismic-rna"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name="Matty Allan"},
     {name="Yves Martin"},
     {name="Scott Grote"},
     {name="Alberic de Lajarte"},
 ]
 description = "RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering"
@@ -35,8 +35,7 @@
 
 [project.scripts]
 srna = "seismicrna.main:main_cli"
 
 [project.urls]
 "Homepage" = "https://github.com/rouskinlab/seismic-rna"
 "Bug Tracker" = "https://github.com/rouskinlab/seismic-rna/issues"
-
```

### Comparing `seismic-rna-0.1.0/src/seismic_rna.egg-info/PKG-INFO` & `seismic-rna-0.1.1/src/seismic_rna.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.1.0
+Version: 0.1.1
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 
 
 ### Contributors
 
 SEISMIC RNA has been developed in [Silvi Rouskin's lab](https://rouskinlab.com)
 at Harvard Medical School by the following individuals:
 
-- [Matty Allan](https://github.com/matthewfallan)
+- [Matthew "Matty" Allan](https://github.com/matthewfallan)
 - [Yves Martin](https://github.com/yvesmartindestaillades)
 - [Scott Grote](https://github.com/heWhosShouldersBlockTheSun)
 - [Albéric de Lajarte](https://github.com/AlbericDeLajarte)
 
 
 ## Installation
 
@@ -56,8 +56,7 @@
 
 
 ## Issues
 
 The [issue page](https://github.com/rouskinlab/seismic-rna/issues) of the GitHub
 repository is the official location for reporting bugs and other issues. Before
 opening a new issue, please check if a similar issue already exists.
-
```

### Comparing `seismic-rna-0.1.0/src/seismic_rna.egg-info/SOURCES.txt` & `seismic-rna-0.1.1/src/seismic_rna.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,24 +34,28 @@
 src/seismicrna/core/docstring.py
 src/seismicrna/core/dump.py
 src/seismicrna/core/files.py
 src/seismicrna/core/files_sanity.py
 src/seismicrna/core/load.py
 src/seismicrna/core/logs.py
 src/seismicrna/core/mu.py
+src/seismicrna/core/mu_test.py
 src/seismicrna/core/parallel.py
 src/seismicrna/core/path.py
 src/seismicrna/core/rel.py
+src/seismicrna/core/rel_test.py
 src/seismicrna/core/report.py
 src/seismicrna/core/rna.py
 src/seismicrna/core/sect.py
+src/seismicrna/core/sect_test.py
 src/seismicrna/core/seq.py
+src/seismicrna/core/seq_test.py
 src/seismicrna/core/shell.py
 src/seismicrna/core/sim.py
-src/seismicrna/core/test.py
+src/seismicrna/core/sim_test.py
 src/seismicrna/core/types.py
 src/seismicrna/core/xam.py
 src/seismicrna/demult/__init__.py
 src/seismicrna/demult/demultiplex.py
 src/seismicrna/demult/main.py
 src/seismicrna/draw/__init__.py
 src/seismicrna/draw/load_dataset.py
```

### Comparing `seismic-rna-0.1.0/src/seismicrna/align/fq2bam.py` & `seismic-rna-0.1.1/src/seismicrna/align/fq2bam.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,14 +460,17 @@
 def get_bam_files(fq_units: list[FastqUnit],
                   fasta: Path, *,
                   out_dir: Path,
                   rerun: bool,
                   **kwargs) -> list[Path]:
     """ Run the alignment pipeline and return a tuple of all BAM files
     from the pipeline. """
+    if not fq_units:
+        logger.warning("No FASTQ files or pairs of FASTQ files were given")
+        return list()
     if rerun:
         # Rerun all alignments.
         fqs_to_align = fq_units
         bams = set()
     else:
         # Get the names of all reference sequences.
         refs = {ref for ref, _ in parse_fasta(fasta)}
```

### Comparing `seismic-rna-0.1.0/src/seismicrna/align/fqutil.py` & `seismic-rna-0.1.1/src/seismicrna/align/fqutil.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/align/main.py` & `seismic-rna-0.1.1/src/seismicrna/align/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/align/strandedness.py` & `seismic-rna-0.1.1/src/seismicrna/align/strandedness.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/cluster/compare.py` & `seismic-rna-0.1.1/src/seismicrna/cluster/compare.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/cluster/em.py` & `seismic-rna-0.1.1/src/seismicrna/cluster/em.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/cluster/krun.py` & `seismic-rna-0.1.1/src/seismicrna/cluster/krun.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/cluster/load.py` & `seismic-rna-0.1.1/src/seismicrna/cluster/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/cluster/main.py` & `seismic-rna-0.1.1/src/seismicrna/cluster/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/cluster/report.py` & `seismic-rna-0.1.1/src/seismicrna/cluster/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/cluster/write.py` & `seismic-rna-0.1.1/src/seismicrna/cluster/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/bitcall.py` & `seismic-rna-0.1.1/src/seismicrna/core/bitcall.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/bitvect.py` & `seismic-rna-0.1.1/src/seismicrna/core/bitvect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/cli.py` & `seismic-rna-0.1.1/src/seismicrna/core/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,22 +245,20 @@
                    type=int,
                    default=20,
                    help="Discard reads shorter than this length after trimming")
 
 # Alignment options with Bowtie2
 opt_bt2_local = Option(("--bt2-local/--bt2-end-to-end",),
                        type=bool,
-                       default=False,
+                       default=True,
                        help="Whether to perform local or end-to-end alignment. "
-                            "Note that during local alignment, mutations at or "
-                            "very close to the ends of reads will be clipped "
-                            "off because clipping avoids the penalty for the "
-                            "mutation, thus giving a higher alignment score. "
-                            "As a result, mutations will be under-counted near "
-                            "the ends of reads; if the reads ")
+                            "Use local with fragmented samples, on which "
+                            "end-to-end yields false positives at read ends. "
+                            "Use end-to-end with amplicon-based samples, on "
+                            "which local yields false negatives at read ends.")
 opt_bt2_discordant = Option(("--bt2-discordant/--bt2-no-discordant",),
                             type=bool,
                             default=False,
                             help="Whether to output discordant alignments")
 opt_bt2_mixed = Option(("--bt2-mixed/--bt2-no-mixed",),
                        type=bool,
                        default=False,
```

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/depend.py` & `seismic-rna-0.1.1/src/seismicrna/core/depend.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/docdef.py` & `seismic-rna-0.1.1/src/seismicrna/core/docdef.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/docstring.py` & `seismic-rna-0.1.1/src/seismicrna/core/docstring.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/dump.py` & `seismic-rna-0.1.1/src/seismicrna/core/dump.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/files.py` & `seismic-rna-0.1.1/src/seismicrna/core/files.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/files_sanity.py` & `seismic-rna-0.1.1/src/seismicrna/core/files_sanity.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/load.py` & `seismic-rna-0.1.1/src/seismicrna/core/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/logs.py` & `seismic-rna-0.1.1/src/seismicrna/core/logs.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/mu.py` & `seismic-rna-0.1.1/src/seismicrna/core/mu.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/parallel.py` & `seismic-rna-0.1.1/src/seismicrna/core/parallel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/path.py` & `seismic-rna-0.1.1/src/seismicrna/core/path.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/rel.py` & `seismic-rna-0.1.1/src/seismicrna/core/rel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/report.py` & `seismic-rna-0.1.1/src/seismicrna/core/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/rna.py` & `seismic-rna-0.1.1/src/seismicrna/core/rna.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/sect.py` & `seismic-rna-0.1.1/src/seismicrna/core/sect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/seq.py` & `seismic-rna-0.1.1/src/seismicrna/core/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/shell.py` & `seismic-rna-0.1.1/src/seismicrna/core/shell.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/sim.py` & `seismic-rna-0.1.1/src/seismicrna/core/sim.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/types.py` & `seismic-rna-0.1.1/src/seismicrna/core/types.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/core/xam.py` & `seismic-rna-0.1.1/src/seismicrna/core/xam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/demult/demultiplex.py` & `seismic-rna-0.1.1/src/seismicrna/demult/demultiplex.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/demult/main.py` & `seismic-rna-0.1.1/src/seismicrna/demult/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/draw/main.py` & `seismic-rna-0.1.1/src/seismicrna/draw/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/draw/manipulator.py` & `seismic-rna-0.1.1/src/seismicrna/draw/manipulator.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/draw/plotter.py` & `seismic-rna-0.1.1/src/seismicrna/draw/plotter.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/draw/study.py` & `seismic-rna-0.1.1/src/seismicrna/draw/study.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/draw/util.py` & `seismic-rna-0.1.1/src/seismicrna/draw/util.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/graph/base.py` & `seismic-rna-0.1.1/src/seismicrna/graph/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/graph/color.py` & `seismic-rna-0.1.1/src/seismicrna/graph/color.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/graph/default.py` & `seismic-rna-0.1.1/src/seismicrna/graph/default.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/graph/hist.py` & `seismic-rna-0.1.1/src/seismicrna/graph/hist.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/graph/seq.py` & `seismic-rna-0.1.1/src/seismicrna/graph/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/main.py` & `seismic-rna-0.1.1/src/seismicrna/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/mask/load.py` & `seismic-rna-0.1.1/src/seismicrna/mask/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/mask/main.py` & `seismic-rna-0.1.1/src/seismicrna/mask/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/mask/report.py` & `seismic-rna-0.1.1/src/seismicrna/mask/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/mask/write.py` & `seismic-rna-0.1.1/src/seismicrna/mask/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/export.py` & `seismic-rna-0.1.1/src/seismicrna/relate/export.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/load.py` & `seismic-rna-0.1.1/src/seismicrna/relate/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/main.py` & `seismic-rna-0.1.1/src/seismicrna/relate/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/relate.py` & `seismic-rna-0.1.1/src/seismicrna/relate/relate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/report.py` & `seismic-rna-0.1.1/src/seismicrna/relate/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/sam.py` & `seismic-rna-0.1.1/src/seismicrna/relate/sam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/seqpos.py` & `seismic-rna-0.1.1/src/seismicrna/relate/seqpos.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/test.py` & `seismic-rna-0.1.1/src/seismicrna/relate/test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/relate/write.py` & `seismic-rna-0.1.1/src/seismicrna/relate/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/struct/main.py` & `seismic-rna-0.1.1/src/seismicrna/struct/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/struct/rnastructure.py` & `seismic-rna-0.1.1/src/seismicrna/struct/rnastructure.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/table/base.py` & `seismic-rna-0.1.1/src/seismicrna/table/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/table/load.py` & `seismic-rna-0.1.1/src/seismicrna/table/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/table/main.py` & `seismic-rna-0.1.1/src/seismicrna/table/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/table/tabulate.py` & `seismic-rna-0.1.1/src/seismicrna/table/tabulate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/table/write.py` & `seismic-rna-0.1.1/src/seismicrna/table/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.0/src/seismicrna/test/main.py` & `seismic-rna-0.1.1/src/seismicrna/test/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,11 +24,12 @@
     """
     # Discover all unit test modules.
     main_dir = dirname(dirname(__file__))
     # The line top_level_dir=dirname(main_dir) is needed to make Python
     # treat seismicrna as a package, so that the relative imports work.
     # Omitting this line leads to an ImportError during every test.
     suite = ut.TestLoader().discover(main_dir,
+                                     pattern="*test.py",
                                      top_level_dir=dirname(main_dir))
     # Run all unit tests.
     runner = ut.TextTestRunner(verbosity=verbose)
     runner.run(suite)
```

