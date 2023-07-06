# Comparing `tmp/pmx_biobb-4.1.2.tar.gz` & `tmp/pmx_biobb-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmx_biobb-4.1.2.tar", last modified: Mon Jul  3 12:12:58 2023, max compression
+gzip compressed data, was "dist/pmx_biobb-4.1.3.tar", last modified: Thu Jul  6 09:13:48 2023, max compression
```

## Comparing `pmx_biobb-4.1.2.tar` & `pmx_biobb-4.1.3.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/
--rw-rw-r--   0 pau        (501) staff       (20)     7651 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/LICENSE
--rw-rw-r--   0 pau        (501) staff       (20)       95 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/MANIFEST.in
--rw-r--r--   0 pau        (501) staff       (20)     2616 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/PKG-INFO
--rw-rw-r--   0 pau        (501) staff       (20)     2087 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/README.rst
--rw-rw-r--   0 pau        (501) staff       (20)      194 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/setup.cfg
--rw-rw-r--   0 pau        (501) staff       (20)     2125 2023-07-03 12:09:10.000000 pmx_biobb-4.1.2/setup.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/
--rwxr-xr-x   0 pau        (501) staff       (20)    31247 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/AbsRestraints.py
--rw-rw-r--   0 pau        (501) staff       (20)     2261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)      439 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/_version.py
--rw-rw-r--   0 pau        (501) staff       (20)    81006 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/alchemy.py
--rw-rw-r--   0 pau        (501) staff       (20)    14501 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/analysis.py
--rw-rw-r--   0 pau        (501) staff       (20)    15992 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/atom.py
--rw-rw-r--   0 pau        (501) staff       (20)    14221 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/atomselection.py
--rw-rw-r--   0 pau        (501) staff       (20)    13429 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/builder.py
--rw-rw-r--   0 pau        (501) staff       (20)    34519 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/chain.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/
--rw-rw-r--   0 pau        (501) staff       (20)   233765 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/aminoacids.pkl
--rw-rw-r--   0 pau        (501) staff       (20) 17363760 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/bbdep.pkl
--rw-rw-r--   0 pau        (501) staff       (20)     1786 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/blosum62_new.mat
--rw-rw-r--   0 pau        (501) staff       (20)   144604 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/bp.pkl
--rw-rw-r--   0 pau        (501) staff       (20)   149219 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/bp_amber.pkl
--rw-rw-r--   0 pau        (501) staff       (20)   148935 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/bp_charmm.pkl
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/
--rw-rw-r--   0 pau        (501) staff       (20)      661 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am
--rw-rw-r--   0 pau        (501) staff       (20)    12694 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in
--rw-rw-r--   0 pau        (501) staff       (20)     9997 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn
--rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.c.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     8884 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb
--rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.n.tdb
--rw-rw-r--   0 pau        (501) staff       (20)      849 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    80500 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp
--rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd
--rw-rw-r--   0 pau        (501) staff       (20)     5339 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp
--rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.arn
--rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)    66560 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)     8192 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)       79 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/forcefield.doc
--rw-rw-r--   0 pau        (501) staff       (20)      947 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1948 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp
--rw-rw-r--   0 pau        (501) staff       (20)     3882 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ions.itp
--rw-rw-r--   0 pau        (501) staff       (20)  3071584 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp
--rw-rw-r--   0 pau        (501) staff       (20)  1260735 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp
--rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.arn
--rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/spc.itp
--rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/spce.itp
--rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/urea.itp
--rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/
--rw-rw-r--   0 pau        (501) staff       (20)    21524 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
--rw-rw-r--   0 pau        (501) staff       (20)     2589 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
--rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     9412 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
--rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
--rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
--rw-rw-r--   0 pau        (501) staff       (20)   101863 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
--rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
--rw-rw-r--   0 pau        (501) staff       (20)     5335 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
--rw-rw-r--   0 pau        (501) staff       (20)    36227 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-rw-r--   0 pau        (501) staff       (20)  1202088 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
--rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)      130 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
--rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)    10830 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
--rw-rw-r--   0 pau        (501) staff       (20)    45478 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)     7972 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)      722 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc
--rw-rw-r--   0 pau        (501) staff       (20)      974 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1949 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
--rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
--rw-rw-r--   0 pau        (501) staff       (20)  2805564 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
--rw-rw-r--   0 pau        (501) staff       (20)  1181333 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
--rw-rw-r--   0 pau        (501) staff       (20)   300774 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
--rw-rw-r--   0 pau        (501) staff       (20)   129919 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)    16346 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
--rw-rw-r--   0 pau        (501) staff       (20)    18595 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
--rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
--rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
--rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
--rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
--rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/
--rw-rw-r--   0 pau        (501) staff       (20)     2589 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn
--rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.c.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     9412 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb
--rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.n.tdb
--rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b
--rw-rw-r--   0 pau        (501) staff       (20)   101863 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp
--rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd
--rw-rw-r--   0 pau        (501) staff       (20)     4978 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp
--rw-rw-r--   0 pau        (501) staff       (20)    36227 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-rw-r--   0 pau        (501) staff       (20)  1202088 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres
--rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.arn
--rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)    10830 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp
--rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)     7476 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)      709 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc
--rw-rw-r--   0 pau        (501) staff       (20)      974 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1949 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp
--rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp
--rw-rw-r--   0 pau        (501) staff       (20)  2805564 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp
--rw-rw-r--   0 pau        (501) staff       (20)  1181333 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp
--rw-rw-r--   0 pau        (501) staff       (20)   300774 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp
--rw-rw-r--   0 pau        (501) staff       (20)   129937 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)    16346 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp
--rw-rw-r--   0 pau        (501) staff       (20)    18595 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp
--rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.arn
--rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp
--rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp
--rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp
--rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/
--rw-rw-r--   0 pau        (501) staff       (20)     9997 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn
--rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     9416 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-rw-r--   0 pau        (501) staff       (20)   104467 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp
--rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-rw-r--   0 pau        (501) staff       (20)     4652 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp
--rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.arn
--rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)    36127 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)     6772 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)      704 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc
--rw-rw-r--   0 pau        (501) staff       (20)      951 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1948 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp
--rw-rw-r--   0 pau        (501) staff       (20)  3290968 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp
--rw-rw-r--   0 pau        (501) staff       (20)  1389335 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp
--rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.arn
--rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp
--rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp
--rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp
--rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/watermodels.dat
--rw-rw-r--   0 pau        (501) staff       (20)     3873 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/atommass.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/
--rw-rw-r--   0 pau        (501) staff       (20)       84 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.arn
--rw-rw-r--   0 pau        (501) staff       (20)     2060 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     8026 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb
--rw-rw-r--   0 pau        (501) staff       (20)     1519 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb
--rw-rw-r--   0 pau        (501) staff       (20)      181 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.r2b
--rw-rw-r--   0 pau        (501) staff       (20)    44420 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp
--rw-rw-r--   0 pau        (501) staff       (20)     6253 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd
--rw-rw-r--   0 pau        (501) staff       (20)    13027 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp
--rw-rw-r--   0 pau        (501) staff       (20)    37937 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp
--rw-rw-r--   0 pau        (501) staff       (20)      244 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.arn
--rw-rw-r--   0 pau        (501) staff       (20)      261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.c.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     1660 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      265 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.n.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     9612 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)    88617 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)    74128 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)    47717 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)   144554 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)     2792 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc
--rw-rw-r--   0 pau        (501) staff       (20)     1208 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp
--rw-rw-r--   0 pau        (501) staff       (20)     2882 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1767 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp
--rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.hdb
--rw-rw-r--   0 pau        (501) staff       (20)    48593 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp
--rw-rw-r--   0 pau        (501) staff       (20)       70 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.arn
--rw-rw-r--   0 pau        (501) staff       (20)  2828420 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp
--rw-rw-r--   0 pau        (501) staff       (20)  1165390 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp
--rw-rw-r--   0 pau        (501) staff       (20)      164 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.arn
--rw-rw-r--   0 pau        (501) staff       (20)      261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.c.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     1884 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb
--rw-rw-r--   0 pau        (501) staff       (20)      265 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.n.tdb
--rw-rw-r--   0 pau        (501) staff       (20)      126 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.r2b
--rw-rw-r--   0 pau        (501) staff       (20)     9712 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)      910 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp
--rw-rw-r--   0 pau        (501) staff       (20)      916 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1369 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1419 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1576 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp
--rw-rw-r--   0 pau        (501) staff       (20)     2237 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp
--rw-rw-r--   0 pau        (501) staff       (20)      915 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp
--rw-rw-r--   0 pau        (501) staff       (20)      306 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/
--rw-rw-r--   0 pau        (501) staff       (20)    24002 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp
--rw-rw-r--   0 pau        (501) staff       (20)    82367 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp
--rw-rw-r--   0 pau        (501) staff       (20)  1123865 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)  1614095 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp
--rw-rw-r--   0 pau        (501) staff       (20)     7941 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc
--rw-rw-r--   0 pau        (501) staff       (20)      435 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.itp
--rw-rw-r--   0 pau        (501) staff       (20)     2734 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp
--rw-rw-r--   0 pau        (501) staff       (20)     2079 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp
--rw-rw-r--   0 pau        (501) staff       (20)       92 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.arn
--rw-rw-r--   0 pau        (501) staff       (20)     1134 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb
--rw-rw-r--   0 pau        (501) staff       (20)     8979 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb
--rw-rw-r--   0 pau        (501) staff       (20)     1397 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb
--rw-rw-r--   0 pau        (501) staff       (20)      198 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.r2b
--rw-rw-r--   0 pau        (501) staff       (20)  1133668 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp
--rw-rw-r--   0 pau        (501) staff       (20)     5220 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd
--rw-rw-r--   0 pau        (501) staff       (20)       92 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.arn
--rw-rw-r--   0 pau        (501) staff       (20)  3015999 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp
--rw-rw-r--   0 pau        (501) staff       (20)  1267062 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp
--rw-rw-r--   0 pau        (501) staff       (20)   283035 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp
--rw-rw-r--   0 pau        (501) staff       (20)   123173 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp
--rw-rw-r--   0 pau        (501) staff       (20)     1339 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp
--rw-rw-r--   0 pau        (501) staff       (20)      619 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp
--rw-rw-r--   0 pau        (501) staff       (20)      625 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1026 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp
--rw-rw-r--   0 pau        (501) staff       (20)     1242 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp
--rw-rw-r--   0 pau        (501) staff       (20)      221 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/watermodels.dat
--rw-rw-r--   0 pau        (501) staff       (20)     3940 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/elements.dat
--rw-rw-r--   0 pau        (501) staff       (20)    10624 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/residuetypes.dat
--rw-rw-r--   0 pau        (501) staff       (20)    29266 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/spc216.gro
--rw-rw-r--   0 pau        (501) staff       (20)      343 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/specbond.dat
--rw-rw-r--   0 pau        (501) staff       (20)      848 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/vdwradii.dat
--rw-rw-r--   0 pau        (501) staff       (20)      447 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/mutff/xlateat.dat
--rw-rw-r--   0 pau        (501) staff       (20)    70529 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/data/rna.pkl
--rw-rw-r--   0 pau        (501) staff       (20)    37772 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/estimators.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx/extensions/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/
--rw-rw-r--   0 pau        (501) staff       (20)    13896 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/Energy.c
--rw-rw-r--   0 pau        (501) staff       (20)    15145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/Geometry.c
--rw-rw-r--   0 pau        (501) staff       (20)    20514 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/Geometry.h
--rw-rw-r--   0 pau        (501) staff       (20)     2086 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/cpp_test.cpp
--rw-rw-r--   0 pau        (501) staff       (20)     3939 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/init.c
--rw-rw-r--   0 pau        (501) staff       (20)     4662 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/pmx.h
--rw-rw-r--   0 pau        (501) staff       (20)    17556 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/pmx/wrap_Geometry.c
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/
--rw-rw-r--   0 pau        (501) staff       (20)     8847 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/trr2xtc.c
--rw-rw-r--   0 pau        (501) staff       (20)    64408 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile.c
--rw-rw-r--   0 pau        (501) staff       (20)    23730 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile.h
--rw-rw-r--   0 pau        (501) staff       (20)    13474 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_c_test.c
--rw-rw-r--   0 pau        (501) staff       (20)    14744 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_trr.c
--rw-rw-r--   0 pau        (501) staff       (20)     2364 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_trr.h
--rw-rw-r--   0 pau        (501) staff       (20)     3629 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_xtc.c
--rw-rw-r--   0 pau        (501) staff       (20)     2255 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_xtc.h
--rw-rw-r--   0 pau        (501) staff       (20)    29075 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/ffparser.py
--rw-rw-r--   0 pau        (501) staff       (20)    97591 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/forcefield.py
--rw-rw-r--   0 pau        (501) staff       (20)     7685 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/geometry.py
--rw-rw-r--   0 pau        (501) staff       (20)     8707 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/gmx.py
--rw-rw-r--   0 pau        (501) staff       (20)     6179 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/jobscript.py
--rw-rw-r--   0 pau        (501) staff       (20)   123096 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/library.py
--rw-rw-r--   0 pau        (501) staff       (20)   117960 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/ligand_alchemy.py
--rw-rw-r--   0 pau        (501) staff       (20)    46805 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/model.py
--rw-rw-r--   0 pau        (501) staff       (20)    28167 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/molecule.py
--rw-rw-r--   0 pau        (501) staff       (20)     7345 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/mutdb.py
--rw-rw-r--   0 pau        (501) staff       (20)     8874 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/ndx.py
--rw-rw-r--   0 pau        (501) staff       (20)    16599 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/options.py
--rw-rw-r--   0 pau        (501) staff       (20)     5036 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/parser.py
--rw-rw-r--   0 pau        (501) staff       (20)    21628 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/rosetta.py
--rw-rw-r--   0 pau        (501) staff       (20)    15211 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/rosetta_analyze.py
--rw-rw-r--   0 pau        (501) staff       (20)    11783 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/rotamer.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/scripts/
--rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)    33900 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/analyze_dhdl.py
--rwxr-xr-x   0 pau        (501) staff       (20)    19864 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/atomMapping.py
--rwxr-xr-x   0 pau        (501) staff       (20)    11939 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/build_cyclic_top.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2988 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/cli.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2955 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/gen_abs_restraints.py
--rwxr-xr-x   0 pau        (501) staff       (20)    73999 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/generate_hybrid_residue.py
--rwxr-xr-x   0 pau        (501) staff       (20)     7099 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/generate_hybrid_topology.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx/scripts/icolos_entrypoints/
--rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/icolos_entrypoints/__init__.py
--rw-rw-r--   0 pau        (501) staff       (20)     7137 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/icolos_entrypoints/assemble_systems.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12867 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/ligandHybrid.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2705 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/make_double_box.py
--rw-rw-r--   0 pau        (501) staff       (20)    19943 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/md_setup.py
--rwxr-xr-x   0 pau        (501) staff       (20)    23072 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/mutate.py
--rwxr-xr-x   0 pau        (501) staff       (20)    38647 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/parameterize_ligands.py
--rw-rw-r--   0 pau        (501) staff       (20)     7795 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/prepare_crooks_runs.py
--rwxr-xr-x   0 pau        (501) staff       (20)     1475 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/set_gmxlib.py
--rw-rw-r--   0 pau        (501) staff       (20)    17636 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/scripts/setup_abfe.py
--rw-rw-r--   0 pau        (501) staff       (20)    13784 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/summary.py
--rw-rw-r--   0 pau        (501) staff       (20)    15258 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/utils.py
--rw-rw-r--   0 pau        (501) staff       (20)    11331 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/xdrfile.py
--rw-rw-r--   0 pau        (501) staff       (20)     1784 2023-05-19 08:30:20.000000 pmx_biobb-4.1.2/src/pmx/xtc.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     2722 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)    14322 2023-07-03 11:43:22.000000 pmx_biobb-4.1.2/src/pmx.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)       53 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/not-zip-safe
--rw-r--r--   0 pau        (501) staff       (20)       29 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)        4 2023-07-03 11:43:21.000000 pmx_biobb-4.1.2/src/pmx.egg-info/top_level.txt
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-03 12:12:58.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     2616 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)    14582 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)       53 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:49:27.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/not-zip-safe
--rw-r--r--   0 pau        (501) staff       (20)       29 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)        4 2023-07-03 12:12:57.000000 pmx_biobb-4.1.2/src/pmx_biobb.egg-info/top_level.txt
--rw-rw-r--   0 pau        (501) staff       (20)    66226 2023-07-03 12:08:52.000000 pmx_biobb-4.1.2/versioneer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/
+-rw-rw-r--   0 pau        (501) staff       (20)     7651 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/LICENSE
+-rw-rw-r--   0 pau        (501) staff       (20)       95 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/MANIFEST.in
+-rw-r--r--   0 pau        (501) staff       (20)     2616 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/PKG-INFO
+-rw-rw-r--   0 pau        (501) staff       (20)     2087 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/README.rst
+-rw-rw-r--   0 pau        (501) staff       (20)      194 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/setup.cfg
+-rw-rw-r--   0 pau        (501) staff       (20)     2125 2023-07-03 12:09:10.000000 pmx_biobb-4.1.3/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/
+-rwxr-xr-x   0 pau        (501) staff       (20)    31247 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/AbsRestraints.py
+-rw-rw-r--   0 pau        (501) staff       (20)     2261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)      439 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/_version.py
+-rw-rw-r--   0 pau        (501) staff       (20)    81006 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/alchemy.py
+-rw-rw-r--   0 pau        (501) staff       (20)    14501 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/analysis.py
+-rw-rw-r--   0 pau        (501) staff       (20)    15992 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/atom.py
+-rw-rw-r--   0 pau        (501) staff       (20)    14221 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/atomselection.py
+-rw-rw-r--   0 pau        (501) staff       (20)    13429 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/builder.py
+-rw-rw-r--   0 pau        (501) staff       (20)    34519 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/chain.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/data/
+-rw-rw-r--   0 pau        (501) staff       (20)   233765 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/aminoacids.pkl
+-rw-rw-r--   0 pau        (501) staff       (20) 17363760 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/bbdep.pkl
+-rw-rw-r--   0 pau        (501) staff       (20)     1786 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/blosum62_new.mat
+-rw-rw-r--   0 pau        (501) staff       (20)   144604 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/bp.pkl
+-rw-rw-r--   0 pau        (501) staff       (20)   149219 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/bp_amber.pkl
+-rw-rw-r--   0 pau        (501) staff       (20)   148935 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/bp_charmm.pkl
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)      661 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am
+-rw-rw-r--   0 pau        (501) staff       (20)    12694 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in
+-rw-rw-r--   0 pau        (501) staff       (20)     9997 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     8884 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      849 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    80500 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)     5339 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/dna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    66560 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     8192 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)       79 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      947 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1948 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     3882 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  3071584 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1260735 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/urea.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)    21524 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     2589 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     9412 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)   101863 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)     5335 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)    36227 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  1202088 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
+-rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      130 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    10830 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    45478 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     7972 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      722 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      974 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1949 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  2805564 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1181333 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)   300774 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)   129919 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    16346 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    18595 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)     2589 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     9412 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)   101863 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)     4978 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)    36227 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  1202088 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres
+-rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    10830 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    36132 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     7476 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      709 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      974 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1949 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  2805564 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1181333 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)   300774 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)   129937 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    16346 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    18595 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)     9997 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     9416 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)       10 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      903 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)   104467 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5207 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)     4652 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     3104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    29892 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    36127 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     6772 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      704 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      951 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1948 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     3886 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  3290968 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1389335 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      116 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     4104 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    30277 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      746 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      802 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1317 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1870 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1250 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      214 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/watermodels.dat
+-rw-rw-r--   0 pau        (501) staff       (20)     3873 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/atommass.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)       84 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     2060 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     8026 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)     1519 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      181 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)    44420 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     6253 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)    13027 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)    37937 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      244 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/dna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)      261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/dna.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     1660 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      265 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/dna.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     9612 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)    88617 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    74128 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)    47717 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)   144554 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2792 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)     1208 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2882 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1767 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/lipids.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)    48593 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)       70 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/mutres.arn
+-rw-rw-r--   0 pau        (501) staff       (20)  2828420 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1165390 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      164 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/rna.arn
+-rw-rw-r--   0 pau        (501) staff       (20)      261 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/rna.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     1884 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)      265 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/rna.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      126 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/rna.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)     9712 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)      910 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      916 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1369 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1419 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1576 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2237 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      915 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      306 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/
+-rw-rw-r--   0 pau        (501) staff       (20)    24002 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp
+-rw-rw-r--   0 pau        (501) staff       (20)    82367 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  1123865 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)  1614095 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     7941 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc
+-rw-rw-r--   0 pau        (501) staff       (20)      435 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2734 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     2079 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp
+-rw-rw-r--   0 pau        (501) staff       (20)       92 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.arn
+-rw-rw-r--   0 pau        (501) staff       (20)     1134 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)     8979 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb
+-rw-rw-r--   0 pau        (501) staff       (20)     1397 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb
+-rw-rw-r--   0 pau        (501) staff       (20)      198 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.r2b
+-rw-rw-r--   0 pau        (501) staff       (20)  1133668 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     5220 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd
+-rw-rw-r--   0 pau        (501) staff       (20)       92 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres.arn
+-rw-rw-r--   0 pau        (501) staff       (20)  3015999 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)  1267062 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)   283035 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp
+-rw-rw-r--   0 pau        (501) staff       (20)   123173 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp
+-rw-rw-r--   0 pau        (501) staff       (20)     1339 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      619 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      625 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1026 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)     1242 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp
+-rw-rw-r--   0 pau        (501) staff       (20)      221 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/watermodels.dat
+-rw-rw-r--   0 pau        (501) staff       (20)     3940 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/elements.dat
+-rw-rw-r--   0 pau        (501) staff       (20)    10624 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/residuetypes.dat
+-rw-rw-r--   0 pau        (501) staff       (20)    29266 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/spc216.gro
+-rw-rw-r--   0 pau        (501) staff       (20)      343 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/specbond.dat
+-rw-rw-r--   0 pau        (501) staff       (20)      848 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/vdwradii.dat
+-rw-rw-r--   0 pau        (501) staff       (20)      447 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/mutff/xlateat.dat
+-rw-rw-r--   0 pau        (501) staff       (20)    70529 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/data/rna.pkl
+-rw-rw-r--   0 pau        (501) staff       (20)    37772 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/estimators.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/extensions/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/extensions/pmx/
+-rw-rw-r--   0 pau        (501) staff       (20)    13896 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/pmx/Energy.c
+-rw-rw-r--   0 pau        (501) staff       (20)    15145 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/pmx/Geometry.c
+-rw-rw-r--   0 pau        (501) staff       (20)    20514 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/pmx/Geometry.h
+-rw-rw-r--   0 pau        (501) staff       (20)     2086 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/pmx/cpp_test.cpp
+-rw-rw-r--   0 pau        (501) staff       (20)     3939 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/pmx/init.c
+-rw-rw-r--   0 pau        (501) staff       (20)     4662 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/pmx/pmx.h
+-rw-rw-r--   0 pau        (501) staff       (20)    17556 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/pmx/wrap_Geometry.c
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/
+-rw-rw-r--   0 pau        (501) staff       (20)     8847 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/trr2xtc.c
+-rw-rw-r--   0 pau        (501) staff       (20)    64408 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile.c
+-rw-rw-r--   0 pau        (501) staff       (20)    23730 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile.h
+-rw-rw-r--   0 pau        (501) staff       (20)    13474 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_c_test.c
+-rw-rw-r--   0 pau        (501) staff       (20)    14744 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_trr.c
+-rw-rw-r--   0 pau        (501) staff       (20)     2364 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_trr.h
+-rw-rw-r--   0 pau        (501) staff       (20)     3629 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_xtc.c
+-rw-rw-r--   0 pau        (501) staff       (20)     2255 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_xtc.h
+-rw-rw-r--   0 pau        (501) staff       (20)    29075 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/ffparser.py
+-rw-rw-r--   0 pau        (501) staff       (20)    97591 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/forcefield.py
+-rw-rw-r--   0 pau        (501) staff       (20)     7685 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/geometry.py
+-rw-rw-r--   0 pau        (501) staff       (20)     8707 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/gmx.py
+-rw-rw-r--   0 pau        (501) staff       (20)     6179 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/jobscript.py
+-rw-rw-r--   0 pau        (501) staff       (20)   123096 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/library.py
+-rw-rw-r--   0 pau        (501) staff       (20)   117960 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/ligand_alchemy.py
+-rw-rw-r--   0 pau        (501) staff       (20)    46805 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/model.py
+-rw-rw-r--   0 pau        (501) staff       (20)    28167 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/molecule.py
+-rw-rw-r--   0 pau        (501) staff       (20)     7345 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/mutdb.py
+-rw-rw-r--   0 pau        (501) staff       (20)     8874 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/ndx.py
+-rw-rw-r--   0 pau        (501) staff       (20)    16599 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/options.py
+-rw-rw-r--   0 pau        (501) staff       (20)     5036 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/parser.py
+-rw-rw-r--   0 pau        (501) staff       (20)    21628 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/rosetta.py
+-rw-rw-r--   0 pau        (501) staff       (20)    15211 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/rosetta_analyze.py
+-rw-rw-r--   0 pau        (501) staff       (20)    11783 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/rotamer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/scripts/
+-rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    33900 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/analyze_dhdl.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    19864 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/atomMapping.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    11939 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/build_cyclic_top.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2988 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/cli.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2955 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/gen_abs_restraints.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    73999 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/generate_hybrid_residue.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     7099 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/generate_hybrid_topology.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx/scripts/icolos_entrypoints/
+-rw-rw-r--   0 pau        (501) staff       (20)        0 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/icolos_entrypoints/__init__.py
+-rw-rw-r--   0 pau        (501) staff       (20)     7137 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/icolos_entrypoints/assemble_systems.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    12867 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/ligandHybrid.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2705 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/make_double_box.py
+-rw-rw-r--   0 pau        (501) staff       (20)    19943 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/md_setup.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    23072 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/mutate.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    38647 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/parameterize_ligands.py
+-rw-rw-r--   0 pau        (501) staff       (20)     7795 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/prepare_crooks_runs.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     1475 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/set_gmxlib.py
+-rw-rw-r--   0 pau        (501) staff       (20)    17636 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/scripts/setup_abfe.py
+-rw-rw-r--   0 pau        (501) staff       (20)    13784 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/summary.py
+-rw-rw-r--   0 pau        (501) staff       (20)    15258 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/utils.py
+-rw-rw-r--   0 pau        (501) staff       (20)    11331 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/xdrfile.py
+-rw-rw-r--   0 pau        (501) staff       (20)     1784 2023-05-19 08:30:20.000000 pmx_biobb-4.1.3/src/pmx/xtc.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     2722 2023-07-03 11:43:21.000000 pmx_biobb-4.1.3/src/pmx.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)    14322 2023-07-03 11:43:22.000000 pmx_biobb-4.1.3/src/pmx.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:43:21.000000 pmx_biobb-4.1.3/src/pmx.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       53 2023-07-03 11:43:21.000000 pmx_biobb-4.1.3/src/pmx.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:43:21.000000 pmx_biobb-4.1.3/src/pmx.egg-info/not-zip-safe
+-rw-r--r--   0 pau        (501) staff       (20)       29 2023-07-03 11:43:21.000000 pmx_biobb-4.1.3/src/pmx.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)        4 2023-07-03 11:43:21.000000 pmx_biobb-4.1.3/src/pmx.egg-info/top_level.txt
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx_biobb.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     2616 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx_biobb.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)    14582 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx_biobb.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx_biobb.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       53 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx_biobb.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-03 11:49:27.000000 pmx_biobb-4.1.3/src/pmx_biobb.egg-info/not-zip-safe
+-rw-r--r--   0 pau        (501) staff       (20)       29 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx_biobb.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)        4 2023-07-06 09:13:48.000000 pmx_biobb-4.1.3/src/pmx_biobb.egg-info/top_level.txt
+-rw-rw-r--   0 pau        (501) staff       (20)    66226 2023-07-06 09:07:32.000000 pmx_biobb-4.1.3/versioneer.py
```

### Comparing `pmx_biobb-4.1.2/LICENSE` & `pmx_biobb-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/PKG-INFO` & `pmx_biobb-4.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmx_biobb
-Version: 4.1.2
+Version: 4.1.3
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger, Vytautas Gapsys
 Author-email: d.seeliger@gmx.net, vytautas.gapsys@gmail.com
 License: LGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pmx_biobb-4.1.2/README.rst` & `pmx_biobb-4.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/setup.py` & `pmx_biobb-4.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/AbsRestraints.py` & `pmx_biobb-4.1.3/src/pmx/AbsRestraints.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/__init__.py` & `pmx_biobb-4.1.3/src/pmx/__init__.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/alchemy.py` & `pmx_biobb-4.1.3/src/pmx/alchemy.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/analysis.py` & `pmx_biobb-4.1.3/src/pmx/analysis.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/atom.py` & `pmx_biobb-4.1.3/src/pmx/atom.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/atomselection.py` & `pmx_biobb-4.1.3/src/pmx/atomselection.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/builder.py` & `pmx_biobb-4.1.3/src/pmx/builder.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/chain.py` & `pmx_biobb-4.1.3/src/pmx/chain.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/aminoacids.pkl` & `pmx_biobb-4.1.3/src/pmx/data/aminoacids.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/bbdep.pkl` & `pmx_biobb-4.1.3/src/pmx/data/bbdep.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/blosum62_new.mat` & `pmx_biobb-4.1.3/src/pmx/data/blosum62_new.mat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/bp.pkl` & `pmx_biobb-4.1.3/src/pmx/data/bp.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/bp_amber.pkl` & `pmx_biobb-4.1.3/src/pmx/data/bp_amber.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/bp_charmm.pkl` & `pmx_biobb-4.1.3/src/pmx/data/bp_charmm.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/ions.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/spc.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/spce.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber14sbmut.ff/urea.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber14sbmut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/atommass.dat` & `pmx_biobb-4.1.3/src/pmx/data/mutff/atommass.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp` & `pmx_biobb-4.1.3/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/elements.dat` & `pmx_biobb-4.1.3/src/pmx/data/mutff/elements.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/residuetypes.dat` & `pmx_biobb-4.1.3/src/pmx/data/mutff/residuetypes.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/spc216.gro` & `pmx_biobb-4.1.3/src/pmx/data/mutff/spc216.gro`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/mutff/vdwradii.dat` & `pmx_biobb-4.1.3/src/pmx/data/mutff/vdwradii.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/data/rna.pkl` & `pmx_biobb-4.1.3/src/pmx/data/rna.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/estimators.py` & `pmx_biobb-4.1.3/src/pmx/estimators.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/pmx/Energy.c` & `pmx_biobb-4.1.3/src/pmx/extensions/pmx/Energy.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/pmx/Geometry.c` & `pmx_biobb-4.1.3/src/pmx/extensions/pmx/Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/pmx/Geometry.h` & `pmx_biobb-4.1.3/src/pmx/extensions/pmx/Geometry.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/pmx/cpp_test.cpp` & `pmx_biobb-4.1.3/src/pmx/extensions/pmx/cpp_test.cpp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/pmx/init.c` & `pmx_biobb-4.1.3/src/pmx/extensions/pmx/init.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/pmx/pmx.h` & `pmx_biobb-4.1.3/src/pmx/extensions/pmx/pmx.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/pmx/wrap_Geometry.c` & `pmx_biobb-4.1.3/src/pmx/extensions/pmx/wrap_Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/xdr/trr2xtc.c` & `pmx_biobb-4.1.3/src/pmx/extensions/xdr/trr2xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile.c` & `pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile.h` & `pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_c_test.c` & `pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_c_test.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_trr.c` & `pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_trr.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_trr.h` & `pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_trr.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_xtc.c` & `pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/extensions/xdr/xdrfile_xtc.h` & `pmx_biobb-4.1.3/src/pmx/extensions/xdr/xdrfile_xtc.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/ffparser.py` & `pmx_biobb-4.1.3/src/pmx/ffparser.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/forcefield.py` & `pmx_biobb-4.1.3/src/pmx/forcefield.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/geometry.py` & `pmx_biobb-4.1.3/src/pmx/geometry.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/gmx.py` & `pmx_biobb-4.1.3/src/pmx/gmx.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/jobscript.py` & `pmx_biobb-4.1.3/src/pmx/jobscript.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/library.py` & `pmx_biobb-4.1.3/src/pmx/library.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/ligand_alchemy.py` & `pmx_biobb-4.1.3/src/pmx/ligand_alchemy.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/model.py` & `pmx_biobb-4.1.3/src/pmx/model.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/molecule.py` & `pmx_biobb-4.1.3/src/pmx/molecule.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/mutdb.py` & `pmx_biobb-4.1.3/src/pmx/mutdb.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/ndx.py` & `pmx_biobb-4.1.3/src/pmx/ndx.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/options.py` & `pmx_biobb-4.1.3/src/pmx/options.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/parser.py` & `pmx_biobb-4.1.3/src/pmx/parser.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/rosetta.py` & `pmx_biobb-4.1.3/src/pmx/rosetta.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/rosetta_analyze.py` & `pmx_biobb-4.1.3/src/pmx/rosetta_analyze.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/rotamer.py` & `pmx_biobb-4.1.3/src/pmx/rotamer.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/analyze_dhdl.py` & `pmx_biobb-4.1.3/src/pmx/scripts/analyze_dhdl.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/atomMapping.py` & `pmx_biobb-4.1.3/src/pmx/scripts/atomMapping.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/build_cyclic_top.py` & `pmx_biobb-4.1.3/src/pmx/scripts/build_cyclic_top.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/cli.py` & `pmx_biobb-4.1.3/src/pmx/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/gen_abs_restraints.py` & `pmx_biobb-4.1.3/src/pmx/scripts/gen_abs_restraints.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/generate_hybrid_residue.py` & `pmx_biobb-4.1.3/src/pmx/scripts/generate_hybrid_residue.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/generate_hybrid_topology.py` & `pmx_biobb-4.1.3/src/pmx/scripts/generate_hybrid_topology.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/icolos_entrypoints/assemble_systems.py` & `pmx_biobb-4.1.3/src/pmx/scripts/icolos_entrypoints/assemble_systems.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/ligandHybrid.py` & `pmx_biobb-4.1.3/src/pmx/scripts/ligandHybrid.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/make_double_box.py` & `pmx_biobb-4.1.3/src/pmx/scripts/make_double_box.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/md_setup.py` & `pmx_biobb-4.1.3/src/pmx/scripts/md_setup.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/mutate.py` & `pmx_biobb-4.1.3/src/pmx/scripts/mutate.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/parameterize_ligands.py` & `pmx_biobb-4.1.3/src/pmx/scripts/parameterize_ligands.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/prepare_crooks_runs.py` & `pmx_biobb-4.1.3/src/pmx/scripts/prepare_crooks_runs.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/set_gmxlib.py` & `pmx_biobb-4.1.3/src/pmx/scripts/set_gmxlib.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/scripts/setup_abfe.py` & `pmx_biobb-4.1.3/src/pmx/scripts/setup_abfe.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/summary.py` & `pmx_biobb-4.1.3/src/pmx/summary.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/utils.py` & `pmx_biobb-4.1.3/src/pmx/utils.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/xdrfile.py` & `pmx_biobb-4.1.3/src/pmx/xdrfile.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx/xtc.py` & `pmx_biobb-4.1.3/src/pmx/xtc.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx.egg-info/PKG-INFO` & `pmx_biobb-4.1.3/src/pmx.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx.egg-info/SOURCES.txt` & `pmx_biobb-4.1.3/src/pmx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/src/pmx_biobb.egg-info/PKG-INFO` & `pmx_biobb-4.1.3/src/pmx_biobb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmx-biobb
-Version: 4.1.2
+Version: 4.1.3
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger, Vytautas Gapsys
 Author-email: d.seeliger@gmx.net, vytautas.gapsys@gmail.com
 License: LGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pmx_biobb-4.1.2/src/pmx_biobb.egg-info/SOURCES.txt` & `pmx_biobb-4.1.3/src/pmx_biobb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmx_biobb-4.1.2/versioneer.py` & `pmx_biobb-4.1.3/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1401,15 +1401,15 @@
 
 def get_versions(verbose=False):
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
 
-    return {"version": "4.1.2", "full-revisionid": "4.1.2",
+    return {"version": "4.1.3", "full-revisionid": "4.1.3",
             "dirty": None, "error": None,
             "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
```

