# Comparing `tmp/wwpdb.utils.nmr-0.27.tar.gz` & `tmp/wwpdb.utils.nmr-0.28.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.nmr-0.27.tar", last modified: Tue Jun 27 11:50:52 2023, max compression
+gzip compressed data, was "wwpdb.utils.nmr-0.28.dev1.tar", last modified: Thu Jul  6 12:26:17 2023, max compression
```

## Comparing `wwpdb.utils.nmr-0.27.tar` & `wwpdb.utils.nmr-0.28.dev1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.036926 wwpdb.utils.nmr-0.27/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      704 2023-06-27 11:50:52.036926 wwpdb.utils.nmr-0.27/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-27 11:50:52.036926 wwpdb.utils.nmr-0.27/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2814 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.008925 wwpdb.utils.nmr-0.27/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.008925 wwpdb.utils.nmr-0.27/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.012925 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/
--rw-r--r--   0 vsts      (1001) docker     (123)   103812 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/AlignUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    72301 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/BMRBChemShiftStat.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12129 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/ChemCompUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26972 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/CifToNmrStar.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.012925 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/
--rw-r--r--   0 vsts      (1001) docker     (123)   517809 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4051 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.016925 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/lib/
--rw-r--r--   0 vsts      (1001) docker     (123)    27217 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     9863 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    10176 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   103535 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NmrDpReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)  2763977 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NmrDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)    23027 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NmrStarToCif.py
--rw-r--r--   0 vsts      (1001) docker     (123)   130980 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NmrVrptUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.016925 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/
--rwxr-xr-x   0 vsts      (1001) docker     (123)    10676 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    25729 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)    10656 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    25737 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3458 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3495 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8742 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)   170036 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/others.csv
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3573 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8327 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3591 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8409 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.016925 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    13142 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/io/ChemCompIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66593 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/io/CifReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10198 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/io/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.036926 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/
--rw-r--r--   0 vsts      (1001) docker     (123)    79462 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   233957 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   493179 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20363 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    42777 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberPTLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   178190 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberPTParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    79373 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberPTParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8451 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberPTReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11409 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/BiosymMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    41669 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/BiosymMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   135928 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/BiosymMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9563 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/BiosymMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    84136 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CharmmMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   212679 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CharmmMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   295091 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CharmmMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9003 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CharmmMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)   151068 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CnsMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   417159 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CnsMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   469882 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CnsMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13554 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CnsMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    32899 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CyanaMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   166923 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CyanaMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   454966 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CyanaMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18196 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CyanaMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    50972 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/DynamoMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   219341 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/DynamoMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   236108 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/DynamoMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9611 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/DynamoMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15500 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    43150 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    92902 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10402 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27535 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsPTLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   159229 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsPTParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    71357 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsPTParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8276 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsPTReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10640 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/IsdMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7446 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/IsdMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    83785 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/IsdMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8792 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/IsdMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3593 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/LexerErrorListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4792 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/ParserErrorListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)   406211 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/ParserListenerUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    33530 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/RosettaMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   119332 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/RosettaMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   215435 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/RosettaMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10471 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/RosettaMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11350 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/SybylMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10246 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/SybylMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    84828 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/SybylMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9089 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/SybylMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)   165077 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/XplorMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   679237 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/XplorMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   684343 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/XplorMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21181 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/XplorMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.036926 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/rci/
--rw-r--r--   0 vsts      (1001) docker     (123)   361662 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/rci/RCI.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 11:46:39.000000 wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/rci/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:50:52.008925 wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      704 2023-06-27 11:50:51.000000 wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3774 2023-06-27 11:50:51.000000 wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 11:50:51.000000 wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 11:47:49.000000 wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      330 2023-06-27 11:50:51.000000 wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-27 11:50:51.000000 wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      709 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2814 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.303945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (123)   103812 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/AlignUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    72301 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/BMRBChemShiftStat.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12129 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/ChemCompUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26972 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/CifToNmrStar.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/
+-rw-r--r--   0 vsts      (1001) docker     (123)   517809 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4051 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/
+-rw-r--r--   0 vsts      (1001) docker     (123)    27217 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     9863 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    10176 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   103535 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2763977 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23027 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrStarToCif.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   130980 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrVrptUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10676 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    25729 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10656 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    25737 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3458 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3495 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8742 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   170036 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/others.csv
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3573 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8327 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3591 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8409 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    13142 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/ChemCompIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66593 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/CifReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10198 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    79462 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   234229 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   493179 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20363 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    42777 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   178190 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    79373 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8451 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11409 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    41669 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   135928 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9563 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    84136 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   212951 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   295091 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9003 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   151068 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   417159 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   469882 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13554 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32899 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   167192 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   454966 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18196 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    50972 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   219341 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   236108 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9611 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15500 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    43150 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    92902 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10402 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27535 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   159229 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    71357 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8276 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10640 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7446 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    83785 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8792 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3593 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/LexerErrorListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4792 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserErrorListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   406211 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserListenerUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33530 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   119610 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   215435 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10471 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11350 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10246 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    84828 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9089 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   165077 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   679237 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   684343 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21181 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/
+-rw-r--r--   0 vsts      (1001) docker     (123)   361662 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/RCI.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      709 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3774 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-06 12:23:12.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      330 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.nmr-0.27/LICENSE` & `wwpdb.utils.nmr-0.28.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/PKG-INFO` & `wwpdb.utils.nmr-0.28.dev1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.nmr
-Version: 0.27
+Version: 0.28.dev1
 Summary: wwPDB NMR utilities
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_nmr
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.nmr-0.27/setup.py` & `wwpdb.utils.nmr-0.28.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/AlignUtil.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/AlignUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/BMRBChemShiftStat.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/BMRBChemShiftStat.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/ChemCompUtil.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/ChemCompUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/CifToNmrStar.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/CifToNmrStar.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/README.md` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NmrDpReport.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NmrDpUtility.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NmrStarToCif.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrStarToCif.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/NmrVrptUtility.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrVrptUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/others.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/others.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/io/ChemCompIo.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/ChemCompIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/io/CifReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/CifReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/io/mmCIFUtil.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,162 +100,162 @@
         12,30,1032,9,30,1,30,1,30,1,30,1,30,1,30,1,30,3,30,1040,8,30,1,30,
         5,30,1043,8,30,10,30,12,30,1046,9,30,1,30,1,30,3,30,1050,8,30,1,
         31,1,31,1,31,4,31,1055,8,31,11,31,12,31,1056,1,32,1,32,1,32,1,32,
         4,32,1063,8,32,11,32,12,32,1064,1,32,1,32,1,33,1,33,1,33,4,33,1072,
         8,33,11,33,12,33,1073,1,34,1,34,1,34,1,34,1,34,4,34,1081,8,34,11,
         34,12,34,1082,1,34,1,34,1,34,0,0,35,0,2,4,6,8,10,12,14,16,18,20,
         22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,62,64,
-        66,68,0,33,2,0,3,3,33,40,1,0,185,186,1,0,182,183,2,0,4,4,32,32,1,
-        0,193,194,1,0,190,191,2,0,6,6,43,50,2,0,7,7,51,58,1,0,203,204,5,
-        0,8,8,11,12,15,15,42,42,59,60,3,0,9,10,13,14,61,63,1,0,16,31,1,0,
-        197,198,1,0,67,68,1,0,69,71,2,0,72,76,78,78,3,0,80,80,89,89,91,92,
-        2,0,81,81,85,85,2,0,84,84,87,88,2,0,89,89,94,94,2,0,85,85,103,103,
-        2,0,86,86,96,100,2,0,88,88,102,102,2,0,105,105,112,113,2,0,106,107,
-        112,112,1,0,108,110,2,0,111,111,119,120,1,0,114,118,2,0,124,124,
-        132,132,1,0,125,127,1,0,128,130,1,0,133,139,2,0,229,229,231,231,
-        1275,0,81,1,0,0,0,2,86,1,0,0,0,4,95,1,0,0,0,6,100,1,0,0,0,8,105,
-        1,0,0,0,10,110,1,0,0,0,12,115,1,0,0,0,14,120,1,0,0,0,16,128,1,0,
-        0,0,18,204,1,0,0,0,20,209,1,0,0,0,22,269,1,0,0,0,24,274,1,0,0,0,
-        26,335,1,0,0,0,28,340,1,0,0,0,30,387,1,0,0,0,32,392,1,0,0,0,34,447,
-        1,0,0,0,36,452,1,0,0,0,38,490,1,0,0,0,40,519,1,0,0,0,42,560,1,0,
-        0,0,44,616,1,0,0,0,46,645,1,0,0,0,48,698,1,0,0,0,50,751,1,0,0,0,
-        52,828,1,0,0,0,54,929,1,0,0,0,56,952,1,0,0,0,58,1005,1,0,0,0,60,
-        1049,1,0,0,0,62,1051,1,0,0,0,64,1058,1,0,0,0,66,1068,1,0,0,0,68,
-        1075,1,0,0,0,70,80,3,2,1,0,71,80,3,4,2,0,72,80,3,6,3,0,73,80,3,8,
-        4,0,74,80,3,10,5,0,75,80,3,12,6,0,76,80,3,14,7,0,77,80,3,62,31,0,
-        78,80,3,66,33,0,79,70,1,0,0,0,79,71,1,0,0,0,79,72,1,0,0,0,79,73,
-        1,0,0,0,79,74,1,0,0,0,79,75,1,0,0,0,79,76,1,0,0,0,79,77,1,0,0,0,
-        79,78,1,0,0,0,80,83,1,0,0,0,81,79,1,0,0,0,81,82,1,0,0,0,82,84,1,
-        0,0,0,83,81,1,0,0,0,84,85,5,0,0,1,85,1,1,0,0,0,86,90,5,145,0,0,87,
-        89,5,158,0,0,88,87,1,0,0,0,89,92,1,0,0,0,90,88,1,0,0,0,90,91,1,0,
-        0,0,91,93,1,0,0,0,92,90,1,0,0,0,93,94,5,160,0,0,94,3,1,0,0,0,95,
-        96,5,2,0,0,96,98,3,16,8,0,97,99,5,1,0,0,98,97,1,0,0,0,98,99,1,0,
-        0,0,99,5,1,0,0,0,100,101,5,64,0,0,101,103,3,20,10,0,102,104,5,1,
-        0,0,103,102,1,0,0,0,103,104,1,0,0,0,104,7,1,0,0,0,105,106,5,79,0,
-        0,106,108,3,24,12,0,107,109,5,1,0,0,108,107,1,0,0,0,108,109,1,0,
-        0,0,109,9,1,0,0,0,110,111,5,93,0,0,111,113,3,28,14,0,112,114,5,1,
-        0,0,113,112,1,0,0,0,113,114,1,0,0,0,114,11,1,0,0,0,115,116,5,104,
-        0,0,116,118,3,32,16,0,117,119,5,1,0,0,118,117,1,0,0,0,118,119,1,
-        0,0,0,119,13,1,0,0,0,120,121,5,123,0,0,121,123,3,36,18,0,122,124,
+        66,68,0,34,1,1,160,160,2,0,3,3,33,40,1,0,185,186,1,0,182,183,2,0,
+        4,4,32,32,1,0,193,194,1,0,190,191,2,0,6,6,43,50,2,0,7,7,51,58,1,
+        0,203,204,5,0,8,8,11,12,15,15,42,42,59,60,3,0,9,10,13,14,61,63,1,
+        0,16,31,1,0,197,198,1,0,67,68,1,0,69,71,2,0,72,76,78,78,3,0,80,80,
+        89,89,91,92,2,0,81,81,85,85,2,0,84,84,87,88,2,0,89,89,94,94,2,0,
+        85,85,103,103,2,0,86,86,96,100,2,0,88,88,102,102,2,0,105,105,112,
+        113,2,0,106,107,112,112,1,0,108,110,2,0,111,111,119,120,1,0,114,
+        118,2,0,124,124,132,132,1,0,125,127,1,0,128,130,1,0,133,139,2,0,
+        229,229,231,231,1275,0,81,1,0,0,0,2,86,1,0,0,0,4,95,1,0,0,0,6,100,
+        1,0,0,0,8,105,1,0,0,0,10,110,1,0,0,0,12,115,1,0,0,0,14,120,1,0,0,
+        0,16,128,1,0,0,0,18,204,1,0,0,0,20,209,1,0,0,0,22,269,1,0,0,0,24,
+        274,1,0,0,0,26,335,1,0,0,0,28,340,1,0,0,0,30,387,1,0,0,0,32,392,
+        1,0,0,0,34,447,1,0,0,0,36,452,1,0,0,0,38,490,1,0,0,0,40,519,1,0,
+        0,0,42,560,1,0,0,0,44,616,1,0,0,0,46,645,1,0,0,0,48,698,1,0,0,0,
+        50,751,1,0,0,0,52,828,1,0,0,0,54,929,1,0,0,0,56,952,1,0,0,0,58,1005,
+        1,0,0,0,60,1049,1,0,0,0,62,1051,1,0,0,0,64,1058,1,0,0,0,66,1068,
+        1,0,0,0,68,1075,1,0,0,0,70,80,3,2,1,0,71,80,3,4,2,0,72,80,3,6,3,
+        0,73,80,3,8,4,0,74,80,3,10,5,0,75,80,3,12,6,0,76,80,3,14,7,0,77,
+        80,3,62,31,0,78,80,3,66,33,0,79,70,1,0,0,0,79,71,1,0,0,0,79,72,1,
+        0,0,0,79,73,1,0,0,0,79,74,1,0,0,0,79,75,1,0,0,0,79,76,1,0,0,0,79,
+        77,1,0,0,0,79,78,1,0,0,0,80,83,1,0,0,0,81,79,1,0,0,0,81,82,1,0,0,
+        0,82,84,1,0,0,0,83,81,1,0,0,0,84,85,5,0,0,1,85,1,1,0,0,0,86,90,5,
+        145,0,0,87,89,5,158,0,0,88,87,1,0,0,0,89,92,1,0,0,0,90,88,1,0,0,
+        0,90,91,1,0,0,0,91,93,1,0,0,0,92,90,1,0,0,0,93,94,7,0,0,0,94,3,1,
+        0,0,0,95,96,5,2,0,0,96,98,3,16,8,0,97,99,5,1,0,0,98,97,1,0,0,0,98,
+        99,1,0,0,0,99,5,1,0,0,0,100,101,5,64,0,0,101,103,3,20,10,0,102,104,
+        5,1,0,0,103,102,1,0,0,0,103,104,1,0,0,0,104,7,1,0,0,0,105,106,5,
+        79,0,0,106,108,3,24,12,0,107,109,5,1,0,0,108,107,1,0,0,0,108,109,
+        1,0,0,0,109,9,1,0,0,0,110,111,5,93,0,0,111,113,3,28,14,0,112,114,
+        5,1,0,0,113,112,1,0,0,0,113,114,1,0,0,0,114,11,1,0,0,0,115,116,5,
+        104,0,0,116,118,3,32,16,0,117,119,5,1,0,0,118,117,1,0,0,0,118,119,
+        1,0,0,0,119,13,1,0,0,0,120,121,5,123,0,0,121,123,3,36,18,0,122,124,
         5,1,0,0,123,122,1,0,0,0,123,124,1,0,0,0,124,15,1,0,0,0,125,127,3,
         18,9,0,126,125,1,0,0,0,127,130,1,0,0,0,128,126,1,0,0,0,128,129,1,
-        0,0,0,129,17,1,0,0,0,130,128,1,0,0,0,131,132,7,0,0,0,132,133,5,181,
-        0,0,133,134,7,1,0,0,134,205,7,2,0,0,135,136,7,3,0,0,136,137,5,189,
-        0,0,137,138,7,4,0,0,138,205,7,5,0,0,139,140,5,5,0,0,140,141,5,153,
+        0,0,0,129,17,1,0,0,0,130,128,1,0,0,0,131,132,7,1,0,0,132,133,5,181,
+        0,0,133,134,7,2,0,0,134,205,7,3,0,0,135,136,7,4,0,0,136,137,5,189,
+        0,0,137,138,7,5,0,0,138,205,7,6,0,0,139,140,5,5,0,0,140,141,5,153,
         0,0,141,150,5,154,0,0,142,151,3,40,20,0,143,151,3,42,21,0,144,151,
         3,48,24,0,145,151,3,44,22,0,146,151,3,46,23,0,147,151,3,50,25,0,
         148,151,3,52,26,0,149,151,3,54,27,0,150,142,1,0,0,0,150,143,1,0,
         0,0,150,144,1,0,0,0,150,145,1,0,0,0,150,146,1,0,0,0,150,147,1,0,
         0,0,150,148,1,0,0,0,150,149,1,0,0,0,151,152,1,0,0,0,152,154,5,227,
         0,0,153,155,5,140,0,0,154,153,1,0,0,0,154,155,1,0,0,0,155,205,1,
-        0,0,0,156,157,7,6,0,0,157,158,5,175,0,0,158,159,5,176,0,0,159,160,
+        0,0,0,156,157,7,7,0,0,157,158,5,175,0,0,158,159,5,176,0,0,159,160,
         5,177,0,0,160,162,5,179,0,0,161,163,5,140,0,0,162,161,1,0,0,0,162,
-        163,1,0,0,0,163,205,1,0,0,0,164,165,7,7,0,0,165,166,5,202,0,0,166,
-        167,5,205,0,0,167,205,7,8,0,0,168,169,7,9,0,0,169,170,5,169,0,0,
+        163,1,0,0,0,163,205,1,0,0,0,164,165,7,8,0,0,165,166,5,202,0,0,166,
+        167,5,205,0,0,167,205,7,9,0,0,168,169,7,10,0,0,169,170,5,169,0,0,
         170,172,5,170,0,0,171,173,5,140,0,0,172,171,1,0,0,0,172,173,1,0,
-        0,0,173,205,1,0,0,0,174,175,7,10,0,0,175,176,5,161,0,0,176,178,5,
+        0,0,173,205,1,0,0,0,174,175,7,11,0,0,175,176,5,161,0,0,176,178,5,
         163,0,0,177,179,5,140,0,0,178,177,1,0,0,0,178,179,1,0,0,0,179,205,
-        1,0,0,0,180,181,7,11,0,0,181,182,5,165,0,0,182,184,5,167,0,0,183,
+        1,0,0,0,180,181,7,12,0,0,181,182,5,165,0,0,182,184,5,167,0,0,183,
         185,5,140,0,0,184,183,1,0,0,0,184,185,1,0,0,0,185,205,1,0,0,0,186,
-        187,5,41,0,0,187,188,5,196,0,0,188,189,5,199,0,0,189,205,7,12,0,
-        0,190,191,7,0,0,0,191,192,5,180,0,0,192,193,5,209,0,0,193,194,5,
-        208,0,0,194,195,5,181,0,0,195,196,5,185,0,0,196,205,7,2,0,0,197,
+        187,5,41,0,0,187,188,5,196,0,0,188,189,5,199,0,0,189,205,7,13,0,
+        0,190,191,7,1,0,0,191,192,5,180,0,0,192,193,5,209,0,0,193,194,5,
+        208,0,0,194,195,5,181,0,0,195,196,5,185,0,0,196,205,7,3,0,0,197,
         198,5,4,0,0,198,199,5,188,0,0,199,200,5,209,0,0,200,201,5,208,0,
-        0,201,202,5,189,0,0,202,203,5,193,0,0,203,205,7,5,0,0,204,131,1,
+        0,201,202,5,189,0,0,202,203,5,193,0,0,203,205,7,6,0,0,204,131,1,
         0,0,0,204,135,1,0,0,0,204,139,1,0,0,0,204,156,1,0,0,0,204,164,1,
         0,0,0,204,168,1,0,0,0,204,174,1,0,0,0,204,180,1,0,0,0,204,186,1,
         0,0,0,204,190,1,0,0,0,204,197,1,0,0,0,205,19,1,0,0,0,206,208,3,22,
         11,0,207,206,1,0,0,0,208,211,1,0,0,0,209,207,1,0,0,0,209,210,1,0,
         0,0,210,21,1,0,0,0,211,209,1,0,0,0,212,213,5,65,0,0,213,214,5,181,
-        0,0,214,215,7,1,0,0,215,270,7,2,0,0,216,217,5,66,0,0,217,218,5,189,
-        0,0,218,219,7,4,0,0,219,270,7,5,0,0,220,221,7,13,0,0,221,222,5,162,
+        0,0,214,215,7,2,0,0,215,270,7,3,0,0,216,217,5,66,0,0,217,218,5,189,
+        0,0,218,219,7,5,0,0,219,270,7,6,0,0,220,221,7,14,0,0,221,222,5,162,
         0,0,222,223,5,209,0,0,223,224,5,207,0,0,224,225,5,209,0,0,225,226,
         5,208,0,0,226,227,5,161,0,0,227,229,5,163,0,0,228,230,5,140,0,0,
-        229,228,1,0,0,0,229,230,1,0,0,0,230,270,1,0,0,0,231,232,7,14,0,0,
+        229,228,1,0,0,0,229,230,1,0,0,0,230,270,1,0,0,0,231,232,7,15,0,0,
         232,233,5,166,0,0,233,234,5,209,0,0,234,235,5,207,0,0,235,236,5,
         209,0,0,236,237,5,208,0,0,237,238,5,165,0,0,238,240,5,167,0,0,239,
         241,5,140,0,0,240,239,1,0,0,0,240,241,1,0,0,0,241,270,1,0,0,0,242,
-        243,7,15,0,0,243,244,5,165,0,0,244,246,5,167,0,0,245,247,5,140,0,
+        243,7,16,0,0,243,244,5,165,0,0,244,246,5,167,0,0,245,247,5,140,0,
         0,246,245,1,0,0,0,246,247,1,0,0,0,247,270,1,0,0,0,248,249,5,77,0,
         0,249,250,5,169,0,0,250,252,5,170,0,0,251,253,5,140,0,0,252,251,
         1,0,0,0,252,253,1,0,0,0,253,270,1,0,0,0,254,255,5,65,0,0,255,256,
         5,180,0,0,256,257,5,209,0,0,257,258,5,208,0,0,258,259,5,181,0,0,
-        259,260,5,185,0,0,260,270,7,2,0,0,261,262,5,66,0,0,262,263,5,188,
+        259,260,5,185,0,0,260,270,7,3,0,0,261,262,5,66,0,0,262,263,5,188,
         0,0,263,264,5,209,0,0,264,265,5,208,0,0,265,266,5,189,0,0,266,267,
-        5,193,0,0,267,270,7,5,0,0,268,270,3,2,1,0,269,212,1,0,0,0,269,216,
+        5,193,0,0,267,270,7,6,0,0,268,270,3,2,1,0,269,212,1,0,0,0,269,216,
         1,0,0,0,269,220,1,0,0,0,269,231,1,0,0,0,269,242,1,0,0,0,269,248,
         1,0,0,0,269,254,1,0,0,0,269,261,1,0,0,0,269,268,1,0,0,0,270,23,1,
         0,0,0,271,273,3,26,13,0,272,271,1,0,0,0,273,276,1,0,0,0,274,272,
         1,0,0,0,274,275,1,0,0,0,275,25,1,0,0,0,276,274,1,0,0,0,277,278,7,
-        16,0,0,278,279,5,161,0,0,279,281,5,163,0,0,280,282,5,140,0,0,281,
-        280,1,0,0,0,281,282,1,0,0,0,282,336,1,0,0,0,283,284,7,17,0,0,284,
+        17,0,0,278,279,5,161,0,0,279,281,5,163,0,0,280,282,5,140,0,0,281,
+        280,1,0,0,0,281,282,1,0,0,0,282,336,1,0,0,0,283,284,7,18,0,0,284,
         285,5,162,0,0,285,286,5,209,0,0,286,287,5,208,0,0,287,288,5,161,
         0,0,288,290,5,163,0,0,289,291,5,140,0,0,290,289,1,0,0,0,290,291,
         1,0,0,0,291,336,1,0,0,0,292,293,5,82,0,0,293,294,5,162,0,0,294,295,
         5,209,0,0,295,296,5,207,0,0,296,297,5,209,0,0,297,298,5,208,0,0,
         298,299,5,161,0,0,299,301,5,163,0,0,300,302,5,140,0,0,301,300,1,
         0,0,0,301,302,1,0,0,0,302,336,1,0,0,0,303,304,5,86,0,0,304,305,5,
         166,0,0,305,306,5,209,0,0,306,307,5,208,0,0,307,308,5,165,0,0,308,
         310,5,167,0,0,309,311,5,140,0,0,310,309,1,0,0,0,310,311,1,0,0,0,
-        311,336,1,0,0,0,312,313,7,18,0,0,313,314,5,188,0,0,314,315,5,209,
-        0,0,315,316,5,208,0,0,316,317,5,189,0,0,317,318,7,4,0,0,318,336,
-        7,5,0,0,319,320,5,83,0,0,320,321,5,172,0,0,321,322,5,209,0,0,322,
+        311,336,1,0,0,0,312,313,7,19,0,0,313,314,5,188,0,0,314,315,5,209,
+        0,0,315,316,5,208,0,0,316,317,5,189,0,0,317,318,7,5,0,0,318,336,
+        7,6,0,0,319,320,5,83,0,0,320,321,5,172,0,0,321,322,5,209,0,0,322,
         323,5,208,0,0,323,324,5,173,0,0,324,326,5,174,0,0,325,327,5,140,
         0,0,326,325,1,0,0,0,326,327,1,0,0,0,327,336,1,0,0,0,328,329,5,90,
         0,0,329,330,5,165,0,0,330,332,5,167,0,0,331,333,5,140,0,0,332,331,
         1,0,0,0,332,333,1,0,0,0,333,336,1,0,0,0,334,336,3,2,1,0,335,277,
         1,0,0,0,335,283,1,0,0,0,335,292,1,0,0,0,335,303,1,0,0,0,335,312,
         1,0,0,0,335,319,1,0,0,0,335,328,1,0,0,0,335,334,1,0,0,0,336,27,1,
         0,0,0,337,339,3,30,15,0,338,337,1,0,0,0,339,342,1,0,0,0,340,338,
         1,0,0,0,340,341,1,0,0,0,341,29,1,0,0,0,342,340,1,0,0,0,343,344,7,
-        19,0,0,344,345,5,161,0,0,345,347,5,163,0,0,346,348,5,140,0,0,347,
+        20,0,0,344,345,5,161,0,0,345,347,5,163,0,0,346,348,5,140,0,0,347,
         346,1,0,0,0,347,348,1,0,0,0,348,388,1,0,0,0,349,350,5,95,0,0,350,
         351,5,173,0,0,351,353,5,174,0,0,352,354,5,140,0,0,353,352,1,0,0,
-        0,353,354,1,0,0,0,354,388,1,0,0,0,355,356,7,20,0,0,356,357,5,162,
+        0,353,354,1,0,0,0,354,388,1,0,0,0,355,356,7,21,0,0,356,357,5,162,
         0,0,357,358,5,209,0,0,358,359,5,208,0,0,359,360,5,161,0,0,360,362,
         5,163,0,0,361,363,5,140,0,0,362,361,1,0,0,0,362,363,1,0,0,0,363,
-        388,1,0,0,0,364,365,7,21,0,0,365,366,5,166,0,0,366,367,5,209,0,0,
+        388,1,0,0,0,364,365,7,22,0,0,365,366,5,166,0,0,366,367,5,209,0,0,
         367,368,5,208,0,0,368,369,5,165,0,0,369,371,5,167,0,0,370,372,5,
         140,0,0,371,370,1,0,0,0,371,372,1,0,0,0,372,388,1,0,0,0,373,374,
-        7,22,0,0,374,375,5,188,0,0,375,376,5,209,0,0,376,377,5,208,0,0,377,
-        378,5,189,0,0,378,379,7,4,0,0,379,388,7,5,0,0,380,381,5,101,0,0,
+        7,23,0,0,374,375,5,188,0,0,375,376,5,209,0,0,376,377,5,208,0,0,377,
+        378,5,189,0,0,378,379,7,5,0,0,379,388,7,6,0,0,380,381,5,101,0,0,
         381,382,5,165,0,0,382,384,5,167,0,0,383,385,5,140,0,0,384,383,1,
         0,0,0,384,385,1,0,0,0,385,388,1,0,0,0,386,388,3,2,1,0,387,343,1,
         0,0,0,387,349,1,0,0,0,387,355,1,0,0,0,387,364,1,0,0,0,387,373,1,
         0,0,0,387,380,1,0,0,0,387,386,1,0,0,0,388,31,1,0,0,0,389,391,3,34,
         17,0,390,389,1,0,0,0,391,394,1,0,0,0,392,390,1,0,0,0,392,393,1,0,
-        0,0,393,33,1,0,0,0,394,392,1,0,0,0,395,396,7,23,0,0,396,397,5,161,
+        0,0,393,33,1,0,0,0,394,392,1,0,0,0,395,396,7,24,0,0,396,397,5,161,
         0,0,397,399,5,163,0,0,398,400,5,140,0,0,399,398,1,0,0,0,399,400,
-        1,0,0,0,400,448,1,0,0,0,401,402,7,24,0,0,402,403,5,162,0,0,403,404,
+        1,0,0,0,400,448,1,0,0,0,401,402,7,25,0,0,402,403,5,162,0,0,403,404,
         5,209,0,0,404,405,5,208,0,0,405,406,5,161,0,0,406,408,5,163,0,0,
         407,409,5,140,0,0,408,407,1,0,0,0,408,409,1,0,0,0,409,448,1,0,0,
-        0,410,411,7,25,0,0,411,412,5,166,0,0,412,413,5,209,0,0,413,414,5,
+        0,410,411,7,26,0,0,411,412,5,166,0,0,412,413,5,209,0,0,413,414,5,
         208,0,0,414,415,5,165,0,0,415,417,5,167,0,0,416,418,5,140,0,0,417,
-        416,1,0,0,0,417,418,1,0,0,0,418,448,1,0,0,0,419,420,7,26,0,0,420,
+        416,1,0,0,0,417,418,1,0,0,0,418,448,1,0,0,0,419,420,7,27,0,0,420,
         421,5,188,0,0,421,422,5,209,0,0,422,423,5,208,0,0,423,424,5,189,
-        0,0,424,425,5,193,0,0,425,448,7,5,0,0,426,427,7,26,0,0,427,428,5,
-        189,0,0,428,429,7,4,0,0,429,448,7,5,0,0,430,431,7,27,0,0,431,432,
-        5,189,0,0,432,433,5,193,0,0,433,448,7,5,0,0,434,435,5,121,0,0,435,
+        0,0,424,425,5,193,0,0,425,448,7,6,0,0,426,427,7,27,0,0,427,428,5,
+        189,0,0,428,429,7,5,0,0,429,448,7,6,0,0,430,431,7,28,0,0,431,432,
+        5,189,0,0,432,433,5,193,0,0,433,448,7,6,0,0,434,435,5,121,0,0,435,
         436,5,165,0,0,436,438,5,167,0,0,437,439,5,140,0,0,438,437,1,0,0,
         0,438,439,1,0,0,0,439,448,1,0,0,0,440,441,5,122,0,0,441,442,5,153,
         0,0,442,444,5,146,0,0,443,445,5,140,0,0,444,443,1,0,0,0,444,445,
         1,0,0,0,445,448,1,0,0,0,446,448,3,2,1,0,447,395,1,0,0,0,447,401,
         1,0,0,0,447,410,1,0,0,0,447,419,1,0,0,0,447,426,1,0,0,0,447,430,
         1,0,0,0,447,434,1,0,0,0,447,440,1,0,0,0,447,446,1,0,0,0,448,35,1,
         0,0,0,449,451,3,38,19,0,450,449,1,0,0,0,451,454,1,0,0,0,452,450,
         1,0,0,0,452,453,1,0,0,0,453,37,1,0,0,0,454,452,1,0,0,0,455,456,7,
-        28,0,0,456,457,5,161,0,0,457,459,5,163,0,0,458,460,5,140,0,0,459,
-        458,1,0,0,0,459,460,1,0,0,0,460,491,1,0,0,0,461,462,7,29,0,0,462,
+        29,0,0,456,457,5,161,0,0,457,459,5,163,0,0,458,460,5,140,0,0,459,
+        458,1,0,0,0,459,460,1,0,0,0,460,491,1,0,0,0,461,462,7,30,0,0,462,
         463,5,162,0,0,463,464,5,209,0,0,464,465,5,208,0,0,465,466,5,161,
         0,0,466,468,5,163,0,0,467,469,5,140,0,0,468,467,1,0,0,0,468,469,
-        1,0,0,0,469,491,1,0,0,0,470,471,7,30,0,0,471,472,5,166,0,0,472,473,
+        1,0,0,0,469,491,1,0,0,0,470,471,7,31,0,0,471,472,5,166,0,0,472,473,
         5,209,0,0,473,474,5,208,0,0,474,475,5,165,0,0,475,477,5,167,0,0,
         476,478,5,140,0,0,477,476,1,0,0,0,477,478,1,0,0,0,478,491,1,0,0,
-        0,479,480,5,131,0,0,480,481,5,189,0,0,481,482,7,4,0,0,482,491,7,
-        5,0,0,483,484,7,31,0,0,484,485,5,165,0,0,485,487,5,167,0,0,486,488,
+        0,479,480,5,131,0,0,480,481,5,189,0,0,481,482,7,5,0,0,482,491,7,
+        6,0,0,483,484,7,32,0,0,484,485,5,165,0,0,485,487,5,167,0,0,486,488,
         5,140,0,0,487,486,1,0,0,0,487,488,1,0,0,0,488,491,1,0,0,0,489,491,
         3,2,1,0,490,455,1,0,0,0,490,461,1,0,0,0,490,470,1,0,0,0,490,479,
         1,0,0,0,490,483,1,0,0,0,490,489,1,0,0,0,491,39,1,0,0,0,492,493,5,
         211,0,0,493,494,5,221,0,0,494,496,3,56,28,0,495,497,5,220,0,0,496,
         495,1,0,0,0,496,497,1,0,0,0,497,498,1,0,0,0,498,499,3,56,28,0,499,
         500,5,222,0,0,500,520,1,0,0,0,501,502,5,211,0,0,502,503,5,223,0,
         0,503,505,3,56,28,0,504,506,5,220,0,0,505,504,1,0,0,0,505,506,1,
@@ -437,15 +437,15 @@
         5,155,0,0,1053,1055,3,64,32,0,1054,1053,1,0,0,0,1055,1056,1,0,0,
         0,1056,1054,1,0,0,0,1056,1057,1,0,0,0,1057,63,1,0,0,0,1058,1059,
         5,142,0,0,1059,1060,5,231,0,0,1060,1062,5,232,0,0,1061,1063,5,231,
         0,0,1062,1061,1,0,0,0,1063,1064,1,0,0,0,1064,1062,1,0,0,0,1064,1065,
         1,0,0,0,1065,1066,1,0,0,0,1066,1067,5,234,0,0,1067,65,1,0,0,0,1068,
         1069,5,141,0,0,1069,1071,5,155,0,0,1070,1072,3,68,34,0,1071,1070,
         1,0,0,0,1072,1073,1,0,0,0,1073,1071,1,0,0,0,1073,1074,1,0,0,0,1074,
-        67,1,0,0,0,1075,1076,5,143,0,0,1076,1077,7,32,0,0,1077,1080,5,232,
+        67,1,0,0,0,1075,1076,5,143,0,0,1076,1077,7,33,0,0,1077,1080,5,232,
         0,0,1078,1079,5,231,0,0,1079,1081,5,230,0,0,1080,1078,1,0,0,0,1081,
         1082,1,0,0,0,1082,1080,1,0,0,0,1082,1083,1,0,0,0,1083,1084,1,0,0,
         0,1084,1085,5,234,0,0,1085,69,1,0,0,0,153,79,81,90,98,103,108,113,
         118,123,128,150,154,162,172,178,184,204,209,229,240,246,252,269,
         274,281,290,301,310,326,332,335,340,347,353,362,371,384,387,392,
         399,408,417,438,444,447,452,459,468,477,487,490,496,505,514,519,
         525,529,538,542,551,555,560,566,575,584,593,602,611,616,622,631,
@@ -1027,14 +1027,17 @@
 
         def COMMENT(self):
             return self.getToken(AmberMRParser.COMMENT, 0)
 
         def RETURN_CM(self):
             return self.getToken(AmberMRParser.RETURN_CM, 0)
 
+        def EOF(self):
+            return self.getToken(AmberMRParser.EOF, 0)
+
         def Any_name(self, i:int=None):
             if i is None:
                 return self.getTokens(AmberMRParser.Any_name)
             else:
                 return self.getToken(AmberMRParser.Any_name, i)
 
         def getRuleIndex(self):
@@ -1067,15 +1070,20 @@
                 self.state = 87
                 self.match(AmberMRParser.Any_name)
                 self.state = 92
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
             self.state = 93
-            self.match(AmberMRParser.RETURN_CM)
+            _la = self._input.LA(1)
+            if not(_la==-1 or _la==160):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
```

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberPTLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberPTParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberPTParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/AmberPTReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/BiosymMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/BiosymMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/BiosymMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/BiosymMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CharmmMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CharmmMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,227 +78,227 @@
         8,45,1,45,3,45,771,8,45,1,45,1,45,1,45,1,45,1,45,3,45,778,8,45,1,
         45,1,45,1,45,3,45,783,8,45,1,45,3,45,786,8,45,1,45,1,45,1,45,1,45,
         3,45,792,8,45,1,45,1,45,1,45,1,45,1,45,1,45,1,45,1,45,1,45,3,45,
         803,8,45,1,45,3,45,806,8,45,5,45,808,8,45,10,45,12,45,811,9,45,1,
         46,1,46,1,47,1,47,1,48,1,48,1,49,1,49,1,49,3,49,822,8,49,1,49,1,
         49,1,49,1,49,0,1,90,50,0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30,
         32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,62,64,66,68,70,72,74,
-        76,78,80,82,84,86,88,90,92,94,96,98,0,18,1,0,16,17,1,0,18,20,4,0,
-        28,28,30,30,46,46,49,49,2,0,85,85,88,89,1,0,90,91,3,0,24,24,95,98,
-        101,101,1,0,18,19,2,0,9,9,109,109,1,0,111,112,4,0,9,9,11,11,109,
-        109,114,114,2,0,111,112,115,115,1,0,149,150,2,0,144,144,151,151,
-        2,0,22,22,127,127,3,0,126,126,128,128,130,130,2,0,144,145,162,162,
-        1,0,144,145,1,0,169,171,991,0,118,1,0,0,0,2,123,1,0,0,0,4,132,1,
-        0,0,0,6,141,1,0,0,0,8,150,1,0,0,0,10,161,1,0,0,0,12,169,1,0,0,0,
-        14,177,1,0,0,0,16,185,1,0,0,0,18,193,1,0,0,0,20,201,1,0,0,0,22,211,
-        1,0,0,0,24,218,1,0,0,0,26,225,1,0,0,0,28,237,1,0,0,0,30,244,1,0,
-        0,0,32,306,1,0,0,0,34,308,1,0,0,0,36,373,1,0,0,0,38,375,1,0,0,0,
-        40,389,1,0,0,0,42,429,1,0,0,0,44,489,1,0,0,0,46,499,1,0,0,0,48,505,
-        1,0,0,0,50,507,1,0,0,0,52,509,1,0,0,0,54,526,1,0,0,0,56,533,1,0,
-        0,0,58,535,1,0,0,0,60,551,1,0,0,0,62,570,1,0,0,0,64,572,1,0,0,0,
-        66,598,1,0,0,0,68,610,1,0,0,0,70,622,1,0,0,0,72,632,1,0,0,0,74,634,
-        1,0,0,0,76,643,1,0,0,0,78,645,1,0,0,0,80,656,1,0,0,0,82,663,1,0,
-        0,0,84,665,1,0,0,0,86,672,1,0,0,0,88,680,1,0,0,0,90,791,1,0,0,0,
-        92,812,1,0,0,0,94,814,1,0,0,0,96,816,1,0,0,0,98,818,1,0,0,0,100,
-        117,3,2,1,0,101,117,3,4,2,0,102,117,3,6,3,0,103,117,3,8,4,0,104,
-        117,3,10,5,0,105,117,3,12,6,0,106,117,3,14,7,0,107,117,3,16,8,0,
-        108,117,3,18,9,0,109,117,3,20,10,0,110,117,3,22,11,0,111,117,3,24,
-        12,0,112,117,3,26,13,0,113,117,3,28,14,0,114,117,3,30,15,0,115,117,
-        3,98,49,0,116,100,1,0,0,0,116,101,1,0,0,0,116,102,1,0,0,0,116,103,
-        1,0,0,0,116,104,1,0,0,0,116,105,1,0,0,0,116,106,1,0,0,0,116,107,
-        1,0,0,0,116,108,1,0,0,0,116,109,1,0,0,0,116,110,1,0,0,0,116,111,
-        1,0,0,0,116,112,1,0,0,0,116,113,1,0,0,0,116,114,1,0,0,0,116,115,
-        1,0,0,0,117,120,1,0,0,0,118,116,1,0,0,0,118,119,1,0,0,0,119,121,
-        1,0,0,0,120,118,1,0,0,0,121,122,5,0,0,1,122,1,1,0,0,0,123,127,5,
-        148,0,0,124,126,5,174,0,0,125,124,1,0,0,0,126,129,1,0,0,0,127,125,
-        1,0,0,0,127,128,1,0,0,0,128,130,1,0,0,0,129,127,1,0,0,0,130,131,
-        5,176,0,0,131,3,1,0,0,0,132,136,5,55,0,0,133,135,3,32,16,0,134,133,
-        1,0,0,0,135,138,1,0,0,0,136,134,1,0,0,0,136,137,1,0,0,0,137,139,
-        1,0,0,0,138,136,1,0,0,0,139,140,5,2,0,0,140,5,1,0,0,0,141,145,5,
-        57,0,0,142,144,3,36,18,0,143,142,1,0,0,0,144,147,1,0,0,0,145,143,
-        1,0,0,0,145,146,1,0,0,0,146,148,1,0,0,0,147,145,1,0,0,0,148,149,
-        5,2,0,0,149,7,1,0,0,0,150,159,5,3,0,0,151,155,5,21,0,0,152,154,3,
-        40,20,0,153,152,1,0,0,0,154,157,1,0,0,0,155,153,1,0,0,0,155,156,
-        1,0,0,0,156,160,1,0,0,0,157,155,1,0,0,0,158,160,5,26,0,0,159,151,
-        1,0,0,0,159,158,1,0,0,0,160,9,1,0,0,0,161,162,5,3,0,0,162,166,5,
-        4,0,0,163,165,3,44,22,0,164,163,1,0,0,0,165,168,1,0,0,0,166,164,
-        1,0,0,0,166,167,1,0,0,0,167,11,1,0,0,0,168,166,1,0,0,0,169,170,5,
-        3,0,0,170,174,5,27,0,0,171,173,3,54,27,0,172,171,1,0,0,0,173,176,
-        1,0,0,0,174,172,1,0,0,0,174,175,1,0,0,0,175,13,1,0,0,0,176,174,1,
-        0,0,0,177,178,5,3,0,0,178,182,5,32,0,0,179,181,3,56,28,0,180,179,
-        1,0,0,0,181,184,1,0,0,0,182,180,1,0,0,0,182,183,1,0,0,0,183,15,1,
-        0,0,0,184,182,1,0,0,0,185,186,5,3,0,0,186,190,5,34,0,0,187,189,3,
-        58,29,0,188,187,1,0,0,0,189,192,1,0,0,0,190,188,1,0,0,0,190,191,
-        1,0,0,0,191,17,1,0,0,0,192,190,1,0,0,0,193,194,5,3,0,0,194,198,5,
-        39,0,0,195,197,3,60,30,0,196,195,1,0,0,0,197,200,1,0,0,0,198,196,
-        1,0,0,0,198,199,1,0,0,0,199,19,1,0,0,0,200,198,1,0,0,0,201,209,5,
-        43,0,0,202,204,3,62,31,0,203,202,1,0,0,0,204,207,1,0,0,0,205,203,
-        1,0,0,0,205,206,1,0,0,0,206,210,1,0,0,0,207,205,1,0,0,0,208,210,
-        5,44,0,0,209,205,1,0,0,0,209,208,1,0,0,0,210,21,1,0,0,0,211,215,
-        5,87,0,0,212,214,3,68,34,0,213,212,1,0,0,0,214,217,1,0,0,0,215,213,
-        1,0,0,0,215,216,1,0,0,0,216,23,1,0,0,0,217,215,1,0,0,0,218,222,5,
-        94,0,0,219,221,3,70,35,0,220,219,1,0,0,0,221,224,1,0,0,0,222,220,
-        1,0,0,0,222,223,1,0,0,0,223,25,1,0,0,0,224,222,1,0,0,0,225,226,5,
-        3,0,0,226,235,5,102,0,0,227,229,3,72,36,0,228,227,1,0,0,0,229,232,
-        1,0,0,0,230,228,1,0,0,0,230,231,1,0,0,0,231,236,1,0,0,0,232,230,
-        1,0,0,0,233,236,5,105,0,0,234,236,5,8,0,0,235,230,1,0,0,0,235,233,
-        1,0,0,0,235,234,1,0,0,0,236,27,1,0,0,0,237,241,5,108,0,0,238,240,
-        3,80,40,0,239,238,1,0,0,0,240,243,1,0,0,0,241,239,1,0,0,0,241,242,
-        1,0,0,0,242,29,1,0,0,0,243,241,1,0,0,0,244,248,5,113,0,0,245,247,
-        3,82,41,0,246,245,1,0,0,0,247,250,1,0,0,0,248,246,1,0,0,0,248,249,
-        1,0,0,0,249,31,1,0,0,0,250,248,1,0,0,0,251,307,3,34,17,0,252,307,
-        5,56,0,0,253,254,5,59,0,0,254,307,3,96,48,0,255,256,5,61,0,0,256,
-        307,3,96,48,0,257,258,5,60,0,0,258,307,3,96,48,0,259,260,5,62,0,
-        0,260,307,3,96,48,0,261,262,5,63,0,0,262,307,3,96,48,0,263,307,5,
-        64,0,0,264,265,5,65,0,0,265,307,3,96,48,0,266,267,5,66,0,0,267,307,
-        3,96,48,0,268,307,5,67,0,0,269,270,5,68,0,0,270,307,3,96,48,0,271,
-        272,5,69,0,0,272,307,3,96,48,0,273,274,5,73,0,0,274,275,5,74,0,0,
-        275,276,5,144,0,0,276,277,5,75,0,0,277,278,3,96,48,0,278,279,5,76,
-        0,0,279,280,3,96,48,0,280,281,5,77,0,0,281,282,3,96,48,0,282,307,
-        1,0,0,0,283,284,5,78,0,0,284,307,5,144,0,0,285,286,5,79,0,0,286,
-        287,5,81,0,0,287,307,5,144,0,0,288,289,5,80,0,0,289,290,5,81,0,0,
-        290,292,5,144,0,0,291,293,5,83,0,0,292,291,1,0,0,0,292,293,1,0,0,
-        0,293,307,1,0,0,0,294,300,5,82,0,0,295,298,5,83,0,0,296,297,5,84,
-        0,0,297,299,3,96,48,0,298,296,1,0,0,0,298,299,1,0,0,0,299,301,1,
-        0,0,0,300,295,1,0,0,0,300,301,1,0,0,0,301,307,1,0,0,0,302,303,5,
-        85,0,0,303,307,3,96,48,0,304,305,5,86,0,0,305,307,3,96,48,0,306,
-        251,1,0,0,0,306,252,1,0,0,0,306,253,1,0,0,0,306,255,1,0,0,0,306,
-        257,1,0,0,0,306,259,1,0,0,0,306,261,1,0,0,0,306,263,1,0,0,0,306,
-        264,1,0,0,0,306,266,1,0,0,0,306,268,1,0,0,0,306,269,1,0,0,0,306,
-        271,1,0,0,0,306,273,1,0,0,0,306,283,1,0,0,0,306,285,1,0,0,0,306,
-        288,1,0,0,0,306,294,1,0,0,0,306,302,1,0,0,0,306,304,1,0,0,0,307,
-        33,1,0,0,0,308,309,5,58,0,0,309,310,3,84,42,0,310,311,3,84,42,0,
-        311,35,1,0,0,0,312,374,3,38,19,0,313,374,5,56,0,0,314,315,5,59,0,
-        0,315,374,3,96,48,0,316,317,5,61,0,0,317,374,3,96,48,0,318,319,5,
-        60,0,0,319,374,3,96,48,0,320,321,5,62,0,0,321,374,3,96,48,0,322,
-        323,5,63,0,0,323,374,3,96,48,0,324,325,5,70,0,0,325,374,3,96,48,
-        0,326,327,5,71,0,0,327,374,3,96,48,0,328,329,5,72,0,0,329,374,3,
-        96,48,0,330,374,5,64,0,0,331,332,5,65,0,0,332,374,3,96,48,0,333,
-        334,5,66,0,0,334,374,3,96,48,0,335,374,5,67,0,0,336,337,5,68,0,0,
-        337,374,3,96,48,0,338,339,5,69,0,0,339,374,3,96,48,0,340,341,5,73,
-        0,0,341,342,5,74,0,0,342,343,5,144,0,0,343,344,5,75,0,0,344,345,
-        3,96,48,0,345,346,5,76,0,0,346,347,3,96,48,0,347,348,5,77,0,0,348,
-        349,3,96,48,0,349,374,1,0,0,0,350,351,5,78,0,0,351,374,5,144,0,0,
-        352,353,5,79,0,0,353,354,5,81,0,0,354,374,5,144,0,0,355,356,5,80,
-        0,0,356,357,5,81,0,0,357,359,5,144,0,0,358,360,5,83,0,0,359,358,
-        1,0,0,0,359,360,1,0,0,0,360,374,1,0,0,0,361,367,5,82,0,0,362,365,
-        5,83,0,0,363,364,5,84,0,0,364,366,3,96,48,0,365,363,1,0,0,0,365,
-        366,1,0,0,0,366,368,1,0,0,0,367,362,1,0,0,0,367,368,1,0,0,0,368,
-        374,1,0,0,0,369,370,5,85,0,0,370,374,3,96,48,0,371,372,5,86,0,0,
-        372,374,3,96,48,0,373,312,1,0,0,0,373,313,1,0,0,0,373,314,1,0,0,
-        0,373,316,1,0,0,0,373,318,1,0,0,0,373,320,1,0,0,0,373,322,1,0,0,
-        0,373,324,1,0,0,0,373,326,1,0,0,0,373,328,1,0,0,0,373,330,1,0,0,
-        0,373,331,1,0,0,0,373,333,1,0,0,0,373,335,1,0,0,0,373,336,1,0,0,
-        0,373,338,1,0,0,0,373,340,1,0,0,0,373,350,1,0,0,0,373,352,1,0,0,
-        0,373,355,1,0,0,0,373,361,1,0,0,0,373,369,1,0,0,0,373,371,1,0,0,
-        0,374,37,1,0,0,0,375,376,5,58,0,0,376,377,3,84,42,0,377,39,1,0,0,
-        0,378,390,3,42,21,0,379,380,5,9,0,0,380,390,3,96,48,0,381,382,5,
-        23,0,0,382,390,3,96,48,0,383,384,5,24,0,0,384,390,5,144,0,0,385,
-        390,5,19,0,0,386,387,5,25,0,0,387,390,3,96,48,0,388,390,5,18,0,0,
-        389,378,1,0,0,0,389,379,1,0,0,0,389,381,1,0,0,0,389,383,1,0,0,0,
-        389,385,1,0,0,0,389,386,1,0,0,0,389,388,1,0,0,0,390,41,1,0,0,0,391,
-        392,3,84,42,0,392,393,3,84,42,0,393,394,3,84,42,0,394,395,3,84,42,
-        0,395,430,1,0,0,0,396,397,5,22,0,0,397,398,5,144,0,0,398,399,5,144,
-        0,0,399,400,5,144,0,0,400,430,5,144,0,0,401,402,5,144,0,0,402,403,
-        5,149,0,0,403,404,5,144,0,0,404,405,5,149,0,0,405,406,5,144,0,0,
-        406,407,5,149,0,0,407,408,5,144,0,0,408,430,5,149,0,0,409,411,5,
-        149,0,0,410,409,1,0,0,0,410,411,1,0,0,0,411,412,1,0,0,0,412,413,
-        5,144,0,0,413,415,5,149,0,0,414,416,5,149,0,0,415,414,1,0,0,0,415,
-        416,1,0,0,0,416,417,1,0,0,0,417,418,5,144,0,0,418,420,5,149,0,0,
-        419,421,5,149,0,0,420,419,1,0,0,0,420,421,1,0,0,0,421,422,1,0,0,
-        0,422,423,5,144,0,0,423,425,5,149,0,0,424,426,5,149,0,0,425,424,
-        1,0,0,0,425,426,1,0,0,0,426,427,1,0,0,0,427,428,5,144,0,0,428,430,
-        5,149,0,0,429,391,1,0,0,0,429,396,1,0,0,0,429,401,1,0,0,0,429,410,
-        1,0,0,0,430,43,1,0,0,0,431,433,5,5,0,0,432,431,1,0,0,0,432,433,1,
-        0,0,0,433,437,1,0,0,0,434,436,3,46,23,0,435,434,1,0,0,0,436,439,
-        1,0,0,0,437,435,1,0,0,0,437,438,1,0,0,0,438,443,1,0,0,0,439,437,
-        1,0,0,0,440,442,3,48,24,0,441,440,1,0,0,0,442,445,1,0,0,0,443,441,
-        1,0,0,0,443,444,1,0,0,0,444,446,1,0,0,0,445,443,1,0,0,0,446,450,
-        3,84,42,0,447,449,3,48,24,0,448,447,1,0,0,0,449,452,1,0,0,0,450,
-        448,1,0,0,0,450,451,1,0,0,0,451,454,1,0,0,0,452,450,1,0,0,0,453,
-        455,3,52,26,0,454,453,1,0,0,0,454,455,1,0,0,0,455,490,1,0,0,0,456,
-        458,5,6,0,0,457,459,3,50,25,0,458,457,1,0,0,0,458,459,1,0,0,0,459,
-        463,1,0,0,0,460,462,3,48,24,0,461,460,1,0,0,0,462,465,1,0,0,0,463,
-        461,1,0,0,0,463,464,1,0,0,0,464,467,1,0,0,0,465,463,1,0,0,0,466,
-        468,3,52,26,0,467,466,1,0,0,0,467,468,1,0,0,0,468,490,1,0,0,0,469,
-        471,5,7,0,0,470,472,3,50,25,0,471,470,1,0,0,0,471,472,1,0,0,0,472,
-        476,1,0,0,0,473,475,3,48,24,0,474,473,1,0,0,0,475,478,1,0,0,0,476,
-        474,1,0,0,0,476,477,1,0,0,0,477,479,1,0,0,0,478,476,1,0,0,0,479,
-        483,3,84,42,0,480,482,3,48,24,0,481,480,1,0,0,0,482,485,1,0,0,0,
-        483,481,1,0,0,0,483,484,1,0,0,0,484,486,1,0,0,0,485,483,1,0,0,0,
-        486,487,3,84,42,0,487,490,1,0,0,0,488,490,5,8,0,0,489,432,1,0,0,
-        0,489,456,1,0,0,0,489,469,1,0,0,0,489,488,1,0,0,0,490,45,1,0,0,0,
-        491,492,5,12,0,0,492,500,5,144,0,0,493,494,5,13,0,0,494,500,3,92,
-        46,0,495,496,5,14,0,0,496,500,3,92,46,0,497,498,5,15,0,0,498,500,
-        3,92,46,0,499,491,1,0,0,0,499,493,1,0,0,0,499,495,1,0,0,0,499,497,
-        1,0,0,0,500,47,1,0,0,0,501,502,5,9,0,0,502,506,3,92,46,0,503,506,
-        5,10,0,0,504,506,5,11,0,0,505,501,1,0,0,0,505,503,1,0,0,0,505,504,
-        1,0,0,0,506,49,1,0,0,0,507,508,7,0,0,0,508,51,1,0,0,0,509,510,7,
-        1,0,0,510,53,1,0,0,0,511,512,5,28,0,0,512,515,3,92,46,0,513,514,
-        5,12,0,0,514,516,5,144,0,0,515,513,1,0,0,0,515,516,1,0,0,0,516,518,
-        1,0,0,0,517,519,5,29,0,0,518,517,1,0,0,0,518,519,1,0,0,0,519,527,
-        1,0,0,0,520,521,5,30,0,0,521,527,3,92,46,0,522,523,5,21,0,0,523,
-        527,3,92,46,0,524,525,5,31,0,0,525,527,3,92,46,0,526,511,1,0,0,0,
-        526,520,1,0,0,0,526,522,1,0,0,0,526,524,1,0,0,0,527,55,1,0,0,0,528,
-        529,5,9,0,0,529,534,3,92,46,0,530,531,5,12,0,0,531,534,5,144,0,0,
-        532,534,5,33,0,0,533,528,1,0,0,0,533,530,1,0,0,0,533,532,1,0,0,0,
-        534,57,1,0,0,0,535,537,3,84,42,0,536,538,5,35,0,0,537,536,1,0,0,
-        0,537,538,1,0,0,0,538,540,1,0,0,0,539,541,5,28,0,0,540,539,1,0,0,
-        0,540,541,1,0,0,0,541,543,1,0,0,0,542,544,5,36,0,0,543,542,1,0,0,
-        0,543,544,1,0,0,0,544,546,1,0,0,0,545,547,5,37,0,0,546,545,1,0,0,
-        0,546,547,1,0,0,0,547,549,1,0,0,0,548,550,5,38,0,0,549,548,1,0,0,
-        0,549,550,1,0,0,0,550,59,1,0,0,0,551,552,5,9,0,0,552,554,3,92,46,
-        0,553,555,5,11,0,0,554,553,1,0,0,0,554,555,1,0,0,0,555,556,1,0,0,
-        0,556,557,5,40,0,0,557,558,3,92,46,0,558,559,5,41,0,0,559,560,3,
-        92,46,0,560,561,5,42,0,0,561,562,3,92,46,0,562,563,3,84,42,0,563,
-        61,1,0,0,0,564,565,3,84,42,0,565,566,3,84,42,0,566,567,3,64,32,0,
-        567,571,1,0,0,0,568,571,3,66,33,0,569,571,5,45,0,0,570,564,1,0,0,
-        0,570,568,1,0,0,0,570,569,1,0,0,0,571,63,1,0,0,0,572,578,7,2,0,0,
-        573,575,5,18,0,0,574,573,1,0,0,0,574,575,1,0,0,0,575,579,1,0,0,0,
-        576,579,5,19,0,0,577,579,5,50,0,0,578,574,1,0,0,0,578,576,1,0,0,
-        0,578,577,1,0,0,0,579,582,1,0,0,0,580,581,5,47,0,0,581,583,3,92,
-        46,0,582,580,1,0,0,0,582,583,1,0,0,0,583,586,1,0,0,0,584,585,5,48,
-        0,0,585,587,5,144,0,0,586,584,1,0,0,0,586,587,1,0,0,0,587,590,1,
-        0,0,0,588,589,5,51,0,0,589,591,3,92,46,0,590,588,1,0,0,0,590,591,
+        76,78,80,82,84,86,88,90,92,94,96,98,0,19,1,1,176,176,1,0,16,17,1,
+        0,18,20,4,0,28,28,30,30,46,46,49,49,2,0,85,85,88,89,1,0,90,91,3,
+        0,24,24,95,98,101,101,1,0,18,19,2,0,9,9,109,109,1,0,111,112,4,0,
+        9,9,11,11,109,109,114,114,2,0,111,112,115,115,1,0,149,150,2,0,144,
+        144,151,151,2,0,22,22,127,127,3,0,126,126,128,128,130,130,2,0,144,
+        145,162,162,1,0,144,145,1,0,169,171,991,0,118,1,0,0,0,2,123,1,0,
+        0,0,4,132,1,0,0,0,6,141,1,0,0,0,8,150,1,0,0,0,10,161,1,0,0,0,12,
+        169,1,0,0,0,14,177,1,0,0,0,16,185,1,0,0,0,18,193,1,0,0,0,20,201,
+        1,0,0,0,22,211,1,0,0,0,24,218,1,0,0,0,26,225,1,0,0,0,28,237,1,0,
+        0,0,30,244,1,0,0,0,32,306,1,0,0,0,34,308,1,0,0,0,36,373,1,0,0,0,
+        38,375,1,0,0,0,40,389,1,0,0,0,42,429,1,0,0,0,44,489,1,0,0,0,46,499,
+        1,0,0,0,48,505,1,0,0,0,50,507,1,0,0,0,52,509,1,0,0,0,54,526,1,0,
+        0,0,56,533,1,0,0,0,58,535,1,0,0,0,60,551,1,0,0,0,62,570,1,0,0,0,
+        64,572,1,0,0,0,66,598,1,0,0,0,68,610,1,0,0,0,70,622,1,0,0,0,72,632,
+        1,0,0,0,74,634,1,0,0,0,76,643,1,0,0,0,78,645,1,0,0,0,80,656,1,0,
+        0,0,82,663,1,0,0,0,84,665,1,0,0,0,86,672,1,0,0,0,88,680,1,0,0,0,
+        90,791,1,0,0,0,92,812,1,0,0,0,94,814,1,0,0,0,96,816,1,0,0,0,98,818,
+        1,0,0,0,100,117,3,2,1,0,101,117,3,4,2,0,102,117,3,6,3,0,103,117,
+        3,8,4,0,104,117,3,10,5,0,105,117,3,12,6,0,106,117,3,14,7,0,107,117,
+        3,16,8,0,108,117,3,18,9,0,109,117,3,20,10,0,110,117,3,22,11,0,111,
+        117,3,24,12,0,112,117,3,26,13,0,113,117,3,28,14,0,114,117,3,30,15,
+        0,115,117,3,98,49,0,116,100,1,0,0,0,116,101,1,0,0,0,116,102,1,0,
+        0,0,116,103,1,0,0,0,116,104,1,0,0,0,116,105,1,0,0,0,116,106,1,0,
+        0,0,116,107,1,0,0,0,116,108,1,0,0,0,116,109,1,0,0,0,116,110,1,0,
+        0,0,116,111,1,0,0,0,116,112,1,0,0,0,116,113,1,0,0,0,116,114,1,0,
+        0,0,116,115,1,0,0,0,117,120,1,0,0,0,118,116,1,0,0,0,118,119,1,0,
+        0,0,119,121,1,0,0,0,120,118,1,0,0,0,121,122,5,0,0,1,122,1,1,0,0,
+        0,123,127,5,148,0,0,124,126,5,174,0,0,125,124,1,0,0,0,126,129,1,
+        0,0,0,127,125,1,0,0,0,127,128,1,0,0,0,128,130,1,0,0,0,129,127,1,
+        0,0,0,130,131,7,0,0,0,131,3,1,0,0,0,132,136,5,55,0,0,133,135,3,32,
+        16,0,134,133,1,0,0,0,135,138,1,0,0,0,136,134,1,0,0,0,136,137,1,0,
+        0,0,137,139,1,0,0,0,138,136,1,0,0,0,139,140,5,2,0,0,140,5,1,0,0,
+        0,141,145,5,57,0,0,142,144,3,36,18,0,143,142,1,0,0,0,144,147,1,0,
+        0,0,145,143,1,0,0,0,145,146,1,0,0,0,146,148,1,0,0,0,147,145,1,0,
+        0,0,148,149,5,2,0,0,149,7,1,0,0,0,150,159,5,3,0,0,151,155,5,21,0,
+        0,152,154,3,40,20,0,153,152,1,0,0,0,154,157,1,0,0,0,155,153,1,0,
+        0,0,155,156,1,0,0,0,156,160,1,0,0,0,157,155,1,0,0,0,158,160,5,26,
+        0,0,159,151,1,0,0,0,159,158,1,0,0,0,160,9,1,0,0,0,161,162,5,3,0,
+        0,162,166,5,4,0,0,163,165,3,44,22,0,164,163,1,0,0,0,165,168,1,0,
+        0,0,166,164,1,0,0,0,166,167,1,0,0,0,167,11,1,0,0,0,168,166,1,0,0,
+        0,169,170,5,3,0,0,170,174,5,27,0,0,171,173,3,54,27,0,172,171,1,0,
+        0,0,173,176,1,0,0,0,174,172,1,0,0,0,174,175,1,0,0,0,175,13,1,0,0,
+        0,176,174,1,0,0,0,177,178,5,3,0,0,178,182,5,32,0,0,179,181,3,56,
+        28,0,180,179,1,0,0,0,181,184,1,0,0,0,182,180,1,0,0,0,182,183,1,0,
+        0,0,183,15,1,0,0,0,184,182,1,0,0,0,185,186,5,3,0,0,186,190,5,34,
+        0,0,187,189,3,58,29,0,188,187,1,0,0,0,189,192,1,0,0,0,190,188,1,
+        0,0,0,190,191,1,0,0,0,191,17,1,0,0,0,192,190,1,0,0,0,193,194,5,3,
+        0,0,194,198,5,39,0,0,195,197,3,60,30,0,196,195,1,0,0,0,197,200,1,
+        0,0,0,198,196,1,0,0,0,198,199,1,0,0,0,199,19,1,0,0,0,200,198,1,0,
+        0,0,201,209,5,43,0,0,202,204,3,62,31,0,203,202,1,0,0,0,204,207,1,
+        0,0,0,205,203,1,0,0,0,205,206,1,0,0,0,206,210,1,0,0,0,207,205,1,
+        0,0,0,208,210,5,44,0,0,209,205,1,0,0,0,209,208,1,0,0,0,210,21,1,
+        0,0,0,211,215,5,87,0,0,212,214,3,68,34,0,213,212,1,0,0,0,214,217,
+        1,0,0,0,215,213,1,0,0,0,215,216,1,0,0,0,216,23,1,0,0,0,217,215,1,
+        0,0,0,218,222,5,94,0,0,219,221,3,70,35,0,220,219,1,0,0,0,221,224,
+        1,0,0,0,222,220,1,0,0,0,222,223,1,0,0,0,223,25,1,0,0,0,224,222,1,
+        0,0,0,225,226,5,3,0,0,226,235,5,102,0,0,227,229,3,72,36,0,228,227,
+        1,0,0,0,229,232,1,0,0,0,230,228,1,0,0,0,230,231,1,0,0,0,231,236,
+        1,0,0,0,232,230,1,0,0,0,233,236,5,105,0,0,234,236,5,8,0,0,235,230,
+        1,0,0,0,235,233,1,0,0,0,235,234,1,0,0,0,236,27,1,0,0,0,237,241,5,
+        108,0,0,238,240,3,80,40,0,239,238,1,0,0,0,240,243,1,0,0,0,241,239,
+        1,0,0,0,241,242,1,0,0,0,242,29,1,0,0,0,243,241,1,0,0,0,244,248,5,
+        113,0,0,245,247,3,82,41,0,246,245,1,0,0,0,247,250,1,0,0,0,248,246,
+        1,0,0,0,248,249,1,0,0,0,249,31,1,0,0,0,250,248,1,0,0,0,251,307,3,
+        34,17,0,252,307,5,56,0,0,253,254,5,59,0,0,254,307,3,96,48,0,255,
+        256,5,61,0,0,256,307,3,96,48,0,257,258,5,60,0,0,258,307,3,96,48,
+        0,259,260,5,62,0,0,260,307,3,96,48,0,261,262,5,63,0,0,262,307,3,
+        96,48,0,263,307,5,64,0,0,264,265,5,65,0,0,265,307,3,96,48,0,266,
+        267,5,66,0,0,267,307,3,96,48,0,268,307,5,67,0,0,269,270,5,68,0,0,
+        270,307,3,96,48,0,271,272,5,69,0,0,272,307,3,96,48,0,273,274,5,73,
+        0,0,274,275,5,74,0,0,275,276,5,144,0,0,276,277,5,75,0,0,277,278,
+        3,96,48,0,278,279,5,76,0,0,279,280,3,96,48,0,280,281,5,77,0,0,281,
+        282,3,96,48,0,282,307,1,0,0,0,283,284,5,78,0,0,284,307,5,144,0,0,
+        285,286,5,79,0,0,286,287,5,81,0,0,287,307,5,144,0,0,288,289,5,80,
+        0,0,289,290,5,81,0,0,290,292,5,144,0,0,291,293,5,83,0,0,292,291,
+        1,0,0,0,292,293,1,0,0,0,293,307,1,0,0,0,294,300,5,82,0,0,295,298,
+        5,83,0,0,296,297,5,84,0,0,297,299,3,96,48,0,298,296,1,0,0,0,298,
+        299,1,0,0,0,299,301,1,0,0,0,300,295,1,0,0,0,300,301,1,0,0,0,301,
+        307,1,0,0,0,302,303,5,85,0,0,303,307,3,96,48,0,304,305,5,86,0,0,
+        305,307,3,96,48,0,306,251,1,0,0,0,306,252,1,0,0,0,306,253,1,0,0,
+        0,306,255,1,0,0,0,306,257,1,0,0,0,306,259,1,0,0,0,306,261,1,0,0,
+        0,306,263,1,0,0,0,306,264,1,0,0,0,306,266,1,0,0,0,306,268,1,0,0,
+        0,306,269,1,0,0,0,306,271,1,0,0,0,306,273,1,0,0,0,306,283,1,0,0,
+        0,306,285,1,0,0,0,306,288,1,0,0,0,306,294,1,0,0,0,306,302,1,0,0,
+        0,306,304,1,0,0,0,307,33,1,0,0,0,308,309,5,58,0,0,309,310,3,84,42,
+        0,310,311,3,84,42,0,311,35,1,0,0,0,312,374,3,38,19,0,313,374,5,56,
+        0,0,314,315,5,59,0,0,315,374,3,96,48,0,316,317,5,61,0,0,317,374,
+        3,96,48,0,318,319,5,60,0,0,319,374,3,96,48,0,320,321,5,62,0,0,321,
+        374,3,96,48,0,322,323,5,63,0,0,323,374,3,96,48,0,324,325,5,70,0,
+        0,325,374,3,96,48,0,326,327,5,71,0,0,327,374,3,96,48,0,328,329,5,
+        72,0,0,329,374,3,96,48,0,330,374,5,64,0,0,331,332,5,65,0,0,332,374,
+        3,96,48,0,333,334,5,66,0,0,334,374,3,96,48,0,335,374,5,67,0,0,336,
+        337,5,68,0,0,337,374,3,96,48,0,338,339,5,69,0,0,339,374,3,96,48,
+        0,340,341,5,73,0,0,341,342,5,74,0,0,342,343,5,144,0,0,343,344,5,
+        75,0,0,344,345,3,96,48,0,345,346,5,76,0,0,346,347,3,96,48,0,347,
+        348,5,77,0,0,348,349,3,96,48,0,349,374,1,0,0,0,350,351,5,78,0,0,
+        351,374,5,144,0,0,352,353,5,79,0,0,353,354,5,81,0,0,354,374,5,144,
+        0,0,355,356,5,80,0,0,356,357,5,81,0,0,357,359,5,144,0,0,358,360,
+        5,83,0,0,359,358,1,0,0,0,359,360,1,0,0,0,360,374,1,0,0,0,361,367,
+        5,82,0,0,362,365,5,83,0,0,363,364,5,84,0,0,364,366,3,96,48,0,365,
+        363,1,0,0,0,365,366,1,0,0,0,366,368,1,0,0,0,367,362,1,0,0,0,367,
+        368,1,0,0,0,368,374,1,0,0,0,369,370,5,85,0,0,370,374,3,96,48,0,371,
+        372,5,86,0,0,372,374,3,96,48,0,373,312,1,0,0,0,373,313,1,0,0,0,373,
+        314,1,0,0,0,373,316,1,0,0,0,373,318,1,0,0,0,373,320,1,0,0,0,373,
+        322,1,0,0,0,373,324,1,0,0,0,373,326,1,0,0,0,373,328,1,0,0,0,373,
+        330,1,0,0,0,373,331,1,0,0,0,373,333,1,0,0,0,373,335,1,0,0,0,373,
+        336,1,0,0,0,373,338,1,0,0,0,373,340,1,0,0,0,373,350,1,0,0,0,373,
+        352,1,0,0,0,373,355,1,0,0,0,373,361,1,0,0,0,373,369,1,0,0,0,373,
+        371,1,0,0,0,374,37,1,0,0,0,375,376,5,58,0,0,376,377,3,84,42,0,377,
+        39,1,0,0,0,378,390,3,42,21,0,379,380,5,9,0,0,380,390,3,96,48,0,381,
+        382,5,23,0,0,382,390,3,96,48,0,383,384,5,24,0,0,384,390,5,144,0,
+        0,385,390,5,19,0,0,386,387,5,25,0,0,387,390,3,96,48,0,388,390,5,
+        18,0,0,389,378,1,0,0,0,389,379,1,0,0,0,389,381,1,0,0,0,389,383,1,
+        0,0,0,389,385,1,0,0,0,389,386,1,0,0,0,389,388,1,0,0,0,390,41,1,0,
+        0,0,391,392,3,84,42,0,392,393,3,84,42,0,393,394,3,84,42,0,394,395,
+        3,84,42,0,395,430,1,0,0,0,396,397,5,22,0,0,397,398,5,144,0,0,398,
+        399,5,144,0,0,399,400,5,144,0,0,400,430,5,144,0,0,401,402,5,144,
+        0,0,402,403,5,149,0,0,403,404,5,144,0,0,404,405,5,149,0,0,405,406,
+        5,144,0,0,406,407,5,149,0,0,407,408,5,144,0,0,408,430,5,149,0,0,
+        409,411,5,149,0,0,410,409,1,0,0,0,410,411,1,0,0,0,411,412,1,0,0,
+        0,412,413,5,144,0,0,413,415,5,149,0,0,414,416,5,149,0,0,415,414,
+        1,0,0,0,415,416,1,0,0,0,416,417,1,0,0,0,417,418,5,144,0,0,418,420,
+        5,149,0,0,419,421,5,149,0,0,420,419,1,0,0,0,420,421,1,0,0,0,421,
+        422,1,0,0,0,422,423,5,144,0,0,423,425,5,149,0,0,424,426,5,149,0,
+        0,425,424,1,0,0,0,425,426,1,0,0,0,426,427,1,0,0,0,427,428,5,144,
+        0,0,428,430,5,149,0,0,429,391,1,0,0,0,429,396,1,0,0,0,429,401,1,
+        0,0,0,429,410,1,0,0,0,430,43,1,0,0,0,431,433,5,5,0,0,432,431,1,0,
+        0,0,432,433,1,0,0,0,433,437,1,0,0,0,434,436,3,46,23,0,435,434,1,
+        0,0,0,436,439,1,0,0,0,437,435,1,0,0,0,437,438,1,0,0,0,438,443,1,
+        0,0,0,439,437,1,0,0,0,440,442,3,48,24,0,441,440,1,0,0,0,442,445,
+        1,0,0,0,443,441,1,0,0,0,443,444,1,0,0,0,444,446,1,0,0,0,445,443,
+        1,0,0,0,446,450,3,84,42,0,447,449,3,48,24,0,448,447,1,0,0,0,449,
+        452,1,0,0,0,450,448,1,0,0,0,450,451,1,0,0,0,451,454,1,0,0,0,452,
+        450,1,0,0,0,453,455,3,52,26,0,454,453,1,0,0,0,454,455,1,0,0,0,455,
+        490,1,0,0,0,456,458,5,6,0,0,457,459,3,50,25,0,458,457,1,0,0,0,458,
+        459,1,0,0,0,459,463,1,0,0,0,460,462,3,48,24,0,461,460,1,0,0,0,462,
+        465,1,0,0,0,463,461,1,0,0,0,463,464,1,0,0,0,464,467,1,0,0,0,465,
+        463,1,0,0,0,466,468,3,52,26,0,467,466,1,0,0,0,467,468,1,0,0,0,468,
+        490,1,0,0,0,469,471,5,7,0,0,470,472,3,50,25,0,471,470,1,0,0,0,471,
+        472,1,0,0,0,472,476,1,0,0,0,473,475,3,48,24,0,474,473,1,0,0,0,475,
+        478,1,0,0,0,476,474,1,0,0,0,476,477,1,0,0,0,477,479,1,0,0,0,478,
+        476,1,0,0,0,479,483,3,84,42,0,480,482,3,48,24,0,481,480,1,0,0,0,
+        482,485,1,0,0,0,483,481,1,0,0,0,483,484,1,0,0,0,484,486,1,0,0,0,
+        485,483,1,0,0,0,486,487,3,84,42,0,487,490,1,0,0,0,488,490,5,8,0,
+        0,489,432,1,0,0,0,489,456,1,0,0,0,489,469,1,0,0,0,489,488,1,0,0,
+        0,490,45,1,0,0,0,491,492,5,12,0,0,492,500,5,144,0,0,493,494,5,13,
+        0,0,494,500,3,92,46,0,495,496,5,14,0,0,496,500,3,92,46,0,497,498,
+        5,15,0,0,498,500,3,92,46,0,499,491,1,0,0,0,499,493,1,0,0,0,499,495,
+        1,0,0,0,499,497,1,0,0,0,500,47,1,0,0,0,501,502,5,9,0,0,502,506,3,
+        92,46,0,503,506,5,10,0,0,504,506,5,11,0,0,505,501,1,0,0,0,505,503,
+        1,0,0,0,505,504,1,0,0,0,506,49,1,0,0,0,507,508,7,1,0,0,508,51,1,
+        0,0,0,509,510,7,2,0,0,510,53,1,0,0,0,511,512,5,28,0,0,512,515,3,
+        92,46,0,513,514,5,12,0,0,514,516,5,144,0,0,515,513,1,0,0,0,515,516,
+        1,0,0,0,516,518,1,0,0,0,517,519,5,29,0,0,518,517,1,0,0,0,518,519,
+        1,0,0,0,519,527,1,0,0,0,520,521,5,30,0,0,521,527,3,92,46,0,522,523,
+        5,21,0,0,523,527,3,92,46,0,524,525,5,31,0,0,525,527,3,92,46,0,526,
+        511,1,0,0,0,526,520,1,0,0,0,526,522,1,0,0,0,526,524,1,0,0,0,527,
+        55,1,0,0,0,528,529,5,9,0,0,529,534,3,92,46,0,530,531,5,12,0,0,531,
+        534,5,144,0,0,532,534,5,33,0,0,533,528,1,0,0,0,533,530,1,0,0,0,533,
+        532,1,0,0,0,534,57,1,0,0,0,535,537,3,84,42,0,536,538,5,35,0,0,537,
+        536,1,0,0,0,537,538,1,0,0,0,538,540,1,0,0,0,539,541,5,28,0,0,540,
+        539,1,0,0,0,540,541,1,0,0,0,541,543,1,0,0,0,542,544,5,36,0,0,543,
+        542,1,0,0,0,543,544,1,0,0,0,544,546,1,0,0,0,545,547,5,37,0,0,546,
+        545,1,0,0,0,546,547,1,0,0,0,547,549,1,0,0,0,548,550,5,38,0,0,549,
+        548,1,0,0,0,549,550,1,0,0,0,550,59,1,0,0,0,551,552,5,9,0,0,552,554,
+        3,92,46,0,553,555,5,11,0,0,554,553,1,0,0,0,554,555,1,0,0,0,555,556,
+        1,0,0,0,556,557,5,40,0,0,557,558,3,92,46,0,558,559,5,41,0,0,559,
+        560,3,92,46,0,560,561,5,42,0,0,561,562,3,92,46,0,562,563,3,84,42,
+        0,563,61,1,0,0,0,564,565,3,84,42,0,565,566,3,84,42,0,566,567,3,64,
+        32,0,567,571,1,0,0,0,568,571,3,66,33,0,569,571,5,45,0,0,570,564,
+        1,0,0,0,570,568,1,0,0,0,570,569,1,0,0,0,571,63,1,0,0,0,572,578,7,
+        3,0,0,573,575,5,18,0,0,574,573,1,0,0,0,574,575,1,0,0,0,575,579,1,
+        0,0,0,576,579,5,19,0,0,577,579,5,50,0,0,578,574,1,0,0,0,578,576,
+        1,0,0,0,578,577,1,0,0,0,579,582,1,0,0,0,580,581,5,47,0,0,581,583,
+        3,92,46,0,582,580,1,0,0,0,582,583,1,0,0,0,583,586,1,0,0,0,584,585,
+        5,48,0,0,585,587,5,144,0,0,586,584,1,0,0,0,586,587,1,0,0,0,587,590,
+        1,0,0,0,588,589,5,51,0,0,589,591,3,92,46,0,590,588,1,0,0,0,590,591,
         1,0,0,0,591,65,1,0,0,0,592,595,5,52,0,0,593,594,5,53,0,0,594,596,
         5,149,0,0,595,593,1,0,0,0,595,596,1,0,0,0,596,599,1,0,0,0,597,599,
         5,54,0,0,598,592,1,0,0,0,598,597,1,0,0,0,599,67,1,0,0,0,600,611,
-        5,56,0,0,601,602,7,3,0,0,602,611,3,92,46,0,603,604,7,4,0,0,604,611,
+        5,56,0,0,601,602,7,4,0,0,602,611,3,92,46,0,603,604,7,5,0,0,604,611,
         5,144,0,0,605,611,5,92,0,0,606,611,5,93,0,0,607,608,3,84,42,0,608,
         609,3,84,42,0,609,611,1,0,0,0,610,600,1,0,0,0,610,601,1,0,0,0,610,
         603,1,0,0,0,610,605,1,0,0,0,610,606,1,0,0,0,610,607,1,0,0,0,611,
-        69,1,0,0,0,612,613,5,9,0,0,613,623,3,92,46,0,614,615,7,5,0,0,615,
+        69,1,0,0,0,612,613,5,9,0,0,613,623,3,92,46,0,614,615,7,6,0,0,615,
         623,3,92,46,0,616,623,5,44,0,0,617,623,5,99,0,0,618,619,5,100,0,
         0,619,623,5,144,0,0,620,623,5,11,0,0,621,623,3,84,42,0,622,612,1,
         0,0,0,622,614,1,0,0,0,622,616,1,0,0,0,622,617,1,0,0,0,622,618,1,
         0,0,0,622,620,1,0,0,0,622,621,1,0,0,0,623,71,1,0,0,0,624,633,5,7,
         0,0,625,626,5,103,0,0,626,633,5,144,0,0,627,633,5,104,0,0,628,633,
         3,74,37,0,629,633,3,76,38,0,630,633,3,78,39,0,631,633,3,84,42,0,
         632,624,1,0,0,0,632,625,1,0,0,0,632,627,1,0,0,0,632,628,1,0,0,0,
         632,629,1,0,0,0,632,630,1,0,0,0,632,631,1,0,0,0,633,73,1,0,0,0,634,
-        635,7,0,0,0,635,75,1,0,0,0,636,637,5,9,0,0,637,644,3,92,46,0,638,
+        635,7,1,0,0,635,75,1,0,0,0,636,637,5,9,0,0,637,644,3,92,46,0,638,
         644,5,10,0,0,639,640,5,106,0,0,640,644,3,92,46,0,641,642,5,107,0,
         0,642,644,3,92,46,0,643,636,1,0,0,0,643,638,1,0,0,0,643,639,1,0,
-        0,0,643,641,1,0,0,0,644,77,1,0,0,0,645,646,7,6,0,0,646,79,1,0,0,
-        0,647,657,5,56,0,0,648,649,7,7,0,0,649,657,3,92,46,0,650,657,5,102,
-        0,0,651,657,5,19,0,0,652,657,5,110,0,0,653,654,7,8,0,0,654,657,5,
+        0,0,643,641,1,0,0,0,644,77,1,0,0,0,645,646,7,7,0,0,646,79,1,0,0,
+        0,647,657,5,56,0,0,648,649,7,8,0,0,649,657,3,92,46,0,650,657,5,102,
+        0,0,651,657,5,19,0,0,652,657,5,110,0,0,653,654,7,9,0,0,654,657,5,
         144,0,0,655,657,3,84,42,0,656,647,1,0,0,0,656,648,1,0,0,0,656,650,
         1,0,0,0,656,651,1,0,0,0,656,652,1,0,0,0,656,653,1,0,0,0,656,655,
-        1,0,0,0,657,81,1,0,0,0,658,659,7,9,0,0,659,664,3,92,46,0,660,661,
-        7,10,0,0,661,664,5,144,0,0,662,664,3,84,42,0,663,658,1,0,0,0,663,
+        1,0,0,0,657,81,1,0,0,0,658,659,7,10,0,0,659,664,3,92,46,0,660,661,
+        7,11,0,0,661,664,5,144,0,0,662,664,3,84,42,0,663,658,1,0,0,0,663,
         660,1,0,0,0,663,662,1,0,0,0,664,83,1,0,0,0,665,666,5,116,0,0,666,
         668,3,86,43,0,667,669,5,105,0,0,668,667,1,0,0,0,668,669,1,0,0,0,
         669,670,1,0,0,0,670,671,5,2,0,0,671,85,1,0,0,0,672,677,3,88,44,0,
         673,674,5,117,0,0,674,676,3,88,44,0,675,673,1,0,0,0,676,679,1,0,
         0,0,677,675,1,0,0,0,677,678,1,0,0,0,678,87,1,0,0,0,679,677,1,0,0,
         0,680,685,3,90,45,0,681,682,5,118,0,0,682,684,3,90,45,0,683,681,
         1,0,0,0,684,687,1,0,0,0,685,683,1,0,0,0,685,686,1,0,0,0,686,89,1,
         0,0,0,687,685,1,0,0,0,688,689,6,45,-1,0,689,690,5,152,0,0,690,691,
         3,86,43,0,691,692,5,153,0,0,692,792,1,0,0,0,693,792,5,142,0,0,694,
-        695,5,133,0,0,695,696,7,11,0,0,696,697,7,12,0,0,697,792,7,11,0,0,
+        695,5,133,0,0,695,696,7,12,0,0,696,697,7,13,0,0,697,792,7,12,0,0,
         698,700,5,134,0,0,699,701,5,177,0,0,700,699,1,0,0,0,700,701,1,0,
         0,0,701,702,1,0,0,0,702,703,5,178,0,0,703,704,5,179,0,0,704,792,
         3,94,47,0,705,706,5,122,0,0,706,792,3,90,45,18,707,708,5,124,0,0,
         708,792,3,90,45,17,709,710,5,123,0,0,710,792,3,90,45,16,711,719,
         5,131,0,0,712,720,5,150,0,0,713,716,5,149,0,0,714,715,5,154,0,0,
         715,717,5,149,0,0,716,714,1,0,0,0,716,717,1,0,0,0,717,720,1,0,0,
         0,718,720,5,162,0,0,719,712,1,0,0,0,719,713,1,0,0,0,719,718,1,0,
@@ -307,43 +307,43 @@
         727,1,0,0,0,727,730,1,0,0,0,728,730,5,162,0,0,729,722,1,0,0,0,729,
         723,1,0,0,0,729,728,1,0,0,0,730,792,1,0,0,0,731,792,5,136,0,0,732,
         792,5,137,0,0,733,792,5,138,0,0,734,792,5,143,0,0,735,736,5,119,
         0,0,736,792,3,90,45,9,737,738,5,135,0,0,738,739,3,94,47,0,739,740,
         3,94,47,0,740,743,3,94,47,0,741,742,5,84,0,0,742,744,3,94,47,0,743,
         741,1,0,0,0,743,744,1,0,0,0,744,746,1,0,0,0,745,747,5,24,0,0,746,
         745,1,0,0,0,746,747,1,0,0,0,747,792,1,0,0,0,748,792,5,139,0,0,749,
-        792,5,140,0,0,750,751,5,141,0,0,751,792,5,144,0,0,752,760,7,13,0,
+        792,5,140,0,0,750,751,5,141,0,0,751,792,5,144,0,0,752,760,7,14,0,
         0,753,761,5,151,0,0,754,757,5,144,0,0,755,756,5,154,0,0,756,758,
         5,144,0,0,757,755,1,0,0,0,757,758,1,0,0,0,758,761,1,0,0,0,759,761,
         5,162,0,0,760,753,1,0,0,0,760,754,1,0,0,0,760,759,1,0,0,0,761,792,
         1,0,0,0,762,770,5,129,0,0,763,771,5,150,0,0,764,767,5,149,0,0,765,
         766,5,154,0,0,766,768,5,149,0,0,767,765,1,0,0,0,767,768,1,0,0,0,
         768,771,1,0,0,0,769,771,5,162,0,0,770,763,1,0,0,0,770,764,1,0,0,
         0,770,769,1,0,0,0,771,792,1,0,0,0,772,785,5,125,0,0,773,786,5,150,
         0,0,774,777,5,149,0,0,775,776,5,154,0,0,776,778,5,149,0,0,777,775,
         1,0,0,0,777,778,1,0,0,0,778,786,1,0,0,0,779,782,5,146,0,0,780,781,
         5,154,0,0,781,783,5,146,0,0,782,780,1,0,0,0,782,783,1,0,0,0,783,
         786,1,0,0,0,784,786,5,162,0,0,785,773,1,0,0,0,785,774,1,0,0,0,785,
-        779,1,0,0,0,785,784,1,0,0,0,786,792,1,0,0,0,787,788,7,14,0,0,788,
+        779,1,0,0,0,785,784,1,0,0,0,786,792,1,0,0,0,787,788,7,15,0,0,788,
         789,5,144,0,0,789,790,5,154,0,0,790,792,5,144,0,0,791,688,1,0,0,
         0,791,693,1,0,0,0,791,694,1,0,0,0,791,698,1,0,0,0,791,705,1,0,0,
         0,791,707,1,0,0,0,791,709,1,0,0,0,791,711,1,0,0,0,791,721,1,0,0,
         0,791,731,1,0,0,0,791,732,1,0,0,0,791,733,1,0,0,0,791,734,1,0,0,
         0,791,735,1,0,0,0,791,737,1,0,0,0,791,748,1,0,0,0,791,749,1,0,0,
         0,791,750,1,0,0,0,791,752,1,0,0,0,791,762,1,0,0,0,791,772,1,0,0,
         0,791,787,1,0,0,0,792,809,1,0,0,0,793,794,10,22,0,0,794,795,5,120,
         0,0,795,808,3,94,47,0,796,797,10,21,0,0,797,805,5,121,0,0,798,806,
         5,151,0,0,799,802,5,144,0,0,800,801,5,154,0,0,801,803,5,144,0,0,
         802,800,1,0,0,0,802,803,1,0,0,0,803,806,1,0,0,0,804,806,5,162,0,
         0,805,798,1,0,0,0,805,799,1,0,0,0,805,804,1,0,0,0,806,808,1,0,0,
         0,807,793,1,0,0,0,807,796,1,0,0,0,808,811,1,0,0,0,809,807,1,0,0,
-        0,809,810,1,0,0,0,810,91,1,0,0,0,811,809,1,0,0,0,812,813,7,15,0,
-        0,813,93,1,0,0,0,814,815,7,16,0,0,815,95,1,0,0,0,816,817,7,15,0,
+        0,809,810,1,0,0,0,810,91,1,0,0,0,811,809,1,0,0,0,812,813,7,16,0,
+        0,813,93,1,0,0,0,814,815,7,17,0,0,815,95,1,0,0,0,816,817,7,16,0,
         0,817,97,1,0,0,0,818,819,5,1,0,0,819,821,5,171,0,0,820,822,5,168,
-        0,0,821,820,1,0,0,0,821,822,1,0,0,0,822,823,1,0,0,0,823,824,7,17,
+        0,0,821,820,1,0,0,0,821,822,1,0,0,0,822,823,1,0,0,0,823,824,7,18,
         0,0,824,825,5,173,0,0,825,99,1,0,0,0,95,116,118,127,136,145,155,
         159,166,174,182,190,198,205,209,215,222,230,235,241,248,292,298,
         300,306,359,365,367,373,389,410,415,420,425,429,432,437,443,450,
         454,458,463,467,471,476,483,489,499,505,515,518,526,533,537,540,
         543,546,549,554,570,574,578,582,586,590,595,598,610,622,632,643,
         656,663,668,677,685,700,716,719,726,729,743,746,757,760,767,770,
         777,782,785,791,802,805,807,809,821
@@ -946,14 +946,17 @@
 
         def COMMENT(self):
             return self.getToken(CharmmMRParser.COMMENT, 0)
 
         def RETURN_CM(self):
             return self.getToken(CharmmMRParser.RETURN_CM, 0)
 
+        def EOF(self):
+            return self.getToken(CharmmMRParser.EOF, 0)
+
         def Any_name(self, i:int=None):
             if i is None:
                 return self.getTokens(CharmmMRParser.Any_name)
             else:
                 return self.getToken(CharmmMRParser.Any_name, i)
 
         def getRuleIndex(self):
@@ -986,15 +989,20 @@
                 self.state = 124
                 self.match(CharmmMRParser.Any_name)
                 self.state = 129
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
             self.state = 130
-            self.match(CharmmMRParser.RETURN_CM)
+            _la = self._input.LA(1)
+            if not(_la==-1 or _la==176):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
```

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CharmmMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CharmmMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CnsMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CnsMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CnsMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CnsMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CyanaMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CyanaMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,192 +62,192 @@
         1,43,1,43,1,43,1,44,1,44,1,44,3,44,583,8,44,1,44,1,44,4,44,587,8,
         44,11,44,12,44,588,1,45,1,45,1,45,1,45,4,45,595,8,45,11,45,12,45,
         596,1,45,1,45,1,46,1,46,1,46,3,46,604,8,46,1,46,1,46,4,46,608,8,
         46,11,46,12,46,609,1,47,1,47,1,47,1,47,1,47,4,47,617,8,47,11,47,
         12,47,618,1,47,1,47,1,48,1,48,1,49,1,49,1,49,0,0,50,0,2,4,6,8,10,
         12,14,16,18,20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,
         56,58,60,62,64,66,68,70,72,74,76,78,80,82,84,86,88,90,92,94,96,98,
-        0,4,1,0,8,9,2,0,51,51,53,53,1,0,2,3,2,0,1,1,25,25,683,0,131,1,0,
-        0,0,2,136,1,0,0,0,4,146,1,0,0,0,6,150,1,0,0,0,8,173,1,0,0,0,10,177,
-        1,0,0,0,12,194,1,0,0,0,14,209,1,0,0,0,16,217,1,0,0,0,18,234,1,0,
-        0,0,20,249,1,0,0,0,22,257,1,0,0,0,24,269,1,0,0,0,26,273,1,0,0,0,
-        28,289,1,0,0,0,30,293,1,0,0,0,32,311,1,0,0,0,34,315,1,0,0,0,36,334,
-        1,0,0,0,38,338,1,0,0,0,40,354,1,0,0,0,42,358,1,0,0,0,44,376,1,0,
-        0,0,46,380,1,0,0,0,48,399,1,0,0,0,50,403,1,0,0,0,52,413,1,0,0,0,
-        54,417,1,0,0,0,56,433,1,0,0,0,58,437,1,0,0,0,60,453,1,0,0,0,62,457,
-        1,0,0,0,64,473,1,0,0,0,66,477,1,0,0,0,68,495,1,0,0,0,70,499,1,0,
-        0,0,72,519,1,0,0,0,74,522,1,0,0,0,76,545,1,0,0,0,78,551,1,0,0,0,
-        80,555,1,0,0,0,82,564,1,0,0,0,84,566,1,0,0,0,86,575,1,0,0,0,88,579,
-        1,0,0,0,90,590,1,0,0,0,92,600,1,0,0,0,94,611,1,0,0,0,96,622,1,0,
-        0,0,98,624,1,0,0,0,100,130,5,4,0,0,101,130,5,5,0,0,102,130,3,2,1,
-        0,103,130,3,4,2,0,104,130,3,24,12,0,105,130,3,28,14,0,106,130,3,
-        32,16,0,107,130,3,36,18,0,108,130,3,40,20,0,109,130,3,44,22,0,110,
-        130,3,48,24,0,111,130,3,52,26,0,112,130,3,56,28,0,113,130,3,60,30,
-        0,114,130,3,8,4,0,115,130,3,64,32,0,116,130,3,12,6,0,117,130,3,18,
-        9,0,118,130,3,68,34,0,119,130,3,72,36,0,120,130,3,74,37,0,121,130,
-        3,76,38,0,122,130,3,78,39,0,123,130,3,80,40,0,124,130,3,82,41,0,
-        125,130,3,84,42,0,126,130,3,86,43,0,127,130,3,88,44,0,128,130,3,
-        92,46,0,129,100,1,0,0,0,129,101,1,0,0,0,129,102,1,0,0,0,129,103,
-        1,0,0,0,129,104,1,0,0,0,129,105,1,0,0,0,129,106,1,0,0,0,129,107,
-        1,0,0,0,129,108,1,0,0,0,129,109,1,0,0,0,129,110,1,0,0,0,129,111,
-        1,0,0,0,129,112,1,0,0,0,129,113,1,0,0,0,129,114,1,0,0,0,129,115,
-        1,0,0,0,129,116,1,0,0,0,129,117,1,0,0,0,129,118,1,0,0,0,129,119,
-        1,0,0,0,129,120,1,0,0,0,129,121,1,0,0,0,129,122,1,0,0,0,129,123,
-        1,0,0,0,129,124,1,0,0,0,129,125,1,0,0,0,129,126,1,0,0,0,129,127,
-        1,0,0,0,129,128,1,0,0,0,130,133,1,0,0,0,131,129,1,0,0,0,131,132,
-        1,0,0,0,132,134,1,0,0,0,133,131,1,0,0,0,134,135,5,0,0,1,135,1,1,
-        0,0,0,136,140,5,7,0,0,137,139,5,30,0,0,138,137,1,0,0,0,139,142,1,
-        0,0,0,140,138,1,0,0,0,140,141,1,0,0,0,141,143,1,0,0,0,142,140,1,
-        0,0,0,143,144,5,32,0,0,144,3,1,0,0,0,145,147,3,6,3,0,146,145,1,0,
-        0,0,147,148,1,0,0,0,148,146,1,0,0,0,148,149,1,0,0,0,149,5,1,0,0,
-        0,150,151,5,2,0,0,151,152,5,25,0,0,152,153,3,98,49,0,153,154,5,2,
-        0,0,154,155,5,25,0,0,155,156,3,98,49,0,156,158,3,96,48,0,157,159,
-        3,96,48,0,158,157,1,0,0,0,158,159,1,0,0,0,159,161,1,0,0,0,160,162,
-        3,96,48,0,161,160,1,0,0,0,161,162,1,0,0,0,162,164,1,0,0,0,163,165,
-        3,96,48,0,164,163,1,0,0,0,164,165,1,0,0,0,165,167,1,0,0,0,166,168,
-        3,96,48,0,167,166,1,0,0,0,167,168,1,0,0,0,168,170,1,0,0,0,169,171,
-        3,96,48,0,170,169,1,0,0,0,170,171,1,0,0,0,171,7,1,0,0,0,172,174,
-        3,10,5,0,173,172,1,0,0,0,174,175,1,0,0,0,175,173,1,0,0,0,175,176,
-        1,0,0,0,176,9,1,0,0,0,177,178,5,2,0,0,178,179,5,25,0,0,179,180,5,
-        25,0,0,180,181,3,96,48,0,181,183,3,96,48,0,182,184,3,96,48,0,183,
-        182,1,0,0,0,183,184,1,0,0,0,184,188,1,0,0,0,185,186,5,10,0,0,186,
-        187,5,11,0,0,187,189,5,2,0,0,188,185,1,0,0,0,188,189,1,0,0,0,189,
-        191,1,0,0,0,190,192,5,12,0,0,191,190,1,0,0,0,191,192,1,0,0,0,192,
-        11,1,0,0,0,193,195,3,14,7,0,194,193,1,0,0,0,195,196,1,0,0,0,196,
-        194,1,0,0,0,196,197,1,0,0,0,197,201,1,0,0,0,198,200,3,2,1,0,199,
-        198,1,0,0,0,200,203,1,0,0,0,201,199,1,0,0,0,201,202,1,0,0,0,202,
-        205,1,0,0,0,203,201,1,0,0,0,204,206,3,16,8,0,205,204,1,0,0,0,206,
-        207,1,0,0,0,207,205,1,0,0,0,207,208,1,0,0,0,208,13,1,0,0,0,209,210,
-        5,2,0,0,210,211,3,96,48,0,211,212,3,96,48,0,212,213,5,2,0,0,213,
-        15,1,0,0,0,214,216,3,2,1,0,215,214,1,0,0,0,216,219,1,0,0,0,217,215,
-        1,0,0,0,217,218,1,0,0,0,218,220,1,0,0,0,219,217,1,0,0,0,220,221,
-        5,2,0,0,221,222,5,25,0,0,222,223,5,25,0,0,223,224,5,2,0,0,224,225,
-        5,25,0,0,225,226,5,25,0,0,226,227,3,96,48,0,227,228,3,96,48,0,228,
-        229,3,96,48,0,229,231,5,2,0,0,230,232,3,96,48,0,231,230,1,0,0,0,
-        231,232,1,0,0,0,232,17,1,0,0,0,233,235,3,20,10,0,234,233,1,0,0,0,
-        235,236,1,0,0,0,236,234,1,0,0,0,236,237,1,0,0,0,237,241,1,0,0,0,
-        238,240,3,2,1,0,239,238,1,0,0,0,240,243,1,0,0,0,241,239,1,0,0,0,
-        241,242,1,0,0,0,242,245,1,0,0,0,243,241,1,0,0,0,244,246,3,22,11,
-        0,245,244,1,0,0,0,246,247,1,0,0,0,247,245,1,0,0,0,247,248,1,0,0,
-        0,248,19,1,0,0,0,249,250,5,2,0,0,250,251,3,96,48,0,251,252,3,96,
-        48,0,252,253,5,2,0,0,253,21,1,0,0,0,254,256,3,2,1,0,255,254,1,0,
-        0,0,256,259,1,0,0,0,257,255,1,0,0,0,257,258,1,0,0,0,258,260,1,0,
-        0,0,259,257,1,0,0,0,260,261,5,2,0,0,261,262,5,25,0,0,262,263,5,25,
-        0,0,263,264,3,96,48,0,264,265,3,96,48,0,265,266,3,96,48,0,266,267,
-        5,2,0,0,267,23,1,0,0,0,268,270,3,26,13,0,269,268,1,0,0,0,270,271,
-        1,0,0,0,271,269,1,0,0,0,271,272,1,0,0,0,272,25,1,0,0,0,273,274,5,
-        2,0,0,274,276,5,25,0,0,275,277,3,2,1,0,276,275,1,0,0,0,276,277,1,
-        0,0,0,277,284,1,0,0,0,278,279,5,25,0,0,279,280,5,2,0,0,280,281,5,
-        25,0,0,281,282,5,25,0,0,282,285,3,96,48,0,283,285,3,2,1,0,284,278,
-        1,0,0,0,284,283,1,0,0,0,285,286,1,0,0,0,286,284,1,0,0,0,286,287,
-        1,0,0,0,287,27,1,0,0,0,288,290,3,30,15,0,289,288,1,0,0,0,290,291,
-        1,0,0,0,291,289,1,0,0,0,291,292,1,0,0,0,292,29,1,0,0,0,293,294,5,
-        2,0,0,294,296,5,25,0,0,295,297,3,2,1,0,296,295,1,0,0,0,296,297,1,
-        0,0,0,297,306,1,0,0,0,298,299,5,25,0,0,299,300,5,2,0,0,300,301,5,
-        25,0,0,301,302,5,25,0,0,302,303,3,96,48,0,303,304,3,96,48,0,304,
-        307,1,0,0,0,305,307,3,2,1,0,306,298,1,0,0,0,306,305,1,0,0,0,307,
-        308,1,0,0,0,308,306,1,0,0,0,308,309,1,0,0,0,309,31,1,0,0,0,310,312,
-        3,34,17,0,311,310,1,0,0,0,312,313,1,0,0,0,313,311,1,0,0,0,313,314,
-        1,0,0,0,314,33,1,0,0,0,315,316,5,2,0,0,316,318,5,25,0,0,317,319,
-        3,2,1,0,318,317,1,0,0,0,318,319,1,0,0,0,319,329,1,0,0,0,320,321,
-        5,25,0,0,321,322,5,2,0,0,322,323,5,25,0,0,323,324,5,25,0,0,324,325,
-        3,96,48,0,325,326,3,96,48,0,326,327,3,96,48,0,327,330,1,0,0,0,328,
-        330,3,2,1,0,329,320,1,0,0,0,329,328,1,0,0,0,330,331,1,0,0,0,331,
-        329,1,0,0,0,331,332,1,0,0,0,332,35,1,0,0,0,333,335,3,38,19,0,334,
-        333,1,0,0,0,335,336,1,0,0,0,336,334,1,0,0,0,336,337,1,0,0,0,337,
-        37,1,0,0,0,338,339,5,2,0,0,339,340,5,25,0,0,340,342,5,25,0,0,341,
-        343,3,2,1,0,342,341,1,0,0,0,342,343,1,0,0,0,343,349,1,0,0,0,344,
-        345,5,2,0,0,345,346,5,25,0,0,346,347,5,25,0,0,347,350,3,96,48,0,
-        348,350,3,2,1,0,349,344,1,0,0,0,349,348,1,0,0,0,350,351,1,0,0,0,
-        351,349,1,0,0,0,351,352,1,0,0,0,352,39,1,0,0,0,353,355,3,42,21,0,
-        354,353,1,0,0,0,355,356,1,0,0,0,356,354,1,0,0,0,356,357,1,0,0,0,
-        357,41,1,0,0,0,358,359,5,2,0,0,359,360,5,25,0,0,360,362,5,25,0,0,
-        361,363,3,2,1,0,362,361,1,0,0,0,362,363,1,0,0,0,363,371,1,0,0,0,
-        364,365,5,2,0,0,365,366,5,25,0,0,366,367,5,25,0,0,367,368,3,96,48,
-        0,368,369,3,96,48,0,369,372,1,0,0,0,370,372,3,2,1,0,371,364,1,0,
-        0,0,371,370,1,0,0,0,372,373,1,0,0,0,373,371,1,0,0,0,373,374,1,0,
-        0,0,374,43,1,0,0,0,375,377,3,46,23,0,376,375,1,0,0,0,377,378,1,0,
-        0,0,378,376,1,0,0,0,378,379,1,0,0,0,379,45,1,0,0,0,380,381,5,2,0,
-        0,381,382,5,25,0,0,382,384,5,25,0,0,383,385,3,2,1,0,384,383,1,0,
-        0,0,384,385,1,0,0,0,385,394,1,0,0,0,386,387,5,2,0,0,387,388,5,25,
-        0,0,388,389,5,25,0,0,389,390,3,96,48,0,390,391,3,96,48,0,391,392,
-        3,96,48,0,392,395,1,0,0,0,393,395,3,2,1,0,394,386,1,0,0,0,394,393,
-        1,0,0,0,395,396,1,0,0,0,396,394,1,0,0,0,396,397,1,0,0,0,397,47,1,
-        0,0,0,398,400,3,50,25,0,399,398,1,0,0,0,400,401,1,0,0,0,401,399,
-        1,0,0,0,401,402,1,0,0,0,402,49,1,0,0,0,403,404,7,0,0,0,404,405,5,
-        25,0,0,405,406,5,2,0,0,406,407,5,25,0,0,407,408,5,25,0,0,408,409,
-        5,2,0,0,409,410,5,25,0,0,410,411,3,96,48,0,411,51,1,0,0,0,412,414,
-        3,54,27,0,413,412,1,0,0,0,414,415,1,0,0,0,415,413,1,0,0,0,415,416,
-        1,0,0,0,416,53,1,0,0,0,417,418,5,2,0,0,418,419,5,25,0,0,419,420,
-        5,25,0,0,420,421,5,25,0,0,421,422,5,2,0,0,422,423,5,25,0,0,423,424,
-        5,25,0,0,424,425,5,25,0,0,425,427,3,96,48,0,426,428,3,96,48,0,427,
-        426,1,0,0,0,427,428,1,0,0,0,428,430,1,0,0,0,429,431,3,96,48,0,430,
-        429,1,0,0,0,430,431,1,0,0,0,431,55,1,0,0,0,432,434,3,58,29,0,433,
-        432,1,0,0,0,434,435,1,0,0,0,435,433,1,0,0,0,435,436,1,0,0,0,436,
-        57,1,0,0,0,437,438,5,25,0,0,438,439,5,2,0,0,439,440,5,25,0,0,440,
-        441,5,25,0,0,441,442,5,25,0,0,442,443,5,2,0,0,443,444,5,25,0,0,444,
-        445,5,25,0,0,445,447,3,96,48,0,446,448,3,96,48,0,447,446,1,0,0,0,
-        447,448,1,0,0,0,448,450,1,0,0,0,449,451,3,96,48,0,450,449,1,0,0,
-        0,450,451,1,0,0,0,451,59,1,0,0,0,452,454,3,62,31,0,453,452,1,0,0,
-        0,454,455,1,0,0,0,455,453,1,0,0,0,455,456,1,0,0,0,456,61,1,0,0,0,
-        457,458,5,25,0,0,458,459,5,25,0,0,459,460,5,2,0,0,460,461,5,25,0,
-        0,461,462,5,25,0,0,462,463,5,25,0,0,463,464,5,2,0,0,464,465,5,25,
-        0,0,465,467,3,96,48,0,466,468,3,96,48,0,467,466,1,0,0,0,467,468,
-        1,0,0,0,468,470,1,0,0,0,469,471,3,96,48,0,470,469,1,0,0,0,470,471,
-        1,0,0,0,471,63,1,0,0,0,472,474,3,66,33,0,473,472,1,0,0,0,474,475,
-        1,0,0,0,475,473,1,0,0,0,475,476,1,0,0,0,476,65,1,0,0,0,477,478,5,
-        25,0,0,478,479,5,2,0,0,479,480,5,25,0,0,480,481,5,25,0,0,481,482,
-        3,96,48,0,482,484,3,96,48,0,483,485,3,96,48,0,484,483,1,0,0,0,484,
-        485,1,0,0,0,485,489,1,0,0,0,486,487,5,10,0,0,487,488,5,11,0,0,488,
-        490,5,2,0,0,489,486,1,0,0,0,489,490,1,0,0,0,490,492,1,0,0,0,491,
-        493,5,12,0,0,492,491,1,0,0,0,492,493,1,0,0,0,493,67,1,0,0,0,494,
-        496,3,70,35,0,495,494,1,0,0,0,496,497,1,0,0,0,497,495,1,0,0,0,497,
-        498,1,0,0,0,498,69,1,0,0,0,499,500,5,2,0,0,500,501,5,25,0,0,501,
-        502,5,25,0,0,502,503,5,25,0,0,503,505,3,96,48,0,504,506,3,96,48,
-        0,505,504,1,0,0,0,505,506,1,0,0,0,506,508,1,0,0,0,507,509,3,96,48,
-        0,508,507,1,0,0,0,508,509,1,0,0,0,509,511,1,0,0,0,510,512,3,96,48,
-        0,511,510,1,0,0,0,511,512,1,0,0,0,512,514,1,0,0,0,513,515,3,96,48,
-        0,514,513,1,0,0,0,514,515,1,0,0,0,515,517,1,0,0,0,516,518,3,96,48,
-        0,517,516,1,0,0,0,517,518,1,0,0,0,518,71,1,0,0,0,519,520,5,13,0,
-        0,520,521,5,14,0,0,521,73,1,0,0,0,522,525,5,15,0,0,523,524,5,33,
-        0,0,524,526,5,37,0,0,525,523,1,0,0,0,525,526,1,0,0,0,526,527,1,0,
-        0,0,527,530,5,39,0,0,528,529,5,35,0,0,529,531,5,37,0,0,530,528,1,
-        0,0,0,530,531,1,0,0,0,531,532,1,0,0,0,532,535,5,38,0,0,533,534,5,
-        34,0,0,534,536,5,37,0,0,535,533,1,0,0,0,535,536,1,0,0,0,536,537,
-        1,0,0,0,537,540,5,39,0,0,538,539,5,36,0,0,539,541,5,37,0,0,540,538,
-        1,0,0,0,540,541,1,0,0,0,541,542,1,0,0,0,542,543,5,38,0,0,543,544,
-        5,41,0,0,544,75,1,0,0,0,545,546,5,16,0,0,546,547,5,25,0,0,547,548,
-        5,2,0,0,548,549,5,25,0,0,549,550,5,2,0,0,550,77,1,0,0,0,551,552,
-        5,17,0,0,552,553,5,43,0,0,553,554,5,45,0,0,554,79,1,0,0,0,555,559,
-        5,18,0,0,556,558,5,47,0,0,557,556,1,0,0,0,558,561,1,0,0,0,559,557,
-        1,0,0,0,559,560,1,0,0,0,560,562,1,0,0,0,561,559,1,0,0,0,562,563,
-        5,49,0,0,563,81,1,0,0,0,564,565,5,20,0,0,565,83,1,0,0,0,566,570,
-        5,19,0,0,567,569,5,47,0,0,568,567,1,0,0,0,569,572,1,0,0,0,570,568,
-        1,0,0,0,570,571,1,0,0,0,571,573,1,0,0,0,572,570,1,0,0,0,573,574,
-        5,49,0,0,574,85,1,0,0,0,575,576,5,21,0,0,576,577,5,43,0,0,577,578,
-        5,45,0,0,578,87,1,0,0,0,579,580,5,22,0,0,580,582,5,25,0,0,581,583,
-        3,2,1,0,582,581,1,0,0,0,582,583,1,0,0,0,583,586,1,0,0,0,584,587,
-        3,90,45,0,585,587,3,2,1,0,586,584,1,0,0,0,586,585,1,0,0,0,587,588,
-        1,0,0,0,588,586,1,0,0,0,588,589,1,0,0,0,589,89,1,0,0,0,590,591,5,
-        23,0,0,591,592,5,53,0,0,592,594,5,54,0,0,593,595,5,53,0,0,594,593,
-        1,0,0,0,595,596,1,0,0,0,596,594,1,0,0,0,596,597,1,0,0,0,597,598,
-        1,0,0,0,598,599,5,56,0,0,599,91,1,0,0,0,600,601,5,22,0,0,601,603,
-        5,25,0,0,602,604,3,2,1,0,603,602,1,0,0,0,603,604,1,0,0,0,604,607,
-        1,0,0,0,605,608,3,94,47,0,606,608,3,2,1,0,607,605,1,0,0,0,607,606,
-        1,0,0,0,608,609,1,0,0,0,609,607,1,0,0,0,609,610,1,0,0,0,610,93,1,
-        0,0,0,611,612,5,24,0,0,612,613,7,1,0,0,613,616,5,54,0,0,614,615,
-        5,53,0,0,615,617,5,52,0,0,616,614,1,0,0,0,617,618,1,0,0,0,618,616,
-        1,0,0,0,618,619,1,0,0,0,619,620,1,0,0,0,620,621,5,56,0,0,621,95,
-        1,0,0,0,622,623,7,2,0,0,623,97,1,0,0,0,624,625,7,3,0,0,625,99,1,
-        0,0,0,80,129,131,140,148,158,161,164,167,170,175,183,188,191,196,
-        201,207,217,231,236,241,247,257,271,276,284,286,291,296,306,308,
-        313,318,329,331,336,342,349,351,356,362,371,373,378,384,394,396,
-        401,415,427,430,435,447,450,455,467,470,475,484,489,492,497,505,
-        508,511,514,517,525,530,535,540,559,570,582,586,588,596,603,607,
-        609,618
+        0,5,1,1,32,32,1,0,8,9,2,0,51,51,53,53,1,0,2,3,2,0,1,1,25,25,683,
+        0,131,1,0,0,0,2,136,1,0,0,0,4,146,1,0,0,0,6,150,1,0,0,0,8,173,1,
+        0,0,0,10,177,1,0,0,0,12,194,1,0,0,0,14,209,1,0,0,0,16,217,1,0,0,
+        0,18,234,1,0,0,0,20,249,1,0,0,0,22,257,1,0,0,0,24,269,1,0,0,0,26,
+        273,1,0,0,0,28,289,1,0,0,0,30,293,1,0,0,0,32,311,1,0,0,0,34,315,
+        1,0,0,0,36,334,1,0,0,0,38,338,1,0,0,0,40,354,1,0,0,0,42,358,1,0,
+        0,0,44,376,1,0,0,0,46,380,1,0,0,0,48,399,1,0,0,0,50,403,1,0,0,0,
+        52,413,1,0,0,0,54,417,1,0,0,0,56,433,1,0,0,0,58,437,1,0,0,0,60,453,
+        1,0,0,0,62,457,1,0,0,0,64,473,1,0,0,0,66,477,1,0,0,0,68,495,1,0,
+        0,0,70,499,1,0,0,0,72,519,1,0,0,0,74,522,1,0,0,0,76,545,1,0,0,0,
+        78,551,1,0,0,0,80,555,1,0,0,0,82,564,1,0,0,0,84,566,1,0,0,0,86,575,
+        1,0,0,0,88,579,1,0,0,0,90,590,1,0,0,0,92,600,1,0,0,0,94,611,1,0,
+        0,0,96,622,1,0,0,0,98,624,1,0,0,0,100,130,5,4,0,0,101,130,5,5,0,
+        0,102,130,3,2,1,0,103,130,3,4,2,0,104,130,3,24,12,0,105,130,3,28,
+        14,0,106,130,3,32,16,0,107,130,3,36,18,0,108,130,3,40,20,0,109,130,
+        3,44,22,0,110,130,3,48,24,0,111,130,3,52,26,0,112,130,3,56,28,0,
+        113,130,3,60,30,0,114,130,3,8,4,0,115,130,3,64,32,0,116,130,3,12,
+        6,0,117,130,3,18,9,0,118,130,3,68,34,0,119,130,3,72,36,0,120,130,
+        3,74,37,0,121,130,3,76,38,0,122,130,3,78,39,0,123,130,3,80,40,0,
+        124,130,3,82,41,0,125,130,3,84,42,0,126,130,3,86,43,0,127,130,3,
+        88,44,0,128,130,3,92,46,0,129,100,1,0,0,0,129,101,1,0,0,0,129,102,
+        1,0,0,0,129,103,1,0,0,0,129,104,1,0,0,0,129,105,1,0,0,0,129,106,
+        1,0,0,0,129,107,1,0,0,0,129,108,1,0,0,0,129,109,1,0,0,0,129,110,
+        1,0,0,0,129,111,1,0,0,0,129,112,1,0,0,0,129,113,1,0,0,0,129,114,
+        1,0,0,0,129,115,1,0,0,0,129,116,1,0,0,0,129,117,1,0,0,0,129,118,
+        1,0,0,0,129,119,1,0,0,0,129,120,1,0,0,0,129,121,1,0,0,0,129,122,
+        1,0,0,0,129,123,1,0,0,0,129,124,1,0,0,0,129,125,1,0,0,0,129,126,
+        1,0,0,0,129,127,1,0,0,0,129,128,1,0,0,0,130,133,1,0,0,0,131,129,
+        1,0,0,0,131,132,1,0,0,0,132,134,1,0,0,0,133,131,1,0,0,0,134,135,
+        5,0,0,1,135,1,1,0,0,0,136,140,5,7,0,0,137,139,5,30,0,0,138,137,1,
+        0,0,0,139,142,1,0,0,0,140,138,1,0,0,0,140,141,1,0,0,0,141,143,1,
+        0,0,0,142,140,1,0,0,0,143,144,7,0,0,0,144,3,1,0,0,0,145,147,3,6,
+        3,0,146,145,1,0,0,0,147,148,1,0,0,0,148,146,1,0,0,0,148,149,1,0,
+        0,0,149,5,1,0,0,0,150,151,5,2,0,0,151,152,5,25,0,0,152,153,3,98,
+        49,0,153,154,5,2,0,0,154,155,5,25,0,0,155,156,3,98,49,0,156,158,
+        3,96,48,0,157,159,3,96,48,0,158,157,1,0,0,0,158,159,1,0,0,0,159,
+        161,1,0,0,0,160,162,3,96,48,0,161,160,1,0,0,0,161,162,1,0,0,0,162,
+        164,1,0,0,0,163,165,3,96,48,0,164,163,1,0,0,0,164,165,1,0,0,0,165,
+        167,1,0,0,0,166,168,3,96,48,0,167,166,1,0,0,0,167,168,1,0,0,0,168,
+        170,1,0,0,0,169,171,3,96,48,0,170,169,1,0,0,0,170,171,1,0,0,0,171,
+        7,1,0,0,0,172,174,3,10,5,0,173,172,1,0,0,0,174,175,1,0,0,0,175,173,
+        1,0,0,0,175,176,1,0,0,0,176,9,1,0,0,0,177,178,5,2,0,0,178,179,5,
+        25,0,0,179,180,5,25,0,0,180,181,3,96,48,0,181,183,3,96,48,0,182,
+        184,3,96,48,0,183,182,1,0,0,0,183,184,1,0,0,0,184,188,1,0,0,0,185,
+        186,5,10,0,0,186,187,5,11,0,0,187,189,5,2,0,0,188,185,1,0,0,0,188,
+        189,1,0,0,0,189,191,1,0,0,0,190,192,5,12,0,0,191,190,1,0,0,0,191,
+        192,1,0,0,0,192,11,1,0,0,0,193,195,3,14,7,0,194,193,1,0,0,0,195,
+        196,1,0,0,0,196,194,1,0,0,0,196,197,1,0,0,0,197,201,1,0,0,0,198,
+        200,3,2,1,0,199,198,1,0,0,0,200,203,1,0,0,0,201,199,1,0,0,0,201,
+        202,1,0,0,0,202,205,1,0,0,0,203,201,1,0,0,0,204,206,3,16,8,0,205,
+        204,1,0,0,0,206,207,1,0,0,0,207,205,1,0,0,0,207,208,1,0,0,0,208,
+        13,1,0,0,0,209,210,5,2,0,0,210,211,3,96,48,0,211,212,3,96,48,0,212,
+        213,5,2,0,0,213,15,1,0,0,0,214,216,3,2,1,0,215,214,1,0,0,0,216,219,
+        1,0,0,0,217,215,1,0,0,0,217,218,1,0,0,0,218,220,1,0,0,0,219,217,
+        1,0,0,0,220,221,5,2,0,0,221,222,5,25,0,0,222,223,5,25,0,0,223,224,
+        5,2,0,0,224,225,5,25,0,0,225,226,5,25,0,0,226,227,3,96,48,0,227,
+        228,3,96,48,0,228,229,3,96,48,0,229,231,5,2,0,0,230,232,3,96,48,
+        0,231,230,1,0,0,0,231,232,1,0,0,0,232,17,1,0,0,0,233,235,3,20,10,
+        0,234,233,1,0,0,0,235,236,1,0,0,0,236,234,1,0,0,0,236,237,1,0,0,
+        0,237,241,1,0,0,0,238,240,3,2,1,0,239,238,1,0,0,0,240,243,1,0,0,
+        0,241,239,1,0,0,0,241,242,1,0,0,0,242,245,1,0,0,0,243,241,1,0,0,
+        0,244,246,3,22,11,0,245,244,1,0,0,0,246,247,1,0,0,0,247,245,1,0,
+        0,0,247,248,1,0,0,0,248,19,1,0,0,0,249,250,5,2,0,0,250,251,3,96,
+        48,0,251,252,3,96,48,0,252,253,5,2,0,0,253,21,1,0,0,0,254,256,3,
+        2,1,0,255,254,1,0,0,0,256,259,1,0,0,0,257,255,1,0,0,0,257,258,1,
+        0,0,0,258,260,1,0,0,0,259,257,1,0,0,0,260,261,5,2,0,0,261,262,5,
+        25,0,0,262,263,5,25,0,0,263,264,3,96,48,0,264,265,3,96,48,0,265,
+        266,3,96,48,0,266,267,5,2,0,0,267,23,1,0,0,0,268,270,3,26,13,0,269,
+        268,1,0,0,0,270,271,1,0,0,0,271,269,1,0,0,0,271,272,1,0,0,0,272,
+        25,1,0,0,0,273,274,5,2,0,0,274,276,5,25,0,0,275,277,3,2,1,0,276,
+        275,1,0,0,0,276,277,1,0,0,0,277,284,1,0,0,0,278,279,5,25,0,0,279,
+        280,5,2,0,0,280,281,5,25,0,0,281,282,5,25,0,0,282,285,3,96,48,0,
+        283,285,3,2,1,0,284,278,1,0,0,0,284,283,1,0,0,0,285,286,1,0,0,0,
+        286,284,1,0,0,0,286,287,1,0,0,0,287,27,1,0,0,0,288,290,3,30,15,0,
+        289,288,1,0,0,0,290,291,1,0,0,0,291,289,1,0,0,0,291,292,1,0,0,0,
+        292,29,1,0,0,0,293,294,5,2,0,0,294,296,5,25,0,0,295,297,3,2,1,0,
+        296,295,1,0,0,0,296,297,1,0,0,0,297,306,1,0,0,0,298,299,5,25,0,0,
+        299,300,5,2,0,0,300,301,5,25,0,0,301,302,5,25,0,0,302,303,3,96,48,
+        0,303,304,3,96,48,0,304,307,1,0,0,0,305,307,3,2,1,0,306,298,1,0,
+        0,0,306,305,1,0,0,0,307,308,1,0,0,0,308,306,1,0,0,0,308,309,1,0,
+        0,0,309,31,1,0,0,0,310,312,3,34,17,0,311,310,1,0,0,0,312,313,1,0,
+        0,0,313,311,1,0,0,0,313,314,1,0,0,0,314,33,1,0,0,0,315,316,5,2,0,
+        0,316,318,5,25,0,0,317,319,3,2,1,0,318,317,1,0,0,0,318,319,1,0,0,
+        0,319,329,1,0,0,0,320,321,5,25,0,0,321,322,5,2,0,0,322,323,5,25,
+        0,0,323,324,5,25,0,0,324,325,3,96,48,0,325,326,3,96,48,0,326,327,
+        3,96,48,0,327,330,1,0,0,0,328,330,3,2,1,0,329,320,1,0,0,0,329,328,
+        1,0,0,0,330,331,1,0,0,0,331,329,1,0,0,0,331,332,1,0,0,0,332,35,1,
+        0,0,0,333,335,3,38,19,0,334,333,1,0,0,0,335,336,1,0,0,0,336,334,
+        1,0,0,0,336,337,1,0,0,0,337,37,1,0,0,0,338,339,5,2,0,0,339,340,5,
+        25,0,0,340,342,5,25,0,0,341,343,3,2,1,0,342,341,1,0,0,0,342,343,
+        1,0,0,0,343,349,1,0,0,0,344,345,5,2,0,0,345,346,5,25,0,0,346,347,
+        5,25,0,0,347,350,3,96,48,0,348,350,3,2,1,0,349,344,1,0,0,0,349,348,
+        1,0,0,0,350,351,1,0,0,0,351,349,1,0,0,0,351,352,1,0,0,0,352,39,1,
+        0,0,0,353,355,3,42,21,0,354,353,1,0,0,0,355,356,1,0,0,0,356,354,
+        1,0,0,0,356,357,1,0,0,0,357,41,1,0,0,0,358,359,5,2,0,0,359,360,5,
+        25,0,0,360,362,5,25,0,0,361,363,3,2,1,0,362,361,1,0,0,0,362,363,
+        1,0,0,0,363,371,1,0,0,0,364,365,5,2,0,0,365,366,5,25,0,0,366,367,
+        5,25,0,0,367,368,3,96,48,0,368,369,3,96,48,0,369,372,1,0,0,0,370,
+        372,3,2,1,0,371,364,1,0,0,0,371,370,1,0,0,0,372,373,1,0,0,0,373,
+        371,1,0,0,0,373,374,1,0,0,0,374,43,1,0,0,0,375,377,3,46,23,0,376,
+        375,1,0,0,0,377,378,1,0,0,0,378,376,1,0,0,0,378,379,1,0,0,0,379,
+        45,1,0,0,0,380,381,5,2,0,0,381,382,5,25,0,0,382,384,5,25,0,0,383,
+        385,3,2,1,0,384,383,1,0,0,0,384,385,1,0,0,0,385,394,1,0,0,0,386,
+        387,5,2,0,0,387,388,5,25,0,0,388,389,5,25,0,0,389,390,3,96,48,0,
+        390,391,3,96,48,0,391,392,3,96,48,0,392,395,1,0,0,0,393,395,3,2,
+        1,0,394,386,1,0,0,0,394,393,1,0,0,0,395,396,1,0,0,0,396,394,1,0,
+        0,0,396,397,1,0,0,0,397,47,1,0,0,0,398,400,3,50,25,0,399,398,1,0,
+        0,0,400,401,1,0,0,0,401,399,1,0,0,0,401,402,1,0,0,0,402,49,1,0,0,
+        0,403,404,7,1,0,0,404,405,5,25,0,0,405,406,5,2,0,0,406,407,5,25,
+        0,0,407,408,5,25,0,0,408,409,5,2,0,0,409,410,5,25,0,0,410,411,3,
+        96,48,0,411,51,1,0,0,0,412,414,3,54,27,0,413,412,1,0,0,0,414,415,
+        1,0,0,0,415,413,1,0,0,0,415,416,1,0,0,0,416,53,1,0,0,0,417,418,5,
+        2,0,0,418,419,5,25,0,0,419,420,5,25,0,0,420,421,5,25,0,0,421,422,
+        5,2,0,0,422,423,5,25,0,0,423,424,5,25,0,0,424,425,5,25,0,0,425,427,
+        3,96,48,0,426,428,3,96,48,0,427,426,1,0,0,0,427,428,1,0,0,0,428,
+        430,1,0,0,0,429,431,3,96,48,0,430,429,1,0,0,0,430,431,1,0,0,0,431,
+        55,1,0,0,0,432,434,3,58,29,0,433,432,1,0,0,0,434,435,1,0,0,0,435,
+        433,1,0,0,0,435,436,1,0,0,0,436,57,1,0,0,0,437,438,5,25,0,0,438,
+        439,5,2,0,0,439,440,5,25,0,0,440,441,5,25,0,0,441,442,5,25,0,0,442,
+        443,5,2,0,0,443,444,5,25,0,0,444,445,5,25,0,0,445,447,3,96,48,0,
+        446,448,3,96,48,0,447,446,1,0,0,0,447,448,1,0,0,0,448,450,1,0,0,
+        0,449,451,3,96,48,0,450,449,1,0,0,0,450,451,1,0,0,0,451,59,1,0,0,
+        0,452,454,3,62,31,0,453,452,1,0,0,0,454,455,1,0,0,0,455,453,1,0,
+        0,0,455,456,1,0,0,0,456,61,1,0,0,0,457,458,5,25,0,0,458,459,5,25,
+        0,0,459,460,5,2,0,0,460,461,5,25,0,0,461,462,5,25,0,0,462,463,5,
+        25,0,0,463,464,5,2,0,0,464,465,5,25,0,0,465,467,3,96,48,0,466,468,
+        3,96,48,0,467,466,1,0,0,0,467,468,1,0,0,0,468,470,1,0,0,0,469,471,
+        3,96,48,0,470,469,1,0,0,0,470,471,1,0,0,0,471,63,1,0,0,0,472,474,
+        3,66,33,0,473,472,1,0,0,0,474,475,1,0,0,0,475,473,1,0,0,0,475,476,
+        1,0,0,0,476,65,1,0,0,0,477,478,5,25,0,0,478,479,5,2,0,0,479,480,
+        5,25,0,0,480,481,5,25,0,0,481,482,3,96,48,0,482,484,3,96,48,0,483,
+        485,3,96,48,0,484,483,1,0,0,0,484,485,1,0,0,0,485,489,1,0,0,0,486,
+        487,5,10,0,0,487,488,5,11,0,0,488,490,5,2,0,0,489,486,1,0,0,0,489,
+        490,1,0,0,0,490,492,1,0,0,0,491,493,5,12,0,0,492,491,1,0,0,0,492,
+        493,1,0,0,0,493,67,1,0,0,0,494,496,3,70,35,0,495,494,1,0,0,0,496,
+        497,1,0,0,0,497,495,1,0,0,0,497,498,1,0,0,0,498,69,1,0,0,0,499,500,
+        5,2,0,0,500,501,5,25,0,0,501,502,5,25,0,0,502,503,5,25,0,0,503,505,
+        3,96,48,0,504,506,3,96,48,0,505,504,1,0,0,0,505,506,1,0,0,0,506,
+        508,1,0,0,0,507,509,3,96,48,0,508,507,1,0,0,0,508,509,1,0,0,0,509,
+        511,1,0,0,0,510,512,3,96,48,0,511,510,1,0,0,0,511,512,1,0,0,0,512,
+        514,1,0,0,0,513,515,3,96,48,0,514,513,1,0,0,0,514,515,1,0,0,0,515,
+        517,1,0,0,0,516,518,3,96,48,0,517,516,1,0,0,0,517,518,1,0,0,0,518,
+        71,1,0,0,0,519,520,5,13,0,0,520,521,5,14,0,0,521,73,1,0,0,0,522,
+        525,5,15,0,0,523,524,5,33,0,0,524,526,5,37,0,0,525,523,1,0,0,0,525,
+        526,1,0,0,0,526,527,1,0,0,0,527,530,5,39,0,0,528,529,5,35,0,0,529,
+        531,5,37,0,0,530,528,1,0,0,0,530,531,1,0,0,0,531,532,1,0,0,0,532,
+        535,5,38,0,0,533,534,5,34,0,0,534,536,5,37,0,0,535,533,1,0,0,0,535,
+        536,1,0,0,0,536,537,1,0,0,0,537,540,5,39,0,0,538,539,5,36,0,0,539,
+        541,5,37,0,0,540,538,1,0,0,0,540,541,1,0,0,0,541,542,1,0,0,0,542,
+        543,5,38,0,0,543,544,5,41,0,0,544,75,1,0,0,0,545,546,5,16,0,0,546,
+        547,5,25,0,0,547,548,5,2,0,0,548,549,5,25,0,0,549,550,5,2,0,0,550,
+        77,1,0,0,0,551,552,5,17,0,0,552,553,5,43,0,0,553,554,5,45,0,0,554,
+        79,1,0,0,0,555,559,5,18,0,0,556,558,5,47,0,0,557,556,1,0,0,0,558,
+        561,1,0,0,0,559,557,1,0,0,0,559,560,1,0,0,0,560,562,1,0,0,0,561,
+        559,1,0,0,0,562,563,5,49,0,0,563,81,1,0,0,0,564,565,5,20,0,0,565,
+        83,1,0,0,0,566,570,5,19,0,0,567,569,5,47,0,0,568,567,1,0,0,0,569,
+        572,1,0,0,0,570,568,1,0,0,0,570,571,1,0,0,0,571,573,1,0,0,0,572,
+        570,1,0,0,0,573,574,5,49,0,0,574,85,1,0,0,0,575,576,5,21,0,0,576,
+        577,5,43,0,0,577,578,5,45,0,0,578,87,1,0,0,0,579,580,5,22,0,0,580,
+        582,5,25,0,0,581,583,3,2,1,0,582,581,1,0,0,0,582,583,1,0,0,0,583,
+        586,1,0,0,0,584,587,3,90,45,0,585,587,3,2,1,0,586,584,1,0,0,0,586,
+        585,1,0,0,0,587,588,1,0,0,0,588,586,1,0,0,0,588,589,1,0,0,0,589,
+        89,1,0,0,0,590,591,5,23,0,0,591,592,5,53,0,0,592,594,5,54,0,0,593,
+        595,5,53,0,0,594,593,1,0,0,0,595,596,1,0,0,0,596,594,1,0,0,0,596,
+        597,1,0,0,0,597,598,1,0,0,0,598,599,5,56,0,0,599,91,1,0,0,0,600,
+        601,5,22,0,0,601,603,5,25,0,0,602,604,3,2,1,0,603,602,1,0,0,0,603,
+        604,1,0,0,0,604,607,1,0,0,0,605,608,3,94,47,0,606,608,3,2,1,0,607,
+        605,1,0,0,0,607,606,1,0,0,0,608,609,1,0,0,0,609,607,1,0,0,0,609,
+        610,1,0,0,0,610,93,1,0,0,0,611,612,5,24,0,0,612,613,7,2,0,0,613,
+        616,5,54,0,0,614,615,5,53,0,0,615,617,5,52,0,0,616,614,1,0,0,0,617,
+        618,1,0,0,0,618,616,1,0,0,0,618,619,1,0,0,0,619,620,1,0,0,0,620,
+        621,5,56,0,0,621,95,1,0,0,0,622,623,7,3,0,0,623,97,1,0,0,0,624,625,
+        7,4,0,0,625,99,1,0,0,0,80,129,131,140,148,158,161,164,167,170,175,
+        183,188,191,196,201,207,217,231,236,241,247,257,271,276,284,286,
+        291,296,306,308,313,318,329,331,336,342,349,351,356,362,371,373,
+        378,384,394,396,401,415,427,430,435,447,450,455,467,470,475,484,
+        489,492,497,505,508,511,514,517,525,530,535,540,559,570,582,586,
+        588,596,603,607,609,618
     ]
 
 class CyanaMRParser ( Parser ):
 
     grammarFileName = "CyanaMRParser.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
@@ -828,14 +828,17 @@
 
         def COMMENT(self):
             return self.getToken(CyanaMRParser.COMMENT, 0)
 
         def RETURN_CM(self):
             return self.getToken(CyanaMRParser.RETURN_CM, 0)
 
+        def EOF(self):
+            return self.getToken(CyanaMRParser.EOF, 0)
+
         def Any_name(self, i:int=None):
             if i is None:
                 return self.getTokens(CyanaMRParser.Any_name)
             else:
                 return self.getToken(CyanaMRParser.Any_name, i)
 
         def getRuleIndex(self):
@@ -868,15 +871,20 @@
                 self.state = 137
                 self.match(CyanaMRParser.Any_name)
                 self.state = 142
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
             self.state = 143
-            self.match(CyanaMRParser.RETURN_CM)
+            _la = self._input.LA(1)
+            if not(_la==-1 or _la==32):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
```

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CyanaMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/CyanaMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/DynamoMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/DynamoMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/DynamoMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/DynamoMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsPTLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsPTParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsPTParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/GromacsPTReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/IsdMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/IsdMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/IsdMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/IsdMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/LexerErrorListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/LexerErrorListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/ParserErrorListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserErrorListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/ParserListenerUtil.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserListenerUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/RosettaMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/RosettaMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,149 +47,150 @@
         25,1,25,5,25,414,8,25,10,25,12,25,417,9,25,1,25,1,25,1,25,1,25,1,
         25,1,25,1,25,4,25,426,8,25,11,25,12,25,427,1,25,1,25,1,25,1,25,1,
         25,1,25,1,25,1,25,1,25,4,25,439,8,25,11,25,12,25,440,3,25,443,8,
         25,1,25,3,25,446,8,25,1,26,4,26,449,8,26,11,26,12,26,450,1,27,1,
         27,1,27,1,27,1,27,1,27,1,28,4,28,460,8,28,11,28,12,28,461,1,29,1,
         29,1,29,1,30,1,30,1,31,1,31,1,31,0,0,32,0,2,4,6,8,10,12,14,16,18,
         20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,62,
-        0,8,1,0,60,62,2,0,1,2,9,9,1,0,3,4,3,0,18,18,25,25,39,40,3,0,21,22,
-        26,26,46,46,2,0,23,23,43,43,2,0,31,31,44,45,1,0,50,51,519,0,80,1,
-        0,0,0,2,85,1,0,0,0,4,95,1,0,0,0,6,99,1,0,0,0,8,107,1,0,0,0,10,111,
-        1,0,0,0,12,121,1,0,0,0,14,125,1,0,0,0,16,137,1,0,0,0,18,141,1,0,
-        0,0,20,161,1,0,0,0,22,165,1,0,0,0,24,176,1,0,0,0,26,180,1,0,0,0,
-        28,193,1,0,0,0,30,197,1,0,0,0,32,204,1,0,0,0,34,208,1,0,0,0,36,216,
-        1,0,0,0,38,220,1,0,0,0,40,226,1,0,0,0,42,230,1,0,0,0,44,236,1,0,
-        0,0,46,244,1,0,0,0,48,263,1,0,0,0,50,442,1,0,0,0,52,448,1,0,0,0,
-        54,452,1,0,0,0,56,459,1,0,0,0,58,463,1,0,0,0,60,466,1,0,0,0,62,468,
-        1,0,0,0,64,79,3,2,1,0,65,79,3,4,2,0,66,79,3,8,4,0,67,79,3,12,6,0,
-        68,79,3,16,8,0,69,79,3,20,10,0,70,79,3,24,12,0,71,79,3,28,14,0,72,
-        79,3,32,16,0,73,79,3,36,18,0,74,79,3,40,20,0,75,79,3,44,22,0,76,
-        79,3,52,26,0,77,79,3,56,28,0,78,64,1,0,0,0,78,65,1,0,0,0,78,66,1,
-        0,0,0,78,67,1,0,0,0,78,68,1,0,0,0,78,69,1,0,0,0,78,70,1,0,0,0,78,
-        71,1,0,0,0,78,72,1,0,0,0,78,73,1,0,0,0,78,74,1,0,0,0,78,75,1,0,0,
-        0,78,76,1,0,0,0,78,77,1,0,0,0,79,82,1,0,0,0,80,78,1,0,0,0,80,81,
-        1,0,0,0,81,83,1,0,0,0,82,80,1,0,0,0,83,84,5,0,0,1,84,1,1,0,0,0,85,
-        89,5,54,0,0,86,88,7,0,0,0,87,86,1,0,0,0,88,91,1,0,0,0,89,87,1,0,
-        0,0,89,90,1,0,0,0,90,92,1,0,0,0,91,89,1,0,0,0,92,93,5,64,0,0,93,
-        3,1,0,0,0,94,96,3,6,3,0,95,94,1,0,0,0,96,97,1,0,0,0,97,95,1,0,0,
-        0,97,98,1,0,0,0,98,5,1,0,0,0,99,100,7,1,0,0,100,101,5,55,0,0,101,
-        102,5,50,0,0,102,103,5,55,0,0,103,104,5,50,0,0,104,105,3,50,25,0,
-        105,7,1,0,0,0,106,108,3,10,5,0,107,106,1,0,0,0,108,109,1,0,0,0,109,
-        107,1,0,0,0,109,110,1,0,0,0,110,9,1,0,0,0,111,112,7,2,0,0,112,113,
-        5,55,0,0,113,114,5,50,0,0,114,115,5,55,0,0,115,116,5,50,0,0,116,
-        117,5,55,0,0,117,118,5,50,0,0,118,119,3,50,25,0,119,11,1,0,0,0,120,
-        122,3,14,7,0,121,120,1,0,0,0,122,123,1,0,0,0,123,121,1,0,0,0,123,
-        124,1,0,0,0,124,13,1,0,0,0,125,126,5,5,0,0,126,127,5,55,0,0,127,
-        128,5,50,0,0,128,129,5,55,0,0,129,130,5,50,0,0,130,131,5,55,0,0,
-        131,132,5,50,0,0,132,133,5,55,0,0,133,134,5,50,0,0,134,135,3,50,
-        25,0,135,15,1,0,0,0,136,138,3,18,9,0,137,136,1,0,0,0,138,139,1,0,
-        0,0,139,137,1,0,0,0,139,140,1,0,0,0,140,17,1,0,0,0,141,142,5,6,0,
-        0,142,143,5,55,0,0,143,144,5,50,0,0,144,145,5,55,0,0,145,146,5,50,
-        0,0,146,147,5,55,0,0,147,148,5,50,0,0,148,149,5,55,0,0,149,150,5,
-        50,0,0,150,151,5,55,0,0,151,152,5,50,0,0,152,153,5,55,0,0,153,154,
-        5,50,0,0,154,155,5,55,0,0,155,156,5,50,0,0,156,157,5,55,0,0,157,
-        158,5,50,0,0,158,159,3,50,25,0,159,19,1,0,0,0,160,162,3,22,11,0,
-        161,160,1,0,0,0,162,163,1,0,0,0,163,161,1,0,0,0,163,164,1,0,0,0,
-        164,21,1,0,0,0,165,166,5,7,0,0,166,167,5,55,0,0,167,168,5,55,0,0,
-        168,169,5,55,0,0,169,170,5,55,0,0,170,171,3,60,30,0,171,172,3,60,
-        30,0,172,173,3,60,30,0,173,174,3,50,25,0,174,23,1,0,0,0,175,177,
-        3,26,13,0,176,175,1,0,0,0,177,178,1,0,0,0,178,176,1,0,0,0,178,179,
-        1,0,0,0,179,25,1,0,0,0,180,181,5,8,0,0,181,182,5,55,0,0,182,183,
-        5,50,0,0,183,184,5,55,0,0,184,185,5,55,0,0,185,186,5,55,0,0,186,
-        187,5,50,0,0,187,188,3,60,30,0,188,189,3,60,30,0,189,190,3,60,30,
-        0,190,191,3,50,25,0,191,27,1,0,0,0,192,194,3,30,15,0,193,192,1,0,
-        0,0,194,195,1,0,0,0,195,193,1,0,0,0,195,196,1,0,0,0,196,29,1,0,0,
-        0,197,198,5,10,0,0,198,199,5,55,0,0,199,200,5,50,0,0,200,201,5,55,
-        0,0,201,202,3,50,25,0,202,31,1,0,0,0,203,205,3,34,17,0,204,203,1,
-        0,0,0,205,206,1,0,0,0,206,204,1,0,0,0,206,207,1,0,0,0,207,33,1,0,
-        0,0,208,209,5,11,0,0,209,210,5,50,0,0,210,211,5,55,0,0,211,212,5,
-        50,0,0,212,213,5,50,0,0,213,214,3,50,25,0,214,35,1,0,0,0,215,217,
-        3,38,19,0,216,215,1,0,0,0,217,218,1,0,0,0,218,216,1,0,0,0,218,219,
-        1,0,0,0,219,37,1,0,0,0,220,221,5,12,0,0,221,222,5,50,0,0,222,223,
-        5,50,0,0,223,224,3,60,30,0,224,39,1,0,0,0,225,227,3,42,21,0,226,
-        225,1,0,0,0,227,228,1,0,0,0,228,226,1,0,0,0,228,229,1,0,0,0,229,
-        41,1,0,0,0,230,231,5,13,0,0,231,232,5,50,0,0,232,233,5,55,0,0,233,
-        234,3,60,30,0,234,43,1,0,0,0,235,237,3,46,23,0,236,235,1,0,0,0,237,
-        238,1,0,0,0,238,236,1,0,0,0,238,239,1,0,0,0,239,45,1,0,0,0,240,245,
-        5,14,0,0,241,245,5,15,0,0,242,243,5,16,0,0,243,245,5,50,0,0,244,
-        240,1,0,0,0,244,241,1,0,0,0,244,242,1,0,0,0,245,247,1,0,0,0,246,
-        248,3,48,24,0,247,246,1,0,0,0,248,249,1,0,0,0,249,247,1,0,0,0,249,
-        250,1,0,0,0,250,251,1,0,0,0,251,252,5,17,0,0,252,47,1,0,0,0,253,
-        264,3,6,3,0,254,264,3,10,5,0,255,264,3,14,7,0,256,264,3,18,9,0,257,
-        264,3,22,11,0,258,264,3,26,13,0,259,264,3,30,15,0,260,264,3,34,17,
-        0,261,264,3,38,19,0,262,264,3,42,21,0,263,253,1,0,0,0,263,254,1,
-        0,0,0,263,255,1,0,0,0,263,256,1,0,0,0,263,257,1,0,0,0,263,258,1,
-        0,0,0,263,259,1,0,0,0,263,260,1,0,0,0,263,261,1,0,0,0,263,262,1,
-        0,0,0,264,49,1,0,0,0,265,266,7,3,0,0,266,267,3,62,31,0,267,268,3,
-        62,31,0,268,443,1,0,0,0,269,270,5,27,0,0,270,271,3,62,31,0,271,272,
-        3,62,31,0,272,274,3,62,31,0,273,275,3,62,31,0,274,273,1,0,0,0,274,
-        275,1,0,0,0,275,280,1,0,0,0,276,279,5,55,0,0,277,279,3,62,31,0,278,
-        276,1,0,0,0,278,277,1,0,0,0,279,282,1,0,0,0,280,278,1,0,0,0,280,
-        281,1,0,0,0,281,443,1,0,0,0,282,280,1,0,0,0,283,284,5,19,0,0,284,
-        285,3,62,31,0,285,286,3,62,31,0,286,287,3,62,31,0,287,289,3,62,31,
-        0,288,290,3,62,31,0,289,288,1,0,0,0,289,290,1,0,0,0,290,295,1,0,
-        0,0,291,294,5,55,0,0,292,294,3,62,31,0,293,291,1,0,0,0,293,292,1,
-        0,0,0,294,297,1,0,0,0,295,293,1,0,0,0,295,296,1,0,0,0,296,443,1,
-        0,0,0,297,295,1,0,0,0,298,299,5,20,0,0,299,300,3,62,31,0,300,301,
-        3,62,31,0,301,302,3,62,31,0,302,303,3,62,31,0,303,305,3,62,31,0,
-        304,306,3,62,31,0,305,304,1,0,0,0,305,306,1,0,0,0,306,311,1,0,0,
-        0,307,310,5,55,0,0,308,310,3,62,31,0,309,307,1,0,0,0,309,308,1,0,
-        0,0,310,313,1,0,0,0,311,309,1,0,0,0,311,312,1,0,0,0,312,443,1,0,
-        0,0,313,311,1,0,0,0,314,315,7,4,0,0,315,316,3,62,31,0,316,317,3,
-        62,31,0,317,318,3,62,31,0,318,443,1,0,0,0,319,320,7,5,0,0,320,321,
-        3,62,31,0,321,322,3,62,31,0,322,323,3,62,31,0,323,324,3,62,31,0,
-        324,443,1,0,0,0,325,327,5,24,0,0,326,328,3,62,31,0,327,326,1,0,0,
-        0,328,329,1,0,0,0,329,327,1,0,0,0,329,330,1,0,0,0,330,443,1,0,0,
-        0,331,332,5,28,0,0,332,333,3,62,31,0,333,334,3,62,31,0,334,337,5,
-        55,0,0,335,336,5,29,0,0,336,338,3,62,31,0,337,335,1,0,0,0,337,338,
-        1,0,0,0,338,443,1,0,0,0,339,340,5,30,0,0,340,345,5,50,0,0,341,342,
-        3,62,31,0,342,343,3,62,31,0,343,344,3,62,31,0,344,346,1,0,0,0,345,
-        341,1,0,0,0,346,347,1,0,0,0,347,345,1,0,0,0,347,348,1,0,0,0,348,
-        443,1,0,0,0,349,350,7,6,0,0,350,351,3,62,31,0,351,352,3,62,31,0,
-        352,353,3,62,31,0,353,354,3,62,31,0,354,355,3,62,31,0,355,356,3,
-        62,31,0,356,443,1,0,0,0,357,358,5,32,0,0,358,443,3,62,31,0,359,443,
-        5,33,0,0,360,361,5,34,0,0,361,362,3,62,31,0,362,363,3,50,25,0,363,
-        443,1,0,0,0,364,365,5,35,0,0,365,367,5,50,0,0,366,368,3,50,25,0,
-        367,366,1,0,0,0,368,369,1,0,0,0,369,367,1,0,0,0,369,370,1,0,0,0,
-        370,443,1,0,0,0,371,372,5,36,0,0,372,392,5,55,0,0,373,374,3,62,31,
-        0,374,375,3,62,31,0,375,376,3,62,31,0,376,393,1,0,0,0,377,378,5,
-        37,0,0,378,379,3,62,31,0,379,380,3,62,31,0,380,388,3,62,31,0,381,
-        385,5,55,0,0,382,384,3,62,31,0,383,382,1,0,0,0,384,387,1,0,0,0,385,
-        383,1,0,0,0,385,386,1,0,0,0,386,389,1,0,0,0,387,385,1,0,0,0,388,
-        381,1,0,0,0,389,390,1,0,0,0,390,388,1,0,0,0,390,391,1,0,0,0,391,
-        393,1,0,0,0,392,373,1,0,0,0,392,377,1,0,0,0,393,443,1,0,0,0,394,
-        395,5,38,0,0,395,396,3,62,31,0,396,397,3,62,31,0,397,398,3,62,31,
-        0,398,400,3,62,31,0,399,401,3,62,31,0,400,399,1,0,0,0,400,401,1,
-        0,0,0,401,443,1,0,0,0,402,403,5,41,0,0,403,404,3,62,31,0,404,405,
-        3,62,31,0,405,407,3,62,31,0,406,408,5,42,0,0,407,406,1,0,0,0,407,
-        408,1,0,0,0,408,443,1,0,0,0,409,410,5,47,0,0,410,411,3,62,31,0,411,
-        415,3,62,31,0,412,414,3,62,31,0,413,412,1,0,0,0,414,417,1,0,0,0,
-        415,413,1,0,0,0,415,416,1,0,0,0,416,443,1,0,0,0,417,415,1,0,0,0,
-        418,419,5,48,0,0,419,425,5,50,0,0,420,421,3,62,31,0,421,422,3,62,
-        31,0,422,423,3,62,31,0,423,424,3,62,31,0,424,426,1,0,0,0,425,420,
-        1,0,0,0,426,427,1,0,0,0,427,425,1,0,0,0,427,428,1,0,0,0,428,443,
-        1,0,0,0,429,430,5,49,0,0,430,438,5,50,0,0,431,432,3,62,31,0,432,
-        433,3,62,31,0,433,434,3,62,31,0,434,435,3,62,31,0,435,436,3,62,31,
-        0,436,437,3,62,31,0,437,439,1,0,0,0,438,431,1,0,0,0,439,440,1,0,
-        0,0,440,438,1,0,0,0,440,441,1,0,0,0,441,443,1,0,0,0,442,265,1,0,
-        0,0,442,269,1,0,0,0,442,283,1,0,0,0,442,298,1,0,0,0,442,314,1,0,
-        0,0,442,319,1,0,0,0,442,325,1,0,0,0,442,331,1,0,0,0,442,339,1,0,
-        0,0,442,349,1,0,0,0,442,357,1,0,0,0,442,359,1,0,0,0,442,360,1,0,
-        0,0,442,364,1,0,0,0,442,371,1,0,0,0,442,394,1,0,0,0,442,402,1,0,
-        0,0,442,409,1,0,0,0,442,418,1,0,0,0,442,429,1,0,0,0,443,445,1,0,
-        0,0,444,446,3,2,1,0,445,444,1,0,0,0,445,446,1,0,0,0,446,51,1,0,0,
-        0,447,449,3,54,27,0,448,447,1,0,0,0,449,450,1,0,0,0,450,448,1,0,
-        0,0,450,451,1,0,0,0,451,53,1,0,0,0,452,453,5,50,0,0,453,454,5,55,
-        0,0,454,455,5,50,0,0,455,456,5,55,0,0,456,457,3,60,30,0,457,55,1,
-        0,0,0,458,460,3,58,29,0,459,458,1,0,0,0,460,461,1,0,0,0,461,459,
-        1,0,0,0,461,462,1,0,0,0,462,57,1,0,0,0,463,464,5,50,0,0,464,465,
-        5,50,0,0,465,59,1,0,0,0,466,467,7,7,0,0,467,61,1,0,0,0,468,469,7,
-        7,0,0,469,63,1,0,0,0,42,78,80,89,97,109,123,139,163,178,195,206,
-        218,228,238,244,249,263,274,278,280,289,293,295,305,309,311,329,
-        337,347,369,385,390,392,400,407,415,427,440,442,445,450,461
+        0,9,1,0,60,62,1,1,64,64,2,0,1,2,9,9,1,0,3,4,3,0,18,18,25,25,39,40,
+        3,0,21,22,26,26,46,46,2,0,23,23,43,43,2,0,31,31,44,45,1,0,50,51,
+        519,0,80,1,0,0,0,2,85,1,0,0,0,4,95,1,0,0,0,6,99,1,0,0,0,8,107,1,
+        0,0,0,10,111,1,0,0,0,12,121,1,0,0,0,14,125,1,0,0,0,16,137,1,0,0,
+        0,18,141,1,0,0,0,20,161,1,0,0,0,22,165,1,0,0,0,24,176,1,0,0,0,26,
+        180,1,0,0,0,28,193,1,0,0,0,30,197,1,0,0,0,32,204,1,0,0,0,34,208,
+        1,0,0,0,36,216,1,0,0,0,38,220,1,0,0,0,40,226,1,0,0,0,42,230,1,0,
+        0,0,44,236,1,0,0,0,46,244,1,0,0,0,48,263,1,0,0,0,50,442,1,0,0,0,
+        52,448,1,0,0,0,54,452,1,0,0,0,56,459,1,0,0,0,58,463,1,0,0,0,60,466,
+        1,0,0,0,62,468,1,0,0,0,64,79,3,2,1,0,65,79,3,4,2,0,66,79,3,8,4,0,
+        67,79,3,12,6,0,68,79,3,16,8,0,69,79,3,20,10,0,70,79,3,24,12,0,71,
+        79,3,28,14,0,72,79,3,32,16,0,73,79,3,36,18,0,74,79,3,40,20,0,75,
+        79,3,44,22,0,76,79,3,52,26,0,77,79,3,56,28,0,78,64,1,0,0,0,78,65,
+        1,0,0,0,78,66,1,0,0,0,78,67,1,0,0,0,78,68,1,0,0,0,78,69,1,0,0,0,
+        78,70,1,0,0,0,78,71,1,0,0,0,78,72,1,0,0,0,78,73,1,0,0,0,78,74,1,
+        0,0,0,78,75,1,0,0,0,78,76,1,0,0,0,78,77,1,0,0,0,79,82,1,0,0,0,80,
+        78,1,0,0,0,80,81,1,0,0,0,81,83,1,0,0,0,82,80,1,0,0,0,83,84,5,0,0,
+        1,84,1,1,0,0,0,85,89,5,54,0,0,86,88,7,0,0,0,87,86,1,0,0,0,88,91,
+        1,0,0,0,89,87,1,0,0,0,89,90,1,0,0,0,90,92,1,0,0,0,91,89,1,0,0,0,
+        92,93,7,1,0,0,93,3,1,0,0,0,94,96,3,6,3,0,95,94,1,0,0,0,96,97,1,0,
+        0,0,97,95,1,0,0,0,97,98,1,0,0,0,98,5,1,0,0,0,99,100,7,2,0,0,100,
+        101,5,55,0,0,101,102,5,50,0,0,102,103,5,55,0,0,103,104,5,50,0,0,
+        104,105,3,50,25,0,105,7,1,0,0,0,106,108,3,10,5,0,107,106,1,0,0,0,
+        108,109,1,0,0,0,109,107,1,0,0,0,109,110,1,0,0,0,110,9,1,0,0,0,111,
+        112,7,3,0,0,112,113,5,55,0,0,113,114,5,50,0,0,114,115,5,55,0,0,115,
+        116,5,50,0,0,116,117,5,55,0,0,117,118,5,50,0,0,118,119,3,50,25,0,
+        119,11,1,0,0,0,120,122,3,14,7,0,121,120,1,0,0,0,122,123,1,0,0,0,
+        123,121,1,0,0,0,123,124,1,0,0,0,124,13,1,0,0,0,125,126,5,5,0,0,126,
+        127,5,55,0,0,127,128,5,50,0,0,128,129,5,55,0,0,129,130,5,50,0,0,
+        130,131,5,55,0,0,131,132,5,50,0,0,132,133,5,55,0,0,133,134,5,50,
+        0,0,134,135,3,50,25,0,135,15,1,0,0,0,136,138,3,18,9,0,137,136,1,
+        0,0,0,138,139,1,0,0,0,139,137,1,0,0,0,139,140,1,0,0,0,140,17,1,0,
+        0,0,141,142,5,6,0,0,142,143,5,55,0,0,143,144,5,50,0,0,144,145,5,
+        55,0,0,145,146,5,50,0,0,146,147,5,55,0,0,147,148,5,50,0,0,148,149,
+        5,55,0,0,149,150,5,50,0,0,150,151,5,55,0,0,151,152,5,50,0,0,152,
+        153,5,55,0,0,153,154,5,50,0,0,154,155,5,55,0,0,155,156,5,50,0,0,
+        156,157,5,55,0,0,157,158,5,50,0,0,158,159,3,50,25,0,159,19,1,0,0,
+        0,160,162,3,22,11,0,161,160,1,0,0,0,162,163,1,0,0,0,163,161,1,0,
+        0,0,163,164,1,0,0,0,164,21,1,0,0,0,165,166,5,7,0,0,166,167,5,55,
+        0,0,167,168,5,55,0,0,168,169,5,55,0,0,169,170,5,55,0,0,170,171,3,
+        60,30,0,171,172,3,60,30,0,172,173,3,60,30,0,173,174,3,50,25,0,174,
+        23,1,0,0,0,175,177,3,26,13,0,176,175,1,0,0,0,177,178,1,0,0,0,178,
+        176,1,0,0,0,178,179,1,0,0,0,179,25,1,0,0,0,180,181,5,8,0,0,181,182,
+        5,55,0,0,182,183,5,50,0,0,183,184,5,55,0,0,184,185,5,55,0,0,185,
+        186,5,55,0,0,186,187,5,50,0,0,187,188,3,60,30,0,188,189,3,60,30,
+        0,189,190,3,60,30,0,190,191,3,50,25,0,191,27,1,0,0,0,192,194,3,30,
+        15,0,193,192,1,0,0,0,194,195,1,0,0,0,195,193,1,0,0,0,195,196,1,0,
+        0,0,196,29,1,0,0,0,197,198,5,10,0,0,198,199,5,55,0,0,199,200,5,50,
+        0,0,200,201,5,55,0,0,201,202,3,50,25,0,202,31,1,0,0,0,203,205,3,
+        34,17,0,204,203,1,0,0,0,205,206,1,0,0,0,206,204,1,0,0,0,206,207,
+        1,0,0,0,207,33,1,0,0,0,208,209,5,11,0,0,209,210,5,50,0,0,210,211,
+        5,55,0,0,211,212,5,50,0,0,212,213,5,50,0,0,213,214,3,50,25,0,214,
+        35,1,0,0,0,215,217,3,38,19,0,216,215,1,0,0,0,217,218,1,0,0,0,218,
+        216,1,0,0,0,218,219,1,0,0,0,219,37,1,0,0,0,220,221,5,12,0,0,221,
+        222,5,50,0,0,222,223,5,50,0,0,223,224,3,60,30,0,224,39,1,0,0,0,225,
+        227,3,42,21,0,226,225,1,0,0,0,227,228,1,0,0,0,228,226,1,0,0,0,228,
+        229,1,0,0,0,229,41,1,0,0,0,230,231,5,13,0,0,231,232,5,50,0,0,232,
+        233,5,55,0,0,233,234,3,60,30,0,234,43,1,0,0,0,235,237,3,46,23,0,
+        236,235,1,0,0,0,237,238,1,0,0,0,238,236,1,0,0,0,238,239,1,0,0,0,
+        239,45,1,0,0,0,240,245,5,14,0,0,241,245,5,15,0,0,242,243,5,16,0,
+        0,243,245,5,50,0,0,244,240,1,0,0,0,244,241,1,0,0,0,244,242,1,0,0,
+        0,245,247,1,0,0,0,246,248,3,48,24,0,247,246,1,0,0,0,248,249,1,0,
+        0,0,249,247,1,0,0,0,249,250,1,0,0,0,250,251,1,0,0,0,251,252,5,17,
+        0,0,252,47,1,0,0,0,253,264,3,6,3,0,254,264,3,10,5,0,255,264,3,14,
+        7,0,256,264,3,18,9,0,257,264,3,22,11,0,258,264,3,26,13,0,259,264,
+        3,30,15,0,260,264,3,34,17,0,261,264,3,38,19,0,262,264,3,42,21,0,
+        263,253,1,0,0,0,263,254,1,0,0,0,263,255,1,0,0,0,263,256,1,0,0,0,
+        263,257,1,0,0,0,263,258,1,0,0,0,263,259,1,0,0,0,263,260,1,0,0,0,
+        263,261,1,0,0,0,263,262,1,0,0,0,264,49,1,0,0,0,265,266,7,4,0,0,266,
+        267,3,62,31,0,267,268,3,62,31,0,268,443,1,0,0,0,269,270,5,27,0,0,
+        270,271,3,62,31,0,271,272,3,62,31,0,272,274,3,62,31,0,273,275,3,
+        62,31,0,274,273,1,0,0,0,274,275,1,0,0,0,275,280,1,0,0,0,276,279,
+        5,55,0,0,277,279,3,62,31,0,278,276,1,0,0,0,278,277,1,0,0,0,279,282,
+        1,0,0,0,280,278,1,0,0,0,280,281,1,0,0,0,281,443,1,0,0,0,282,280,
+        1,0,0,0,283,284,5,19,0,0,284,285,3,62,31,0,285,286,3,62,31,0,286,
+        287,3,62,31,0,287,289,3,62,31,0,288,290,3,62,31,0,289,288,1,0,0,
+        0,289,290,1,0,0,0,290,295,1,0,0,0,291,294,5,55,0,0,292,294,3,62,
+        31,0,293,291,1,0,0,0,293,292,1,0,0,0,294,297,1,0,0,0,295,293,1,0,
+        0,0,295,296,1,0,0,0,296,443,1,0,0,0,297,295,1,0,0,0,298,299,5,20,
+        0,0,299,300,3,62,31,0,300,301,3,62,31,0,301,302,3,62,31,0,302,303,
+        3,62,31,0,303,305,3,62,31,0,304,306,3,62,31,0,305,304,1,0,0,0,305,
+        306,1,0,0,0,306,311,1,0,0,0,307,310,5,55,0,0,308,310,3,62,31,0,309,
+        307,1,0,0,0,309,308,1,0,0,0,310,313,1,0,0,0,311,309,1,0,0,0,311,
+        312,1,0,0,0,312,443,1,0,0,0,313,311,1,0,0,0,314,315,7,5,0,0,315,
+        316,3,62,31,0,316,317,3,62,31,0,317,318,3,62,31,0,318,443,1,0,0,
+        0,319,320,7,6,0,0,320,321,3,62,31,0,321,322,3,62,31,0,322,323,3,
+        62,31,0,323,324,3,62,31,0,324,443,1,0,0,0,325,327,5,24,0,0,326,328,
+        3,62,31,0,327,326,1,0,0,0,328,329,1,0,0,0,329,327,1,0,0,0,329,330,
+        1,0,0,0,330,443,1,0,0,0,331,332,5,28,0,0,332,333,3,62,31,0,333,334,
+        3,62,31,0,334,337,5,55,0,0,335,336,5,29,0,0,336,338,3,62,31,0,337,
+        335,1,0,0,0,337,338,1,0,0,0,338,443,1,0,0,0,339,340,5,30,0,0,340,
+        345,5,50,0,0,341,342,3,62,31,0,342,343,3,62,31,0,343,344,3,62,31,
+        0,344,346,1,0,0,0,345,341,1,0,0,0,346,347,1,0,0,0,347,345,1,0,0,
+        0,347,348,1,0,0,0,348,443,1,0,0,0,349,350,7,7,0,0,350,351,3,62,31,
+        0,351,352,3,62,31,0,352,353,3,62,31,0,353,354,3,62,31,0,354,355,
+        3,62,31,0,355,356,3,62,31,0,356,443,1,0,0,0,357,358,5,32,0,0,358,
+        443,3,62,31,0,359,443,5,33,0,0,360,361,5,34,0,0,361,362,3,62,31,
+        0,362,363,3,50,25,0,363,443,1,0,0,0,364,365,5,35,0,0,365,367,5,50,
+        0,0,366,368,3,50,25,0,367,366,1,0,0,0,368,369,1,0,0,0,369,367,1,
+        0,0,0,369,370,1,0,0,0,370,443,1,0,0,0,371,372,5,36,0,0,372,392,5,
+        55,0,0,373,374,3,62,31,0,374,375,3,62,31,0,375,376,3,62,31,0,376,
+        393,1,0,0,0,377,378,5,37,0,0,378,379,3,62,31,0,379,380,3,62,31,0,
+        380,388,3,62,31,0,381,385,5,55,0,0,382,384,3,62,31,0,383,382,1,0,
+        0,0,384,387,1,0,0,0,385,383,1,0,0,0,385,386,1,0,0,0,386,389,1,0,
+        0,0,387,385,1,0,0,0,388,381,1,0,0,0,389,390,1,0,0,0,390,388,1,0,
+        0,0,390,391,1,0,0,0,391,393,1,0,0,0,392,373,1,0,0,0,392,377,1,0,
+        0,0,393,443,1,0,0,0,394,395,5,38,0,0,395,396,3,62,31,0,396,397,3,
+        62,31,0,397,398,3,62,31,0,398,400,3,62,31,0,399,401,3,62,31,0,400,
+        399,1,0,0,0,400,401,1,0,0,0,401,443,1,0,0,0,402,403,5,41,0,0,403,
+        404,3,62,31,0,404,405,3,62,31,0,405,407,3,62,31,0,406,408,5,42,0,
+        0,407,406,1,0,0,0,407,408,1,0,0,0,408,443,1,0,0,0,409,410,5,47,0,
+        0,410,411,3,62,31,0,411,415,3,62,31,0,412,414,3,62,31,0,413,412,
+        1,0,0,0,414,417,1,0,0,0,415,413,1,0,0,0,415,416,1,0,0,0,416,443,
+        1,0,0,0,417,415,1,0,0,0,418,419,5,48,0,0,419,425,5,50,0,0,420,421,
+        3,62,31,0,421,422,3,62,31,0,422,423,3,62,31,0,423,424,3,62,31,0,
+        424,426,1,0,0,0,425,420,1,0,0,0,426,427,1,0,0,0,427,425,1,0,0,0,
+        427,428,1,0,0,0,428,443,1,0,0,0,429,430,5,49,0,0,430,438,5,50,0,
+        0,431,432,3,62,31,0,432,433,3,62,31,0,433,434,3,62,31,0,434,435,
+        3,62,31,0,435,436,3,62,31,0,436,437,3,62,31,0,437,439,1,0,0,0,438,
+        431,1,0,0,0,439,440,1,0,0,0,440,438,1,0,0,0,440,441,1,0,0,0,441,
+        443,1,0,0,0,442,265,1,0,0,0,442,269,1,0,0,0,442,283,1,0,0,0,442,
+        298,1,0,0,0,442,314,1,0,0,0,442,319,1,0,0,0,442,325,1,0,0,0,442,
+        331,1,0,0,0,442,339,1,0,0,0,442,349,1,0,0,0,442,357,1,0,0,0,442,
+        359,1,0,0,0,442,360,1,0,0,0,442,364,1,0,0,0,442,371,1,0,0,0,442,
+        394,1,0,0,0,442,402,1,0,0,0,442,409,1,0,0,0,442,418,1,0,0,0,442,
+        429,1,0,0,0,443,445,1,0,0,0,444,446,3,2,1,0,445,444,1,0,0,0,445,
+        446,1,0,0,0,446,51,1,0,0,0,447,449,3,54,27,0,448,447,1,0,0,0,449,
+        450,1,0,0,0,450,448,1,0,0,0,450,451,1,0,0,0,451,53,1,0,0,0,452,453,
+        5,50,0,0,453,454,5,55,0,0,454,455,5,50,0,0,455,456,5,55,0,0,456,
+        457,3,60,30,0,457,55,1,0,0,0,458,460,3,58,29,0,459,458,1,0,0,0,460,
+        461,1,0,0,0,461,459,1,0,0,0,461,462,1,0,0,0,462,57,1,0,0,0,463,464,
+        5,50,0,0,464,465,5,50,0,0,465,59,1,0,0,0,466,467,7,8,0,0,467,61,
+        1,0,0,0,468,469,7,8,0,0,469,63,1,0,0,0,42,78,80,89,97,109,123,139,
+        163,178,195,206,218,228,238,244,249,263,274,278,280,289,293,295,
+        305,309,311,329,337,347,369,385,390,392,400,407,415,427,440,442,
+        445,450,461
     ]
 
 class RosettaMRParser ( Parser ):
 
     grammarFileName = "RosettaMRParser.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
@@ -584,14 +585,17 @@
 
         def COMMENT(self):
             return self.getToken(RosettaMRParser.COMMENT, 0)
 
         def RETURN_CM(self):
             return self.getToken(RosettaMRParser.RETURN_CM, 0)
 
+        def EOF(self):
+            return self.getToken(RosettaMRParser.EOF, 0)
+
         def Atom_pair_selection(self, i:int=None):
             if i is None:
                 return self.getTokens(RosettaMRParser.Atom_pair_selection)
             else:
                 return self.getToken(RosettaMRParser.Atom_pair_selection, i)
 
         def Atom_selection(self, i:int=None):
@@ -641,15 +645,20 @@
                     self._errHandler.reportMatch(self)
                     self.consume()
                 self.state = 91
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
             self.state = 92
-            self.match(RosettaMRParser.RETURN_CM)
+            _la = self._input.LA(1)
+            if not(_la==-1 or _la==64):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
```

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/RosettaMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/RosettaMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/SybylMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/SybylMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/SybylMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/SybylMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/XplorMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/XplorMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/XplorMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/mr/XplorMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb/utils/nmr/rci/RCI.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/RCI.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/PKG-INFO` & `wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.nmr
-Version: 0.27
+Version: 0.28.dev1
 Summary: wwPDB NMR utilities
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_nmr
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.nmr-0.27/wwpdb.utils.nmr.egg-info/SOURCES.txt` & `wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

