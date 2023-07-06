# Comparing `tmp/tmkit-0.0.0.2.tar.gz` & `tmp/tmkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmkit-0.0.0.2.tar", last modified: Mon Jun 19 23:19:13 2023, max compression
+gzip compressed data, was "tmkit-0.0.2.tar", last modified: Thu Jul  6 18:43:43 2023, max compression
```

## Comparing `tmkit-0.0.0.2.tar` & `tmkit-0.0.2.tar`

### file list

```diff
@@ -1,195 +1,182 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.635598 tmkit-0.0.0.2/
--rw-rw-rw-   0        0        0    35823 2022-10-06 19:26:08.000000 tmkit-0.0.0.2/LICENSE
--rw-rw-rw-   0        0        0      302 2023-06-19 23:19:13.633599 tmkit-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1506 2023-03-29 23:16:56.000000 tmkit-0.0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 23:19:13.636599 tmkit-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      715 2023-06-19 23:18:35.000000 tmkit-0.0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.258597 tmkit-0.0.0.2/tmkit/
--rw-rw-rw-   0        0        0      458 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/Path.py
--rw-rw-rw-   0        0        0     4375 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/SeqNetRR.py
--rw-rw-rw-   0        0        0      261 2023-06-19 23:18:35.000000 tmkit-0.0.0.2/tmkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.287598 tmkit-0.0.0.2/tmkit/base/
--rw-rw-rw-   0        0        0     2936 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/base/PDB.py
--rw-rw-rw-   0        0        0     1004 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/base/Position.py
--rw-rw-rw-   0        0        0       76 2019-09-15 16:59:06.000000 tmkit-0.0.0.2/tmkit/base/__init__.py
--rw-rw-rw-   0        0        0     2114 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/cath.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.302625 tmkit-0.0.0.2/tmkit/chain/
--rw-rw-rw-   0        0        0     5301 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/chain/Collate.py
--rw-rw-rw-   0        0        0     8052 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/chain/CollateBatch.py
--rw-rw-rw-   0        0        0      599 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/chain/PDB.py
--rw-rw-rw-   0        0        0        0 2022-08-06 11:29:10.000000 tmkit-0.0.0.2/tmkit/chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.307627 tmkit-0.0.0.2/tmkit/channel/
--rw-rw-rw-   0        0        0     7568 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/channel/Workbench.py
--rw-rw-rw-   0        0        0        0 2019-08-11 19:08:40.000000 tmkit-0.0.0.2/tmkit/channel/__init__.py
--rw-rw-rw-   0        0        0     3047 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/collate.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.316600 tmkit-0.0.0.2/tmkit/contact/
--rw-rw-rw-   0        0        0     7971 2023-06-19 13:33:30.000000 tmkit-0.0.0.2/tmkit/contact/Evaluator.py
--rw-rw-rw-   0        0        0    24790 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/contact/Reader.py
--rw-rw-rw-   0        0        0        0 2019-08-11 18:38:08.000000 tmkit-0.0.0.2/tmkit/contact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.324598 tmkit-0.0.0.2/tmkit/db/
--rw-rw-rw-   0        0        0     7934 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/db/Connectivity.py
--rw-rw-rw-   0        0        0     3676 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/db/Reader.py
--rw-rw-rw-   0        0        0        0 2019-05-10 13:10:28.000000 tmkit-0.0.0.2/tmkit/db/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.329597 tmkit-0.0.0.2/tmkit/db/biogrid/
--rw-rw-rw-   0        0        0     1710 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/biogrid/Reader.py
--rw-rw-rw-   0        0        0        0 2020-07-08 14:38:06.000000 tmkit-0.0.0.2/tmkit/db/biogrid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.334596 tmkit-0.0.0.2/tmkit/db/cath/
--rw-rw-rw-   0        0        0     5065 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/cath/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-11 11:28:12.000000 tmkit-0.0.0.2/tmkit/db/cath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.339598 tmkit-0.0.0.2/tmkit/db/construct/
--rw-rw-rw-   0        0        0     3320 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/construct/Network.py
--rw-rw-rw-   0        0        0        0 2020-08-28 22:57:35.000000 tmkit-0.0.0.2/tmkit/db/construct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.344596 tmkit-0.0.0.2/tmkit/db/intact/
--rw-rw-rw-   0        0        0     2075 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/intact/Reader.py
--rw-rw-rw-   0        0        0        0 2020-07-11 22:05:59.000000 tmkit-0.0.0.2/tmkit/db/intact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.350596 tmkit-0.0.0.2/tmkit/db/muthtp/
--rw-rw-rw-   0        0        0     3703 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/muthtp/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-07 05:11:20.000000 tmkit-0.0.0.2/tmkit/db/muthtp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.355597 tmkit-0.0.0.2/tmkit/db/predmuthtp/
--rw-rw-rw-   0        0        0     2939 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/predmuthtp/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-07 05:11:42.000000 tmkit-0.0.0.2/tmkit/db/predmuthtp/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/edge.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.361599 tmkit-0.0.0.2/tmkit/feature/
--rw-rw-rw-   0        0        0     8018 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/feature/HelixSurface.py
--rw-rw-rw-   0        0        0        0 2022-07-15 21:53:29.000000 tmkit-0.0.0.2/tmkit/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.363597 tmkit-0.0.0.2/tmkit/feature/lips/
--rw-rw-rw-   0        0        0        0 2019-08-01 10:52:35.000000 tmkit-0.0.0.2/tmkit/feature/lips/__init__.py
--rw-rw-rw-   0        0        0     9415 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/feature.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.375596 tmkit-0.0.0.2/tmkit/id/
--rw-rw-rw-   0        0        0      568 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/id/Fasta.py
--rw-rw-rw-   0        0        0     2717 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/id/Mapping.py
--rw-rw-rw-   0        0        0     1035 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/id/PDB.py
--rw-rw-rw-   0        0        0        0 2020-04-26 23:07:36.000000 tmkit-0.0.0.2/tmkit/id/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.385598 tmkit-0.0.0.2/tmkit/interface/
--rw-rw-rw-   0        0        0      387 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/interface/Tool.py
--rw-rw-rw-   0        0        0      398 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/interface/Topology.py
--rw-rw-rw-   0        0        0        0 2020-07-09 17:22:43.000000 tmkit-0.0.0.2/tmkit/interface/__init__.py
--rw-rw-rw-   0        0        0      811 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/mapping.py
--rw-rw-rw-   0        0        0     6409 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/msa.py
--rw-rw-rw-   0        0        0     1928 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/mut.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.390596 tmkit-0.0.0.2/tmkit/name/
--rw-rw-rw-   0        0        0     4437 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/name/Mapping.py
--rw-rw-rw-   0        0        0        0 2022-08-06 12:13:25.000000 tmkit-0.0.0.2/tmkit/name/__init__.py
--rw-rw-rw-   0        0        0        0 2022-07-16 21:39:03.000000 tmkit-0.0.0.2/tmkit/pl.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.392596 tmkit-0.0.0.2/tmkit/position/
--rw-rw-rw-   0        0        0       16 2019-09-15 17:43:20.000000 tmkit-0.0.0.2/tmkit/position/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.401596 tmkit-0.0.0.2/tmkit/position/scenario/
--rw-rw-rw-   0        0        0     1724 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/position/scenario/Segment.py
--rw-rw-rw-   0        0        0     2421 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/position/scenario/Separation.py
--rw-rw-rw-   0        0        0        0 2019-09-21 21:40:26.000000 tmkit-0.0.0.2/tmkit/position/scenario/__init__.py
--rw-rw-rw-   0        0        0     4938 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/ppi.py
--rw-rw-rw-   0        0        0     2260 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/qc.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.412598 tmkit-0.0.0.2/tmkit/retrieve/
--rw-rw-rw-   0        0        0    15864 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/retrieve/MSA.py
--rw-rw-rw-   0        0        0     3976 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/retrieve/PDB.py
--rw-rw-rw-   0        0        0     2142 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/retrieve/XML.py
--rw-rw-rw-   0        0        0        0 2019-05-10 15:10:49.000000 tmkit-0.0.0.2/tmkit/retrieve/__init__.py
--rw-rw-rw-   0        0        0     5100 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/rrc.py
--rw-rw-rw-   0        0        0     4126 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seq.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.427598 tmkit-0.0.0.2/tmkit/seqnetrr/
--rw-rw-rw-   0        0        0     9679 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/Compare.py
--rw-rw-rw-   0        0        0    13327 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/Controller.py
--rw-rw-rw-   0        0        0      491 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/Path.py
--rw-rw-rw-   0        0        0    34474 2022-10-06 14:12:35.000000 tmkit-0.0.0.2/tmkit/seqnetrr/Plot.py
--rw-rw-rw-   0        0        0        0 2022-05-17 20:55:49.000000 tmkit-0.0.0.2/tmkit/seqnetrr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.442597 tmkit-0.0.0.2/tmkit/seqnetrr/combo/
--rw-rw-rw-   0        0        0     2183 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/Length.py
--rw-rw-rw-   0        0        0      470 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/Param.py
--rw-rw-rw-   0        0        0     1676 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/Position.py
--rw-rw-rw-   0        0        0     2494 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/Separation.py
--rw-rw-rw-   0        0        0        0 2019-08-11 16:35:38.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.452597 tmkit-0.0.0.2/tmkit/seqnetrr/graph/
--rw-rw-rw-   0        0        0    19034 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/graph/Bipartite.py
--rw-rw-rw-   0        0        0     4855 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/graph/Cumulative.py
--rw-rw-rw-   0        0        0    21160 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/graph/Unipartite.py
--rw-rw-rw-   0        0        0        0 2022-05-18 21:29:35.000000 tmkit-0.0.0.2/tmkit/seqnetrr/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.458632 tmkit-0.0.0.2/tmkit/seqnetrr/net/
--rw-rw-rw-   0        0        0    25261 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/net/Reader.py
--rw-rw-rw-   0        0        0        0 2022-06-12 23:19:50.000000 tmkit-0.0.0.2/tmkit/seqnetrr/net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.462630 tmkit-0.0.0.2/tmkit/seqnetrr/sequence/
--rw-rw-rw-   0        0        0     1965 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/sequence/Fasta.py
--rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.0.2/tmkit/seqnetrr/sequence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.476624 tmkit-0.0.0.2/tmkit/seqnetrr/util/
--rw-rw-rw-   0        0        0     5609 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/ComputLib.py
--rw-rw-rw-   0        0        0      838 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/Console.py
--rw-rw-rw-   0        0        0     2866 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/Reader.py
--rw-rw-rw-   0        0        0     2201 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/Writer.py
--rw-rw-rw-   0        0        0        0 2022-05-18 16:43:31.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.484597 tmkit-0.0.0.2/tmkit/seqnetrr/window/
--rw-rw-rw-   0        0        0     5855 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/Pair.py
--rw-rw-rw-   0        0        0     5780 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/Single.py
--rw-rw-rw-   0        0        0        0 2019-09-18 20:19:22.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.492598 tmkit-0.0.0.2/tmkit/seqnetrr/window/base/
--rw-rw-rw-   0        0        0     1316 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/base/Pair.py
--rw-rw-rw-   0        0        0     1318 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/base/Single.py
--rw-rw-rw-   0        0        0        0 2019-09-19 13:22:58.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.508597 tmkit-0.0.0.2/tmkit/sequence/
--rw-rw-rw-   0        0        0      590 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/sequence/Fasta.py
--rw-rw-rw-   0        0        0      454 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/sequence/Index.py
--rw-rw-rw-   0        0        0     2052 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/sequence/PDB.py
--rw-rw-rw-   0        0        0     1685 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/sequence/XML.py
--rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.0.2/tmkit/sequence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.514597 tmkit-0.0.0.2/tmkit/structure/
--rw-rw-rw-   0        0        0      578 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/structure/PDB.py
--rw-rw-rw-   0        0        0        0 2019-08-02 11:11:48.000000 tmkit-0.0.0.2/tmkit/structure/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.521603 tmkit-0.0.0.2/tmkit/structure/ppi/
--rw-rw-rw-   0        0        0     1451 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/structure/ppi/Label.py
--rw-rw-rw-   0        0        0        0 2019-09-15 17:30:37.000000 tmkit-0.0.0.2/tmkit/structure/ppi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.526598 tmkit-0.0.0.2/tmkit/structure/rrc/
--rw-rw-rw-   0        0        0     1811 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/structure/rrc/Label.py
--rw-rw-rw-   0        0        0        0 2019-09-15 17:30:31.000000 tmkit-0.0.0.2/tmkit/structure/rrc/__init__.py
--rw-rw-rw-   0        0        0     5542 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topo.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.533629 tmkit-0.0.0.2/tmkit/topology/
--rw-rw-rw-   0        0        0     4387 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/Phobius.py
--rw-rw-rw-   0        0        0     7728 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/TMHMM.py
--rw-rw-rw-   0        0        0        0 2019-05-10 13:11:26.000000 tmkit-0.0.0.2/tmkit/topology/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.537612 tmkit-0.0.0.2/tmkit/topology/lib/
--rw-rw-rw-   0        0        0    25043 2022-07-15 23:01:47.000000 tmkit-0.0.0.2/tmkit/topology/lib/Phobius.py
--rw-rw-rw-   0        0        0        0 2022-07-16 23:17:45.000000 tmkit-0.0.0.2/tmkit/topology/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.553631 tmkit-0.0.0.2/tmkit/topology/pdbtm/
--rw-rw-rw-   0        0        0     4886 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/Component.py
--rw-rw-rw-   0        0        0     3293 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/Determine.py
--rw-rw-rw-   0        0        0     3737 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/Segment.py
--rw-rw-rw-   0        0        0     1683 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/TMH.py
--rw-rw-rw-   0        0        0     2224 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/ToFastaId.py
--rw-rw-rw-   0        0        0        0 2019-11-07 10:51:46.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.565627 tmkit-0.0.0.2/tmkit/util/
--rw-rw-rw-   0        0        0      890 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/util/Console.py
--rw-rw-rw-   0        0        0     4073 2023-06-19 11:34:17.000000 tmkit-0.0.0.2/tmkit/util/Kit.py
--rw-rw-rw-   0        0        0     2948 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/util/Reader.py
--rw-rw-rw-   0        0        0     1272 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/util/Writer.py
--rw-rw-rw-   0        0        0        0 2022-07-15 19:58:41.000000 tmkit-0.0.0.2/tmkit/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.567629 tmkit-0.0.0.2/tmkit/visualize/
--rw-rw-rw-   0        0        0        0 2022-08-07 22:43:33.000000 tmkit-0.0.0.2/tmkit/visualize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.572597 tmkit-0.0.0.2/tmkit/visualize/func/
--rw-rw-rw-   0        0        0     2028 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/func/Coloring.py
--rw-rw-rw-   0        0        0        0 2022-08-11 11:29:35.000000 tmkit-0.0.0.2/tmkit/visualize/func/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.581602 tmkit-0.0.0.2/tmkit/visualize/isite/
--rw-rw-rw-   0        0        0     5480 2023-06-19 11:53:42.000000 tmkit-0.0.0.2/tmkit/visualize/isite/Labelling.py
--rw-rw-rw-   0        0        0     3958 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/visualize/isite/ProtocolDeepTMInter.py
--rw-rw-rw-   0        0        0        0 2020-12-31 08:21:51.000000 tmkit-0.0.0.2/tmkit/visualize/isite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.600603 tmkit-0.0.0.2/tmkit/visualize/lib/
--rw-rw-rw-   0        0        0      394 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/lib/Color.py
--rw-rw-rw-   0        0        0     3872 2021-01-03 13:07:00.000000 tmkit-0.0.0.2/tmkit/visualize/lib/InterfaceResidues.py
--rw-rw-rw-   0        0        0      418 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/lib/Select.py
--rw-rw-rw-   0        0        0        0 2022-07-20 21:45:22.000000 tmkit-0.0.0.2/tmkit/visualize/lib/__init__.py
--rw-rw-rw-   0        0        0     2955 2022-07-21 00:23:12.000000 tmkit-0.0.0.2/tmkit/visualize/lib/focal_blur.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.608598 tmkit-0.0.0.2/tmkit/visualize/lib/palette/
--rw-rw-rw-   0        0        0        0 2022-08-11 11:29:11.000000 tmkit-0.0.0.2/tmkit/visualize/lib/palette/__init__.py
--rw-rw-rw-   0        0        0     8267 2021-02-09 21:44:23.000000 tmkit-0.0.0.2/tmkit/visualize/lib/palette/data2bfactor.py
--rw-rw-rw-   0        0        0     3582 2021-02-09 22:35:52.000000 tmkit-0.0.0.2/tmkit/visualize/lib/palette/spectrumany.py
--rw-rw-rw-   0        0        0    14191 2022-07-15 18:10:13.000000 tmkit-0.0.0.2/tmkit/visualize/lib/show_contacts.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.631598 tmkit-0.0.0.2/tmkit/visualize/small/
--rw-rw-rw-   0        0        0      697 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/visualize/small/Label.py
--rw-rw-rw-   0        0        0     2579 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/small/Local.py
--rw-rw-rw-   0        0        0      471 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/small/Palette.py
--rw-rw-rw-   0        0        0      678 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/visualize/small/Select.py
--rw-rw-rw-   0        0        0      217 2022-08-07 23:17:31.000000 tmkit-0.0.0.2/tmkit/visualize/small/Style.py
--rw-rw-rw-   0        0        0        0 2021-01-01 12:44:05.000000 tmkit-0.0.0.2/tmkit/visualize/small/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-06-19 13:41:00.000000 tmkit-0.0.0.2/tmkit/vs.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.277627 tmkit-0.0.0.2/tmkit.egg-info/
--rw-rw-rw-   0        0        0      302 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3999 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.233837 tmkit-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2022-10-06 19:26:08.000000 tmkit-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      300 2023-07-06 18:43:43.230837 tmkit-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1437 2023-07-06 18:01:52.000000 tmkit-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 18:43:43.233837 tmkit-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      712 2023-07-06 18:43:38.000000 tmkit-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.859837 tmkit-0.0.2/tmkit/
+-rw-rw-rw-   0        0        0      458 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/Path.py
+-rw-rw-rw-   0        0        0     1169 2023-07-03 17:00:04.000000 tmkit-0.0.2/tmkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.889838 tmkit-0.0.2/tmkit/base/
+-rw-rw-rw-   0        0        0     3169 2023-07-03 17:00:04.000000 tmkit-0.0.2/tmkit/base/PDB.py
+-rw-rw-rw-   0        0        0      996 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/base/Position.py
+-rw-rw-rw-   0        0        0       76 2019-09-15 16:59:06.000000 tmkit-0.0.2/tmkit/base/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/cath.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.904837 tmkit-0.0.2/tmkit/chain/
+-rw-rw-rw-   0        0        0     4217 2023-07-06 12:47:01.000000 tmkit-0.0.2/tmkit/chain/Collate.py
+-rw-rw-rw-   0        0        0     6767 2023-07-06 12:46:03.000000 tmkit-0.0.2/tmkit/chain/CollateBatch.py
+-rw-rw-rw-   0        0        0      599 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/chain/PDB.py
+-rw-rw-rw-   0        0        0        0 2022-08-06 11:29:10.000000 tmkit-0.0.2/tmkit/chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.910837 tmkit-0.0.2/tmkit/channel/
+-rw-rw-rw-   0        0        0     6299 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/channel/Workbench.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 19:08:40.000000 tmkit-0.0.2/tmkit/channel/__init__.py
+-rw-rw-rw-   0        0        0     1807 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/collate.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.919836 tmkit-0.0.2/tmkit/contact/
+-rw-rw-rw-   0        0        0     7748 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/contact/Evaluator.py
+-rw-rw-rw-   0        0        0    24764 2023-07-02 17:52:28.000000 tmkit-0.0.2/tmkit/contact/Reader.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 18:38:08.000000 tmkit-0.0.2/tmkit/contact/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.927835 tmkit-0.0.2/tmkit/db/
+-rw-rw-rw-   0        0        0     6480 2023-07-04 23:50:26.000000 tmkit-0.0.2/tmkit/db/Connectivity.py
+-rw-rw-rw-   0        0        0     3438 2023-06-29 21:49:55.000000 tmkit-0.0.2/tmkit/db/Reader.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 13:10:28.000000 tmkit-0.0.2/tmkit/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.933869 tmkit-0.0.2/tmkit/db/biogrid/
+-rw-rw-rw-   0        0        0     1902 2023-07-02 19:30:12.000000 tmkit-0.0.2/tmkit/db/biogrid/Reader.py
+-rw-rw-rw-   0        0        0        0 2020-07-08 14:38:06.000000 tmkit-0.0.2/tmkit/db/biogrid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.940836 tmkit-0.0.2/tmkit/db/cath/
+-rw-rw-rw-   0        0        0     4864 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/db/cath/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-11 11:28:12.000000 tmkit-0.0.2/tmkit/db/cath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.945836 tmkit-0.0.2/tmkit/db/construct/
+-rw-rw-rw-   0        0        0     3077 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/db/construct/Network.py
+-rw-rw-rw-   0        0        0        0 2020-08-28 22:57:35.000000 tmkit-0.0.2/tmkit/db/construct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.950837 tmkit-0.0.2/tmkit/db/intact/
+-rw-rw-rw-   0        0        0     2497 2023-07-02 19:38:00.000000 tmkit-0.0.2/tmkit/db/intact/Reader.py
+-rw-rw-rw-   0        0        0        0 2020-07-11 22:05:59.000000 tmkit-0.0.2/tmkit/db/intact/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.956836 tmkit-0.0.2/tmkit/db/muthtp/
+-rw-rw-rw-   0        0        0     4168 2023-07-02 19:38:00.000000 tmkit-0.0.2/tmkit/db/muthtp/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-07 05:11:20.000000 tmkit-0.0.2/tmkit/db/muthtp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.960836 tmkit-0.0.2/tmkit/db/predmuthtp/
+-rw-rw-rw-   0        0        0     2911 2023-07-02 19:59:20.000000 tmkit-0.0.2/tmkit/db/predmuthtp/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-07 05:11:42.000000 tmkit-0.0.2/tmkit/db/predmuthtp/__init__.py
+-rw-rw-rw-   0        0        0      979 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/edge.py
+-rw-rw-rw-   0        0        0     3053 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/feature.py
+-rw-rw-rw-   0        0        0      450 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/fetch.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.972836 tmkit-0.0.2/tmkit/id/
+-rw-rw-rw-   0        0        0      525 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/id/Fasta.py
+-rw-rw-rw-   0        0        0     2476 2023-07-05 23:15:24.000000 tmkit-0.0.2/tmkit/id/Mapping.py
+-rw-rw-rw-   0        0        0     1035 2023-06-19 10:50:52.000000 tmkit-0.0.2/tmkit/id/PDB.py
+-rw-rw-rw-   0        0        0        0 2020-04-26 23:07:36.000000 tmkit-0.0.2/tmkit/id/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.984839 tmkit-0.0.2/tmkit/interface/
+-rw-rw-rw-   0        0        0      387 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/interface/Tool.py
+-rw-rw-rw-   0        0        0      398 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/interface/Topology.py
+-rw-rw-rw-   0        0        0        0 2020-07-09 17:22:43.000000 tmkit-0.0.2/tmkit/interface/__init__.py
+-rw-rw-rw-   0        0        0      511 2023-06-29 21:39:11.000000 tmkit-0.0.2/tmkit/mapping.py
+-rw-rw-rw-   0        0        0     3353 2023-07-02 17:26:33.000000 tmkit-0.0.2/tmkit/msa.py
+-rw-rw-rw-   0        0        0     1817 2023-07-02 19:59:20.000000 tmkit-0.0.2/tmkit/mut.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.990838 tmkit-0.0.2/tmkit/name/
+-rw-rw-rw-   0        0        0     3179 2023-07-04 23:49:09.000000 tmkit-0.0.2/tmkit/name/Mapping.py
+-rw-rw-rw-   0        0        0        0 2022-08-06 12:13:25.000000 tmkit-0.0.2/tmkit/name/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.992835 tmkit-0.0.2/tmkit/position/
+-rw-rw-rw-   0        0        0       16 2019-09-15 17:43:20.000000 tmkit-0.0.2/tmkit/position/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.002836 tmkit-0.0.2/tmkit/position/scenario/
+-rw-rw-rw-   0        0        0     1724 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/position/scenario/Segment.py
+-rw-rw-rw-   0        0        0     2421 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/position/scenario/Separation.py
+-rw-rw-rw-   0        0        0        0 2019-09-21 21:40:26.000000 tmkit-0.0.2/tmkit/position/scenario/__init__.py
+-rw-rw-rw-   0        0        0     3245 2023-07-02 18:50:26.000000 tmkit-0.0.2/tmkit/ppi.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.008869 tmkit-0.0.2/tmkit/property/
+-rw-rw-rw-   0        0        0     7715 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/property/HelixSurface.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/property/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-06-29 21:41:10.000000 tmkit-0.0.2/tmkit/qc.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.021835 tmkit-0.0.2/tmkit/retrieve/
+-rw-rw-rw-   0        0        0    11431 2023-07-02 17:14:47.000000 tmkit-0.0.2/tmkit/retrieve/MSA.py
+-rw-rw-rw-   0        0        0     4362 2023-07-04 11:15:51.000000 tmkit-0.0.2/tmkit/retrieve/PDB.py
+-rw-rw-rw-   0        0        0     1688 2023-07-04 11:15:51.000000 tmkit-0.0.2/tmkit/retrieve/XML.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 15:10:49.000000 tmkit-0.0.2/tmkit/retrieve/__init__.py
+-rw-rw-rw-   0        0        0     4241 2023-07-05 23:13:50.000000 tmkit-0.0.2/tmkit/rrc.py
+-rw-rw-rw-   0        0        0     3626 2023-07-04 10:19:01.000000 tmkit-0.0.2/tmkit/seq.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.033840 tmkit-0.0.2/tmkit/seqnetrr/
+-rw-rw-rw-   0        0        0     7758 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/Compare.py
+-rw-rw-rw-   0        0        0     3507 2023-07-02 16:12:58.000000 tmkit-0.0.2/tmkit/seqnetrr/ComputLib.py
+-rw-rw-rw-   0        0        0    11463 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/Controller.py
+-rw-rw-rw-   0        0        0        0 2022-05-17 20:55:49.000000 tmkit-0.0.2/tmkit/seqnetrr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.049836 tmkit-0.0.2/tmkit/seqnetrr/combo/
+-rw-rw-rw-   0        0        0     1989 2023-07-02 17:02:29.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/Length.py
+-rw-rw-rw-   0        0        0      461 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/Param.py
+-rw-rw-rw-   0        0        0     1674 2023-06-29 20:10:11.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/Position.py
+-rw-rw-rw-   0        0        0     2494 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/Separation.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 16:35:38.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.061838 tmkit-0.0.2/tmkit/seqnetrr/graph/
+-rw-rw-rw-   0        0        0    16660 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/seqnetrr/graph/Bipartite.py
+-rw-rw-rw-   0        0        0     2961 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/seqnetrr/graph/Cumulative.py
+-rw-rw-rw-   0        0        0    19134 2023-07-02 17:04:50.000000 tmkit-0.0.2/tmkit/seqnetrr/graph/Unipartite.py
+-rw-rw-rw-   0        0        0        0 2022-05-18 21:29:35.000000 tmkit-0.0.2/tmkit/seqnetrr/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.066835 tmkit-0.0.2/tmkit/seqnetrr/net/
+-rw-rw-rw-   0        0        0    25230 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/net/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-06-12 23:19:50.000000 tmkit-0.0.2/tmkit/seqnetrr/net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.074835 tmkit-0.0.2/tmkit/seqnetrr/window/
+-rw-rw-rw-   0        0        0     4902 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/seqnetrr/window/Pair.py
+-rw-rw-rw-   0        0        0     4471 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/seqnetrr/window/Single.py
+-rw-rw-rw-   0        0        0        0 2019-09-18 20:19:22.000000 tmkit-0.0.2/tmkit/seqnetrr/window/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.082840 tmkit-0.0.2/tmkit/seqnetrr/window/base/
+-rw-rw-rw-   0        0        0     1309 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/window/base/Pair.py
+-rw-rw-rw-   0        0        0     1311 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/window/base/Single.py
+-rw-rw-rw-   0        0        0        0 2019-09-19 13:22:58.000000 tmkit-0.0.2/tmkit/seqnetrr/window/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.099867 tmkit-0.0.2/tmkit/sequence/
+-rw-rw-rw-   0        0        0      535 2023-07-05 23:14:23.000000 tmkit-0.0.2/tmkit/sequence/Fasta.py
+-rw-rw-rw-   0        0        0      446 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/sequence/Index.py
+-rw-rw-rw-   0        0        0     1881 2023-07-02 13:50:17.000000 tmkit-0.0.2/tmkit/sequence/PDB.py
+-rw-rw-rw-   0        0        0     1640 2023-07-02 15:53:41.000000 tmkit-0.0.2/tmkit/sequence/XML.py
+-rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.2/tmkit/sequence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.106835 tmkit-0.0.2/tmkit/structure/
+-rw-rw-rw-   0        0        0     3163 2023-07-03 17:00:04.000000 tmkit-0.0.2/tmkit/structure/PDB.py
+-rw-rw-rw-   0        0        0        0 2019-08-02 11:11:48.000000 tmkit-0.0.2/tmkit/structure/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.111837 tmkit-0.0.2/tmkit/structure/ppi/
+-rw-rw-rw-   0        0        0     1445 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/structure/ppi/Label.py
+-rw-rw-rw-   0        0        0        0 2019-09-15 17:30:37.000000 tmkit-0.0.2/tmkit/structure/ppi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.116835 tmkit-0.0.2/tmkit/structure/rrc/
+-rw-rw-rw-   0        0        0     1803 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/structure/rrc/Label.py
+-rw-rw-rw-   0        0        0        0 2019-09-15 17:30:31.000000 tmkit-0.0.2/tmkit/structure/rrc/__init__.py
+-rw-rw-rw-   0        0        0     4335 2023-07-04 17:11:34.000000 tmkit-0.0.2/tmkit/topo.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.124835 tmkit-0.0.2/tmkit/topology/
+-rw-rw-rw-   0        0        0     4174 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/topology/Phobius.py
+-rw-rw-rw-   0        0        0     7643 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/topology/TMHMM.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 13:11:26.000000 tmkit-0.0.2/tmkit/topology/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.129835 tmkit-0.0.2/tmkit/topology/lib/
+-rw-rw-rw-   0        0        0    25043 2022-07-15 23:01:47.000000 tmkit-0.0.2/tmkit/topology/lib/Phobius.py
+-rw-rw-rw-   0        0        0        0 2022-07-16 23:17:45.000000 tmkit-0.0.2/tmkit/topology/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.147835 tmkit-0.0.2/tmkit/topology/pdbtm/
+-rw-rw-rw-   0        0        0     4882 2023-07-04 14:03:11.000000 tmkit-0.0.2/tmkit/topology/pdbtm/Component.py
+-rw-rw-rw-   0        0        0     3246 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/topology/pdbtm/Determine.py
+-rw-rw-rw-   0        0        0     3729 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/topology/pdbtm/Segment.py
+-rw-rw-rw-   0        0        0     1486 2023-06-29 22:02:28.000000 tmkit-0.0.2/tmkit/topology/pdbtm/TMH.py
+-rw-rw-rw-   0        0        0     2216 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/topology/pdbtm/ToFastaId.py
+-rw-rw-rw-   0        0        0        0 2019-11-07 10:51:46.000000 tmkit-0.0.2/tmkit/topology/pdbtm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.160836 tmkit-0.0.2/tmkit/util/
+-rw-rw-rw-   0        0        0      890 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/util/Console.py
+-rw-rw-rw-   0        0        0     3398 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/util/Kit.py
+-rw-rw-rw-   0        0        0     2782 2023-07-02 17:02:29.000000 tmkit-0.0.2/tmkit/util/Reader.py
+-rw-rw-rw-   0        0        0     2525 2023-07-02 15:53:41.000000 tmkit-0.0.2/tmkit/util/Writer.py
+-rw-rw-rw-   0        0        0        0 2022-07-15 19:58:41.000000 tmkit-0.0.2/tmkit/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.163835 tmkit-0.0.2/tmkit/visualize/
+-rw-rw-rw-   0        0        0        0 2022-08-07 22:43:33.000000 tmkit-0.0.2/tmkit/visualize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.182836 tmkit-0.0.2/tmkit/visualize/component/
+-rw-rw-rw-   0        0        0      398 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/Color.py
+-rw-rw-rw-   0        0        0     3872 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/InterfaceResidues.py
+-rw-rw-rw-   0        0        0      416 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/Select.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/__init__.py
+-rw-rw-rw-   0        0        0     2955 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/focal_blur.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.189868 tmkit-0.0.2/tmkit/visualize/component/palette/
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/palette/__init__.py
+-rw-rw-rw-   0        0        0     8639 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/palette/data2bfactor.py
+-rw-rw-rw-   0        0        0     3699 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/palette/spectrumany.py
+-rw-rw-rw-   0        0        0    14522 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/show_contacts.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.195837 tmkit-0.0.2/tmkit/visualize/func/
+-rw-rw-rw-   0        0        0     2040 2023-07-02 13:29:15.000000 tmkit-0.0.2/tmkit/visualize/func/Coloring.py
+-rw-rw-rw-   0        0        0        0 2022-08-11 11:29:35.000000 tmkit-0.0.2/tmkit/visualize/func/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.204839 tmkit-0.0.2/tmkit/visualize/isite/
+-rw-rw-rw-   0        0        0     5478 2023-06-29 20:10:11.000000 tmkit-0.0.2/tmkit/visualize/isite/Labelling.py
+-rw-rw-rw-   0        0        0     4010 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/isite/ProtocolDeepTMInter.py
+-rw-rw-rw-   0        0        0        0 2020-12-31 08:21:51.000000 tmkit-0.0.2/tmkit/visualize/isite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.228837 tmkit-0.0.2/tmkit/visualize/small/
+-rw-rw-rw-   0        0        0      640 2023-07-02 13:35:02.000000 tmkit-0.0.2/tmkit/visualize/small/Label.py
+-rw-rw-rw-   0        0        0     2313 2023-07-02 13:29:15.000000 tmkit-0.0.2/tmkit/visualize/small/Local.py
+-rw-rw-rw-   0        0        0      473 2023-07-02 13:33:44.000000 tmkit-0.0.2/tmkit/visualize/small/Palette.py
+-rw-rw-rw-   0        0        0      664 2023-07-02 15:53:41.000000 tmkit-0.0.2/tmkit/visualize/small/Select.py
+-rw-rw-rw-   0        0        0      405 2023-07-02 13:35:02.000000 tmkit-0.0.2/tmkit/visualize/small/Style.py
+-rw-rw-rw-   0        0        0        0 2021-01-01 12:44:05.000000 tmkit-0.0.2/tmkit/visualize/small/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-06-29 21:36:51.000000 tmkit-0.0.2/tmkit/vs.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.877836 tmkit-0.0.2/tmkit.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/top_level.txt
```

### Comparing `tmkit-0.0.0.2/LICENSE` & `tmkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/README.md` & `tmkit-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,15 @@
 
 ## Installation
 * ### PyPI
 ```angular2html
 pip install tmkitx --upgrade
 ```
 
-## API documentation
-https://tmkit.readthedocs.io/en/latest/
-
-## Tutorial of TMKit
+## Documentation
 Website: https://tmkit-guide.herokuapp.com/doc/overview
 
 Source: https://github.com/2003100127/tmkit-guide
 
 ## Citation
 Please cite our work if you use TMKit in your research.
```

### Comparing `tmkit-0.0.0.2/setup.py` & `tmkit-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tmkit",
-    # name="tmkitx",
-    version="0.0.0.2",
+    version="0.0.2",
     keywords=("pip", "tmkit"),
     description="TMKit",
     long_description="TMKit",
     license="GNU GENERAL V3.0",
 
     url="https://github.com/2003100127/tmkit",
     author="Jianfeng Sun",
     author_email="jianfeng.sun@ndorms.ox.ac.uk",
 
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
-    python_requires='>3.6',
+    python_requires='>3.8',
     install_requires=[
         'scikit-learn',
         'pandas',
         'numpy',
+        'openpyxl',
         'biopandas',
-        # 'tmhmm.py',
+        'pypdb==2.2',
         'xmltramp2==3.1.1',
         'biopython==1.79',
         'pyfiglet==0.8.post1',
     ],
 )
```

### Comparing `tmkit-0.0.0.2/tmkit/base/PDB.py` & `tmkit-0.0.2/tmkit/base/PDB.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
+import warnings
 from Bio.PDB.PDBParser import PDBParser
 from Bio.PDB.Polypeptide import PPBuilder
 
 
-class sequence():
+class sequence:
 
     def __init__(self, pdb_fp, prot_name, seq_chain, file_chain):
-        self.pdb_fp = pdb_fp
-        self.prot_name = prot_name
-        self.file_chain = file_chain
-        self.seq_chain = seq_chain
-        self.pdb_fpn = self.pdb_fp + self.prot_name + self.file_chain + '.pdb'
+        from Bio import BiopythonWarning
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', BiopythonWarning)
+            self.pdb_fp = pdb_fp
+            self.prot_name = prot_name
+            self.file_chain = file_chain
+            self.seq_chain = seq_chain
+            self.pdb_fpn = self.pdb_fp + self.prot_name + self.file_chain + '.pdb'
+
+            self.bio_parser = PDBParser()
+            self.structure = self.bio_parser.get_structure(self.prot_name, self.pdb_fpn)
+            self.model = self.structure[0]
+            self.pdb_chain = self.model[self.seq_chain]
+            self.ppb = PPBuilder()
 
-        self.bio_parser = PDBParser()
-        self.structure = self.bio_parser.get_structure(self.prot_name, self.pdb_fpn)
-        self.model = self.structure[0]
-        self.pdb_chain = self.model[self.seq_chain]
-        self.ppb = PPBuilder()
 
-
-class id():
+class id:
 
     def __init__(self, pdb_fp, prot_name, seq_chain, file_chain):
         self.pdb_fp = pdb_fp
         self.prot_name = prot_name
         self.file_chain = file_chain
         self.seq_chain = seq_chain
         self.pdb_fpn = self.pdb_fp + self.prot_name + self.file_chain + '.pdb'
 
         self.bio_parser = PDBParser()
         self.structure = self.bio_parser.get_structure(self.prot_name, self.pdb_fpn)
         self.model = self.structure[0]
         self.pdb_chain = self.model[self.seq_chain]
 
 
-class structure():
+class structure:
 
     def __init__(self, pdb_fp, prot_name, seq_chain, file_chain):
         self.pdb_fp = pdb_fp
         self.prot_name = prot_name
         self.file_chain = file_chain
         self.seq_chain = seq_chain
         self.pdb_fpn = self.pdb_fp + self.prot_name + self.file_chain + '.pdb'
 
         self.bio_parser = PDBParser()
         self.structure = self.bio_parser.get_structure(self.prot_name, self.pdb_fpn)
         self.model = self.structure[0]
-        self.pdb_chain = self.model[self.seq_chain]
+        if self.seq_chain != '':
+            self.pdb_chain = self.model[self.seq_chain]
 
     @property
     def name(self, ):
         return self.structure.header['name']
 
     @property
     def rez(self, ):
@@ -77,15 +82,15 @@
     @property
     def psi_phi(self, ):
         for pp in PPBuilder().build_peptides(self.structure):
             print(pp.get_phi_psi_list())
         return PPBuilder().build_peptides(self.structure).get_phi_psi_list()
 
 
-class chain():
+class chain:
 
     def __init__(self, pdb_fp, prot_name):
         self.pdb_fp = pdb_fp
         self.prot_name = prot_name
         self.pdb_fpn = self.pdb_fp + self.prot_name + '.pdb'
         self.bio_parser = PDBParser(QUIET=True)
         self.structure = self.bio_parser.get_structure(self.prot_name, self.pdb_fpn)
```

### Comparing `tmkit-0.0.0.2/tmkit/base/Position.py` & `tmkit-0.0.2/tmkit/base/Position.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import numpy as np
 
 
-class position(object):
+class position:
 
     def __init__(self, seq_sep_inferior=None, seq_sep_superior=None):
         self.seq_sep_inferior = seq_sep_inferior
         self.seq_sep_superior = seq_sep_superior
         # self.asp = scheme()
 
     def interv2combi(self, inf_arr, sup_arr):
```

### Comparing `tmkit-0.0.0.2/tmkit/chain/Collate.py` & `tmkit-0.0.2/tmkit/chain/Collate.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,29 @@
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import warnings
+from Bio import BiopythonWarning
 import pandas as pd
-from tmkit.Path import to
 from tmkit.sequence.PDB import pdb as spdb
 from tmkit.chain.PDB import pdb as cpdb
 from tmkit.util.Kit import seqchainid
-from Bio import BiopythonWarning
-from tmkit.util.Console import console
 
 
-class collate(object):
+class collate:
 
     def __init__(
             self,
             prot_name,
             chain_focus,
             pdb_pdbtm_fp,
             pdb_rcsb_fp,
-            verbose=True,
     ):
         self.prot_name = prot_name
         self.chain_focus = chain_focus
         self.pdb_pdbtm_fp = pdb_pdbtm_fp
         self.pdb_rcsb_fp = pdb_rcsb_fp
 
         self.chains_pdbtm = cpdb(
@@ -49,18 +46,15 @@
             self.df['source'] = 'pdbtm_tr'
         else:
             self.df['source'] = 'rcsb'
 
         self.df['diff'] = ''.join(list(set(self.chains_pdbtm).difference(set(self.chains_rcsb))))
         self.df['same'] = ''.join(list(set(self.chains_pdbtm).intersection(set(self.chains_rcsb))))
 
-        self.console = console()
-        self.console.verbose = verbose
-
-        self.console.print('======>basic info: \n{}'.format(self.df))
+        # print('======>basic info: \n{}'.format(self.df))
 
     def throwback(self, symbol):
         """
 
         Notes
         -----
             throw_backs is a dict with keys being the collated protein chains
@@ -82,15 +76,15 @@
         """
         throw_backs = {}
         if self.df.loc[0, 'source'] == 'rcsb':
             throw_backs[self.prot_name + symbol + self.chain_focus] = 'untransformed'
         else:
             pdbtm_to_rcsb_dict = self.isSameSeq(symbol=symbol)
             if len([*pdbtm_to_rcsb_dict.values()]) > 0:
-                self.console.print('======>master is collated: {} '.format([*pdbtm_to_rcsb_dict.values()][0]))
+                print('======>master is collated: {} '.format([*pdbtm_to_rcsb_dict.values()][0]))
                 throw_backs[self.prot_name + symbol + self.chain_focus] = [*pdbtm_to_rcsb_dict.values()][0]
             else:
                 throw_backs[self.prot_name + symbol + self.chain_focus] = 'transformed & uncollated'
         return throw_backs
 
     def isSameSeq(self, symbol='.'):
         """
@@ -121,39 +115,14 @@
                 seq_rcsb = spdb(
                     pdb_fp=self.pdb_rcsb_fp,
                     prot_name=self.prot_name,
                     seq_chain=seqchainid(chain_rcsb),
                     file_chain='',
                 ).chain()
                 if seq_pdbtm == seq_rcsb:
-                    self.console.print('=========>{}.{} in PDBTM corresponds to {}.{} in RCSB.'.format(
+                    print('=========>{}.{} in PDBTM corresponds to {}.{} in RCSB.'.format(
                         self.prot_name, self.chain_focus, self.prot_name, chain_rcsb)
                     )
                     pdbtm_to_rcsb_dict[self.prot_name + symbol + self.chain_focus].append(
                         self.prot_name + symbol + chain_rcsb
                     )
-        return pdbtm_to_rcsb_dict
-
-
-if __name__ == "__main__":
-    from tmkit.util.Reader import reader
-
-    DEFINE = {
-        'pdb_rcsb_fp': to('data/example/pdb/indepdata/rcsb/'),
-        'pdb_pdbtm_fp': to('data/example/pdb/indepdata/pdbtm/'),
-        'prot_fpn': to('data/example/pdb/indepdata/prot_n30.txt'),
-        'prot_pdbtm_fpn': to('data/example/pdb/indepdata/prot_n30_complex_pdbtm_full.txt'),
-        'prot_rcsb_fpn': to('data/example/pdb/indepdata/prot_n30_complex_rcsb_full.txt'),
-    }
-
-    prot_df = reader().generic(DEFINE['prot_fpn'])
-    prot_pdbtm_df = reader().generic(DEFINE['prot_pdbtm_fpn'])
-    prot_rcsb_df = reader().generic(DEFINE['prot_rcsb_fpn'])
-
-    p = collate(
-        prot_name='3pux',
-        chain_focus='G',
-        pdb_rcsb_fp=DEFINE['pdb_rcsb_fp'],
-        pdb_pdbtm_fp=DEFINE['pdb_pdbtm_fp'],
-    )
-
-    print(p.throwback(symbol='.'))
+        return pdbtm_to_rcsb_dict
```

### Comparing `tmkit-0.0.0.2/tmkit/chain/CollateBatch.py` & `tmkit-0.0.2/tmkit/chain/CollateBatch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from tmkit.Path import to
 from tmkit.util.Kit import tactic5
 from tmkit.sequence.PDB import pdb as spdb
 from tmkit.util.Kit import seqchainid
-from tmkit.util.Console import console
 from Bio import BiopythonWarning
 import warnings
 
 
-class collateBatch(object):
+class collateBatch:
 
     def __init__(
             self,
             prot_df,
             pdb_rcsb_fp,
             pdb_pdbtm_fp,
             prot_pdbtm_df,
             prot_rcsb_df,
             strategy='diff',
-            verbose=True,
     ):
         self.prot_df = prot_df
         self.pdb_rcsb_fp = pdb_rcsb_fp
         self.pdb_pdbtm_fp = pdb_pdbtm_fp
 
-        self.console = console()
-        self.console.verbose = verbose
-
         self.prot_collated_df = self.rcsb(
             prot_pdbtm_df=prot_pdbtm_df,
             prot_rcsb_df=prot_rcsb_df,
             strategy=strategy,
         )
 
-        self.console.print('======>basic info: \n{}'.format(self.prot_collated_df))
+        # print('======>basic info: \n{}'.format(self.prot_collated_df))
 
     def rcsb(self, prot_pdbtm_df, prot_rcsb_df, strategy):
         """
 
         Notes
         -----
             It contains 6 columns:
@@ -144,15 +138,15 @@
                 chain_collated_dict = self.areSameSeqs(
                     prot_name=prot_name,
                     chain_to_be_collated=[prot_chain],
                     rcsb_chains=list(prot_collated_df['rcsb'][id]),
                     symbol='.',
                 )
                 if len([*chain_collated_dict.values()]) > 0:
-                    self.console.print('======>master is collated: {} '.format([*chain_collated_dict.values()][0]))
+                    print('======>master is collated: {} '.format([*chain_collated_dict.values()][0]))
                     throw_backs[[*chain_collated_dict.values()][0]] = 'collated'
                 else:
                     throw_backs[[*chain_collated_dict]] = 'transformed'
         return throw_backs
 
     def areSameSeqs(self, prot_name, chain_to_be_collated=[], rcsb_chains=[], symbol='.'):
         """
@@ -183,45 +177,12 @@
                     seq_rcsb = spdb(
                         pdb_fp=self.pdb_rcsb_fp,
                         prot_name=prot_name,
                         seq_chain=seqchainid(chain_rcsb),
                         file_chain='',
                     ).chain()
                     if seq_pdbtm == seq_rcsb:
-                        self.console.print('=========>{}.{} in PDBTM corresponds to {}.{} in RCSB.'.format(
+                        print('=========>{}.{} in PDBTM corresponds to {}.{} in RCSB.'.format(
                             prot_name, seqchainid(chain_pdbtm), prot_name, seqchainid(chain_rcsb))
                         )
                         chain_collated_dict[prot_name + symbol + seqchainid(chain_pdbtm)].append(prot_name + symbol + seqchainid(chain_rcsb))
-        return chain_collated_dict
-
-
-if __name__ == "__main__":
-    from tmkit.util.Reader import reader
-    DEFINE = {
-        'pdb_rcsb_fp': to('data/example/pdb/testdata/rcsb/'),
-        'pdb_pdbtm_fp': to('data/example/pdb/testdata/pdbtm/'),
-        'prot_fpn': to('data/example/pdb/testdata/prot_n36.txt'),
-        'prot_pdbtm_fpn': to('data/example/pdb/testdata/prot_n36_complex_pdbtm_full.txt'),
-        'prot_rcsb_fpn': to('data/example/pdb/testdata/prot_n36_complex_rcsb_full.txt'),
-    }
-
-    prot_df = reader().generic(DEFINE['prot_fpn'])
-    prot_pdbtm_df = reader().generic(DEFINE['prot_pdbtm_fpn'])
-    prot_rcsb_df = reader().generic(DEFINE['prot_rcsb_fpn'])
-
-    p = collateBatch(
-        prot_df=prot_df,
-        pdb_rcsb_fp=DEFINE['pdb_rcsb_fp'],
-        pdb_pdbtm_fp=DEFINE['pdb_pdbtm_fp'],
-    )
-
-    prot_collated_df = p.rcsb(
-        prot_pdbtm_df=prot_pdbtm_df,
-        prot_rcsb_df=prot_rcsb_df,
-        strategy='diff',
-    )
-    print(prot_collated_df)
-
-    print(p.throwback(
-        prot_collated_df=prot_collated_df,
-        symbol='.'
-    ))
+        return chain_collated_dict
```

### Comparing `tmkit-0.0.0.2/tmkit/chain/PDB.py` & `tmkit-0.0.2/tmkit/chain/PDB.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/tmkit/channel/Workbench.py` & `tmkit-0.0.2/tmkit/channel/Workbench.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,51 +6,46 @@
 __maintainer__ = "Jianfeng Sun"
 
 import warnings
 import pandas as pd
 from Bio.PDB import *
 from Bio import BiopythonWarning
 from tmkit.topology.pdbtm.TMH import tmh as tmhseg
-from tmkit.sequence.Fasta import fasta as sfasta
+from tmkit.sequence import Fasta as sfasta
 from tmkit.util.Kit import chainid
 from tmkit.util.Reader import reader
 from tmkit.util.Writer import writer
 from tmkit.base import PDB
-from tmkit.util.Console import console
 
 
-class workbench():
+class workbench:
 
     def __init__(
             self,
             df_prot,
             pdb_cplx_fp,
             fasta_fp,
             xml_fp=None,
             sv_fp=None,
-            verbose=True,
     ):
         self.df_prot = df_prot
         self.pdb_cplx_fp = pdb_cplx_fp
         self.fasta_fp = fasta_fp
         self.xml_fp = xml_fp
         self.sv_fp = sv_fp
 
         self.parser = PDBParser()
         self.reader = reader()
         self.writer = writer()
-        self.console = console()
 
         self.num_pc = self.df_prot.shape[0]
 
         self.df_prot_uniq = pd.DataFrame(pd.unique(self.df_prot['prot']), columns=['prot'])
         # print(self.df_prot_uniq)
 
-        self.console.verbose = verbose
-
     def template(
             self,
             metric,
     ):
         """
 
         Parameters
@@ -113,35 +108,35 @@
                             tmh_beg, tmh_last = tmhseg(
                                 xml_fp=self.xml_fp,
                                 prot_name=prot_name,
                                 seq_chain=seq_chain,
                             ).get()
                             self.df_prot.loc[i, metric] = len(tmh_beg)
                         elif metric == 'seq':
-                            seq = sfasta().get(
+                            seq = sfasta.get(
                                 fasta_fpn=self.fasta_fp + prot_name + chainid(seq_chain) + '.fasta'
                             )
                             self.df_prot.loc[i, metric + '_aa'] = seq
                             self.df_prot.loc[i, metric + '_len'] = len(seq)
 
-                    self.console.print('=========>protein {} chain {} with {} {}'.format(
+                    print('=========>protein {} chain {} with {} {}'.format(
                         self.df_prot.loc[i, 'prot'],
                         self.df_prot.loc[i, 'chain'],
                         metric,
                         self.df_prot.loc[i, metric],
                     ))
                 except:
-                    self.console.print('=========>File failed: {} {}'.format(
+                    print('=========>File failed: {} {}'.format(
                         self.df_prot.loc[i, 'prot'],
                         self.df_prot.loc[i, 'chain'],
                     ))
                     fail_list.append([self.df_prot.loc[i, 'prot'], self.df_prot.loc[i, 'chain']])
                     fail_count = fail_count + 1
                     continue
-        self.console.print('======>{} extraction items failed using {}.'.format(fail_count, metric))
+        print('======>{} extraction items failed using {}.'.format(fail_count, metric))
         self.writer.generic(df=self.df_prot, sv_fpn=self.sv_fp + 'wb_' + metric + '_c.txt')
         return self.df_prot
 
     def integrate(self, metrics):
         """
 
         Parameters
@@ -150,58 +145,18 @@
 
         Returns
         -------
 
         """
         self.df_prot['prot_mark'] = self.df_prot['prot'] + self.df_prot['chain']
         for i, metric in enumerate(metrics):
-            self.console.print('======>metric: {}'.format(metric))
+            print('======>metric: {}'.format(metric))
             self.template(metric=metric)
         # self.writer.generic(df=self.df_prot, sv_fpn=self.sv_fp + 'wb_integrate.txt', header=True,)
         self.writer.excel(
             df=self.df_prot,
             sv_fpn=self.sv_fp + 'integrate.xlsx',
             sheet_name='Sheet1',
             header=True,
             index=False
         )
-        return self.df_prot
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    DEFINE = {
-        'list_fpn': to('data/example/pdb/indepdata/prot_n30.txt'),
-        'pdb_cplx_fp': to('data/example/pdb/indepdata/pdbtm/'),
-        'fasta_fp': to('data/example/fasta/indepdata/'),
-        'xml_fp': to('data/example/xml/indepdata/'),
-        'sv_fp': to('data/example/pdb/indepdata/'),
-    }
-
-    df_prot = reader().generic(DEFINE['list_fpn'])
-    df_prot = df_prot.rename(columns={
-        0: 'prot',
-        1: 'chain',
-    })
-
-    p = workbench(
-        df_prot=df_prot,
-        pdb_cplx_fp=DEFINE['pdb_cplx_fp'],
-        fasta_fp=DEFINE['fasta_fp'],
-        xml_fp=DEFINE['xml_fp'],
-        sv_fp=DEFINE['sv_fp']
-    )
-
-    # print(p.template(
-    #     # metric='rez',
-    #     # metric='met',
-    #     # metric='bio_name',
-    #     # metric='head',
-    #     # metric='desc',
-    #     # metric='mthm',
-    #     metric='seq',
-    # ))
-
-    print(p.integrate(
-        metrics=['rez', 'met', 'bio_name', 'head', 'mthm', 'seq']
-    ))
+        return self.df_prot
```

### Comparing `tmkit-0.0.0.2/tmkit/collate.py` & `tmkit-0.0.2/tmkit/collate.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,29 +4,25 @@
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 from tmkit.chain.PDB import pdb as cpdb
 from tmkit.chain.Collate import collate as coll
 from tmkit.chain.CollateBatch import collateBatch as collb
-from tmkit.util.Console import console
 
 
 def chain(
         pdb_fp,
         prot_name,
-        verbose=True,
 ):
-    c = console()
-    c.verbose = verbose
     chains = cpdb(
         pdb_fp=pdb_fp,
         prot_name=prot_name,
     ).chains()
-    c.print('======>protein has chains {}'.format(chains))
+    print('======>protein has chains {}'.format(chains))
     return chains
 
 
 def single(
         prot_name,
         chain_focus,
         pdb_rcsb_fp,
@@ -88,46 +84,8 @@
         prot_pdbtm_df=prot_pdbtm_df,
         prot_rcsb_df=prot_rcsb_df,
         strategy=strategy,
     )
     return coll_batch.prot_collated_df, coll_batch.throwback(
         prot_collated_df=coll_batch.prot_collated_df,
         symbol=symbol
-    )
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-    from tmkit.util.Reader import reader as reader
-
-    pdb_rcsb_fp = to('data/example/pdb/indepdata/rcsb/')
-    pdb_pdbtm_fp = to('data/example/pdb/indepdata/pdbtm/')
-    prot_fpn = to('data/example/pdb/indepdata/prot_n30.txt')
-    prot_pdbtm_fpn = to('data/example/pdb/indepdata/prot_n30_complex_pdbtm_full.txt')
-    prot_rcsb_fpn = to('data/example/pdb/indepdata/prot_n30_complex_rcsb_full.txt')
-
-    print(chain(
-        prot_name='3pux',
-        pdb_fp=pdb_pdbtm_fp,
-        # pdb_fp=pdb_rcsb_fp,
-    ))
-
-    print(single(
-        prot_name='3pux',
-        chain_focus='G',
-        pdb_rcsb_fp=pdb_rcsb_fp,
-        pdb_pdbtm_fp=pdb_pdbtm_fp,
-    ))
-
-    prot_df = reader().generic(prot_fpn)
-    prot_pdbtm_df = reader().generic(prot_pdbtm_fpn)
-    prot_rcsb_df = reader().generic(prot_rcsb_fpn)
-
-    print(batch(
-        prot_df=prot_df,
-        prot_pdbtm_df=prot_pdbtm_df,
-        prot_rcsb_df=prot_rcsb_df,
-        pdb_rcsb_fp=pdb_rcsb_fp,
-        pdb_pdbtm_fp=pdb_pdbtm_fp,
-        strategy='diff',
-        symbol='.'
-    ))
+    )
```

### Comparing `tmkit-0.0.0.2/tmkit/contact/Evaluator.py` & `tmkit-0.0.2/tmkit/contact/Evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,30 @@
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import numpy as np
 import pandas as pd
 from sklearn import metrics
 from tmkit.contact.Reader import reader as rrcreader
-from tmkit.util.Console import console
 
 
-class evaluator():
+class evaluator:
 
     def __init__(
             self,
             prot_name,
             file_chain,
             dist_df,
             pair_list,
             dist_limit=None,
             tool=None,
             tool_fp=None,
             sort_=None,
             seq_sep_inferior=None,
             seq_sep_superior=None,
-            verbose=True,
     ):
         self.tool_fp = tool_fp
         self.prot_name = prot_name
         self.file_chain = file_chain
         self.dist_limit = dist_limit
         self.pair_list = pair_list
         self.tool = tool
@@ -50,18 +48,15 @@
             'aa_2',
             'pdb_id_2',
             'dist',
             'is_contact'
         ]
         self.row_real_dist = self.dist_df.shape[0]
 
-        self.console = console()
-        self.console.verbose = verbose
-
-        self.console.print('======>Evaluating protein {}'.format(prot_name + file_chain))
+        print('======>Evaluating protein {}'.format(prot_name + file_chain))
 
     def fetch(self):
         switch = {
             'psicov': self.psicov,
             'freecontact': self.freecontact,
             'ccmpred': self.ccmpred,
             'gremlin': self.gremlin,
@@ -98,27 +93,27 @@
             np.concatenate(
                 [np.zeros([row_cutoff]) + 1, np.zeros([row_offset])],
                 axis=0
             ).astype(np.int64)
         )
         # #/*** block precision ***/
         precision = metrics.precision_score(y_true=y_true_all, y_pred=y_pred_all)
-        self.console.print('=========>precision: {}'.format(precision))
+        print('=========>precision: {}'.format(precision))
         # #/*** block recall ***/
         recall = metrics.recall_score(y_true=y_true_all, y_pred=y_pred_all)
-        self.console.print('=========>recall: {}'.format(recall))
+        print('=========>recall: {}'.format(recall))
         # #/*** block mcc ***/
         mcc = metrics.matthews_corrcoef(y_true=y_true_all, y_pred=y_pred_all)
-        self.console.print('=========>mcc: {}'.format(mcc))
+        print('=========>mcc: {}'.format(mcc))
         # #/*** block f1score ***/
         f1score = metrics.f1_score(y_true=y_true_all, y_pred=y_pred_all)
-        self.console.print('=========>f1score: {}'.format(f1score))
+        print('=========>f1score: {}'.format(f1score))
         # #/*** block accuracy ***/
         accuracy = metrics.accuracy_score(y_true=y_true_all, y_pred=y_pred_all)
-        self.console.print('=========>accuracy: {}'.format(accuracy))
+        print('=========>accuracy: {}'.format(accuracy))
         metrics_summary = {
             'precision': precision,
             'recall': recall,
             'f1score': f1score,
             'mcc': mcc,
             'accuracy': accuracy,
         }
```

### Comparing `tmkit-0.0.0.2/tmkit/contact/Reader.py` & `tmkit-0.0.2/tmkit/contact/Reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import pandas as pd
 from tmkit.util.Kit import tactic1
 from tmkit.util.Reader import reader as greader
 from tmkit.position.scenario.Separation import separation as ppssep
 
 
-class reader(object):
+class reader:
 
     def __init__(self, seq_sep_inferior=None, seq_sep_superior=None):
         self.__sort_ = -1
         self.seq_sep_inferior = seq_sep_inferior
         self.seq_sep_superior = seq_sep_superior
         self.greader = greader()
 
@@ -43,16 +43,16 @@
         else:
             self.__sort_ = value
 
     def sort_1(self, recombine, dist_df):
         dists_ = dist_df
         recombine_ = recombine
         len_recombine_ = recombine_.shape[0]
-        dists_['fasta_id_1'] = dists_['fasta_id_1'].astype(np.int)
-        dists_['fasta_id_2'] = dists_['fasta_id_2'].astype(np.int)
+        dists_['fasta_id_1'] = dists_['fasta_id_1'].astype(int)
+        dists_['fasta_id_2'] = dists_['fasta_id_2'].astype(int)
         dists__ = pd.DataFrame()
         dists__[0] = dists_['fasta_id_1']
         dists__[1] = dists_['fasta_id_2']
         dists__[2] = dists_.index.values
         dist_dict = self.todict(dists__)
         dist_ids = []
         for i in range(len_recombine_):
@@ -553,16 +553,16 @@
             'contact_id_1',
             'contact_id_2',
             'score',
             'isContact',
             'ph1',
             'ph2'
         ]
-        results['contact_id_1'] = results['contact_id_1'].astype(np.int)
-        results['contact_id_2'] = results['contact_id_2'].astype(np.int)
+        results['contact_id_1'] = results['contact_id_1'].astype(int)
+        results['contact_id_2'] = results['contact_id_2'].astype(int)
         results['score'] = results['score'].astype(np.float64)
         # print(results.dtypes)
         recombine = results[[
             'contact_id_1',
             'contact_id_2',
             'score',
         ]]
@@ -611,16 +611,16 @@
             'contact_id_1',
             'aa_1',
             'TMH2',
             'contact_id_2',
             'aa_2',
             'score'
         ]
-        results['contact_id_1'] = results['contact_id_1'].astype(np.int)
-        results['contact_id_2'] = results['contact_id_2'].astype(np.int)
+        results['contact_id_1'] = results['contact_id_1'].astype(int)
+        results['contact_id_2'] = results['contact_id_2'].astype(int)
         results['score'] = results['score'].astype(np.float64)
         # print(results.dtypes)
         recombine = results[[
             'contact_id_1',
             'contact_id_2',
             'score'
         ]]
```

### Comparing `tmkit-0.0.0.2/tmkit/db/Connectivity.py` & `tmkit-0.0.2/tmkit/db/Connectivity.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,54 +9,50 @@
 import pandas as pd
 from tmkit.util.Reader import reader
 from tmkit.util.Writer import writer
 from tmkit.chain.Collate import collate
 from tmkit.util.Kit import seqchainid
 from tmkit.db.construct.Network import network as ppinet
 from tmkit.name.Mapping import mapping as idmap
-from tmkit.util.Console import console
 
 
-class connectivity(object):
+class connectivity:
 
     def __init__(
             self,
             prot_name,
             seq_chain,
             prot_idmap,
             interacting_partner_idmap,
             pdb_pdbtm_fp=None,
             pdb_rcsb_fp=None,
             sv_fpn=None,
             symbol='.',
-            verbose=True,
     ):
         self.reader = reader()
         self.writer = writer()
         self.idmap = idmap()
-        self.console = console()
-        self.console.verbose = verbose
 
         self.pdb_pdbtm_fp = pdb_pdbtm_fp
         self.pdb_rcsb_fp = pdb_rcsb_fp
         self.symbol = symbol
         self.sv_fpn = sv_fpn
 
         self.collate = collate(
             prot_name=prot_name,
             chain_focus=seq_chain,
             pdb_rcsb_fp=self.pdb_rcsb_fp,
             pdb_pdbtm_fp=self.pdb_pdbtm_fp,
         )
 
         self.df_collate = self.collate.df
-        self.console.print('===>df collated chains:\n {}'.format(self.df_collate))
+        # print('===>df collated chains:\n {}'.format(self.df_collate))
 
         self.prot_collate_dict = self.collate.throwback(symbol=symbol)
-        self.console.print('===>collated {}'.format(self.prot_collate_dict))
+        # print('===>collated {}'.format(self.prot_collate_dict))
 
         self.prot_master_idmap = self.idmap.pdb2uniprot(
             self.prot_collate_dict.keys()
         )
 
         self.prot_master_idmap = prot_idmap
         self.interacting_partner_idmap = interacting_partner_idmap
@@ -79,45 +75,45 @@
         ----------
         ppi_db_fpns
 
         Returns
         -------
 
         """
-        self.console.print('===>UniProt protein id: {}'.format(self.prot_master_idmap))
+        print('===>UniProt protein id: {}'.format(self.prot_master_idmap))
         for i, key in enumerate(self.prot_master_idmap.keys()):
             prot_name = key[:4]
             seq_chain = seqchainid(key[5])
-            self.console.print('===>protein {} chain {}'.format(i+1, prot_name, seq_chain))
+            print('===>protein {} chain {}'.format(i+1, prot_name, seq_chain))
             master_networks = self.strategy(
                 ppi_db_fpns=ppi_db_fpns,
                 uniprot_id=key,
                 is_del_reflexive=False,
                 is_del_repeated=False,
                 overlap=True,
             )
-            self.console.print('======>interacting partners from the ppi databases:\n{}'.format(master_networks))
+            print('======>interacting partners from the ppi databases:\n{}'.format(master_networks))
             len_master_nets = len(master_networks)
 
-            self.console.print('======>interacting partner idmap: {}'.format(self.interacting_partner_idmap))
+            print('======>interacting partner idmap: {}'.format(self.interacting_partner_idmap))
             ip_all = [*self.interacting_partner_idmap.keys()]
-            self.console.print('======>interacting partners from its complex: {}'.format(ip_all))
+            print('======>interacting partners from its complex: {}'.format(ip_all))
             ip_uniprot_ids = [*self.interacting_partner_idmap.values()]
-            self.console.print('======>uniprot ids of interacting partners from its complex:{}'.format(ip_uniprot_ids))
+            print('======>uniprot ids of interacting partners from its complex:{}'.format(ip_uniprot_ids))
             count_ip_in_network = 0
             if len(master_networks[:, 1]) > 0:
                 for ip in ip_uniprot_ids:
                     for ele_mnet in master_networks[:, 1].tolist():
                         if len(ele_mnet.split('|')) != 1:
                             print(ele_mnet.split('|'))  # e.g. ['P68187']
                         if ip in ele_mnet.split('|'):
                             count_ip_in_network += 1
-            self.console.print('======>{} records found from the ppi databases'.format(len_master_nets))
-            self.console.print('======>{} interacting partners from its complex'.format(len(ip_all)))
-            self.console.print('======>{} interacting partners from its complex and found in the ppi databases as well'.format(
+            print('======>{} records found from the ppi databases'.format(len_master_nets))
+            print('======>{} interacting partners from its complex'.format(len(ip_all)))
+            print('======>{} interacting partners from its complex and found in the ppi databases as well'.format(
                 count_ip_in_network)
             )
 
             self.df_collate.loc[i, 'num_overlapped_db'] = len_master_nets
             self.df_collate.loc[i, 'num_ip'] = len(ip_all)
             self.df_collate.loc[i, 'ip_chains'] = ''.join([i.split(self.symbol)[1] for i in ip_all])
             self.df_collate.loc[i, 'num_ip_overlapped_db'] = count_ip_in_network
@@ -141,75 +137,37 @@
 
         Returns
         -------
 
         """
         res = {}
         for db_name, db_fpn in ppi_db_fpns.items():
-            self.console.print('======>scanning ppi db: {}'.format(db_name))
-            db_df = self.reader.generic(db_fpn, header=0)
+            print('======>scanning ppi db: {}'.format(db_name))
+            db_df = self.reader.generic(db_fpn, header=0, comment=None)
             res[db_name] = ppinet().single(
                 interacting_df=db_df,
                 uniprot_id=self.prot_master_idmap[uniprot_id],
                 # uniprot_id=uniprot_id,
                 by=self.switch2by[db_name],
                 is_del_reflexive=is_del_reflexive,
                 is_del_repeated=is_del_repeated,
             )
         if overlap:
             res_ = np.unique(np.concatenate([*res.values()], axis=0)[:, 1])
         else:
             if len(res.keys()) == 1:
                 res_ = [*res.values()][0][:, 1]
-                self.console.print('============>no overlap + len == 1')
+                print('============>no overlap + len == 1')
             else:
-                self.console.print('============>no overlap + len > 2')
+                print('============>no overlap + len > 2')
                 df1 = pd.DataFrame(res['biogrid'])
                 df2 = pd.DataFrame(res['intact'])
                 biogrid_gaps = df1[1].loc[df1[1].isin(['-'])].values.tolist()
                 biogrid_non_gaps = df1[1].loc[~df1[1].isin(['-'])].values.tolist()
                 intact_no_overlap = df2[1].loc[df2[1].isin(biogrid_non_gaps)].values.tolist()
                 res_ = np.array(biogrid_gaps + biogrid_non_gaps + intact_no_overlap)
         # print(res_)
         # print(res_.shape[0])
         return np.concatenate(
             (np.array([uniprot_id] * res_.shape[0])[:, np.newaxis], res_[:, np.newaxis]),
             axis=1,
-        )
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    DEFINE = {
-        'ppi_db_fpns': {
-            'biogrid': to('data/example/ppi/BIOGRID-ALL-4.4.212.biogrid'),
-            'intact': to('data/example/ppi/interA_B.intact'),
-        },
-        'pdb_rcsb_fp': to('data/example/pdb/indepdata/rcsb/'),
-        'pdb_pdbtm_fp': to('data/example/pdb/indepdata/pdbtm/'),
-        'sv_fpn': to('data/example/ppi/indepdata.ppidb'),
-    }
-    p = connectivity(
-        prot_name='3pux',
-        seq_chain='G',
-        prot_idmap={'3pux.G': 'P68183'},
-        interacting_partner_idmap={
-            '3pux.A': 'P68187',
-            '3pux.B': 'P68187',
-            '3pux.E': 'P0AEX9',
-            '3pux.F': 'P02916',
-        },
-        pdb_rcsb_fp=DEFINE['pdb_rcsb_fp'],
-        pdb_pdbtm_fp=DEFINE['pdb_pdbtm_fp'],
-        sv_fpn=DEFINE['sv_fpn'],
-    )
-
-    print(p.extract(ppi_db_fpns=DEFINE['ppi_db_fpns']))
-
-    # ### test
-    # print(p.strategy(
-    #     ppi_db_fpns=DEFINE['ppi_db_fpns'],
-    #     uniprot_id='Q29Q28',
-    #     is_del_reflexive=False,
-    #     is_del_repeated=False,
-    # ))
+        )
```

### Comparing `tmkit-0.0.0.2/tmkit/db/Reader.py` & `tmkit-0.0.2/tmkit/db/Reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 __maintainer__ = "Jianfeng Sun"
 
 import numpy as np
 import pandas as pd
 from tmkit.util.Reader import reader as greader
 
 
-class reader(object):
+class reader:
 
     def __init__(self, ):
         self.__sort_ = -1
         self.greader = greader()
 
     @property
     def sort_(self):
@@ -114,17 +114,8 @@
             'score',
         ]
         results['aa'] = results['aa'].astype(str)
         recombine = results[[
             'interact_id',
             'score',
         ]]
-        return recombine
-
-
-if __name__ == "__main__":
-    p = reader()
-    from Path import to
-    print(p.graphppis(
-        graphppis_path=to('data/example/isite/graphppis/pdbtm_fast/'),
-        file_name='5b0w', file_chain='A', sort_=0
-    ))
+        return recombine
```

### Comparing `tmkit-0.0.0.2/tmkit/db/cath/Reader.py` & `tmkit-0.0.2/tmkit/db/cath/Reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,41 +7,55 @@
 
 import json
 import requests
 import pandas as pd
 from tmkit.util.Reader import reader as greader
 from tmkit.util.Writer import writer
 from tmkit.util.Kit import tactic7
-from tmkit.util.Console import console
 
 
-class reader(object):
+class reader:
 
     def __init__(
             self,
-            verbose=True,
     ):
         self.greader = greader()
         self.writer = writer()
 
-        self.console = console()
-        self.console.verbose = verbose
-
     def api(self, identifier):
         """
 
         :param identifier: complex_name + chain_id + domain_id; e.g., 1h2sB00
         :return:
         """
         return {
             'domain': 'http://www.cathdb.info/version/v4_2_0/api/rest/domain_summary/' + identifier,
             'funfam': 'http://www.cathdb.info/version/v4_2_0/api/rest/superfamily/1.10.8.10/funfam/' + identifier,
             'superfamily': 'http://www.cathdb.info/version/v4_2_0/api/rest/superfamily/' + identifier,
         }
 
+    def download(self, sv_fp, version='newest'):
+        from tmkit.util.Kit import urlliby
+        print('===>The CATH database of version ' + version + ' is being downloaded...')
+        urlliby(
+            url='ftp://orengoftp.biochem.ucl.ac.uk/cath/releases/daily-release/' + version + '/cath-b-' + version + '-all.gz',
+            fpn=sv_fp + 'cath-b-' + version + '-all.gz',
+        )
+        print('===>The CATH database of version ' + version + ' is successfully downloaded!')
+        print('===>The CATH database of version ' + version + ' is being decompressed...')
+        from tmkit.util.Kit import ungz
+        ungz(
+            file_path=sv_fp,
+            file_name='cath-b-' + version + '-all',
+            sv_fp=sv_fp,
+            new_suffix='.txt',
+        )
+        print('===>The CATH database of version ' + version + ' is successfully decompressed!')
+        return 'Finished!'
+
     def fetch(self, domain_id, sort):
         """
         domain_id='4ni4H02', sort='domain'
         :param domain_id:
         :param sort:
         :return:
         """
@@ -50,25 +64,25 @@
             # this is to avoid a domain in the file
             # exist but the domain via api does not exist.
             return json['data']
         else:
             return {}
 
     def domain(self, cath_fpn, groupby='version', group='v4_2_0'):
-        self.console.print('======>reading CATH...')
+        print('======>reading CATH...')
         df_domain = self.greader.generic(df_fpn=cath_fpn, df_sep='\s+')
         df_domain = df_domain.rename(columns={
             0: 'domain',
             1: 'version',
             2: 'superfamily',
             3: 'bound',
         })
-        self.console.print('======>CATH features are: '.format())
+        print('======>CATH features are: '.format())
         for i, e in enumerate(df_domain.columns):
-            self.console.print('=========>No.{}: {}'.format(i + 1, e))
+            print('=========>No.{}: {}'.format(i + 1, e))
         domain_info_grouped = df_domain.groupby(by=[groupby]).get_group(group)
         return domain_info_grouped
 
     def funfamsToJson(self, df_prot, df_domain, sv_fpn='./results.json', targets=['funfam_number']):
         complex_ids = df_domain['domain'].apply(lambda x: x[:4])
         chain_ids = df_domain['domain'].apply(lambda x: x[4])
         domain_ids = df_domain['domain'].apply(lambda x: x[5:])
@@ -76,64 +90,27 @@
         domain_dict = tactic7(complex_info)
         # print(domain_dict)
         cands = {}
         for i in df_prot.index:
             prot_name = df_prot.loc[i, 'prot']
             # seq_chain = self.df_prot.loc[i, 1]
             # print('----> No.{} protein {} chain {}'.format(i + 1, prot_name, seq_chain))
-            self.console.print('======>No.{} protein complex: {}'.format(i + 1, prot_name))
+            print('======>No.{} protein complex: {}'.format(i + 1, prot_name))
             if prot_name in domain_dict.keys():
                 cands[prot_name] = {}
                 # if seq_chain in domain_dict[prot_name].keys():
                 for seq_chain in domain_dict[prot_name].keys():
                     cands[prot_name][seq_chain] = {}
                     for domain_id in domain_dict[prot_name][seq_chain]:
-                        self.console.print('=========>domain id is: {}'.format(prot_name + seq_chain + domain_id))
+                        print('=========>domain id is: {}'.format(prot_name + seq_chain + domain_id))
                         domain_data = self.fetch(
                             domain_id=prot_name + seq_chain + domain_id,
                             sort='domain'
                         )
                         cands[prot_name][seq_chain][domain_id] = {}
                         for target in targets:
                             if target in domain_data.keys():
                                 cands[prot_name][seq_chain][domain_id][target] = domain_data[target]
         with open(sv_fpn, 'w') as fp:
             json.dump(cands, fp)
-        self.console.print('======>The file is saved.')
-        return cands
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    DEFINE = {
-        'prot_fpn': to('data/example/pdb/indepdata/prot_n30.txt'),
-        'cath_fpn': to('data/example/cath/cath_b.20200812.all'),
-        'sv_fpn': to('data/example/cath/compdata.json'),
-    }
-
-    p = reader()
-
-    # print(p.api(identifier='1cukA01'))
-    #
-    # print(p.domain(DEFINE['cath_fpn']))
-    #
-    # print(p.fetch(domain_id='4ni4H02', sort='domain'))
-
-    df_prot = greader().generic(DEFINE['prot_fpn'])
-
-    dm_reviewed = p.domain(
-        cath_fpn=DEFINE['cath_fpn'],
-        groupby='version',
-        group='v4_2_0'
-    )
-
-    print(p.funfamsToJson(
-        df_prot=df_prot,
-        df_domain=dm_reviewed,
-        sv_fpn=DEFINE['sv_fpn'],
-        targets=[
-            'funfam_number',
-            'superfamily_id',
-            'pdb_segments',
-        ],
-    ))
+        print('======>The file is saved.')
+        return cands
```

### Comparing `tmkit-0.0.0.2/tmkit/db/construct/Network.py` & `tmkit-0.0.2/tmkit/db/construct/Network.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,17 @@
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import numpy as np
-from tmkit.util.Console import console
 
 
-class network():
-
-    def __init__(
-            self,
-            verbose=True,
-    ):
-        self.console = console()
-        self.console.verbose = verbose
+class network:
 
     def single(self, interacting_df, uniprot_id, by=[], is_del_reflexive=False, is_del_repeated=False):
         """
 
         Parameters
         ----------
         interacting_df
@@ -38,24 +30,24 @@
         """
         interacting_left = interacting_df.groupby(by=[by[0]])
         interacting_right = interacting_df.groupby(by=[by[1]])
         # print(interacting_left.groups.keys())
         if uniprot_id in interacting_left.groups.keys():
             interacting_left_grouped = np.array(interacting_left.get_group(uniprot_id))
             # print(interacting_left_grouped)
-            self.console.print('=========>Record(s) for {} found in the left column.'.format(uniprot_id))
+            print('=========>Record(s) for {} found in the left column.'.format(uniprot_id))
         else:
-            self.console.print('=========>No record(s) for {} found in the left column.'.format(uniprot_id))
+            print('=========>No record(s) for {} found in the left column.'.format(uniprot_id))
             interacting_left_grouped = np.empty(shape=[0, 2])
         if uniprot_id in interacting_right.groups.keys():
             interacting_right_grouped = np.array(interacting_right.get_group(uniprot_id))[:, [1, 0]]  # exchange the order of the two
             # print(interacting_right_grouped)
-            self.console.print('=========>Record(s) for {} found in the left column.'.format(uniprot_id))
+            print('=========>Record(s) for {} found in the left column.'.format(uniprot_id))
         else:
-            self.console.print('=========>No record(s) for {} found on the right column.'.format(uniprot_id))
+            print('=========>No record(s) for {} found on the right column.'.format(uniprot_id))
             interacting_right_grouped = np.empty(shape=[0, 2])
         if is_del_reflexive:
             A_row_marker = np.where(
                 interacting_left_grouped[:, 0] == interacting_left_grouped[:, 1]
             )
             B_row_marker = np.where(
                 interacting_right_grouped[:, 0] == interacting_right_grouped[:, 1]
```

### Comparing `tmkit-0.0.0.2/tmkit/db/muthtp/Reader.py` & `tmkit-0.0.2/tmkit/db/muthtp/Reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,23 @@
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 from tmkit.util.Reader import reader as greader
-from tmkit.util.Console import console
 
 
-class reader(object):
+class reader:
 
     def __init__(
             self,
-            verbose=True,
     ):
         self.greader = greader()
 
-        self.console = console()
-        self.console.verbose = verbose
-
         self.muthtp_dz_std_keys = {
             'cancers': '1',
             'Cancers': '1',
             'cardiovascular diseases': '2',
             'congenital disorders of metabolism': '3',
             'digestive system diseases': '4',
             'endocrine and metabolic diseases': '5',
@@ -53,25 +48,40 @@
             '10': 'urinary system diseases',
             '11': 'reproductive system diseases',
             '12': 'respiratory diseases',
             '13': 'skin diseases',
             '14': 'unknown',
         }
 
+    def fetch(self, sv_fp, version='2020'):
+        from tmkit.util.Kit import urlliby
+        print('===>The MutHTP database of version ' + version + ' is being downloaded...')
+        urlliby(
+            url='https://github.com/2003100127/tmkit/releases/download/muthtp/MutHTP_' + version + '.zip',
+            fpn=sv_fp + 'MutHTP_' + version + '.zip',
+        )
+        print('===>The MutHTP database of version ' + version + ' is successfully downloaded!')
+        print('===>The MutHTP database of version ' + version + ' is being decompressed...')
+        import zipfile
+        with zipfile.ZipFile(sv_fp + 'MutHTP_' + version + '.zip', 'r') as zip_ref:
+            zip_ref.extractall(sv_fp)
+        print('===>The MutHTP database of version ' + version + ' is successfully decompressed!')
+        return 'Finished!'
+
     def full(self, muthtp_fpn):
         """
 
         origin:
             Germline: mutation occurs in a germ cell
             Somatic: mutation occurs in a somatic cell
             Unknown: origin unknown
         :param muthtp_fpn:
         :return:
         """
-        self.console.print('======>reading MutHTP...')
+        print('======>reading MutHTP...')
         all = self.greader.generic(muthtp_fpn, header=0)
         all = all.rename(columns={
             'Entry': 'id',
             'genename': 'gene_id',
             'uniportid': 'uniprot_id',
             'type_of_mutation': 'mutation_type',
             'chromosome_number': 'chromosome_number',
@@ -89,21 +99,11 @@
             'isoform': 'uniprot_id_isoform',
             'neighbour': 'neighbouring_residue',
             'source': 'source_database',
             'cs': 'conservation_score',
             'exac_freq': 'odds_ratio',
             'type_pass': 'type_passing_membrane',
         })
-        self.console.print('======>MutHTP features are: '.format())
+        print('======>MutHTP features are: '.format())
         for i, e in enumerate(all.columns):
-            self.console.print('=========>No.{}: {}'.format(i+1, e))
-        return all
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    p = reader()
-
-    print(p.full(
-        muthtp_fpn=to('data/example/mut/final_to_upload_17Mar_2020.txt')
-    ))
+            print('=========>No.{}: {}'.format(i+1, e))
+        return all
```

### Comparing `tmkit-0.0.0.2/tmkit/db/predmuthtp/Reader.py` & `tmkit-0.0.2/tmkit/db/predmuthtp/Reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,46 +3,56 @@
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 from tmkit.util.Reader import reader as greader
 from tmkit.util.Writer import writer as gwriter
-from tmkit.util.Console import console
 
 
-class reader(object):
+class reader:
 
     def __init__(
             self,
-            verbose=True,
     ):
         self.greader = greader()
         self.gwriter = gwriter()
 
-        self.console = console()
-        self.console.verbose = verbose
+    def fetch(self, sv_fp, ):
+        from tmkit.util.Kit import urlliby
+        print('===>The Pred-MutHTP database is being downloaded...')
+        urlliby(
+            url='https://www.iitm.ac.in/bioinfo/PredMutHTP/pred_varhtp_mut.zip',
+            fpn=sv_fp + 'pred_varhtp_mut.zip',
+        )
+        print('===>The Pred-MutHTP database is successfully downloaded!')
+        print('===>The Pred-MutHTP database is being decompressed...')
+        import zipfile
+        with zipfile.ZipFile(sv_fp + 'pred_varhtp_mut.zip', 'r') as zip_ref:
+            zip_ref.extractall(sv_fp)
+        print('===>The Pred-MutHTP database is successfully decompressed!')
+        return 'Finished!'
 
     def readall(self, pred_muthtp_fpn):
-        self.console.print('======>reading Pred-MutHTP...')
+        print('======>reading Pred-MutHTP...')
         all = self.greader.generic(pred_muthtp_fpn, df_sep=',')
         all = all.rename(columns={
             0: 'uniprot_id',
             1: 'protein_mutation_site',
             2: 'topology',
             3: 'mutation_type',
             4: 'mut_prob',
         })
-        self.console.print('======>Pred-MutHTP features are: '.format())
+        print('======>Pred-MutHTP features are: '.format())
         for i, e in enumerate(all.columns):
-            self.console.print('=========>No.{}: {}'.format(i + 1, e))
+            print('=========>No.{}: {}'.format(i + 1, e))
         return all
 
     def readsingle(self, pred_split_muthtp_fpn):
-        self.console.print('======>reading split Pred-MutHTP...')
+        print('======>reading split Pred-MutHTP...')
         all = self.greader.generic(pred_split_muthtp_fpn, header=0)
         return all
 
     def split(self, pred_muthtp_df, sv_fp):
         """
 
         Parameters
@@ -59,37 +69,16 @@
             'protein_mutation_site',
             'mut_prob',
         ]]
         # uniprot_ids = pd.unique(muthtp_df['uniprot_id'])
         # pred_muthtp_uniprot_ids = pd.unique(pred_muthtp_df['uniprot_id'])
         pred_muthtp_df_gp = pred_muthtp_df.groupby(['uniprot_id'])
         pred_muthtp_df_gp_keys = pred_muthtp_df_gp.groups.keys()
-        self.console.print('======>{} uniprot proteins'.format(len(pred_muthtp_df_gp_keys)))
+        print('======>{} uniprot proteins'.format(len(pred_muthtp_df_gp_keys)))
         for i, prot_id in enumerate(pred_muthtp_df_gp_keys):
-            self.console.print('=========>Splitting No.{} protein from Pred-MutHTP'.format(i))
+            print('=========>Splitting No.{} protein from Pred-MutHTP'.format(i))
             cc = pred_muthtp_df_gp.get_group(prot_id)
             self.gwriter.generic(
                 df=cc, sv_fpn=sv_fp + prot_id + '.predmuthtp',
                 header=True,
             )
-        return 0
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    p = reader()
-    from tmkit.db.muthtp.Reader import reader as muthtpreader
-
-    pred_muthtp_df = p.readall(
-        pred_muthtp_fpn=to('data/example/mut/pred_varhtp_mut.csv')
-    )
-    print(pred_muthtp_df)
-
-    muthtp_df = muthtpreader().full(
-        muthtp_fpn=to('data/example/mut/final_to_upload_17Mar_2020.txt')
-    )
-
-    print(p.split(
-        pred_muthtp_df,
-        sv_fp=to('data/example/mut/')
-    ))
+        return 0
```

### Comparing `tmkit-0.0.0.2/tmkit/feature/HelixSurface.py` & `tmkit-0.0.2/tmkit/property/HelixSurface.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,63 +6,52 @@
 __maintainer__ = "Jianfeng Sun"
 
 import subprocess
 import numpy as np
 import pandas as pd
 from tmkit.util.Kit import chainid
 from tmkit.util.Kit import tactic5, tactic6
-from tmkit.util.Console import console
 
 
-class helixSurface(object):
+class helixSurface:
 
     def __init__(
             self,
             msa_path=None,
             lips_fpn=None,
             prot_name=None,
             file_chain=None,
             sv_fp=None,
             df_prot=None,
-            verbose=True,
     ):
         self.msa_path = msa_path
         self.lips_fpn = lips_fpn
         self.sv_fp = sv_fp
         self.df_prot = df_prot
         self.prot_name = prot_name
         self.file_chain = file_chain
 
-        self.console = console()
-        self.console.verbose = verbose
-
     def generate(self):
-        """
-        single generate
-        :return:
-        """
+        """"""
         msa_fpn = self.msa_path + self.prot_name + self.file_chain + '.aln'
         sv_fpn = self.sv_fp + self.prot_name + self.file_chain + '/'
         self.surf = subprocess.call([
             'perl',
             self.lips_fpn,
             msa_fpn,
             sv_fpn,
         ], shell=True)
         return 0
 
     def bgenerate(self):
-        """
-        batch generate
-        :return:
-        """
+        """"""
         for i, prot_name in enumerate(self.df_prot['prot']):
             prot_chain = self.df_prot['chain'][i]
             file_chain = chainid(prot_chain)
-            self.console.print('=========>No.{} protein {}'.format(i, prot_name + file_chain))
+            print('=========>No.{} protein {}'.format(i, prot_name + file_chain))
             self.msa_fpn = self.msa_path + prot_name + file_chain + '.aln'
             sv_fpn = self.sv_fp + prot_name + file_chain + '/'
             self.surf = subprocess.call([
                 'perl',
                 self.lips_fpn,
                 self.msa_fpn,
                 sv_fpn,
@@ -78,26 +67,26 @@
                 columns=[
                     'aa_ids',
                     'aa_names',
                     'lipos',
                     'ents',
                 ],
             )
-            surf_x['aa_ids'] = surf_x['aa_ids'].apply(np.int)
-            surf_x['lipos'] = surf_x['lipos'].apply(np.float)
-            surf_x['ents'] = surf_x['ents'].apply(np.float)
+            surf_x['aa_ids'] = surf_x['aa_ids'].apply(int)
+            surf_x['lipos'] = surf_x['lipos'].apply(float)
+            surf_x['ents'] = surf_x['ents'].apply(float)
             surf_x['surf'] = int(i)
         return surf_x
 
     def transformToRosseta(self, df_surf_lips):
         d = []
         for i in df_surf_lips.index:
             o = df_surf_lips['surfs'][i]
             b = self.surface(o)
-            self.console.print('======>reading surface {}'.format(o))
+            print('======>reading surface {}'.format(o))
             b['mean_lipo']= df_surf_lips.loc[o]['lxe']
             b = b[[
                 'aa_ids',
                 'mean_lipo',
                 'lipos',
                 'ents',
             ]]
@@ -113,18 +102,18 @@
                 columns=[
                     'surfs',
                     'lipos',
                     'ents',
                     'lxe'
                 ]
             )
-            lips_surf['surfs'] = lips_surf['surfs'].apply(np.int)
-            lips_surf['lipos'] = lips_surf['lipos'].apply(np.float)
-            lips_surf['ents'] = lips_surf['ents'].apply(np.float)
-            lips_surf['lxe'] = lips_surf['lxe'].apply(np.float)
+            lips_surf['surfs'] = lips_surf['surfs'].apply(int)
+            lips_surf['lipos'] = lips_surf['lipos'].apply(float)
+            lips_surf['ents'] = lips_surf['ents'].apply(float)
+            lips_surf['lxe'] = lips_surf['lxe'].apply(float)
         return lips_surf
 
     def read(self):
         surfs = pd.DataFrame()
         surf_lipos = pd.DataFrame()
         surf_ents = pd.DataFrame()
         for i in range(7):
```

### Comparing `tmkit-0.0.0.2/tmkit/id/Mapping.py` & `tmkit-0.0.2/tmkit/id/Mapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,18 @@
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import numpy as np
-from tmkit.util.Console import console
 from tmkit.util.Reader import reader as tmkreader
 
 
-class mapping(object):
-
-    def __init__(
-            self,
-            verbose=True,
-    ):
-        self.console = console()
-        self.console.verbose = verbose
+class mapping:
 
     def tofas(
             self,
             pdbid_map,
             fasid_map,
             pdb_lower,
             pdb_upper,
@@ -45,27 +37,27 @@
         -------
 
         """
         pdb_fas_id_map = dict(zip([*pdbid_map.keys()], [*fasid_map.keys()]))
         pdb_ids = [*pdbid_map.keys()]
         pdb_seg_lower = np.array(pdb_lower)
         pdb_seg_upper = np.array(pdb_upper)
-        self.console.print('=========>Segment lower pdb id: {}'.format(pdb_seg_lower))
-        self.console.print('=========>Segment upper pdb id: {}'.format(pdb_seg_upper))
+        # print('=========>Segment lower pdb id: {}'.format(pdb_seg_lower))
+        # print('=========>Segment upper pdb id: {}'.format(pdb_seg_upper))
         fasta_seg_lower = []
         fasta_seg_upper = []
         num_segments = pdb_seg_lower.shape[0]
         for j in range(num_segments):
             if pdb_seg_lower[j] in pdb_ids:
                 fasta_seg_lower.append(pdb_fas_id_map[pdb_seg_lower[j]])
                 fasta_seg_upper.append(pdb_fas_id_map[pdb_seg_upper[j]])
             else:
                 continue
-        self.console.print('=========>Segment lower fasta id: {}'.format(fasta_seg_lower))
-        self.console.print('=========>Segment upper fasta id: {}'.format(fasta_seg_upper))
+        # print('=========>Segment lower fasta id: {}'.format(fasta_seg_lower))
+        # print('=========>Segment upper fasta id: {}'.format(fasta_seg_upper))
         return fasta_seg_lower, fasta_seg_upper
 
     def entryConvert(
             self,
             id,
             ref_fpn,
             mode,
```

### Comparing `tmkit-0.0.0.2/tmkit/id/PDB.py` & `tmkit-0.0.2/tmkit/id/PDB.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/tmkit/mut.py` & `tmkit-0.0.2/tmkit/mut.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,35 @@
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 from tmkit.db.muthtp.Reader import reader as muthtpreader
 from tmkit.db.predmuthtp.Reader import reader as predmuthtpreader
 
 
+def download_muthtp_db(
+        sv_fp,
+        version='2020',
+):
+    """
+
+    Parameters
+    ----------
+    sv_fp
+    version
+
+    Returns
+    -------
+
+    """
+    return muthtpreader().fetch(
+        version=version,
+        sv_fp=sv_fp,
+    )
+
+
 def read_muthtp_db(
         muthtp_fpn
 ):
     """
 
     Parameters
     ----------
@@ -23,14 +44,33 @@
 
     """
     return muthtpreader().full(
         muthtp_fpn
     )
 
 
+def download_predmuthtp_db(
+        sv_fp,
+):
+    """
+
+    Parameters
+    ----------
+    sv_fp
+    version
+
+    Returns
+    -------
+
+    """
+    return predmuthtpreader().fetch(
+        sv_fp=sv_fp,
+    )
+
+
 def read_predmuthtp_db(
         pred_muthtp_fpn
 ):
     """
 
     Parameters
     ----------
@@ -77,31 +117,8 @@
 
     Returns
     -------
 
     """
     return predmuthtpreader().readsingle(
         pred_split_muthtp_fpn=pred_split_muthtp_fpn,
-    )
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    # print(read_muthtp_db(
-    #     muthtp_fpn=to('data/example/mut/final_to_upload_17Mar_2020.txt')
-    # ))
-
-    # pred_muthtp_df = read_predmuthtp_db(
-    #     pred_muthtp_fpn=to('data/example/mut/pred_varhtp_mut.csv')
-    # )
-    # print(pred_muthtp_df)
-
-    # split_predmuthtp(
-    #     pred_muthtp_df=pred_muthtp_df,
-    #     sv_fp=to('data/example/mut/')
-    # )
-
-    pred_muthtp_df = read_split_predmuthtp(
-        pred_split_muthtp_fpn=to('data/example/mut/W5XKT8.predmuthtp')
-    )
-    print(pred_muthtp_df)
+    )
```

### Comparing `tmkit-0.0.0.2/tmkit/position/scenario/Segment.py` & `tmkit-0.0.2/tmkit/position/scenario/Segment.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/tmkit/position/scenario/Separation.py` & `tmkit-0.0.2/tmkit/position/scenario/Separation.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/tmkit/retrieve/PDB.py` & `tmkit-0.0.2/tmkit/retrieve/PDB.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,23 @@
 __maintainer__ = "Jianfeng Sun"
 
 from Bio.PDB import PDBList
 from tmkit.util.Kit import ungz
 from tmkit.util.Kit import urlliby
 from tmkit.util.Kit import delete
 from tmkit.util.Kit import batchRename
-from tmkit.util.Console import console
 
 
-class pdb(object):
+class pdb:
 
     def __init__(
             self,
             prot_series,
-            verbose=True,
     ):
         self.prot_dedup = prot_series.unique()
-        self.console = console()
-        self.console.verbose = verbose
 
     def rcsb(self, sv_fp, route='biopython'):
         """
 
         Notes
         -----
             Downloading a PDB file from RCSB PDB.
@@ -49,29 +45,30 @@
         Returns
         -------
 
         """
         pdb_list = PDBList()
         if route == 'biopython':
             for i, prot_name in enumerate(self.prot_dedup):
-                self.console.print('===>No.{} protein name: {}'.format(i + 1, prot_name))
+                print('===>No.{} protein name: {}'.format(i + 1, prot_name))
                 pdb_list.retrieve_pdb_file(
                     pdb_code=str(prot_name),
                     file_format='pdb',
                     pdir=sv_fp,
                 )
+                print("======>successfully downloaded!")
             batchRename(
                 file_path=sv_fp,
                 old_suffix='ent',
                 new_suffix='pdb',
                 flag=0,
             )
         else:
             for i, prot_name in enumerate(self.prot_dedup):
-                self.console.print('===>No.{} protein name: {}'.format(i + 1, prot_name))
+                print('===>No.{} protein name: {}'.format(i + 1, prot_name))
                 url = 'https://files.rcsb.org/download/' + prot_name + '.pdb'
                 urlliby(
                     url=url,
                     fpn=sv_fp + str(prot_name) + '.pdb',
                 )
         return 0
 
@@ -94,44 +91,48 @@
         -------
 
         """
         count = 0
         for i, prot_name in enumerate(self.prot_dedup):
             mark = str(prot_name[1] + prot_name[2])
             url = 'http://pdbtm.enzim.hu/data/database/' + mark + '/' + str(prot_name) + '.' + kind + 'pdb.gz'
-            self.console.print('===>No.{} protein name: {}'.format(i + 1, prot_name))
+            print('===>No.{} protein name: {}'.format(i + 1, prot_name))
             try:
                 urlliby(
                     url=url,
                     fpn=sv_fp + str(prot_name) + '.gz'
                 )
                 ungz(
                     file_path=sv_fp,
                     file_name=prot_name,
                     sv_fp=sv_fp,
                     new_suffix='.pdb'
                 )
                 delete(sv_fp + str(prot_name) + '.gz')
+                print("======>successfully downloaded!")
             except:
                 count = count + 1
-                print(count)
+                # print(count)
                 continue
         return 0
 
+    def alphafold(self, sv_fp: str) -> None:
+        """
+        Download a PDB file of a protein from the AlphaFold database.
 
-if __name__ == "__main__":
-    from tmkit.util.Reader import reader
-    from tmkit.Path import to
-
-    DEFINE = {
-        'list_fpn': to('data/example/pdb/indepdata/prot_n30_.txt'),
-        'sv_fp': to('data/'),
-    }
-
-    prot_series = reader().generic(DEFINE['list_fpn'])
-    print(prot_series[0].unique())
-
-    p = pdb(prot_series=prot_series[0])
-
-    print(p.rcsb(sv_fp=DEFINE['sv_fp'], route='biopython'))
+        Args:
+            sv_fp (str): The path to save the downloaded PDB file.
 
-    # print(p.pdbtm(sv_fp=DEFINE['sv_fp']))
+        Examples:
+            >>> alphafold("Q5VSL9", "Q5VSL9.pdb")
+        """
+        import requests
+        for i, uniprot_acc in enumerate(self.prot_dedup):
+            print("===>No.{} protein name: {}".format(i + 1, uniprot_acc))
+            url = f"https://alphafold.ebi.ac.uk/files/AF-{uniprot_acc}-F1-model_v4.pdb"
+            result = requests.get(url, allow_redirects=True)
+            if result.status_code == 200:
+                with open(sv_fp + uniprot_acc + '.pdb', 'wb') as f:
+                    f.write(result.content)
+                print("======>successfully downloaded!")
+            else:
+                print(f"Failed to download. HTTP status code: {result.status_code}")
```

### Comparing `tmkit-0.0.0.2/tmkit/retrieve/XML.py` & `tmkit-0.0.2/tmkit/retrieve/XML.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,67 +4,46 @@
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import subprocess
 import urllib.request
 from tmkit.util.Writer import writer
-from tmkit.util.Console import console
 
 
-class xml(object):
+class xml:
 
     def __init__(
             self,
             prot_series,
-            verbose=True,
     ):
         self.write = writer()
         self.prot_dedup = prot_series.unique()
-        self.console = console()
-        self.console.verbose = verbose
 
     def pdbtm(self, sv_fp, is_cmd=False):
         count = 0
         fails = []
         for i, prot_name in enumerate(self.prot_dedup):
-            self.console.print('===>No.{} protein name: {}'.format(i, prot_name))
+            print('===>No.{} protein name: {}'.format(i + 1, prot_name))
             try:
                 url = 'http://pdbtm.enzim.hu/data/database/' + str(prot_name[1]) + str(prot_name[2]) + '/' + str(prot_name) + '.xml'
                 if is_cmd:
                     subprocess.Popen(
                         'wget ' + url,
                         stderr=subprocess.PIPE,
                         stdout=subprocess.PIPE,
                         shell=True
                     ).communicate()
+                    print("======>successfully downloaded!")
                 else:
                     urllib.request.urlretrieve(
                         url=url,
                         filename=sv_fp + str(prot_name) + '.xml'
                     )
+                    print("======>successfully downloaded!")
             except:
                 count = count + 1
                 fails.append(prot_name)
-                self.console.print('===>number of xml that cannot be downloaded {}'.format(count))
+                print('===>number of xml that cannot be downloaded {}'.format(count))
                 continue
         self.write.generic(fails, sv_fp + 'log_fail_ids.txt')
-        return 0
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-    from tmkit.util.Reader import reader
-
-    DEFINE = {
-        'list_fpn': to('data/example/pdb/indepdata/prot_n30_.txt'),
-        'sv_fp': to('data/'),
-    }
-
-    prot_df = reader().generic(DEFINE['list_fpn'])
-
-    p = xml(prot_series=prot_df[0])
-
-    print(p.pdbtm(
-        sv_fp=DEFINE['sv_fp'],
-        is_cmd=False
-    ))
+        return 0
```

### Comparing `tmkit-0.0.0.2/tmkit/rrc.py` & `tmkit-0.0.2/tmkit/rrc.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         fasid_map=fasids,
         xml_fp=xml_fp,
         prot_name=prot_name,
         seq_chain=seq_chain,
     )
     pair_arr = ppssegment().toPair(fasta_lower_tmh, fasta_upper_tmh)
 
-    sdist, _ = m(
+    sdist = m(
         tool_fp,
         file_name=prot_name,
         file_chain=seq_chain,
         pair_list=pair_arr,
         dist_df=dist_df,
         sort_=2
     )
@@ -173,40 +173,8 @@
         tool=tool,
         seq_sep_inferior=seq_sep_inferior,
         seq_sep_superior=seq_sep_superior,
         sort_=sort
     )
     tool_results = p.fetch()
     p.compare(target=tool_results, cut_off=110)
-    return
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    # print(read(
-    #     prot_name='1xqf',
-    #     seq_chain='A',
-    #     pdb_fp=to('data/example/'),
-    #     dist_fp=to('data/example/'),
-    #     xml_fp=to('data/example/'),
-    #     fasta_fp=to('data/example/'),
-    #     tool_fp=to('data/example/contact/'),
-    #     seq_sep_inferior=1,
-    #     seq_sep_superior=None,
-    #     tool='deephelicon'
-    # ))
-
-    print(evaluate(
-        prot_name='1xqf',
-        seq_chain='A',
-        pdb_fp=to('data/example/'),
-        dist_fp=to('data/example/'),
-        xml_fp=to('data/example/'),
-        fasta_fp=to('data/example/'),
-        cutoff=5.5,
-        tool_fp=to('data/example/contact/'),
-        tool='membrain2',
-        seq_sep_inferior=1,
-        seq_sep_superior=None,
-        sort=2,
-    ))
+    return
```

### Comparing `tmkit-0.0.0.2/tmkit/seq.py` & `tmkit-0.0.2/tmkit/seq.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,36 +2,155 @@
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 from tmkit.sequence.PDB import pdb as spdb
-from tmkit.sequence.Fasta import fasta as sfasta
+from tmkit.sequence import Fasta as sfasta
 from tmkit.sequence.XML import xml as sxml
 from tmkit.id.Fasta import fasta as idfas
 from tmkit.id.PDB import pdb as idpdb
 from tmkit.retrieve.PDB import pdb as repdb
+from tmkit.structure.PDB import pdb as stpdb
 from tmkit.retrieve.XML import xml as rexml
 
 
+def retrieve_pdb_from_rcsb(
+        prot_series,
+        sv_fp,
+        route='biopython'
+):
+    """
+
+    Parameters
+    ----------
+    prot_series
+    sv_fp
+    route
+
+    Returns
+    -------
+
+    """
+    return repdb(
+        prot_series=prot_series
+    ).rcsb(
+        sv_fp=sv_fp,
+        route=route,
+    )
+
+
+def retrieve_pdb_from_pdbtm(
+        prot_series,
+        sv_fp,
+        kind='tr',
+):
+    """
+
+    Parameters
+    ----------
+    prot_series
+    sv_fp
+    kind
+
+    Returns
+    -------
+
+    """
+    return repdb(
+        prot_series=prot_series
+    ).pdbtm(
+        sv_fp=sv_fp,
+        kind=kind,
+    )
+
+
+def retrieve_xml_from_pdbtm(
+        prot_series,
+        sv_fp,
+):
+    """
+
+    Parameters
+    ----------
+    prot_series
+    sv_fp
+
+    Returns
+    -------
+
+    """
+    return rexml(
+        prot_series=prot_series,
+    ).pdbtm(
+        sv_fp=sv_fp,
+        is_cmd=False,
+    )
+
+
+def retrieve_pdb_alphafold(
+        prot_series,
+        sv_fp,
+):
+    """
+
+    Notes
+    -----
+        sth
+
+    Parameters
+    ----------
+    prot_series
+        sth
+    sv_fp
+        sth
+
+    Returns
+    -------
+        sth
+
+    """
+    return repdb(
+        prot_series=prot_series
+    ).alphafold(
+        sv_fp=sv_fp,
+    )
+
+
+def retrieve_foldseek(
+        pdb_fp,
+        prot_name,
+        sv_fp,
+        file_chain='',
+):
+    """"""
+    return stpdb(
+        pdb_fp=pdb_fp,
+        prot_name=prot_name,
+        file_chain=file_chain,
+    ).search_foldseek(
+        sv_fp=sv_fp,
+    )
+
+
 def read_from_fasta(
     fasta_fpn,
 ):
     """
 
     Parameters
     ----------
     fasta_fpn
 
     Returns
     -------
 
     """
-    return sfasta().get(fasta_fpn=fasta_fpn)
+    return sfasta.get(fasta_fpn=fasta_fpn)
 
 
 def read_from_xml(
         xml_fp,
         xml_name,
         seq_chain,
 ):
@@ -117,131 +236,8 @@
 
     """
     return idpdb(
         pdb_fp=pdb_fp,
         prot_name=prot_name,
         seq_chain=seq_chain,
         file_chain=file_chain,
-    ).chain()
-
-
-def retrieve_pdb_from_rcsb(
-        prot_series,
-        sv_fp,
-        route='biopython'
-):
-    """
-
-    Parameters
-    ----------
-    prot_series
-    sv_fp
-    route
-
-    Returns
-    -------
-
-    """
-    return repdb(
-        prot_series=prot_series
-    ).rcsb(
-        sv_fp=sv_fp,
-        route=route,
-    )
-
-
-def retrieve_pdb_from_pdbtm(
-        prot_series,
-        sv_fp,
-        kind='tr',
-):
-    """
-
-    Parameters
-    ----------
-    prot_series
-    sv_fp
-    kind
-
-    Returns
-    -------
-
-    """
-    return repdb(
-        prot_series=prot_series
-    ).pdbtm(
-        sv_fp=sv_fp,
-        kind=kind,
-    )
-
-
-def retrieve_xml_from_pdbtm(
-        prot_series,
-        sv_fp,
-):
-    """
-
-    Parameters
-    ----------
-    prot_series
-    sv_fp
-
-    Returns
-    -------
-
-    """
-    return rexml(
-        prot_series=prot_series,
-    ).pdbtm(
-        sv_fp=sv_fp,
-        is_cmd=False,
-    )
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-    import pandas as pd
-
-    # print(fasid(
-    #     fasta_fpn=to('data/example/3puxG.fasta')
-    # ))
-
-    # print(read_from_pdb(
-    #     pdb_fp=to('data/example/'),
-    #     prot_name='1aig',
-    #     seq_chain='L',
-    #     file_chain='',
-    # ))
-
-    # print(read_from_xml(
-    #     xml_fp=to('data/example/'),
-    #     xml_name='1xqf',
-    #     seq_chain='A',
-    # ))
-
-    # print(read_from_fasta(
-    #     fasta_fpn=to('data/example/1xqfA.fasta')
-    # ))
-
-    # print(pdbid(
-    #     pdb_fp=to('data/example/'),
-    #     prot_name='3pux',
-    #     seq_chain='G',
-    #     file_chain='G',
-    # ))
-
-    # print(retrieve_pdb_from_rcsb(
-    #     prot_series=pd.Series(['6e3y', '6rfq', '6t0b']),
-    #     # route='biopython',
-    #     sv_fp=to('data/'),
-    # ))
-
-    # print(retrieve_pdb_from_pdbtm(
-    #     prot_series=pd.Series(['6e3y', '6rfq', '6t0b']),
-    #     kind='tr',
-    #     sv_fp=to('data/'),
-    # ))
-
-    print(retrieve_xml_from_pdbtm(
-        prot_series=pd.Series(['6e3y', '6rfq', '6t0b']),
-        sv_fp=to('data/'),
-    ))
+    ).chain()
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/Compare.py` & `tmkit-0.0.2/tmkit/seqnetrr/Compare.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,93 +2,104 @@
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import time
-from tmkit.seqnetrr.Path import to
 from tmkit.seqnetrr.window.Pair import pair
 from tmkit.seqnetrr.window.Single import single
-from tmkit.seqnetrr.util.Reader import reader as prrcreader
-from tmkit.seqnetrr.util.Writer import writer as pfwriter
 from tmkit.seqnetrr.combo.Length import length as plength
-from tmkit.seqnetrr.sequence.Fasta import fasta as sfasta
+from tmkit.sequence import Fasta as sfasta
 from tmkit.seqnetrr.combo.Position import position as pfasta
 from tmkit.seqnetrr.graph.Bipartite import bipartite as bigraph
 from tmkit.seqnetrr.graph.Unipartite import unipartite as unigraph
 from tmkit.seqnetrr.graph.Cumulative import cumulative as cumugraph
-from tmkit.seqnetrr.util.Console import console
+from tmkit.util.Reader import reader as prrcreader
+from tmkit.util.Writer import writer as pfwriter
 
 
-class compare(object):
+class compare:
 
     def __init__(
             self,
             fasta_path,
             window_size,
             seq_sep_inferior,
             pair_mode='patch',
             mode='hash',
             input_kind='general',
             list_fpn=None,
             fc_path=None,
             sv_fpn=None,
             is_sv=False,
             len_thres=500,
-            verbose=True,
     ):
+        """
+
+        Parameters
+        ----------
+        fasta_path
+        window_size
+        seq_sep_inferior
+        pair_mode
+        mode
+        input_kind
+        list_fpn
+        fc_path
+        sv_fpn
+        is_sv
+        len_thres
+        """
         self.sv_fpn = sv_fpn
         self.pfreader = prrcreader()
         self.pfwriter = pfwriter()
-        self.console = console()
-        self.console.verbose = verbose
         self.is_sv = is_sv
         self.fc_path = fc_path
         self.seq_sep_inferior = seq_sep_inferior
         self.pair_mode = pair_mode
         self.mode = mode
         self.len_thres = len_thres
         self.input_kind = input_kind
         self.window_size = window_size
         self.prot_df = self.pfreader.generic(list_fpn)
         self.prot_df['len_seq'] = -1
         for i in self.prot_df.index:
             prot_name = self.prot_df.iloc[i, 0]
             file_chain = self.chain(self.prot_df.iloc[i, 1])
-            sequence = sfasta().get(
+            sequence = sfasta.get(
                 fasta_fpn=fasta_path + prot_name + file_chain + '.fasta',
             )
             # print(sequence)
             self.prot_df.loc[i, 'seq'] = sequence
             self.prot_df.loc[i, 'len_seq'] = len(sequence)
         self.prot_df = self.prot_df.loc[self.prot_df['len_seq'] < len_thres].reset_index(drop=True)
-        self.console.print('Sequence separation inf: {}'.format(self.seq_sep_inferior))
-        self.console.print('Length thres: {}'.format(self.len_thres))
-        self.console.print('Window size: {}'.format(self.window_size))
-        self.console.print('Input kind: {}'.format(self.input_kind))
-        self.console.print('\n{}'.format(self.prot_df))
-        self.console.print(self.prot_df.shape)
+        print('Sequence separation inf: {}'.format(self.seq_sep_inferior))
+        print('Length thres: {}'.format(self.len_thres))
+        print('Window size: {}'.format(self.window_size))
+        print('Input kind: {}'.format(self.input_kind))
+        print('\n{}'.format(self.prot_df))
+        print(self.prot_df.shape)
 
     def chain(self, prot_chain):
         return str(prot_chain) + 'l' if str(prot_chain).islower() else str(prot_chain)
 
     def unipartite(self, mode):
-        self.console.print('Mode: {}'.format(mode))
+        print('Mode: {}'.format(mode))
         for i in self.prot_df.index:
             stime = time.time()
             sequence = self.prot_df.loc[i, 'seq']
             prot_name = self.prot_df.iloc[i, 0]
             file_chain = self.chain(self.prot_df.iloc[i, 1])
-            self.console.print('===>ID.{}'.format(i))
-            self.console.print('===>protein: {}'.format(prot_name + file_chain))
-            self.console.print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
+            print('===>ID.{}'.format(i))
+            print('===>protein: {}'.format(prot_name + file_chain))
+            print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
             # /* scenario of position */
             pos_list = plength(seq_sep_inferior=self.seq_sep_inferior).topair(len(sequence))
-            self.console.print('===>pair number: {}'.format(len(pos_list)))
+            print('===>pair number: {}'.format(len(pos_list)))
 
             # /* position */
             position = pfasta(sequence).pair(pos_list=pos_list)
 
             # /* window */
             window_m_ids = pair(
                 sequence=sequence,
@@ -105,31 +116,31 @@
             # /* local ec scores */
             list_2d = position
             p.assign(
                 fpn=self.fc_path + prot_name + file_chain + '.evfold',
                 list_2d=list_2d,
                 mode=mode,
             )
-            self.console.print('===>total time: {time}s.'.format(time=time.time() - stime))
+            print('===>total time: {time}s.'.format(time=time.time() - stime))
             # print(vec)
 
     def bipartite(self, pair_mode, mode):
-        self.console.print('Pair mode: {}'.format(pair_mode))
-        self.console.print('Mode: {}'.format(mode))
+        print('Pair mode: {}'.format(pair_mode))
+        print('Mode: {}'.format(mode))
         for i in self.prot_df.index:
             stime = time.time()
             sequence = self.prot_df.loc[i, 'seq']
             prot_name = self.prot_df.iloc[i, 0]
             file_chain = self.chain(self.prot_df.iloc[i, 1])
-            self.console.print('===>ID.{}'.format(i))
-            self.console.print('===>protein: {}'.format(prot_name + file_chain))
-            self.console.print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
+            print('===>ID.{}'.format(i))
+            print('===>protein: {}'.format(prot_name + file_chain))
+            print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
             # /* scenario of position */
             pos_list = plength(seq_sep_inferior=self.seq_sep_inferior).topair(len(sequence))
-            self.console.print('===>pair number: {}'.format(len(pos_list)))
+            print('===>pair number: {}'.format(len(pos_list)))
 
             # /* position */
             position = pfasta(sequence).pair(pos_list=pos_list)
 
             # /* window */
             window_m_ids = pair(
                 sequence=sequence,
@@ -148,30 +159,30 @@
             # /* global ec scores */
             list_2d = position
             p.assign(
                 fpn=self.fc_path + prot_name + file_chain + '.evfold',
                 list_2d=list_2d,
                 mode=mode,
             )
-            self.console.print('===>total time: {time}s.'.format(time=time.time() - stime))
+            print('===>total time: {time}s.'.format(time=time.time() - stime))
             # print(vec)
 
     def cumulative(self, cumu_ratio=0.5):
-        self.console.print('cumulative ratio: {}'.format(cumu_ratio))
+        print('cumulative ratio: {}'.format(cumu_ratio))
         for i in self.prot_df.index:
             stime = time.time()
             sequence = self.prot_df.loc[i, 'seq']
             prot_name = self.prot_df.iloc[i, 0]
             file_chain = self.chain(self.prot_df.iloc[i, 1])
-            self.console.print('===>ID.{}'.format(i))
-            self.console.print('===>protein: {}'.format(prot_name + file_chain))
-            self.console.print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
+            print('===>ID.{}'.format(i))
+            print('===>protein: {}'.format(prot_name + file_chain))
+            print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
             # /* scenario of position */
             pos_list = plength(seq_sep_inferior=self.seq_sep_inferior).tosgl(len(sequence))
-            self.console.print('===>pair number: {}'.format(len(pos_list)))
+            print('===>pair number: {}'.format(len(pos_list)))
 
             # /* position */
             position = pfasta(sequence).single(pos_list=pos_list)
 
             # /* window */
             window_m_ids = single(
                 sequence=sequence,
@@ -189,65 +200,8 @@
             list_2d = position
             p.assign(
                 list_2d=list_2d,
                 fpn=self.fc_path + prot_name + file_chain + '.evfold',
                 L=int(len(sequence) * cumu_ratio),
                 simu_seq_len=None,
             )
-            self.console.print('===>total time: {time}s.'.format(time=time.time() - stime))
-            # print(vec)
-
-
-if __name__ == "__main__":
-    DEFINE = {
-        # 'list_fpn': to('data/rrc/tm_alpha_n165/fasta/prot_n165.txt'),
-        # 'fasta_path': to('data/rrc/tm_alpha_n165/fasta/'),
-        # 'fc_path': to('data/rrc/tm_alpha_n165/freecontact/'),
-
-        # 'list_fpn': to('data/rrc/tm_alpha_n44/fasta/prot_n44.txt'),
-        # 'fasta_path': to('data/rrc/tm_alpha_n44/fasta/'),
-        # 'fc_path': to('data/rrc/tm_alpha_n44/freecontact/'),
-
-        'list_fpn': to('data/rrc/tm_alpha_n57/fasta/prot_n57.txt'),
-        'fasta_path': to('data/rrc/tm_alpha_n57/fasta/'),
-        'fc_path': to('data/rrc/tm_alpha_n57/freecontact/'),
-
-        'window_size': 2,
-        'seq_sep_inferior': 0,
-    }
-    p = compare(
-        fasta_path=DEFINE['fasta_path'],
-        list_fpn=DEFINE['list_fpn'],
-        fc_path=DEFINE['fc_path'],
-        window_size=DEFINE['window_size'],
-        seq_sep_inferior=DEFINE['seq_sep_inferior'],
-        verbose=True,
-
-        # input_kind='general',
-        input_kind='freecontact',
-        # input_kind='simulate',
-    )
-
-    print(p.unipartite(
-        # mode='hash_rl',
-        # mode='hash_ori',
-        # mode='hash',
-        # mode='pandas',
-        mode='numpy',
-    ))
-
-    # print(p.bipartite(
-    #     pair_mode='patch',
-    #     # pair_mode='cross',
-    #     # pair_mode='memconp',
-    #     # pair_mode='unchanged',
-    #
-    #     # mode='hash_rl',
-    #     # mode='hash_ori',
-    #     # mode='hash',
-    #     mode='pandas',
-    #     # mode='numpy',
-    # ))
-
-    # print(p.cumulative(
-    #     cumu_ratio=1,
-    # ))
+            print('===>total time: {time}s.'.format(time=time.time() - stime))
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/Controller.py` & `tmkit-0.0.2/tmkit/seqnetrr/Controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import time
 import argparse
-from tmkit.seqnetrr.Path import to
 from tmkit.seqnetrr.window.Pair import pair
 from tmkit.seqnetrr.window.Single import single
-from tmkit.seqnetrr.util.Writer import writer as pfwriter
+from tmkit.util.Writer import writer as pfwriter
 from tmkit.seqnetrr.combo.Length import length as plength
-from tmkit.seqnetrr.sequence.Fasta import fasta as sfasta
+from tmkit.sequence import Fasta as sfasta
 from tmkit.seqnetrr.combo.Position import position as pfasta
 from tmkit.seqnetrr.graph.Bipartite import bipartite as bigraph
 from tmkit.seqnetrr.graph.Unipartite import unipartite as unigraph
 from tmkit.seqnetrr.graph.Cumulative import cumulative as cumugraph
-from tmkit.seqnetrr.util.Console import console
 
 
-class controller(object):
+class controller:
 
     def __init__(
             self,
             method,
             fasta_fpn,
             net_fpn,
             window_size=2,
@@ -34,18 +32,15 @@
             pair_mode='patch',
             assign_mode='hash',
             input_kind='general',
             list_2d=None,
             cumu_ratio=None,
             is_sv=False,
             sv_fpn=None,
-            verbose=True,
     ):
-        self.console = console()
-        self.console.verbose = verbose
         self.pfwriter = pfwriter()
 
         if mode == 'internal':
             self.method = method
             self.net_fpn = net_fpn
             self.fasta_fpn = fasta_fpn
             self.window_size = window_size
@@ -170,24 +165,24 @@
             self.assign_mode = args.amode
             self.input_kind = args.ikind
             self.cumu_ratio = args.cr
             self.is_sv = args.issv
             self.sv_fpn = args.o
             self.list_2d = None
 
-        self.sequence = sfasta().get(fasta_fpn=self.fasta_fpn)
+        self.sequence = sfasta.get(fasta_fpn=self.fasta_fpn)
         self.len_seq = len(self.sequence)
 
-        self.console.print('===>Molecular sequence: {}'.format(self.sequence))
-        self.console.print('===>Molecule length: {}'.format(self.len_seq))
-        self.console.print('===>Window size: {}'.format(self.window_size))
-        self.console.print('===>Sequence separation inferior: {}'.format(self.seq_sep_inferior))
-        self.console.print('===>Sequence separation superior: {}'.format(self.seq_sep_superior))
-        self.console.print('===>Mode: {}'.format(mode))
-        self.console.print('===>Input kind: {}'.format(self.input_kind))
+        print('===>Molecular sequence: {}'.format(self.sequence))
+        print('===>Molecule length: {}'.format(self.len_seq))
+        print('===>Window size: {}'.format(self.window_size))
+        print('===>Sequence separation inferior: {}'.format(self.seq_sep_inferior))
+        print('===>Sequence separation superior: {}'.format(self.seq_sep_superior))
+        print('===>Mode: {}'.format(mode))
+        print('===>Input kind: {}'.format(self.input_kind))
 
         if self.method == 'unipartite':
             self.unipartite()
         elif self.method == 'bipartite':
             self.bipartite()
         elif self.method == 'cumulative':
             self.cumulative()
@@ -197,15 +192,15 @@
         # /* scenario of position */
         pos_list = plength(
             seq_sep_superior=self.seq_sep_superior,
             seq_sep_inferior=self.seq_sep_inferior,
         ).topair(self.len_seq)
         # print(pos_list[:10])
 
-        self.console.print('===>pair number: {}'.format(len(pos_list)))
+        print('===>pair number: {}'.format(len(pos_list)))
 
         # /* position */
         position = pfasta(self.sequence).pair(pos_list=pos_list)
         # print(position[:10])
 
         # /* window */
         window_m_ids = pair(
@@ -225,35 +220,35 @@
         list_2d = position if self.list_2d == None else self.list_2d
         p.assign(
             fpn=self.net_fpn,
             list_2d=list_2d,
             mode=self.assign_mode,
         )
         # print(list_2d[:10])
-        self.console.print('===>total time: {time}s.'.format(time=time.time() - stime))
+        print('===>total time: {time}s.'.format(time=time.time() - stime))
         if self.is_sv:
-            self.console.print('===>saving...')
+            print('===>saving...')
             self.pfwriter.generic(
                 df=list_2d,
                 sv_fpn=self.sv_fpn,
                 header=None,
                 index=None,
             )
-            self.console.print('===>saved!')
+            print('===>saved!')
         return list_2d
 
     def bipartite(self, ):
         stime = time.time()
-        self.console.print('===>Pair mode: {}'.format(self.pair_mode))
+        print('===>Pair mode: {}'.format(self.pair_mode))
         # /* scenario of position */
         pos_list = plength(
             seq_sep_superior=self.seq_sep_superior,
             seq_sep_inferior=self.seq_sep_inferior,
         ).topair(self.len_seq)
-        self.console.print('===>pair number: {}'.format(len(pos_list)))
+        print('===>pair number: {}'.format(len(pos_list)))
 
         # /* position */
         position = pfasta(self.sequence).pair(pos_list=pos_list)
 
         # /* window */
         window_m_ids = pair(
             sequence=self.sequence,
@@ -274,35 +269,35 @@
         p.assign(
             fpn=self.net_fpn,
             list_2d=list_2d,
             mode=self.assign_mode,
         )
         # print(list_2d[-5:])
 
-        self.console.print('===>total time: {time}s.'.format(time=time.time() - stime))
+        print('===>total time: {time}s.'.format(time=time.time() - stime))
         if self.is_sv:
-            self.console.print('===>saving...')
+            print('===>saving...')
             self.pfwriter.generic(
                 df=list_2d,
                 sv_fpn=self.sv_fpn,
                 header=None,
                 index=None,
             )
-            self.console.print('===>saved!')
+            print('===>saved!')
         return list_2d
 
     def cumulative(self, ):
-        self.console.print('cumulative ratio: {}'.format(self.cumu_ratio))
+        print('cumulative ratio: {}'.format(self.cumu_ratio))
         stime = time.time()
         # /* scenario of position */
         pos_list = plength(
             seq_sep_superior=None,
             seq_sep_inferior=None,
         ).tosgl(self.len_seq)
-        self.console.print('===>pair number: {}'.format(len(pos_list)))
+        print('===>pair number: {}'.format(len(pos_list)))
 
         # /* position */
         position = pfasta(self.sequence).single(pos_list=pos_list)
 
         # /* window */
         window_m_ids = single(
             sequence=self.sequence,
@@ -321,70 +316,18 @@
         p.assign(
             list_2d=list_2d,
             fpn=self.net_fpn,
             L=int(self.len_seq * self.cumu_ratio),
             simu_seq_len=None,
         )
 
-        self.console.print('===>total time: {time}s.'.format(time=time.time() - stime))
+        print('===>total time: {time}s.'.format(time=time.time() - stime))
         if self.is_sv:
-            self.console.print('===>saving...')
+            print('===>saving...')
             self.pfwriter.generic(
                 df=list_2d,
                 sv_fpn=self.sv_fpn,
                 header=None,
                 index=None,
             )
-            self.console.print('===>saved!')
-        return list_2d
-
-
-if __name__ == "__main__":
-    DEFINE = {
-        'prot_name': '1aig',
-        'file_chain': 'L',
-        'seq_chain': 'L',
-
-        # 'prot_name': '5lki',
-        # 'file_chain': 'A',
-        # 'seq_chain': 'A',
-
-        'seq_sep_inferior': 0,
-        'seq_sep_superior': None,
-
-        'window_size': 2,
-    }
-    p = controller(
-        mode='internal',
-        # mode='external',
-
-        # method='unipartite',
-        # method='bipartite',
-        method='cumulative',
-
-        fasta_fpn=to('data/example/') + DEFINE['prot_name'] + DEFINE['file_chain'] + '.fasta',
-        net_fpn=to('data/example/') + DEFINE['prot_name'] + DEFINE['file_chain'] + '.evfold',
-        window_size=DEFINE['window_size'],
-        seq_sep_inferior=DEFINE['seq_sep_inferior'],
-        seq_sep_superior=DEFINE['seq_sep_superior'],
-        verbose=True,
-
-        pair_mode='patch',
-        # pair_mode='cross',
-        # pair_mode='memconp',
-        # pair_mode='unchanged',
-
-        # assign_mode='hash_rl',
-        # assign_mode='hash_ori',
-        assign_mode='hash',
-        # assign_mode='pandas',
-        # assign_mode='numpy',
-
-        # input_kind='general',
-        input_kind='freecontact',
-        # input_kind='simulate',
-
-        cumu_ratio=1.,
-
-        is_sv=True,
-        sv_fpn=to('data/example/') + 'asd.txt',
-    )
+            print('===>saved!')
+        return list_2d
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/combo/Length.py` & `tmkit-0.0.2/tmkit/seqnetrr/combo/Length.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,19 +62,8 @@
             the length of a molecular sequence
 
         Returns
         -------
             2d array
 
         """
-        return self.computlib.num2arr2d(1, length)
-
-
-if __name__ == "__main__":
-    p = length(
-        seq_sep_inferior=1,
-        seq_sep_superior=None
-    )
-
-    print(p.topair(6, kind='under_triangular'))
-
-    # print(p.tosgl(8))
+        return self.computlib.num2arr2d(1, length)
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/combo/Position.py` & `tmkit-0.0.2/tmkit/seqnetrr/combo/Position.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 
-class position():
+class position:
 
     def __init__(self, sequence):
         self.sequence = sequence
         self.len_seq = len(self.sequence)
 
     def single(self, pos_list):
         """
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/combo/Separation.py` & `tmkit-0.0.2/tmkit/seqnetrr/combo/Separation.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/graph/Bipartite.py` & `tmkit-0.0.2/tmkit/seqnetrr/graph/Bipartite.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import time
 import numpy as np
-from tmkit.seqnetrr.Path import to
 from tmkit.seqnetrr.window.base import Pair as ecabPair
 from tmkit.seqnetrr.net.Reader import reader as prrcreader
-from tmkit.seqnetrr.util.Console import console
 
 
 class bipartite(ecabPair.pair):
     """
     Methods
     -------
         pairids(), assign()
@@ -28,15 +26,14 @@
     def __init__(
             self,
             sequence,
             window_size,
             window_m_ids,
             kind='memconp',
             patch_size=None,
-            verbose=True,
             input_kind='general',
     ):
         """
 
         Parameters
         ----------
         sequence
@@ -68,16 +65,14 @@
             ]
         if kind == 'unchanged':
             self.bigraph = [
                 [0, 0],
             ]
         self.num_to_dos = len(self.bigraph)
         self.num_to_dos_in_window = self.num_to_dos * self.aa_in_window_size
-        self.console = console()
-        self.console.verbose = verbose
         self.input_kind = input_kind
         if self.input_kind == 'general':
             self.file_initiator = self.prrcreader.general
         elif self.input_kind == 'freecontact':
             self.file_initiator = self.prrcreader.freecontact
         elif self.input_kind == 'mutual information':
             self.file_initiator = self.prrcreader.mi
@@ -161,15 +156,15 @@
                         # #/*** block 1.1.2.2 ***/
                         else:
                             if left < right:
                                 global_pair_ids[i].append([left, right])
                             else:
                                 global_pair_ids[i].append([right, left])
         end_time = time.time()
-        self.console.print('======>bipartite pair generation: {time}s.'.format(time=end_time - start_time))
+        print('======>bipartite pair generation: {time}s.'.format(time=end_time - start_time))
         # print(global_pair_ids)
         # print(len(global_pair_ids))
         # print(len(global_pair_ids[0]))
         # print(global_pair_ids[0])
         # print(len(global_pair_ids[0][0]))
         # print(global_pair_ids[0][0])
         return global_pair_ids
@@ -350,87 +345,9 @@
                             else:
                                 if left < right:
                                     # print(evfold_np[2][(evfold_np[0] == left) & (evfold_np[1] == right)][0])
                                     list_2d_[i].append(evfold_np[2][(evfold_np[0] == left) & (evfold_np[1] == right)][0])
                                 else:
                                     list_2d_[i].append(evfold_np[2][(evfold_np[0] == right) & (evfold_np[1] == left)][0])
         end_time = time.time()
-        self.console.print('======>bipartite pair assignment: {time}s.'.format(time=end_time - start_time))
-        return list_2d_
-
-
-if __name__ == "__main__":
-    from tmkit.seqnetrr.window.Pair import pair
-    from tmkit.seqnetrr.sequence.Fasta import fasta as sfasta
-    from tmkit.seqnetrr.combo.Position import position as pfasta
-    from tmkit.seqnetrr.combo.Length import length as plength
-
-    DEFINE = {
-        'prot_name': '1aig',
-        'file_chain': 'L',
-        'seq_chain': 'L',
-
-        # 'prot_name': '5lki',
-        # 'file_chain': 'A',
-        # 'seq_chain': 'A',
-
-        'cutoff': 5.5,
-        'seq_sep_inferior': 4,
-        'seq_sep_superior': None,
-        'fasta_path': to('data/example/'),
-    }
-
-    # /* sequence */
-    fasta_path = to('data/example/1aigL.fasta')
-    # fasta_path = to('data/example/5lkiA.fasta')
-    # sequence = sfasta().get(fasta_path)
-    sequence = sfasta().simulate(seq_len=100)
-
-    # /* scenario of position */
-    pos_list = plength(seq_sep_inferior=0).topair(len(sequence))
-
-    # /* position */
-    position = pfasta(sequence).pair(pos_list=pos_list)
-
-    # /* window */
-    window_size = 3
-    window_m_ids = pair(
-        sequence=sequence,
-        position=position,
-        window_size=window_size,
-    ).mid()
-    print(np.array(window_m_ids).shape)
-    print(window_m_ids[-1])
-    # print(window_m_ids)
-    # print(len(window_m_ids))
-    # print(len(window_m_ids[0]))
-    #
-    # print(window_m_ids[0])
-    # print(len(window_m_ids[0][0]))
-    # print(window_m_ids[0][0])
-
-    # /* global pairs */
-    p = bipartite(
-        sequence=sequence,
-        window_size=window_size,
-        window_m_ids=window_m_ids,
-        kind='patch',
-        # kind='cross',
-        # kind='memconp',
-        # kind='unchanged',
-        patch_size=2,
-        # input_kind='general',
-        # input_kind='freecontact',
-        input_kind='simulate',
-    )
-
-    # /* global ec scores */
-    vec = p.assign(
-        list_2d=position,
-        fpn=to('data/example/') + DEFINE['prot_name'] + DEFINE['file_chain'] + '.evfold',
-        # mode='hash_rf',
-        # mode='hash_ori',
-        mode='hash',
-        # mode='pandas',
-        # mode='numpy',
-    )
-    # print(vec)
+        print('======>bipartite pair assignment: {time}s.'.format(time=end_time - start_time))
+        return list_2d_
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/graph/Unipartite.py` & `tmkit-0.0.2/tmkit/seqnetrr/graph/Unipartite.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import time
 import itertools
 import numpy as np
-from tmkit.seqnetrr.Path import to
 from tmkit.seqnetrr.window.base import Pair as ecabPair
 from tmkit.seqnetrr.net.Reader import reader as prrcreader
-from tmkit.seqnetrr.util.Console import console
 
 
 class unipartite(ecabPair.pair):
     """
 
     Notes
     -----
@@ -32,24 +30,21 @@
     """
 
     def __init__(
             self,
             sequence,
             window_size,
             window_m_ids,
-            verbose=True,
             input_kind='general',
     ):
         super(unipartite, self).__init__(sequence, window_size, window_m_ids)
         self.prrcreader = prrcreader(
             seq_sep_inferior=None,
             seq_sep_superior=None
         )
-        self.console = console()
-        self.console.verbose = verbose
         self.input_kind = input_kind
         if self.input_kind == 'general':
             self.file_initiator = self.prrcreader.general
         elif self.input_kind == 'freecontact':
             self.file_initiator = self.prrcreader.freecontact
         elif self.input_kind == 'mutual information':
             self.file_initiator = self.prrcreader.mi
@@ -143,15 +138,15 @@
                     if l2[0] < l2[1]:
                         local_pairs[i].append([l2[0], l2[1]])
                     else:
                         local_pairs[i].append([l2[1], l2[0]])
                 else:
                     local_pairs[i].append([None, None])
         end_time = time.time()
-        self.console.print('======>unipartite pair generation: {time}s.'.format(time=end_time - start_time))
+        print('======>unipartite pair generation: {time}s.'.format(time=end_time - start_time))
         return local_pairs
 
     def combo2x2(self, array):
         """
 
         Notes
         -----
@@ -412,75 +407,9 @@
                     elif l2[0] is not None and l2[1] is not None:
                         if l2[0] < l2[1]:
                             list_2d_[i].append(evfold_np[2][(evfold_np[0] == l2[0]) & (evfold_np[1] == l2[1])][0])
                         else:
                             list_2d_[i].append(evfold_np[2][(evfold_np[0] == l2[1]) & (evfold_np[1] == l2[0])][0])
                     else:
                         list_2d_[i].append(0)
-        self.console.print('======>unipartite pair assignment: {time}s.'.format(time=time.time() - start_time))
-        return list_2d_
-
-
-if __name__ == "__main__":
-    from tmkit.seqnetrr.window.Pair import pair
-    from tmkit.seqnetrr.sequence.Fasta import fasta as sfasta
-    from tmkit.seqnetrr.combo.Position import position as pfasta
-    from tmkit.seqnetrr.combo.Length import length as plength
-
-    DEFINE = {
-        'prot_name': '1aig',
-        'file_chain': 'L',
-        'seq_chain': 'L',
-
-        # 'prot_name': '5lki',
-        # 'file_chain': 'A',
-        # 'seq_chain': 'A',
-
-        'cutoff': 5.5,
-        'seq_sep_inferior': 4,
-        'seq_sep_superior': None,
-        'fasta_path': to('data/example/'),
-    }
-
-    # /* sequence */
-    fasta_path = to('data/example/1aigL.fasta')
-    # sequence = sfasta().get(fasta_path)
-    sequence = sfasta().simulate(seq_len=100)
-
-    # /* scenario of position */
-    pos_list = plength(seq_sep_inferior=0).topair(len(sequence))
-
-    # /* position */
-    position = pfasta(sequence).pair(pos_list=pos_list)
-
-    # /* window */
-    window_size = 3
-    window_m_ids = pair(
-        sequence=sequence,
-        position=position,
-        window_size=window_size,
-    ).mid()
-    print(np.array(window_m_ids).shape)
-    print(window_m_ids[-1])
-
-    # /* unipartite ec values */
-    p = unipartite(
-        sequence=sequence,
-        window_size=window_size,
-        window_m_ids=window_m_ids,
-        # input_kind='general',
-        # input_kind='freecontact',
-        input_kind='simulate',
-    )
-
-    result = p.assign(
-        list_2d=position,
-        fpn=to('data/example/') + DEFINE['prot_name'] + DEFINE['file_chain'] + '.evfold',
-        # mode='hash_rl',
-        # mode='hash_ori',
-        mode='hash',
-        # mode='pandas',
-        # mode='numpy',
-    )
-    # print(result)
-    print(result[0])
-    print(len(result[0]))
+        print('======>unipartite pair assignment: {time}s.'.format(time=time.time() - start_time))
+        return list_2d_
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/net/Reader.py` & `tmkit-0.0.2/tmkit/seqnetrr/net/Reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import numpy as np
 import pandas as pd
-from tmkit.seqnetrr.util.Reader import reader as pfrreader
-from tmkit.seqnetrr.util.Writer import writer as pfwwriter
+from tmkit.util.Reader import reader as pfrreader
+from tmkit.util.Writer import writer as pfwwriter
 from tmkit.seqnetrr.combo.Separation import separation as ppssep
-from tmkit.seqnetrr.util.ComputLib import computLib
+from tmkit.seqnetrr.ComputLib import computLib
 
 
-class reader(object):
+class reader:
 
     def __init__(self, seq_sep_inferior=None, seq_sep_superior=None):
         self.__sort_ = -1
         self.seq_sep_inferior = seq_sep_inferior
         self.seq_sep_superior = seq_sep_superior
         self.pfrreader = pfrreader()
         self.pfwwriter = pfwwriter()
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/util/ComputLib.py` & `tmkit-0.0.2/tmkit/seqnetrr/ComputLib.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,16 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-import itertools
-import numpy as np
 
-
-class computLib(object):
-
-    def __init__(self, ):
-        pass
-
-    @classmethod
-    def interv2combi(cls, inf_arr, sup_arr):
-        """
-
-        Notes
-        -----
-                        1   2   3
-            inf_arr = [15, 48, 78]
-            sup_arr = [30, 53, 99]
-            element in interval No.1 matches elements in No.2,
-            No.3 one by one. and then, element in interval No.2
-            matches elements in interval No.3 until finished.
-
-        Parameters
-        ----------
-        inf_arr
-            1d list
-        sup_arr
-            1d list
-
-        Returns
-        -------
-
-        """
-        tmp_2d = []
-        num_interv = len(inf_arr)
-        for i in range(num_interv):
-            tmp_2d.append(list(np.arange(inf_arr[i], sup_arr[i] + 1)))
-        combi = []
-        for i in range(num_interv):
-            for j in range(num_interv):
-                if i < j:
-                    for p in range(len(tmp_2d[i])):
-                        for q in range(len(tmp_2d[j])):
-                            combi.append([tmp_2d[i][p], tmp_2d[j][q]])
-        # print(combi)
-        return combi
+class computLib:
 
     def interv2single(self, inf_arr, sup_arr):
         """
 
         Methods
         -------
                         1   2   3
@@ -202,53 +158,8 @@
         -------
 
         """
         arr = []
         for i in range(-length, length + 1, step):
             for j in range(-length, length + 1, step):
                 arr.append([i, j])
-        return arr
-
-    def combo2x2(self, array):
-        """
-
-        Notes
-        -----
-            repeated 2x2 combination of elements of an array.
-
-        Parameters
-        ----------
-        array
-
-        Returns
-        -------
-            amount of combo2x2: L*L.
-
-        """
-        combo = []
-        ob = itertools.product(array, repeat=2)
-        for i in ob:
-            combo.append(list(i))
-        return combo
-
-    def combo2x2_(self, array):
-        """
-
-        Notes
-        -----
-            nonrepeated 2x2 combination of elements of an array.
-
-        Parameters
-        ----------
-        array
-
-        Returns
-        -------
-            amount of combo2x2: L*(L-1)/2.
-
-        """
-        combo = []
-        ob = itertools.combinations(array, 2)
-        # #/*** block 1.1 ***/
-        for i in ob:
-            combo.append(list(i))
-        return combo
+        return arr
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/util/Console.py` & `tmkit-0.0.2/tmkit/util/Console.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-__author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
+__license__ = "MIT"
+__lab__ = "Adam Cribbs lab"
 
 from datetime import datetime
+from pyfiglet import Figlet
 
 
 class console:
 
     def __init__(self, placeholder='logger: ', verbose=False):
         self._verbose = verbose
         self.placeholder = placeholder
+        self.vignette1 = Figlet(font='standard')
+        print(self.vignette1.renderText('TMKit'))
 
     @property
     def verbose(self, ):
         return self._verbose
 
     @verbose.setter
     def verbose(self, value):
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/util/Reader.py` & `tmkit-0.0.2/tmkit/util/Reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import pandas as pd
 from functools import wraps
 
 
-class reader(object):
-
-    def __init__(self, ):
-        pass
+class reader:
 
     def __call__(self, deal):
         generic = self.generic
         excel = self.excel
         @wraps(deal)
         def read(ph, *args, **kwargs):
             deal(ph, **kwargs)
@@ -34,15 +31,15 @@
                     df_fpn=kwargs['df_fpn'],
                     sheet_name='Sheet1' if 'sheet_name' not in keys else kwargs['sheet_name'],
                     header=None if 'header' not in keys else kwargs['header'],
                     is_utf8=False if 'is_utf8' not in keys else kwargs['is_utf8'],
                 )
         return read
 
-    def generic(self, df_fpn, df_sep='\t', skiprows=None, header=None, is_utf8=False):
+    def generic(self, df_fpn, df_sep='\t', skiprows=None, header=None, is_utf8=False, comment='#'):
         """
 
         :param df_fpn:
         :param df_sep:
         :param header:
         :param is_utf8:
         :param dtype:
@@ -51,21 +48,23 @@
         if is_utf8:
             return pd.read_csv(
                 df_fpn,
                 sep=df_sep,
                 header=header,
                 encoding='utf-8',
                 skiprows=skiprows,
+                comment=comment,
             )
         else:
             return pd.read_csv(
                 df_fpn,
                 sep=df_sep,
                 header=header,
-                skiprows=None
+                skiprows=None,
+                comment=comment,
             )
 
     def excel(self, df_fpn, sheet_name='Sheet1', header=None, is_utf8=False):
         """
 
         :param df_fpn:
         :param sheet_name:
@@ -83,13 +82,8 @@
             )
         else:
             return pd.read_excel(
                 df_fpn,
                 sheet_name=sheet_name,
                 header=header,
                 engine='openpyxl',
-            )
-
-
-if __name__ == "__main__":
-    p = reader()
-    print(p.generic('data/drug/similarity/drug_all_07-02.txt'))
+            )
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/util/Writer.py` & `tmkit-0.0.2/tmkit/util/Writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import pandas as pd
 from functools import wraps
 
 
-class writer(object):
-
-    def __init__(self, ):
-        pass
+class writer:
 
     def __call__(self, deal):
         generic = self.generic
         excel = self.excel
         @wraps(deal)
         def write(ph, *args, **kwargs):
             res = deal(ph, **kwargs)
@@ -56,8 +53,19 @@
         df_ = pd.DataFrame(df)
         df_.index = df_.index + id_from
         return df_.to_excel(
             sv_fpn,
             sheet_name=sheet_name,
             header=header,
             index=index
-        )
+        )
+
+    def save(self, list_2d, sv_fp):
+        for i, e in enumerate(list_2d):
+            prot_name = str(e[0])
+            seq = str(e[1])
+            print('No.{} saving {} in FASTA format.'.format(i+1, prot_name))
+            f = open(sv_fp, 'w')
+            f.write('>' + prot_name + '\n')
+            f.write(seq + '\n')
+            f.close()
+        return 0
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/window/Single.py` & `tmkit-0.0.2/tmkit/seqnetrr/window/Single.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import time
-from tmkit.seqnetrr.Path import to
-from tmkit.seqnetrr.util.Console import console
 
 
-class single():
+class single:
     """
     Methods
     -------
        mid(), mname(), bipartite(), make().
 
     Notes
     -----
@@ -31,22 +29,19 @@
     """
 
     def __init__(
             self,
             sequence,
             position,
             window_size,
-            verbose=True,
     ):
         self.sequence = sequence
         self.m_sgls = position
         self.window_size = window_size
         self.len_seq = len(self.sequence)
-        self.console = console()
-        self.console.verbose = verbose
 
     def mid(self):
         """
 
         Notes
         -----
            mid() gets all of residues around central residues with a window size.
@@ -87,15 +82,15 @@
         # print(window_m_id)
         # #/*** block 2 ***/
         for i in range(len(window_m_id)):
             for j in range(len(window_m_id[0])):
                 if window_m_id[i][j] < 1 or window_m_id[i][j] > len(self.sequence):
                     window_m_id[i][j] = None
         # print(window_m_id)
-        self.console.print('=========>Window molecule generation: {time}s.'.format(time=time.time() - start_time))
+        print('=========>Window molecule generation: {time}s.'.format(time=time.time() - start_time))
         return window_m_id
 
     def mname(self, m_idices):
         """
 
         Notes
         -----
@@ -135,51 +130,8 @@
                     window_m_name[i].append(None)
                 # print(window_m_name)
                 for k, character in enumerate(self.sequence):
                     if m_idices[i][j] == k + 1:
                         # print(character)
                         window_m_name[i].append(character)
         # print(len(m_idices), len(window_m_name[92]))
-        return window_m_name
-
-
-if __name__ == "__main__":
-    from tmkit.seqnetrr.sequence.Fasta import fasta as sfasta
-    from tmkit.seqnetrr.combo.Position import position as pfasta
-    from tmkit.seqnetrr.combo.Length import length as plength
-
-    DEFINE = {
-        'prot_name': '1aig',
-        'file_chain': 'L',
-        'seq_chain': 'L',
-
-        # 'prot_name': '5lki',
-        # 'file_chain': 'A',
-        # 'seq_chain': 'A',
-
-        'cutoff': 5.5,
-        'seq_sep_inferior': 4,
-        'seq_sep_superior': None,
-        'fasta_path': to('data/example/'),
-    }
-
-    # /* sequence */
-    fasta_path = to('data/example/1aigL.fasta')
-    sequence = sfasta().get(fasta_path)
-    print(sequence)
-
-    # /* scenario of position */
-    pos_list = plength(seq_sep_inferior=0).tosgl(len(sequence))
-    print(pos_list)
-
-    # /* position */
-    position = pfasta(sequence).single(pos_list=pos_list)
-    print(position)
-
-    window_size = 2
-    window_m_ids = single(
-        sequence=sequence,
-        position=position,
-        window_size=window_size,
-    ).mid()
-    print(window_m_ids)
-
+        return window_m_name
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/window/base/Pair.py` & `tmkit-0.0.2/tmkit/seqnetrr/window/base/Pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from tmkit.seqnetrr.util.ComputLib import computLib
+from tmkit.seqnetrr.ComputLib import computLib
 
 
-class pair():
+class pair:
 
     def __init__(self, sequence, window_size, window_m_ids):
         """
 
         Notes
         -----
             1>. self.stretch_window is the size of all possible
```

### Comparing `tmkit-0.0.0.2/tmkit/seqnetrr/window/base/Single.py` & `tmkit-0.0.2/tmkit/seqnetrr/window/base/Single.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from tmkit.seqnetrr.util.ComputLib import computLib
+from tmkit.seqnetrr.ComputLib import computLib
 
 
-class single():
+class single:
 
     def __init__(self, sequence, window_size, window_m_ids):
         """
 
         Notes
         -----
             1>. self.stretch_window is the size of all possible
```

### Comparing `tmkit-0.0.0.2/tmkit/sequence/Fasta.py` & `tmkit-0.0.2/tmkit/id/Fasta.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-
 from Bio import SeqIO
 
 
-class fasta():
-
-    def __init__(self):
-        pass
+class fasta:
 
     def get(self, fasta_fpn):
         sequence = []
         for seq in SeqIO.parse(fasta_fpn, "fasta"):
-            # print(seq.seq)
             sequence.append(str(seq.seq))
         sequence = ''.join(sequence)
-        if sequence == '':
-            print('The sequence is empty.')
-        return sequence
+        ids = {}
+        for i, aa in enumerate(sequence):
+            ids[i+1] = aa
+        return ids
```

### Comparing `tmkit-0.0.0.2/tmkit/sequence/PDB.py` & `tmkit-0.0.2/tmkit/sequence/PDB.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-import warnings
 from tmkit.base import PDB
-from Bio import BiopythonWarning
 
 
 class pdb(PDB.sequence):
 
     def __init__(self, pdb_fp, prot_name, seq_chain, file_chain=''):
         """
 
@@ -50,15 +48,13 @@
 
         Returns
         -------
             a sequence
 
         """
         seq=[]
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore', BiopythonWarning)
-            for pp in self.ppb.build_peptides(self.pdb_chain):
-                seq_tmp = str(pp.get_sequence())
-                # print(seq_tmp)
-                seq.append(seq_tmp)
+        for pp in self.ppb.build_peptides(self.pdb_chain):
+            seq_tmp = str(pp.get_sequence())
+            # print(seq_tmp)
+            seq.append(seq_tmp)
         return ''.join(seq)
```

### Comparing `tmkit-0.0.0.2/tmkit/sequence/XML.py` & `tmkit-0.0.2/tmkit/sequence/XML.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import xml.etree.ElementTree as ET
 
 
-class xml():
-
-    def __init__(self, ):
-        pass
+class xml:
 
     def get(self, xml_fp, xml_name, seq_chain):
         xml_fpn = xml_fp + xml_name + '.xml'
         tree = ET.parse(xml_fpn)
         parser_pdb = tree.getroot()
         for chains in parser_pdb:
             if chains.tag == '{http://pdbtm.enzim.hu}CHAIN':
```

### Comparing `tmkit-0.0.0.2/tmkit/structure/ppi/Label.py` & `tmkit-0.0.2/tmkit/structure/ppi/Label.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import time
 from tmkit.util.Reader import reader
 
 
-class label(object):
+class label:
 
     def __init__(self, dist_path, prot_name, file_chain, cutoff=6):
         self.prot_name = prot_name
         self.file_chain = file_chain
         self.dist_fpn = dist_path + self.prot_name + self.file_chain + '.dist'
         self.cutoff = cutoff
         self.read = reader()
@@ -23,16 +23,16 @@
         dist_df = self.read.generic(self.dist_fpn)
         dists = dist_df.iloc[:, 3:]
         dist_mins = dists.min(axis=1)
         # print(dist_mins)
         inter_ids = dist_mins.loc[dist_mins < self.cutoff].index.tolist()
         noninter_ids = dist_mins.loc[dist_mins >= self.cutoff].index.tolist()
         dist_df['is_contact'] = -1
-        dist_df.at[inter_ids, 'is_contact'] = 1
-        dist_df.at[noninter_ids, 'is_contact'] = 0
+        dist_df.loc[inter_ids, 'is_contact'] = 1
+        dist_df.loc[noninter_ids, 'is_contact'] = 0
         columns = ['fasta_id', 'aa', 'pdb_id']
         for i in range(dists.shape[1]):
             columns.append('dist_' + str(i+1))
         columns.append('is_contact')
         dist_df.columns = columns
         end_time = time.time()
         print('======>Time to read&label distances for {} {}: {}s.'.format(self.prot_name, self.file_chain, end_time - start_time))
```

### Comparing `tmkit-0.0.0.2/tmkit/structure/rrc/Label.py` & `tmkit-0.0.2/tmkit/structure/rrc/Label.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 import pandas as pd
 from tmkit.util.Reader import reader
 from tmkit.position.scenario.Separation import separation
 
 
-class label(object):
+class label:
     
     def __init__(self, dist_path, prot_name, file_chain, cutoff=5.5, seq_sep_inferior=None, seq_sep_superior=None):
         self.prot_name = prot_name
         self.file_chain = file_chain
         self.dist_fpn = dist_path + self.prot_name + self.file_chain + '.dist'
         self.cutoff = cutoff
         self.seq_sep_inferior = seq_sep_inferior
```

### Comparing `tmkit-0.0.0.2/tmkit/topo.py` & `tmkit-0.0.2/tmkit/topo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-import pandas as pd
 from tmkit.topology.pdbtm.Segment import segment
 from tmkit.topology.Phobius import phobius
 from tmkit.topology.TMHMM import tmhmm
 from tmkit.topology.pdbtm.Determine import determine
 from tmkit.id.Fasta import fasta as idfasta
 from tmkit.id.PDB import pdb as idpdb
 
@@ -93,16 +92,16 @@
     return ptopos[topo + '_lower'], ptopos[topo + '_upper']
 
 
 def from_tmhmm(
         topo=None,
         tag=None,
         tmhmm_fpn=None,
-        from_fasta=True,
-        file_kind='inline',
+        from_fasta=False,
+        file_kind='linux',
         fasta_fpn=None,
         tmhmm_model_fpn=None,
         sv_fpn=None,
 
         # for the linux executable
         decodeanhmm=None,
         options=None,
@@ -198,52 +197,8 @@
     return determine().ce(
         pdbid_map=pdbids,
         fasid_map=fasids,
         pred_fp=topo_fp,
         prot_name=prot_name,
         seq_chain=seq_chain,
         xml_fp=xml_fp,
-    )
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    # print(from_pdbtm(
-    #     xml_fp=to('data/example/'),
-    #     prot_name='1xqf',
-    #     seq_chain='A',
-    #     topo='tmh',
-    # ))
-
-    # print(from_phobius(
-    #     topo='tmh',
-    #     from_fasta=True,
-    #     fasta_fpn=to('data/example/1xqfA.fasta'),
-    #     phobius_fpn=to('data/1xqfA.jphobius'),
-    #     sv_fp=to('data/'),
-    #     tag='1xqfA',
-    # ))
-
-    # print(from_tmhmm(
-    #     topo='tmh',
-    #     tag='1xqfA',
-    #     from_fasta=True,
-    #     file_kind='inline',
-    #     fasta_fpn=to('data/example/1xqfA.fasta'),
-    #     tmhmm_fpn=to('data/1xqfA.tmhmm'),
-    #     tmhmm_model_fpn=to('topology/lib/TMHMM2.0.model'),
-    #     sv_fpn=to('data/1xqfA.tmhmm'),
-    # ))
-
-    # print(cepdbtm(
-    #     pdb_fp=to('data/example/'),
-    #     # prot_name='3pux',
-    #     # seq_chain='G',
-    #     # file_chain='G',
-    #     prot_name='1xqf',
-    #     seq_chain='A',
-    #     file_chain='A',
-    #     topo_fp=to('data/example/1xqfA.jphobius'),
-    #     xml_fp=to('data/example/'),
-    #     fasta_fp=to('data/example/'),
-    # ))
+    )
```

### Comparing `tmkit-0.0.0.2/tmkit/topology/Phobius.py` & `tmkit-0.0.2/tmkit/topology/Phobius.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,46 +5,38 @@
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import os
 import subprocess
 import numpy as np
 import pandas as pd
-from tmkit.util.Console import console
 from tmkit.interface import Topology
 
 
 class phobius(Topology.topology):
 
-    def __init__(
-            self,
-            verbose=True,
-    ):
-        self.console = console()
-        self.console.verbose = verbose
-
     def run(
             self,
             fasta_fpn,
             sv_fpn,
             email='jianfeng.sunmt@gmail.com',
     ):
-        self.console.print('===>Phobius is running python inline...')
+        print('===>Phobius is running python inline...')
         if sv_fpn is None:
             raise 'sv_fpn has to be specified'
         fpnf = os.path.dirname(__file__) + '/lib/Phobius.py'
         order = 'python ' + fpnf + ' --email ' + email + ' --sequence ' + fasta_fpn + ' --stype protein --outfile ' + sv_fpn
-        self.console.print('Command to run Phobius: {}'.format(order))
+        # print('Command to run Phobius: {}'.format(order))
         subprocess.Popen(
             order,
             stderr=subprocess.PIPE,
             stdout=subprocess.PIPE,
             shell=True,
         ).communicate()
-        print(1)
+        # print(1)
         # os.system(order)
         os.rename(
             sv_fpn + '.out.txt',
             sv_fpn + '.jphobius',
         )
         return 'finished.'
 
@@ -64,24 +56,24 @@
         df = df.reset_index(drop=True)
         df['type'] = ''
         # print(df)
         if 4 not in df.columns:
             df[4] = None
         if 5 not in df.columns:
             df[5] = None
-        print(df)
+        # print(df)
         for i in range(df.shape[0]):
             if df.iloc[i][4] is None:
                 df.at[i, 4] = ''
             if df.iloc[i][5] is None:
                 df.at[i, 5] = ''
             df.at[i, 'type'] = df.iloc[i][4] + df.iloc[i][5]
-        print(df)
-        df[2] = df[2].astype(np.int)
-        df[3] = df[3].astype(np.int)
+        # print(df)
+        df[2] = df[2].astype(int)
+        df[3] = df[3].astype(int)
         return df
 
     def extract(self, df):
         # print(df.groupby('type').apply(lambda x: x == 'CYTOPLASMIC.'))
         inside = df[[2, 3]].loc[df['type'].isin(['CYTOPLASMIC.'])].values.tolist()
         tms = df[[2, 3]].loc[df[1].isin(['TRANSMEM'])].values.tolist()
         outside = df[[2, 3]].loc[df['type'].isin(['NONCYTOPLASMIC.'])].values.tolist()
```

### Comparing `tmkit-0.0.0.2/tmkit/topology/TMHMM.py` & `tmkit-0.0.2/tmkit/topology/TMHMM.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,30 +6,25 @@
 __maintainer__ = "Jianfeng Sun"
 
 import os
 import re
 import subprocess
 import linecache
 import numpy as np
-import tmhmm as tmhmmpy
-from tmkit.sequence.Fasta import fasta as sfasta
+from tmkit.sequence import Fasta as sfasta
 from tmkit.util.Reader import reader
 from tmkit.util.Writer import writer
 from tmkit.interface import Topology
-from tmkit.util.Console import console
 
 
 class tmhmm(Topology.topology):
 
     def __init__(
             self,
-            verbose=True,
     ):
-        self.console = console()
-        self.console.verbose = verbose
         self.reader = reader()
         self.writer = writer()
 
     def run(
             self,
             fasta_fpn,
             tmhmm_model_fpn,
@@ -53,21 +48,23 @@
         tag
         sv_fpn
 
         Returns
         -------
 
         """
-        self.console.print('===>TMHMM is running python inline...')
+        print('===>TMHMM is running python inline...')
         if sv_fpn is None:
             raise 'sv_fpn has to be specified'
+        import tmhmm as tmhmmpy
         annotation, posterior = tmhmmpy.predict(
-            sequence=sfasta().get(fasta_fpn=fasta_fpn),
+            sequence=sfasta.get(fasta_fpn=fasta_fpn),
             header=None,
-            model_or_filelike=tmhmm_model_fpn,
+            model_or_filelike=os.path.dirname(__file__) + '/lib/TMHMM2.0.model',
+            # model_or_filelike=tmhmm_model_fpn,
         )
         self.writer.save([[tag + '_tmhmm', annotation]], sv_fp=sv_fpn)
         return annotation
 
     def runLinux(
             self,
             fasta_fpn,
@@ -95,15 +92,15 @@
             path to save files
 
         Returns
         -------
             A message string
 
         """
-        self.console.print('===>TMHMM is running on Linux...')
+        print('===>TMHMM is running on Linux...')
         order = 'cat ' + fasta_fpn + '.fasta | ' + decodeanhmm + ' -f ' + options + ' -modelfile ' + modelfile + ' -noPrintSeq -noPrintScores -noPrintID -noPrintStat > ' + sv_fpn
         # print(order)
         subprocess.Popen(
             order,
             stderr=subprocess.PIPE,
             stdout=subprocess.PIPE,
             shell=True,
@@ -225,15 +222,15 @@
         Returns
         -------
             2D arr
 
         """
         if not os.path.exists(tmhmm_fpn):
             raise FileNotFoundError
-        annot = sfasta().get(tmhmm_fpn)
+        annot = sfasta.get(tmhmm_fpn)
         arr = []
         flag = 1
         for i in range(len(annot)):
             if i + 1 != len(annot):
                 if annot[i] == annot[i+1]:
                     continue
                 else:
```

### Comparing `tmkit-0.0.0.2/tmkit/topology/lib/Phobius.py` & `tmkit-0.0.2/tmkit/topology/lib/Phobius.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/tmkit/topology/pdbtm/Component.py` & `tmkit-0.0.2/tmkit/topology/pdbtm/Component.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 from functools import wraps
 import xml.etree.ElementTree as ET
 
 
-class component(object):
+class component:
 
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
 
     def __call__(self, deal):
         type = self.kwargs['type']
@@ -34,19 +34,19 @@
             # for regions in parser_pdb.iter('REGION'):
             #     print(regions.get('type'))
             # chain_mark = []
             for chains in parser_pdb:
                 if chains.tag == '{http://pdbtm.enzim.hu}CHAIN':
                     for regions in chains.iter('{http://pdbtm.enzim.hu}REGION'):
                         if type == 'side1':
-                            if chains.get('CHAINID') == kwargs['seq_chain'] and regions.get('type') == 1:
+                            if chains.get('CHAINID') == kwargs['seq_chain'] and regions.get('type') == '1':
                                 start_id.append(int(regions.get('pdb_beg')))
                                 last_id.append(int(regions.get('pdb_end')))
                         elif type == 'side2':
-                            if chains.get('CHAINID') == kwargs['seq_chain'] and regions.get('type') == 2:
+                            if chains.get('CHAINID') == kwargs['seq_chain'] and regions.get('type') == '2':
                                 start_id.append(int(regions.get('pdb_beg')))
                                 last_id.append(int(regions.get('pdb_end')))
                         elif type == 'alpha-helix':
                             if chains.get('CHAINID') == kwargs['seq_chain'] and regions.get('type') == 'H':
                                 start_id.append(int(regions.get('pdb_beg')))
                                 last_id.append(int(regions.get('pdb_end')))
                         elif type == 'non-alpha-helix':
```

### Comparing `tmkit-0.0.0.2/tmkit/topology/pdbtm/Determine.py` & `tmkit-0.0.2/tmkit/topology/pdbtm/Determine.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 __maintainer__ = "Jianfeng Sun"
 
 import pandas as pd
 from tmkit.topology.Phobius import phobius
 from tmkit.topology.pdbtm.ToFastaId import toFastaId
 
 
-class determine(object):
-
-    def __init__(self, ):
-        pass
+class determine:
 
     def ce(
             self,
             pred_fp,
             prot_name,
             seq_chain,
             pdbid_map,
@@ -50,16 +47,16 @@
         pdbtm_seg['tmh_lower'] = fasta_lower_tmh
         pdbtm_seg['tmh_upper'] = fasta_upper_tmh
         pdbtm_seg['cyto_lower'] = []
         pdbtm_seg['cyto_upper'] = []
         pdbtm_seg['extra_lower'] = []
         pdbtm_seg['extra_upper'] = []
         # print(pdbtm_seg)
-        print(len(fasta_upper_nontmh))
-        print(len(fasta_lower_nontmh))
+        # print(len(fasta_upper_nontmh))
+        # print(len(fasta_lower_nontmh))
         for i, e in enumerate(fasta_lower_nontmh):
             # print('No. ', i)
             i1 = pd.Interval(e, fasta_upper_nontmh[i], closed='both')
             ic_accumulator = 0
             for j, m in enumerate(pred_seg['cyto_lower']):
                 ic = pd.Interval(m, pred_seg['cyto_upper'][j], closed='both')
                 if i1.overlaps(ic):
```

### Comparing `tmkit-0.0.0.2/tmkit/topology/pdbtm/Segment.py` & `tmkit-0.0.2/tmkit/topology/pdbtm/Segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 __maintainer__ = "Jianfeng Sun"
 
 from functools import wraps
 from tmkit.topology.pdbtm.Component import component
 from tmkit.id.Mapping import mapping as pdbid
 
 
-class segment(object):
+class segment:
 
     def __init__(self, type='tmh'):
         self.type = type
 
     def __call__(self, deal):
         if self.type == 'side1':
             segment = self.side1
```

### Comparing `tmkit-0.0.0.2/tmkit/topology/pdbtm/TMH.py` & `tmkit-0.0.2/tmkit/topology/pdbtm/TMH.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from tmkit.Path import to
 from tmkit.topology.pdbtm.Segment import segment
 
 
-class tmh(object):
+class tmh:
 
     def __init__(self, xml_fp, prot_name, seq_chain):
         self.xml_fp = xml_fp
         self.prot_name = prot_name
         self.seq_chain = seq_chain
 
     def get(self):
@@ -36,18 +35,8 @@
         :return:
         """
         start_id, last_id = segment().tmh(
             xml_fp=self.xml_fp,
             prot_name=self.prot_name,
             seq_chain=self.seq_chain,
         )
-        return start_id, last_id
-
-
-if __name__ == "__main__":
-    p = tmh(
-        xml_fp=to('data/example/'),
-        prot_name='1xqf',
-        seq_chain='A'
-    )
-
-    print(p.get())
+        return start_id, last_id
```

### Comparing `tmkit-0.0.0.2/tmkit/topology/pdbtm/ToFastaId.py` & `tmkit-0.0.2/tmkit/topology/pdbtm/ToFastaId.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 from tmkit.topology.pdbtm.Segment import segment as fetchfasids
 
 
-class toFastaId(object):
+class toFastaId:
 
     def __init__(self, type='tmh'):
         self.type = type
 
     @fetchfasids(type='side1')
     def side1(self, start_id, last_id, fasid_map, pdbid_map, xml_fp='', prot_name='', seq_chain=''):
         return start_id, last_id
```

### Comparing `tmkit-0.0.0.2/tmkit/util/Kit.py` & `tmkit-0.0.2/tmkit/util/Kit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 import os
 import gzip
 import shutil
 import urllib.request
-import pandas as pd
 
 
 def chainid(prot_chain):
     return str(prot_chain) + 'l' if str(prot_chain).islower() else str(prot_chain)
 
 
 def seqchainid(prot_chain):
@@ -46,43 +45,23 @@
                 os.rename(
                     os.path.join(file_path, file_name + old_suffix),
                     os.path.join(file_path, prot_name + chain + new_suffix)
                 )
     return
 
 
-def batchFetchName(file_path):
-    print('asda')
-    small = []
-    capital = []
-    for file_name in os.listdir(file_path):
-        file_name_re = re.sub(r'\.[p]db', "", file_name)
-        file_name_re_sma = re.sub(r'[A-Z]', "", file_name_re)
-        small.append(file_name_re_sma)
-        file_name_re_cap = re.sub(r'.{2}', "", file_name_re)
-        capital.append(file_name_re_cap)
-    conc = pd.concat([pd.DataFrame(small), pd.DataFrame(capital)], axis=1)
-    conc.columns = ['0', '1']
-    print(conc)
-    # conc.to_csv(
-    #     file_path + '/list_fpn.txt',
-    #     sep=' ',
-    # )
-
-
 def urlliby(url, fpn):
     return urllib.request.urlretrieve(
         url=url,
         filename=fpn
     )
 
 
 def ungz(file_path, file_name, sv_fp, new_suffix='.pdb'):
     try:
-        print(file_path + file_name)
         with gzip.open(file_path + file_name + '.gz', 'rb') as f_in:
             with open(sv_fp + file_name + new_suffix, 'wb') as f_out:
                 shutil.copyfileobj(f_in, f_out)
     except FileNotFoundError:
         print('No such file' + file_path + file_name)
     return
 
@@ -135,9 +114,8 @@
     return result
 
 
 def tactic8(arr_1d_1, arr_1d_2):
     map = {}
     for i, e in enumerate(arr_1d_1):
         map[e] = arr_1d_2[i]
-    return map
-
+    return map
```

### Comparing `tmkit-0.0.0.2/tmkit/visualize/func/Coloring.py` & `tmkit-0.0.2/tmkit/visualize/func/Coloring.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from pymol import finish_launching
-from pymol import cmd
 from tmkit.chain.PDB import pdb as cpdb
 
 
-class coloring():
+class coloring:
 
     def __init__(
             self,
             pdb_fp,
             prot_name,
             seq_chain,
             prot_c='sulfur',
@@ -34,15 +32,16 @@
         actions
             residues that pymol selects
         colors
             colors
         forms
             representation of the selected residues
         """
-
+        from pymol import finish_launching
+        from pymol import cmd
         finish_launching()
 
         cmd.bg_color(
             color="black",
             # color="white",
         )
```

### Comparing `tmkit-0.0.0.2/tmkit/visualize/isite/Labelling.py` & `tmkit-0.0.2/tmkit/visualize/isite/Labelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from tmkit.structure.ppi.Label import label as dlable
 from tmkit.util.Kit import chainid, seqchainid
 from tmkit.util.Kit import tactic8
 from tmkit.util.Kit import create
 from tmkit.util.Writer import writer
 
 
-class labelling():
+class labelling:
 
     def __init__(
             self,
             tool,
             prot_name,
             prot_chain,
             pdb_fp,
```

### Comparing `tmkit-0.0.0.2/tmkit/visualize/isite/ProtocolDeepTMInter.py` & `tmkit-0.0.2/tmkit/visualize/isite/ProtocolDeepTMInter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from pymol import finish_launching
-from pymol import cmd
-from tmkit.visualize.lib.Select import select as libsel
-from tmkit.visualize.lib.Color import color as libcolor
-from tmkit.visualize.lib.palette.data2bfactor import data2b_res
-from tmkit.visualize.lib.palette.spectrumany import spectrumany
+from tmkit.visualize.component.Select import select as libsel
+from tmkit.visualize.component.Color import color as libcolor
 from tmkit.visualize.isite.Labelling import labelling
 from tmkit.chain.PDB import pdb as cpdb
 
 
-class protocolDeepTMInter():
+class protocolDeepTMInter:
 
     def __init__(
             self,
             prot_name,
             prot_chain,
             pdb_chain_fp,
             pdb_complex_fp,
@@ -71,15 +67,16 @@
         focus_chain_name
         focus_representation
         color_list
             'white br7', 'white tv_blue'
         bg_color
 
         """
-
+        from pymol import finish_launching
+        from pymol import cmd
         finish_launching()
 
         self.type = {
             'label_actual': 'actual_label_bf',
             'label_predicted': 'predicted_label_bf',
             'probability': 'probs_bf',
         }[draw_type]
@@ -114,19 +111,21 @@
         libsel().chain(chain_name=bg_chain_name, chains=pymol_bg_chain_ids)
 
         libcolor(color=bg_chain_color, sel_name=bg_chain_name)
 
         libsel().chain(chain_name=focus_chain_name, chains=prot_chain + ' and not resn Zn')
         # cmd.alter(selection=focus_chain_name, expression='b=0')
 
+        from tmkit.visualize.component.palette.data2bfactor import data2b_res
         data2b_res(
             mol=focus_chain_name,
             data_file=sv_bfactor_fp + '/' + self.type + '.txt',
         )
 
+        from tmkit.visualize.component.palette.spectrumany import spectrumany
         spectrumany(
             expression='b',
             color_list=color_list,
             selection=focus_chain_name,
             minimum=0.01,
             maximum=1,
             quiet=1,
```

### Comparing `tmkit-0.0.0.2/tmkit/visualize/lib/InterfaceResidues.py` & `tmkit-0.0.2/tmkit/visualize/component/InterfaceResidues.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/tmkit/visualize/lib/focal_blur.py` & `tmkit-0.0.2/tmkit/visualize/component/focal_blur.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.2/tmkit/visualize/lib/palette/data2bfactor.py` & `tmkit-0.0.2/tmkit/visualize/component/palette/data2bfactor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,290 +1,292 @@
-"""
-Copyright (c) 2003 Robert L. Campbell
-Copyright (c) 2010 Thomas Holder
-Copyright (c) 2013 Suguru Asai
-
-Original by RLC, with extensive modifications and improvements by TH.
-
-Atom B-factor data generated by ptraj (amber) is supported by SA.
-
-Please read below for instructions
-
-contains the functions
-   data2b_atom(mol='',data_file='')
-   data2b_res(mol='',data_file='')
-   data2q_atom(mol='',data_file='')
-   data2q_res(mol='',data_file='')
-"""
-
-import sys, re
-from pymol import stored
-
-comment = re.compile('^\s*$|^\s*#')
-
-def atom_data_extract(data_file):
-    """
-    Read the specified 'by-atom' data file and extract the data from it
-    and store it in parallel dictionaries specifying the data
-    and residue names (both with keys of chain and residue number and atom name).
-    The data file can contain comment lines starting with "#" (on lines by themselves).
-    These comment lines are ignored.
-    """
-    bdat = {}
-    chain = ''
-
-    data_lines = open(data_file, 'rU')
-    count = 0
-
-    for line in data_lines:
-        # ignore comment lines (beginning with a '#') or blank lines
-        if not comment.match(line):
-            words = line.split()
-            count += 1
-
-            # check number of columns of data
-            if len(words) >= 5:
-                chain = words[0]
-                resi = words[1]
-                resn = words[2]
-                name = words[3]
-                if chain == '-':
-                    chain = ''
-                ID = None
-                data = float(words[4])
-            elif len(words) == 4:
-                resi = words[0]
-                resn = words[1]
-                name = words[2]
-                ID = None
-                data = float(words[3])
-            elif len(words) == 2:
-                # ptraj `atominfluct` output use ID and data
-                resi = None
-                resn = None
-                name = None
-                ID = int(words[0])
-                data = float(words[1])
-            else:
-                sys.stderr.write("\nError in reading data files -- check number of columns.\n")
-                sys.stderr.write("Number of columns: %d  on line number %d\n" % (len(words),count))
-                sys.exit(1)
-
-            if ID is None:
-                bdat.setdefault(chain, {}).setdefault(resi, {})[name] = (data, resn)
-            else:
-                # it seem `resn` is not used in anywhere
-                bdat.setdefault(chain, {})[ID] = (data, '')
-
-    return bdat
-
-def residue_data_extract(data_file):
-    """
-    Read the specified 'by-residue' data file and extract the data from it
-    and store it in parallel dictionaries specifying the data
-    and residue names (both with keys of chain and residue number).
-    The data file can contain comment lines starting with "#" (on lines by themselves).
-    These comment lines are ignored.
-    """
-    bdat = {}
-    chain = ''
-
-    data_lines = open(data_file, 'rU')
-    count = 0
-
-    for line in data_lines:
-        # ignore comment lines (beginning with a '#') or blank lines
-        if not comment.match(line):
-            words = line.split()
-            count += 1
-
-            # check number of columns of data
-            if len(words) >= 4:
-                chain = words[0]
-                resi = words[1]
-                resn = words[2]
-                if chain == '-':
-                    chain = ''
-                data = float(words[3])
-            elif len(words) == 3:
-                resi = words[0]
-                resn = words[1]
-                data = float(words[2])
-            elif len(words) == 2:
-                resi = words[0]
-                data = float(words[1])
-                resn = ''
-            else:
-                sys.stderr.write("\nError in reading data files -- check number of columns.\n")
-                sys.stderr.write("Number of columns: %d  on line number %d\n" % (len(words),count))
-                sys.exit(1)
-
-            bdat.setdefault(chain, {})[resi] = (data, resn)
-
-    return bdat
-
-###########################################################################################
-# for testing purposes:
-# if calling this as a program on its own, read the data_file name from
-# the command line and run residue_data_extract on it. (does not require
-# importing cmd from pymol
-
-if __name__ == '__main__':
-    data_file_name = sys.argv[1]
-    b_dict = residue_data_extract(data_file_name)
-    for chain in sorted(b_dict):
-        for resi in sorted(b_dict[chain]):
-            b, resn = b_dict[chain][resi]
-            print("b-factors %s %s %s %s  new B='%s'" % (pdb_file, chain, resn, resi, b))
-    sys.exit()
-
-
-###########################################################################################
-# PyMOL stuff
-
-from pymol import cmd
-
-def data2b_atom(mol='', data_file='', property='b', quiet=0):
-    """
-DESCRIPTION
-
-    Alters the B-factor data by atom.
-
-USAGE
-
-    data2b_atom <mol>, <data_file>
-
-    where <mol> is the molecular object whose B-factor data you wish to modify
-    and <data_file> is a file contain the data (one value for each atom)
-    The format of <data_file> should be:
-
-         chain resi resn name data
-    or
-         resi resn name data
-
-    or
-         ID data
-
-    (i.e. "chain" is optional if all atoms are in one chain).
-    Lines beginning with '#' are ignored as comments.
-
-    Example data lines:
-
-      A ALA 1 N 3.5
-      A ALA 1 CA 3.0
-      A ALA 1 CB 3.14159
-      A ALA 1 C  6.23
-      A ALA 1 O    5.1
-      A GLY 2 N 10.3
-      A GLY 2 CA 1.714
-      A GLY 2 C -0.05
-      A GLY 2 O -3.12
-
-SEE ALSO
-
-    data2b_res, data2q_atom, data2q_res
-    """
-
-    b_dict = atom_data_extract(data_file)
-    quiet = int(quiet) == 1
-
-    def b_lookup(chain, resi, name, ID, b):
-        def _lookup(chain, resi, name, ID):
-            if resi in b_dict[chain] and isinstance(b_dict[chain][resi], dict):
-                return b_dict[chain][resi][name][0]
-            else:
-                # find data by ID
-                return b_dict[chain][int(ID)][0]
-        try:
-            if not chain in b_dict:
-                chain = ''
-            b = _lookup(chain, resi, name, ID)
-            if not quiet: print('///%s/%s/%s new: %f' % (chain, resi, name, b))
-        except KeyError:
-            if not quiet: print('///%s/%s/%s keeping: %f' % (chain, resi, name, b))
-        return b
-    stored.b = b_lookup
-
-    cmd.alter(mol, '%s=stored.b(chain, resi, name, ID, %s)' % (property, property))
-    cmd.rebuild()
-
-def data2b_res(mol='', data_file='', property='b', quiet=0):
-    """
-DESCRIPTION
-
-    Alters the B-factor data by residue.
-
-USAGE
-
-    data2b_res <mol>, <data_file>
-
-    where <mol> is the molecular object whose B-factor data you wish to modify
-    and <data_file> is a file contain the data (one value for each residue)
-    The format of <data_file> should be:
-
-         chain resi resn data
-    or
-         resi resn data
-    or
-         resi data
-
-    (i.e. "chain" is optional). Lines beginning with '#' are ignored as comments.
-
-SEE ALSO
-
-    data2b_atom, data2q_atom, data2q_res
-    """
-
-    b_dict = residue_data_extract(data_file)
-    quiet = int(quiet) == 1
-
-    def b_lookup(chain, resi, name, b):
-        try:
-            if chain in b_dict:
-                b = b_dict[chain][resi][0]
-            else:
-                b = b_dict[''][resi][0]
-            if not quiet: print('///%s/%s/%s new: %f' % (chain, resi, name, b))
-        except KeyError:
-            if not quiet: print('///%s/%s/%s keeping: %f' % (chain, resi, name, b))
-        return b
-    stored.b = b_lookup
-
-    cmd.alter(mol, '%s=stored.b(chain, resi, name, %s)' % (property, property))
-    cmd.rebuild()
-
-def data2q_atom(mol='',data_file=''):
-    """
-DESCRIPTION
-
-    Alters the occupancy data by atom.
-
-USAGE
-
-    See data2b_atom
-
-SEE ALSO
-
-    data2q_res, data2b_atom, data2b_res
-    """
-    data2b_atom(mol, data_file, property='q')
-
-def data2q_res(mol='',data_file=''):
-    """
-DESCRIPTION
-
-    Alters the occupancy data by residue.
-
-USAGE
-
-    See data2b_res
-
-SEE ALSO
-
-    data2q_atom, data2b_atom, data2b_res
-    """
-    data2b_res(mol, data_file, property='q')
-
-cmd.extend('data2b_res',data2b_res)
-cmd.extend('data2b_atom',data2b_atom)
-cmd.extend('data2q_res',data2q_res)
-cmd.extend('data2q_atom',data2q_atom)
+"""
+Copyright (c) 2003 Robert L. Campbell
+Copyright (c) 2010 Thomas Holder
+Copyright (c) 2013 Suguru Asai
+
+Original by RLC, with extensive modifications and improvements by TH.
+
+Atom B-factor data generated by ptraj (amber) is supported by SA.
+
+Please read below for instructions
+
+contains the functions
+   data2b_atom(mol='',data_file='')
+   data2b_res(mol='',data_file='')
+   data2q_atom(mol='',data_file='')
+   data2q_res(mol='',data_file='')
+"""
+
+import sys, re
+from pymol import stored
+
+comment = re.compile('^\s*$|^\s*#')
+
+def atom_data_extract(data_file):
+    """
+    Read the specified 'by-atom' data file and extract the data from it
+    and store it in parallel dictionaries specifying the data
+    and residue names (both with keys of chain and residue number and atom name).
+    The data file can contain comment lines starting with "#" (on lines by themselves).
+    These comment lines are ignored.
+    """
+    bdat = {}
+    chain = ''
+
+    data_lines = open(data_file, 'r')
+    # data_lines = open(data_file, 'rU')
+    count = 0
+
+    for line in data_lines:
+        # ignore comment lines (beginning with a '#') or blank lines
+        if not comment.match(line):
+            words = line.split()
+            count += 1
+
+            # check number of columns of data
+            if len(words) >= 5:
+                chain = words[0]
+                resi = words[1]
+                resn = words[2]
+                name = words[3]
+                if chain == '-':
+                    chain = ''
+                ID = None
+                data = float(words[4])
+            elif len(words) == 4:
+                resi = words[0]
+                resn = words[1]
+                name = words[2]
+                ID = None
+                data = float(words[3])
+            elif len(words) == 2:
+                # ptraj `atominfluct` output use ID and data
+                resi = None
+                resn = None
+                name = None
+                ID = int(words[0])
+                data = float(words[1])
+            else:
+                sys.stderr.write("\nError in reading data files -- check number of columns.\n")
+                sys.stderr.write("Number of columns: %d  on line number %d\n" % (len(words),count))
+                sys.exit(1)
+
+            if ID is None:
+                bdat.setdefault(chain, {}).setdefault(resi, {})[name] = (data, resn)
+            else:
+                # it seem `resn` is not used in anywhere
+                bdat.setdefault(chain, {})[ID] = (data, '')
+
+    return bdat
+
+def residue_data_extract(data_file):
+    """
+    Read the specified 'by-residue' data file and extract the data from it
+    and store it in parallel dictionaries specifying the data
+    and residue names (both with keys of chain and residue number).
+    The data file can contain comment lines starting with "#" (on lines by themselves).
+    These comment lines are ignored.
+    """
+    bdat = {}
+    chain = ''
+
+    data_lines = open(data_file, 'r')
+    # data_lines = open(data_file, 'rU')
+    count = 0
+
+    for line in data_lines:
+        # ignore comment lines (beginning with a '#') or blank lines
+        if not comment.match(line):
+            words = line.split()
+            count += 1
+
+            # check number of columns of data
+            if len(words) >= 4:
+                chain = words[0]
+                resi = words[1]
+                resn = words[2]
+                if chain == '-':
+                    chain = ''
+                data = float(words[3])
+            elif len(words) == 3:
+                resi = words[0]
+                resn = words[1]
+                data = float(words[2])
+            elif len(words) == 2:
+                resi = words[0]
+                data = float(words[1])
+                resn = ''
+            else:
+                sys.stderr.write("\nError in reading data files -- check number of columns.\n")
+                sys.stderr.write("Number of columns: %d  on line number %d\n" % (len(words),count))
+                sys.exit(1)
+
+            bdat.setdefault(chain, {})[resi] = (data, resn)
+
+    return bdat
+
+###########################################################################################
+# for testing purposes:
+# if calling this as a program on its own, read the data_file name from
+# the command line and run residue_data_extract on it. (does not require
+# importing cmd from pymol
+
+if __name__ == '__main__':
+    data_file_name = sys.argv[1]
+    b_dict = residue_data_extract(data_file_name)
+    for chain in sorted(b_dict):
+        for resi in sorted(b_dict[chain]):
+            b, resn = b_dict[chain][resi]
+            print("b-factors %s %s %s %s  new B='%s'" % (pdb_file, chain, resn, resi, b))
+    sys.exit()
+
+
+###########################################################################################
+# PyMOL stuff
+
+from pymol import cmd
+
+def data2b_atom(mol='', data_file='', property='b', quiet=0):
+    """
+DESCRIPTION
+
+    Alters the B-factor data by atom.
+
+USAGE
+
+    data2b_atom <mol>, <data_file>
+
+    where <mol> is the molecular object whose B-factor data you wish to modify
+    and <data_file> is a file contain the data (one value for each atom)
+    The format of <data_file> should be:
+
+         chain resi resn name data
+    or
+         resi resn name data
+
+    or
+         ID data
+
+    (i.e. "chain" is optional if all atoms are in one chain).
+    Lines beginning with '#' are ignored as comments.
+
+    Example data lines:
+
+      A ALA 1 N 3.5
+      A ALA 1 CA 3.0
+      A ALA 1 CB 3.14159
+      A ALA 1 C  6.23
+      A ALA 1 O    5.1
+      A GLY 2 N 10.3
+      A GLY 2 CA 1.714
+      A GLY 2 C -0.05
+      A GLY 2 O -3.12
+
+SEE ALSO
+
+    data2b_res, data2q_atom, data2q_res
+    """
+
+    b_dict = atom_data_extract(data_file)
+    quiet = int(quiet) == 1
+
+    def b_lookup(chain, resi, name, ID, b):
+        def _lookup(chain, resi, name, ID):
+            if resi in b_dict[chain] and isinstance(b_dict[chain][resi], dict):
+                return b_dict[chain][resi][name][0]
+            else:
+                # find data by ID
+                return b_dict[chain][int(ID)][0]
+        try:
+            if not chain in b_dict:
+                chain = ''
+            b = _lookup(chain, resi, name, ID)
+            if not quiet: print('///%s/%s/%s new: %f' % (chain, resi, name, b))
+        except KeyError:
+            if not quiet: print('///%s/%s/%s keeping: %f' % (chain, resi, name, b))
+        return b
+    stored.b = b_lookup
+
+    cmd.alter(mol, '%s=stored.b(chain, resi, name, ID, %s)' % (property, property))
+    cmd.rebuild()
+
+def data2b_res(mol='', data_file='', property='b', quiet=0):
+    """
+DESCRIPTION
+
+    Alters the B-factor data by residue.
+
+USAGE
+
+    data2b_res <mol>, <data_file>
+
+    where <mol> is the molecular object whose B-factor data you wish to modify
+    and <data_file> is a file contain the data (one value for each residue)
+    The format of <data_file> should be:
+
+         chain resi resn data
+    or
+         resi resn data
+    or
+         resi data
+
+    (i.e. "chain" is optional). Lines beginning with '#' are ignored as comments.
+
+SEE ALSO
+
+    data2b_atom, data2q_atom, data2q_res
+    """
+
+    b_dict = residue_data_extract(data_file)
+    quiet = int(quiet) == 1
+
+    def b_lookup(chain, resi, name, b):
+        try:
+            if chain in b_dict:
+                b = b_dict[chain][resi][0]
+            else:
+                b = b_dict[''][resi][0]
+            if not quiet: print('///%s/%s/%s new: %f' % (chain, resi, name, b))
+        except KeyError:
+            if not quiet: print('///%s/%s/%s keeping: %f' % (chain, resi, name, b))
+        return b
+    stored.b = b_lookup
+
+    cmd.alter(mol, '%s=stored.b(chain, resi, name, %s)' % (property, property))
+    cmd.rebuild()
+
+def data2q_atom(mol='',data_file=''):
+    """
+DESCRIPTION
+
+    Alters the occupancy data by atom.
+
+USAGE
+
+    See data2b_atom
+
+SEE ALSO
+
+    data2q_res, data2b_atom, data2b_res
+    """
+    data2b_atom(mol, data_file, property='q')
+
+def data2q_res(mol='',data_file=''):
+    """
+DESCRIPTION
+
+    Alters the occupancy data by residue.
+
+USAGE
+
+    See data2b_res
+
+SEE ALSO
+
+    data2q_atom, data2b_atom, data2b_res
+    """
+    data2b_res(mol, data_file, property='q')
+
+cmd.extend('data2b_res',data2b_res)
+cmd.extend('data2b_atom',data2b_atom)
+cmd.extend('data2q_res',data2q_res)
+cmd.extend('data2q_atom',data2q_atom)
```

### Comparing `tmkit-0.0.0.2/tmkit/visualize/lib/palette/spectrumany.py` & `tmkit-0.0.2/tmkit/visualize/component/palette/spectrumany.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-'''
-http://pymolwiki.org/index.php/spectrumany
-
-(c) 2010 Thomas Holder
-
-License: BSD-2-Clause
-'''
-
-from __future__ import print_function
-
-from pymol import cmd, stored
-
-expression_sc = cmd.Shortcut([
-    'count',
-    'resi',
-    'b',
-    'q',
-    'pc',
-])
-
-
-def spectrumany(expression, color_list, selection='(all)', minimum=None, maximum=None, quiet=1):
-    '''
-DESCRIPTION
-
-    Define a color spectrum with as many color-stops as you like (at least 2).
-
-USAGE
-
-    spectrumany expression, color_list [, selection [, minimum [, maximum ]]]
-
-ARGUMENTS
-
-    expression = count, resi, b, q, or pc: respectively, atom count, residue
-    index, temperature factor, occupancy, or partial charge {default: count}
-
-    color_list = string: Space separated list of colors
-
-    ... all other arguments like with `spectrum` command
-
-EXAMPLE
-
-    spectrumany count, forest green yellow white
-    spectrumany b, red yellow white, (polymer), maximum=100.0
-
-SEE ALSO
-
-    spectrum
-    '''
-    quiet = int(quiet)
-    colors = color_list.split()
-    if len(colors) < 2:
-        print('failed! please provide at least 2 colors')
-        return
-
-    colvec = [cmd.get_color_tuple(i) for i in colors]
-    print(colvec)
-    parts = len(colvec) - 1
-
-    expression = {'pc': 'partial_charge', 'fc': 'formal_charge',
-                  'count': 'index'}.get(expression, expression)
-    minmax_expr = {'resi': 'resv'}.get(expression, expression)
-    discrete_expr = ['index', 'resi']
-
-    if cmd.count_atoms(selection) == 0:
-        print('empty selection')
-        return
-
-    if None in [minimum, maximum]:
-        stored.e = list()
-        cmd.iterate(selection, 'stored.e.append(%s)' % (minmax_expr))
-        if minimum is None:
-            minimum = min(stored.e)
-        if maximum is None:
-            maximum = max(stored.e)
-    minimum, maximum = float(minimum), float(maximum)
-    if not quiet:
-        print(' Spectrum: range (%.5f to %.5f)' % (minimum, maximum))
-
-    if maximum == minimum:
-        print('no spectrum possible, only equal %s values' % (expression))
-        return
-
-    if expression in discrete_expr:
-        val_range = int(maximum - minimum + 1)
-    else:
-        val_range = maximum - minimum
-        cmd.color(colors[0], selection)
-
-    # ### /*** the line below is where I modified sth. original: steps = 60 / parts ***/
-    steps = 60 // parts
-    steps_total = steps * parts
-
-    val_start = minimum
-    for p in range(parts):
-        for i in range(steps):
-            ii = float(i) / steps
-            col_list = [colvec[p + 1][j] * ii + colvec[p][j] * (1.0 - ii) for j in range(3)]
-            # print(col_list)
-            # ### /*** the line below is where I modified sth. ***/
-            col_name = '0x%02x%02x%02x' % (int(col_list[0] * 255), int(col_list[1] * 255), int(col_list[2] * 255))
-            # col_name = '0x%02x%02x%02x' % (col_list[0] * 255, col_list[1] * 255, col_list[2] * 255)
-            val_end = val_range * (i + 1 + p * steps) / steps_total + minimum
-            if expression in discrete_expr:
-                cmd.color(col_name, '(%s) and %s %d-%d' % (selection, expression, val_start, val_end))
-            else:
-                cmd.color(col_name, '(%s) and %s > %f' % (selection, expression, val_start))
-            val_start = val_end
-
-cmd.extend('spectrumany', spectrumany)
-
-# tab-completion of arguments
-cmd.auto_arg[0]['spectrumany'] = [expression_sc, 'expression', ', ']
-cmd.auto_arg[1]['spectrumany'] = [cmd.auto_arg[0]['color'][0], 'color', ' ']
-cmd.auto_arg[2]['spectrumany'] = cmd.auto_arg[2]['spectrum']
-
-# vi:expandtab:smarttab
+'''
+http://pymolwiki.org/index.php/spectrumany
+
+(c) 2010 Thomas Holder
+
+License: BSD-2-Clause
+'''
+
+from __future__ import print_function
+
+from pymol import cmd, stored
+
+expression_sc = cmd.Shortcut([
+    'count',
+    'resi',
+    'b',
+    'q',
+    'pc',
+])
+
+
+def spectrumany(expression, color_list, selection='(all)', minimum=None, maximum=None, quiet=1):
+    '''
+DESCRIPTION
+
+    Define a color spectrum with as many color-stops as you like (at least 2).
+
+USAGE
+
+    spectrumany expression, color_list [, selection [, minimum [, maximum ]]]
+
+ARGUMENTS
+
+    expression = count, resi, b, q, or pc: respectively, atom count, residue
+    index, temperature factor, occupancy, or partial charge {default: count}
+
+    color_list = string: Space separated list of colors
+
+    ... all other arguments like with `spectrum` command
+
+EXAMPLE
+
+    spectrumany count, forest green yellow white
+    spectrumany b, red yellow white, (polymer), maximum=100.0
+
+SEE ALSO
+
+    spectrum
+    '''
+    quiet = int(quiet)
+    colors = color_list.split()
+    if len(colors) < 2:
+        print('failed! please provide at least 2 colors')
+        return
+
+    colvec = [cmd.get_color_tuple(i) for i in colors]
+    print(colvec)
+    parts = len(colvec) - 1
+
+    expression = {'pc': 'partial_charge', 'fc': 'formal_charge',
+                  'count': 'index'}.get(expression, expression)
+    minmax_expr = {'resi': 'resv'}.get(expression, expression)
+    discrete_expr = ['index', 'resi']
+
+    if cmd.count_atoms(selection) == 0:
+        print('empty selection')
+        return
+
+    if None in [minimum, maximum]:
+        stored.e = list()
+        cmd.iterate(selection, 'stored.e.append(%s)' % (minmax_expr))
+        if minimum is None:
+            minimum = min(stored.e)
+        if maximum is None:
+            maximum = max(stored.e)
+    minimum, maximum = float(minimum), float(maximum)
+    if not quiet:
+        print(' Spectrum: range (%.5f to %.5f)' % (minimum, maximum))
+
+    if maximum == minimum:
+        print('no spectrum possible, only equal %s values' % (expression))
+        return
+
+    if expression in discrete_expr:
+        val_range = int(maximum - minimum + 1)
+    else:
+        val_range = maximum - minimum
+        cmd.color(colors[0], selection)
+
+    # ### /*** the line below is where I modified sth. original: steps = 60 / parts ***/
+    steps = 60 // parts
+    steps_total = steps * parts
+
+    val_start = minimum
+    for p in range(parts):
+        for i in range(steps):
+            ii = float(i) / steps
+            col_list = [colvec[p + 1][j] * ii + colvec[p][j] * (1.0 - ii) for j in range(3)]
+            # print(col_list)
+            # ### /*** the line below is where I modified sth. ***/
+            col_name = '0x%02x%02x%02x' % (int(col_list[0] * 255), int(col_list[1] * 255), int(col_list[2] * 255))
+            # col_name = '0x%02x%02x%02x' % (col_list[0] * 255, col_list[1] * 255, col_list[2] * 255)
+            val_end = val_range * (i + 1 + p * steps) / steps_total + minimum
+            if expression in discrete_expr:
+                cmd.color(col_name, '(%s) and %s %d-%d' % (selection, expression, val_start, val_end))
+            else:
+                cmd.color(col_name, '(%s) and %s > %f' % (selection, expression, val_start))
+            val_start = val_end
+
+cmd.extend('spectrumany', spectrumany)
+
+# tab-completion of arguments
+cmd.auto_arg[0]['spectrumany'] = [expression_sc, 'expression', ', ']
+cmd.auto_arg[1]['spectrumany'] = [cmd.auto_arg[0]['color'][0], 'color', ' ']
+cmd.auto_arg[2]['spectrumany'] = cmd.auto_arg[2]['spectrum']
+
+# vi:expandtab:smarttab
```

### Comparing `tmkit-0.0.0.2/tmkit/visualize/lib/show_contacts.py` & `tmkit-0.0.2/tmkit/visualize/component/show_contacts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-#!/usr/bin/python
-
-'''PyMOL plugin that provides show_contacts command and GUI
-for highlighting good and bad polar contacts. Factored out of 
-clustermols by Matthew Baumgartner.
-The advantage of this package is it requires many fewer dependencies.
-'''
-from __future__ import print_function
-
-import sys, os
-from pymol import cmd
-
-DEBUG=1
-
-
-def show_contacts(selection, selection2, result="contacts", cutoff=3.6, bigcutoff=4.0, SC_DEBUG = DEBUG):
-    """
-    USAGE
-
-    show_contacts selection, selection2, [result=contacts],[cutoff=3.6],[bigcutoff=4.0]
-
-    Show various polar contacts, the good, the bad, and the ugly.
-
-    Edit MPB 6-26-14: The distances are heavy atom distances, so I upped the default cutoff to 4.0
-    
-    Returns:
-    True/False -  if False, something went wrong
-    """
-    if SC_DEBUG > 4:
-        print('Starting show_contacts')
-        print('selection = "' + selection + '"')
-        print('selection2 = "' + selection2 + '"')
-            
-    result = cmd.get_legal_name(result)
-
-    #if the group of contacts already exist, delete them
-    cmd.delete(result)
-
-    # ensure only N and O atoms are in the selection
-    all_don_acc1 = selection + " and (donor or acceptor)"
-    all_don_acc2 = selection2 + " and  (donor or acceptor)"
-    
-    if SC_DEBUG > 4:
-        print('all_don_acc1 = "' + all_don_acc1 + '"')
-        print('all_don_acc2 = "' + all_don_acc2 + '"')
-    
-    #if theses selections turn out not to have any atoms in them, pymol throws cryptic errors when calling the dist function like:
-    #'Selector-Error: Invalid selection name'
-    #So for each one, manually perform the selection and then pass the reference to the distance command and at the end, clean up the selections
-    #the return values are the count of the number of atoms
-    all1_sele_count = cmd.select('all_don_acc1_sele', all_don_acc1)
-    all2_sele_count = cmd.select('all_don_acc2_sele', all_don_acc2)
-    
-    #print out some warnings
-    if DEBUG > 3:
-        if not all1_sele_count:
-            print('Warning: all_don_acc1 selection empty!')
-        if not all2_sele_count:
-            print('Warning: all_don_acc2 selection empty!')
-    
-    ########################################
-    allres = result + "_all"
-    if all1_sele_count and all2_sele_count:
-        cmd.distance(allres, 'all_don_acc1_sele', 'all_don_acc2_sele', bigcutoff, mode = 0)
-        cmd.set("dash_radius", "0.05", allres)
-        cmd.set("dash_color", "purple", allres)
-        cmd.hide("labels", allres)
-    
-    ########################################
-    #compute good polar interactions according to pymol
-    polres = result + "_polar"
-    if all1_sele_count and all2_sele_count:
-        cmd.distance(polres, 'all_don_acc1_sele', 'all_don_acc2_sele', cutoff, mode = 2) #hopefully this checks angles? Yes
-        cmd.set("dash_radius","0.126",polres)
-    
-    ########################################
-    #When running distance in mode=2, the cutoff parameter is ignored if set higher then the default of 3.6
-    #so set it to the passed in cutoff and change it back when you are done.
-    old_h_bond_cutoff_center = cmd.get('h_bond_cutoff_center') # ideal geometry
-    old_h_bond_cutoff_edge = cmd.get('h_bond_cutoff_edge') # minimally acceptable geometry
-    cmd.set('h_bond_cutoff_center', bigcutoff)
-    cmd.set('h_bond_cutoff_edge', bigcutoff)
-        
-    #compute possibly suboptimal polar interactions using the user specified distance
-    pol_ok_res = result + "_polar_ok"
-    if all1_sele_count and all2_sele_count:
-        cmd.distance(pol_ok_res, 'all_don_acc1_sele', 'all_don_acc2_sele', bigcutoff, mode = 2) 
-        cmd.set("dash_radius", "0.06", pol_ok_res)
-
-    #now reset the h_bond cutoffs
-    cmd.set('h_bond_cutoff_center', old_h_bond_cutoff_center)
-    cmd.set('h_bond_cutoff_edge', old_h_bond_cutoff_edge) 
-    
-    
-    ########################################
-    
-    onlyacceptors1 = selection + " and (acceptor and !donor)"
-    onlyacceptors2 = selection2 + " and (acceptor and !donor)"
-    onlydonors1 = selection + " and (!acceptor and donor)"
-    onlydonors2 = selection2 + " and (!acceptor and donor)"  
-    
-    #perform the selections
-    onlyacceptors1_sele_count = cmd.select('onlyacceptors1_sele', onlyacceptors1)
-    onlyacceptors2_sele_count = cmd.select('onlyacceptors2_sele', onlyacceptors2)
-    onlydonors1_sele_count = cmd.select('onlydonors1_sele', onlydonors1)
-    onlydonors2_sele_count = cmd.select('onlydonors2_sele', onlydonors2)    
-    
-    #print out some warnings
-    if SC_DEBUG > 2:
-        if not onlyacceptors1_sele_count:
-            print('Warning: onlyacceptors1 selection empty!')
-        if not onlyacceptors2_sele_count:
-            print('Warning: onlyacceptors2 selection empty!')
-        if not onlydonors1_sele_count:
-            print('Warning: onlydonors1 selection empty!')
-        if not onlydonors2_sele_count:
-            print('Warning: onlydonors2 selection empty!')    
-            
-    
-    accres = result+"_aa"
-    if onlyacceptors1_sele_count and onlyacceptors2_sele_count:
-        aa_dist_out = cmd.distance(accres, 'onlyacceptors1_sele', 'onlyacceptors2_sele', cutoff, 0)
-
-        if aa_dist_out < 0:
-            print('\n\nCaught a pymol selection error in acceptor-acceptor selection of show_contacts')
-            print('accres:', accres)
-            print('onlyacceptors1', onlyacceptors1)
-            print('onlyacceptors2', onlyacceptors2)
-            return False
-    
-        cmd.set("dash_color","red",accres)
-        cmd.set("dash_radius","0.125",accres)
-    
-    ########################################
-    
-    donres = result+"_dd"
-    if onlydonors1_sele_count and onlydonors2_sele_count:
-        dd_dist_out = cmd.distance(donres, 'onlydonors1_sele', 'onlydonors2_sele', cutoff, 0)
-        
-        #try to catch the error state 
-        if dd_dist_out < 0:
-            print('\n\nCaught a pymol selection error in dd selection of show_contacts')
-            print('donres:', donres)
-            print('onlydonors1', onlydonors1)
-            print('onlydonors2', onlydonors2)
-            print("cmd.distance('" + donres + "', '" + onlydonors1 + "', '" + onlydonors2 + "', " + str(cutoff) + ", 0)")  
-            return False
-        
-        cmd.set("dash_color","red",donres)  
-        cmd.set("dash_radius","0.125",donres)
-    
-    ##########################################################
-    ##### find the buried unpaired atoms of the receptor #####
-    ##########################################################
-    
-    #initialize the variable for when CALC_SASA is False
-    unpaired_atoms = ''
-    
-        
-    ## Group
-    cmd.group(result,"%s %s %s %s %s %s" % (polres, allres, accres, donres, pol_ok_res, unpaired_atoms))
-    
-    ## Clean up the selection objects
-    #if the show_contacts debug level is high enough, don't delete them.
-    if SC_DEBUG < 5:
-        cmd.delete('all_don_acc1_sele')
-        cmd.delete('all_don_acc2_sele')
-        cmd.delete('onlyacceptors1_sele')
-        cmd.delete('onlyacceptors2_sele')
-        cmd.delete('onlydonors1_sele')
-        cmd.delete('onlydonors2_sele')
-    
-    
-    return True
-cmd.extend('contacts', show_contacts) #contacts to avoid clashing with cluster_mols version
-
-
-
-    
-    
-#################################################################################
-########################### Start of pymol plugin code ##########################
-#################################################################################
-
-
-about_text = '''show_contacts was factored out of the much more full-featured cluster_mols
-by Dr. Matt Baumgartner (https://pymolwiki.org/index.php/Cluster_mols).  It provides
-an easy way to highlight polar contacts (and clashes) between two selections without
-requiring the installation of additional dependencies.
-'''
-
-class Show_Contacts:
-    ''' Tk version of the Plugin GUI '''
-    def __init__(self, app):
-        parent = app.root
-        self.parent = parent
-        
-        self.app = app
-        
-        import Pmw
-
-        ############################################################################################
-        ### Open a window with options to select to loaded objects ###
-        ############################################################################################
-
-        self.select_dialog = Pmw.Dialog(parent, 
-                         buttons = ('Ok','Cancel'), 
-                         title = 'Show Contacts Plugin',
-                         command = self.button_pressed )
-    
-        self.select_dialog.withdraw()
-    
-
-        #allow the user to select from objects already loaded in pymol
-        self.select_object_combo_box = Pmw.ComboBox(self.select_dialog.interior(),
-                                                               scrolledlist_items=[],
-                                                               labelpos='w',
-                                                               label_text='Select loaded object:',
-                                                               listbox_height = 2,
-                                                               dropdown=True)
-        self.select_object_combo_box2 = Pmw.ComboBox(self.select_dialog.interior(),
-                                                               scrolledlist_items=[],
-                                                               labelpos='w',
-                                                               label_text='Select loaded object:',
-                                                               listbox_height = 2,
-                                                               dropdown=True)                                                               
-        self.select_object_combo_box.grid(column=1, row=0)
-        self.select_object_combo_box2.grid(column=2, row=0)
-        self.populate_ligand_select_list()
-        self.select_dialog.show()
-        
-
-      
-    def button_pressed(self, result):
-        if hasattr(result,'keycode'):
-            if result.keycode == 36:
-                print('keycode:', result.keycode)
-        elif result == 'Ok' or result == 'Exit' or result == None:
-            s1 = self.select_object_combo_box.get()
-            s2 = self.select_object_combo_box2.get()
-            show_contacts(s1,s2,'%s_%s'%(s1,s2))
-            self.select_dialog.withdraw()            
-        elif result == 'Cancel' or result == None:
-            self.select_dialog.withdraw()
-
-            
-
-    
-    def populate_ligand_select_list(self):
-        ''' Go thourgh the loaded objects in PyMOL and add them to the selected list. '''
-        #get the loaded objects
-        loaded_objects = _get_select_list()
-         
-        self.select_object_combo_box.clear()
-        self.select_object_combo_box2.clear()
-        
-        for ob in loaded_objects:
-            self.select_object_combo_box.insert('end', ob)
-            self.select_object_combo_box2.insert('end', ob)
-        
-
-def _get_select_list():
-    '''
-    Get either a list of object names, or a list of chain selections
-    '''
-    loaded_objects = [name for name in cmd.get_names('all', 1) if '_cluster_' not in name]
-
-    # if single object, try chain selections
-    if len(loaded_objects) == 1:
-        chains = cmd.get_chains(loaded_objects[0])
-        if len(chains) > 1:
-            loaded_objects = ['{} & chain {}'.format(loaded_objects[0], chain) for chain in chains]
-
-    return loaded_objects
-
-
-class Show_Contacts_Qt_Dialog(object):
-    ''' Qt version of the Plugin GUI '''
-    def __init__(self):
-        from pymol.Qt import QtWidgets
-        dialog = QtWidgets.QDialog()
-        self.setupUi(dialog)
-        self.populate_ligand_select_list()
-        dialog.accepted.connect(self.accept)
-        dialog.exec_()
-
-    def accept(self):
-        s1 = self.select_object_combo_box.currentText()
-        s2 = self.select_object_combo_box2.currentText()
-        show_contacts(s1, s2, '%s_%s' % (s1, s2))
-
-    def populate_ligand_select_list(self):
-        loaded_objects = _get_select_list()
-
-        self.select_object_combo_box.clear()
-        self.select_object_combo_box2.clear()
-
-        self.select_object_combo_box.addItems(loaded_objects)
-        self.select_object_combo_box2.addItems(loaded_objects)
-
-        if len(loaded_objects) > 1:
-            self.select_object_combo_box2.setCurrentIndex(1)
-
-    def setupUi(self, Dialog):
-        # Based on auto-generated code from ui file
-        from pymol.Qt import QtCore, QtWidgets
-        Dialog.resize(400, 50)
-        self.gridLayout = QtWidgets.QGridLayout(Dialog)
-        label = QtWidgets.QLabel("Select loaded object:", Dialog)
-        self.gridLayout.addWidget(label, 0, 0, 1, 1)
-        self.select_object_combo_box = QtWidgets.QComboBox(Dialog)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
-        self.select_object_combo_box.setSizePolicy(sizePolicy)
-        self.select_object_combo_box.setEditable(True)
-        self.gridLayout.addWidget(self.select_object_combo_box, 0, 1, 1, 1)
-        label = QtWidgets.QLabel("Select loaded object:", Dialog)
-        self.gridLayout.addWidget(label, 1, 0, 1, 1)
-        self.select_object_combo_box2 = QtWidgets.QComboBox(Dialog)
-        self.select_object_combo_box2.setSizePolicy(sizePolicy)
-        self.select_object_combo_box2.setEditable(True)
-        self.gridLayout.addWidget(self.select_object_combo_box2, 1, 1, 1, 1)
-        self.buttonBox = QtWidgets.QDialogButtonBox(Dialog)
-        self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Ok)
-        self.gridLayout.addWidget(self.buttonBox, 2, 0, 1, 2)
-        self.buttonBox.accepted.connect(Dialog.accept)
-        self.buttonBox.rejected.connect(Dialog.reject)
-
-    
-def __init__(self):
-    try:
-        from pymol.plugins import addmenuitemqt
-        addmenuitemqt('Show Contacts', Show_Contacts_Qt_Dialog)
-        return
-    except Exception as e:
-        print(e)
-    self.menuBar.addmenuitem('Plugin', 'command', 'Show Contacts', label = 'Show Contacts', command = lambda s=self : Show_Contacts(s))  
-        
-
+#!/usr/bin/python
+
+'''PyMOL plugin that provides show_contacts command and GUI
+for highlighting good and bad polar contacts. Factored out of 
+clustermols by Matthew Baumgartner.
+The advantage of this package is it requires many fewer dependencies.
+'''
+from __future__ import print_function
+
+import sys, os
+from pymol import cmd
+
+DEBUG=1
+
+
+def show_contacts(selection, selection2, result="contacts", cutoff=3.6, bigcutoff=4.0, SC_DEBUG = DEBUG):
+    """
+    USAGE
+
+    show_contacts selection, selection2, [result=contacts],[cutoff=3.6],[bigcutoff=4.0]
+
+    Show various polar contacts, the good, the bad, and the ugly.
+
+    Edit MPB 6-26-14: The distances are heavy atom distances, so I upped the default cutoff to 4.0
+    
+    Returns:
+    True/False -  if False, something went wrong
+    """
+    if SC_DEBUG > 4:
+        print('Starting show_contacts')
+        print('selection = "' + selection + '"')
+        print('selection2 = "' + selection2 + '"')
+            
+    result = cmd.get_legal_name(result)
+
+    #if the group of contacts already exist, delete them
+    cmd.delete(result)
+
+    # ensure only N and O atoms are in the selection
+    all_don_acc1 = selection + " and (donor or acceptor)"
+    all_don_acc2 = selection2 + " and  (donor or acceptor)"
+    
+    if SC_DEBUG > 4:
+        print('all_don_acc1 = "' + all_don_acc1 + '"')
+        print('all_don_acc2 = "' + all_don_acc2 + '"')
+    
+    #if theses selections turn out not to have any atoms in them, pymol throws cryptic errors when calling the dist function like:
+    #'Selector-Error: Invalid selection name'
+    #So for each one, manually perform the selection and then pass the reference to the distance command and at the end, clean up the selections
+    #the return values are the count of the number of atoms
+    all1_sele_count = cmd.select('all_don_acc1_sele', all_don_acc1)
+    all2_sele_count = cmd.select('all_don_acc2_sele', all_don_acc2)
+    
+    #print out some warnings
+    if DEBUG > 3:
+        if not all1_sele_count:
+            print('Warning: all_don_acc1 selection empty!')
+        if not all2_sele_count:
+            print('Warning: all_don_acc2 selection empty!')
+    
+    ########################################
+    allres = result + "_all"
+    if all1_sele_count and all2_sele_count:
+        cmd.distance(allres, 'all_don_acc1_sele', 'all_don_acc2_sele', bigcutoff, mode = 0)
+        cmd.set("dash_radius", "0.05", allres)
+        cmd.set("dash_color", "purple", allres)
+        cmd.hide("labels", allres)
+    
+    ########################################
+    #compute good polar interactions according to pymol
+    polres = result + "_polar"
+    if all1_sele_count and all2_sele_count:
+        cmd.distance(polres, 'all_don_acc1_sele', 'all_don_acc2_sele', cutoff, mode = 2) #hopefully this checks angles? Yes
+        cmd.set("dash_radius","0.126",polres)
+    
+    ########################################
+    #When running distance in mode=2, the cutoff parameter is ignored if set higher then the default of 3.6
+    #so set it to the passed in cutoff and change it back when you are done.
+    old_h_bond_cutoff_center = cmd.get('h_bond_cutoff_center') # ideal geometry
+    old_h_bond_cutoff_edge = cmd.get('h_bond_cutoff_edge') # minimally acceptable geometry
+    cmd.set('h_bond_cutoff_center', bigcutoff)
+    cmd.set('h_bond_cutoff_edge', bigcutoff)
+        
+    #compute possibly suboptimal polar interactions using the user specified distance
+    pol_ok_res = result + "_polar_ok"
+    if all1_sele_count and all2_sele_count:
+        cmd.distance(pol_ok_res, 'all_don_acc1_sele', 'all_don_acc2_sele', bigcutoff, mode = 2) 
+        cmd.set("dash_radius", "0.06", pol_ok_res)
+
+    #now reset the h_bond cutoffs
+    cmd.set('h_bond_cutoff_center', old_h_bond_cutoff_center)
+    cmd.set('h_bond_cutoff_edge', old_h_bond_cutoff_edge) 
+    
+    
+    ########################################
+    
+    onlyacceptors1 = selection + " and (acceptor and !donor)"
+    onlyacceptors2 = selection2 + " and (acceptor and !donor)"
+    onlydonors1 = selection + " and (!acceptor and donor)"
+    onlydonors2 = selection2 + " and (!acceptor and donor)"  
+    
+    #perform the selections
+    onlyacceptors1_sele_count = cmd.select('onlyacceptors1_sele', onlyacceptors1)
+    onlyacceptors2_sele_count = cmd.select('onlyacceptors2_sele', onlyacceptors2)
+    onlydonors1_sele_count = cmd.select('onlydonors1_sele', onlydonors1)
+    onlydonors2_sele_count = cmd.select('onlydonors2_sele', onlydonors2)    
+    
+    #print out some warnings
+    if SC_DEBUG > 2:
+        if not onlyacceptors1_sele_count:
+            print('Warning: onlyacceptors1 selection empty!')
+        if not onlyacceptors2_sele_count:
+            print('Warning: onlyacceptors2 selection empty!')
+        if not onlydonors1_sele_count:
+            print('Warning: onlydonors1 selection empty!')
+        if not onlydonors2_sele_count:
+            print('Warning: onlydonors2 selection empty!')    
+            
+    
+    accres = result+"_aa"
+    if onlyacceptors1_sele_count and onlyacceptors2_sele_count:
+        aa_dist_out = cmd.distance(accres, 'onlyacceptors1_sele', 'onlyacceptors2_sele', cutoff, 0)
+
+        if aa_dist_out < 0:
+            print('\n\nCaught a pymol selection error in acceptor-acceptor selection of show_contacts')
+            print('accres:', accres)
+            print('onlyacceptors1', onlyacceptors1)
+            print('onlyacceptors2', onlyacceptors2)
+            return False
+    
+        cmd.set("dash_color","red",accres)
+        cmd.set("dash_radius","0.125",accres)
+    
+    ########################################
+    
+    donres = result+"_dd"
+    if onlydonors1_sele_count and onlydonors2_sele_count:
+        dd_dist_out = cmd.distance(donres, 'onlydonors1_sele', 'onlydonors2_sele', cutoff, 0)
+        
+        #try to catch the error state 
+        if dd_dist_out < 0:
+            print('\n\nCaught a pymol selection error in dd selection of show_contacts')
+            print('donres:', donres)
+            print('onlydonors1', onlydonors1)
+            print('onlydonors2', onlydonors2)
+            print("cmd.distance('" + donres + "', '" + onlydonors1 + "', '" + onlydonors2 + "', " + str(cutoff) + ", 0)")  
+            return False
+        
+        cmd.set("dash_color","red",donres)  
+        cmd.set("dash_radius","0.125",donres)
+    
+    ##########################################################
+    ##### find the buried unpaired atoms of the receptor #####
+    ##########################################################
+    
+    #initialize the variable for when CALC_SASA is False
+    unpaired_atoms = ''
+    
+        
+    ## Group
+    cmd.group(result,"%s %s %s %s %s %s" % (polres, allres, accres, donres, pol_ok_res, unpaired_atoms))
+    
+    ## Clean up the selection objects
+    #if the show_contacts debug level is high enough, don't delete them.
+    if SC_DEBUG < 5:
+        cmd.delete('all_don_acc1_sele')
+        cmd.delete('all_don_acc2_sele')
+        cmd.delete('onlyacceptors1_sele')
+        cmd.delete('onlyacceptors2_sele')
+        cmd.delete('onlydonors1_sele')
+        cmd.delete('onlydonors2_sele')
+    
+    
+    return True
+cmd.extend('contacts', show_contacts) #contacts to avoid clashing with cluster_mols version
+
+
+
+    
+    
+#################################################################################
+########################### Start of pymol plugin code ##########################
+#################################################################################
+
+
+about_text = '''show_contacts was factored out of the much more full-featured cluster_mols
+by Dr. Matt Baumgartner (https://pymolwiki.org/index.php/Cluster_mols).  It provides
+an easy way to highlight polar contacts (and clashes) between two selections without
+requiring the installation of additional dependencies.
+'''
+
+class Show_Contacts:
+    ''' Tk version of the Plugin GUI '''
+    def __init__(self, app):
+        parent = app.root
+        self.parent = parent
+        
+        self.app = app
+        
+        import Pmw
+
+        ############################################################################################
+        ### Open a window with options to select to loaded objects ###
+        ############################################################################################
+
+        self.select_dialog = Pmw.Dialog(parent, 
+                         buttons = ('Ok','Cancel'), 
+                         title = 'Show Contacts Plugin',
+                         command = self.button_pressed )
+    
+        self.select_dialog.withdraw()
+    
+
+        #allow the user to select from objects already loaded in pymol
+        self.select_object_combo_box = Pmw.ComboBox(self.select_dialog.interior(),
+                                                               scrolledlist_items=[],
+                                                               labelpos='w',
+                                                               label_text='Select loaded object:',
+                                                               listbox_height = 2,
+                                                               dropdown=True)
+        self.select_object_combo_box2 = Pmw.ComboBox(self.select_dialog.interior(),
+                                                               scrolledlist_items=[],
+                                                               labelpos='w',
+                                                               label_text='Select loaded object:',
+                                                               listbox_height = 2,
+                                                               dropdown=True)                                                               
+        self.select_object_combo_box.grid(column=1, row=0)
+        self.select_object_combo_box2.grid(column=2, row=0)
+        self.populate_ligand_select_list()
+        self.select_dialog.show()
+        
+
+      
+    def button_pressed(self, result):
+        if hasattr(result,'keycode'):
+            if result.keycode == 36:
+                print('keycode:', result.keycode)
+        elif result == 'Ok' or result == 'Exit' or result == None:
+            s1 = self.select_object_combo_box.get()
+            s2 = self.select_object_combo_box2.get()
+            show_contacts(s1,s2,'%s_%s'%(s1,s2))
+            self.select_dialog.withdraw()            
+        elif result == 'Cancel' or result == None:
+            self.select_dialog.withdraw()
+
+            
+
+    
+    def populate_ligand_select_list(self):
+        ''' Go thourgh the loaded objects in PyMOL and add them to the selected list. '''
+        #get the loaded objects
+        loaded_objects = _get_select_list()
+         
+        self.select_object_combo_box.clear()
+        self.select_object_combo_box2.clear()
+        
+        for ob in loaded_objects:
+            self.select_object_combo_box.insert('end', ob)
+            self.select_object_combo_box2.insert('end', ob)
+        
+
+def _get_select_list():
+    '''
+    Get either a list of object names, or a list of chain selections
+    '''
+    loaded_objects = [name for name in cmd.get_names('all', 1) if '_cluster_' not in name]
+
+    # if single object, try chain selections
+    if len(loaded_objects) == 1:
+        chains = cmd.get_chains(loaded_objects[0])
+        if len(chains) > 1:
+            loaded_objects = ['{} & chain {}'.format(loaded_objects[0], chain) for chain in chains]
+
+    return loaded_objects
+
+
+class Show_Contacts_Qt_Dialog:
+    ''' Qt version of the Plugin GUI '''
+    def __init__(self):
+        from pymol.Qt import QtWidgets
+        dialog = QtWidgets.QDialog()
+        self.setupUi(dialog)
+        self.populate_ligand_select_list()
+        dialog.accepted.connect(self.accept)
+        dialog.exec_()
+
+    def accept(self):
+        s1 = self.select_object_combo_box.currentText()
+        s2 = self.select_object_combo_box2.currentText()
+        show_contacts(s1, s2, '%s_%s' % (s1, s2))
+
+    def populate_ligand_select_list(self):
+        loaded_objects = _get_select_list()
+
+        self.select_object_combo_box.clear()
+        self.select_object_combo_box2.clear()
+
+        self.select_object_combo_box.addItems(loaded_objects)
+        self.select_object_combo_box2.addItems(loaded_objects)
+
+        if len(loaded_objects) > 1:
+            self.select_object_combo_box2.setCurrentIndex(1)
+
+    def setupUi(self, Dialog):
+        # Based on auto-generated code from ui file
+        from pymol.Qt import QtCore, QtWidgets
+        Dialog.resize(400, 50)
+        self.gridLayout = QtWidgets.QGridLayout(Dialog)
+        label = QtWidgets.QLabel("Select loaded object:", Dialog)
+        self.gridLayout.addWidget(label, 0, 0, 1, 1)
+        self.select_object_combo_box = QtWidgets.QComboBox(Dialog)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        self.select_object_combo_box.setSizePolicy(sizePolicy)
+        self.select_object_combo_box.setEditable(True)
+        self.gridLayout.addWidget(self.select_object_combo_box, 0, 1, 1, 1)
+        label = QtWidgets.QLabel("Select loaded object:", Dialog)
+        self.gridLayout.addWidget(label, 1, 0, 1, 1)
+        self.select_object_combo_box2 = QtWidgets.QComboBox(Dialog)
+        self.select_object_combo_box2.setSizePolicy(sizePolicy)
+        self.select_object_combo_box2.setEditable(True)
+        self.gridLayout.addWidget(self.select_object_combo_box2, 1, 1, 1, 1)
+        self.buttonBox = QtWidgets.QDialogButtonBox(Dialog)
+        self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Ok)
+        self.gridLayout.addWidget(self.buttonBox, 2, 0, 1, 2)
+        self.buttonBox.accepted.connect(Dialog.accept)
+        self.buttonBox.rejected.connect(Dialog.reject)
+
+    
+def __init__(self):
+    try:
+        from pymol.plugins import addmenuitemqt
+        addmenuitemqt('Show Contacts', Show_Contacts_Qt_Dialog)
+        return
+    except Exception as e:
+        print(e)
+    self.menuBar.addmenuitem('Plugin', 'command', 'Show Contacts', label = 'Show Contacts', command = lambda s=self : Show_Contacts(s))  
+        
+
```

### Comparing `tmkit-0.0.0.2/tmkit/visualize/small/Label.py` & `tmkit-0.0.2/tmkit/visualize/small/Label.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from pymol import cmd
 
-
-class label(object):
-
-    def __init__(self, ):
-        pass
+class label:
 
     def putup(self, select):
+        from pymol import cmd
         cmd.label2(
             selection=select,
             expression='resn, resi',
         )
         # cmd.set(name='label_font_id', selection=select, value=18)
         # cmd.set(name='label_shadow_mode', selection=select, value=1)
         cmd.set(name='label_color', selection=select, value='orange')
-        cmd.set(name='label_size', value=40, selection=select)
-
-
-
-
-
+        cmd.set(name='label_size', value=40, selection=select)
```

### Comparing `tmkit-0.0.0.2/tmkit/visualize/small/Local.py` & `tmkit-0.0.2/tmkit/visualize/small/Local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from pymol import cmd
-from pymol import finish_launching
-from pymol import preset
 from tmkit.visualize.small.Palette import palette as pppmpalette
 from tmkit.visualize.small.Select import select as pppmselect
 from tmkit.visualize.small.Style import style as pppmstyle
 from tmkit.visualize.small.Label import label as pppmlabel
 from tmkit.chain.PDB import pdb as cpdb
 
 
-class local(object):
+class local:
 
     def __init__(
             self,
             prot_name,
             pdb_complex_fp,
             prot_c,
             sm_c,
@@ -40,14 +37,17 @@
         nby_rep
             'spheres',
         prot_c
             'blue_white_magenta', # 'blue_magenta' rainbow
         sm_c
             'blue_green',
         """
+        from pymol import cmd
+        from pymol import finish_launching
+        from pymol import preset
         finish_launching()
 
         cmd.bg_color(
             color="black"
             # color="white"
         )
 
@@ -86,21 +86,8 @@
         )
         cmd.show(
             selection='pocket',
             representation=pocket_rep,
         )
         pppmlabel().putup(select='nby', )
 
-        cmd.set(name='sphere_scale', value=1.5, selection='nby')
-
-
-if __name__ == "__main__":
-    from tmkit.Path import to
-
-    local(
-        prot_name='6feq',
-        pdb_complex_fp=to('data/example/pymol/'),
-        sm_rep="sticks",
-        nby_rep='spheres',
-        prot_c='blue_white_magenta',
-        sm_c='blue_green',
-    )
+        cmd.set(name='sphere_scale', value=1.5, selection='nby')
```

### Comparing `tmkit-0.0.0.2/tmkit.egg-info/SOURCES.txt` & `tmkit-0.0.2/tmkit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 LICENSE
 README.md
 setup.py
 tmkit/Path.py
-tmkit/SeqNetRR.py
 tmkit/__init__.py
 tmkit/cath.py
 tmkit/collate.py
 tmkit/edge.py
 tmkit/feature.py
+tmkit/fetch.py
 tmkit/mapping.py
 tmkit/msa.py
 tmkit/mut.py
-tmkit/pl.py
 tmkit/ppi.py
 tmkit/qc.py
 tmkit/rrc.py
 tmkit/seq.py
 tmkit/topo.py
 tmkit/vs.py
 tmkit.egg-info/PKG-INFO
@@ -46,57 +45,48 @@
 tmkit/db/construct/__init__.py
 tmkit/db/intact/Reader.py
 tmkit/db/intact/__init__.py
 tmkit/db/muthtp/Reader.py
 tmkit/db/muthtp/__init__.py
 tmkit/db/predmuthtp/Reader.py
 tmkit/db/predmuthtp/__init__.py
-tmkit/feature/HelixSurface.py
-tmkit/feature/__init__.py
-tmkit/feature/lips/__init__.py
 tmkit/id/Fasta.py
 tmkit/id/Mapping.py
 tmkit/id/PDB.py
 tmkit/id/__init__.py
 tmkit/interface/Tool.py
 tmkit/interface/Topology.py
 tmkit/interface/__init__.py
 tmkit/name/Mapping.py
 tmkit/name/__init__.py
 tmkit/position/__init__.py
 tmkit/position/scenario/Segment.py
 tmkit/position/scenario/Separation.py
 tmkit/position/scenario/__init__.py
+tmkit/property/HelixSurface.py
+tmkit/property/__init__.py
 tmkit/retrieve/MSA.py
 tmkit/retrieve/PDB.py
 tmkit/retrieve/XML.py
 tmkit/retrieve/__init__.py
 tmkit/seqnetrr/Compare.py
+tmkit/seqnetrr/ComputLib.py
 tmkit/seqnetrr/Controller.py
-tmkit/seqnetrr/Path.py
-tmkit/seqnetrr/Plot.py
 tmkit/seqnetrr/__init__.py
 tmkit/seqnetrr/combo/Length.py
 tmkit/seqnetrr/combo/Param.py
 tmkit/seqnetrr/combo/Position.py
 tmkit/seqnetrr/combo/Separation.py
 tmkit/seqnetrr/combo/__init__.py
 tmkit/seqnetrr/graph/Bipartite.py
 tmkit/seqnetrr/graph/Cumulative.py
 tmkit/seqnetrr/graph/Unipartite.py
 tmkit/seqnetrr/graph/__init__.py
 tmkit/seqnetrr/net/Reader.py
 tmkit/seqnetrr/net/__init__.py
-tmkit/seqnetrr/sequence/Fasta.py
-tmkit/seqnetrr/sequence/__init__.py
-tmkit/seqnetrr/util/ComputLib.py
-tmkit/seqnetrr/util/Console.py
-tmkit/seqnetrr/util/Reader.py
-tmkit/seqnetrr/util/Writer.py
-tmkit/seqnetrr/util/__init__.py
 tmkit/seqnetrr/window/Pair.py
 tmkit/seqnetrr/window/Single.py
 tmkit/seqnetrr/window/__init__.py
 tmkit/seqnetrr/window/base/Pair.py
 tmkit/seqnetrr/window/base/Single.py
 tmkit/seqnetrr/window/base/__init__.py
 tmkit/sequence/Fasta.py
@@ -123,27 +113,27 @@
 tmkit/topology/pdbtm/__init__.py
 tmkit/util/Console.py
 tmkit/util/Kit.py
 tmkit/util/Reader.py
 tmkit/util/Writer.py
 tmkit/util/__init__.py
 tmkit/visualize/__init__.py
+tmkit/visualize/component/Color.py
+tmkit/visualize/component/InterfaceResidues.py
+tmkit/visualize/component/Select.py
+tmkit/visualize/component/__init__.py
+tmkit/visualize/component/focal_blur.py
+tmkit/visualize/component/show_contacts.py
+tmkit/visualize/component/palette/__init__.py
+tmkit/visualize/component/palette/data2bfactor.py
+tmkit/visualize/component/palette/spectrumany.py
 tmkit/visualize/func/Coloring.py
 tmkit/visualize/func/__init__.py
 tmkit/visualize/isite/Labelling.py
 tmkit/visualize/isite/ProtocolDeepTMInter.py
 tmkit/visualize/isite/__init__.py
-tmkit/visualize/lib/Color.py
-tmkit/visualize/lib/InterfaceResidues.py
-tmkit/visualize/lib/Select.py
-tmkit/visualize/lib/__init__.py
-tmkit/visualize/lib/focal_blur.py
-tmkit/visualize/lib/show_contacts.py
-tmkit/visualize/lib/palette/__init__.py
-tmkit/visualize/lib/palette/data2bfactor.py
-tmkit/visualize/lib/palette/spectrumany.py
 tmkit/visualize/small/Label.py
 tmkit/visualize/small/Local.py
 tmkit/visualize/small/Palette.py
 tmkit/visualize/small/Select.py
 tmkit/visualize/small/Style.py
 tmkit/visualize/small/__init__.py
```

