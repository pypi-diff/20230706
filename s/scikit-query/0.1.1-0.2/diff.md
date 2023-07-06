# Comparing `tmp/scikit-query-0.1.1.tar.gz` & `tmp/scikit-query-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-query-0.1.1.tar", last modified: Sat Jun 10 22:00:25 2023, max compression
+gzip compressed data, was "scikit-query-0.2.tar", last modified: Thu Jul  6 11:40:03 2023, max compression
```

## Comparing `scikit-query-0.1.1.tar` & `scikit-query-0.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-10 21:59:40.000000 scikit-query-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-10 22:00:25.608819 scikit-query-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-10 21:59:40.000000 scikit-query-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.604819 scikit-query-0.1.1/scikit_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 22:00:25.608819 scikit-query-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-10 21:59:40.000000 scikit-query-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-10 21:59:41.000000 scikit-query-0.1.1/skquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/oracle/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/oracle/MLCLOracle.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/oracle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/pairwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/AIPC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/FFQS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/MinMax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/NPU.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/Pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/RandomMLCL.py
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/SASC.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/tests/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/utils/BaseSVDD.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/utils/line_intercept.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:40:03.462624 scikit-query-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 11:39:21.000000 scikit-query-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-06 11:40:03.462624 scikit-query-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-06 11:39:21.000000 scikit-query-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:40:03.462624 scikit-query-0.2/scikit_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-06 11:40:03.000000 scikit-query-0.2/scikit_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-06 11:40:03.000000 scikit-query-0.2/scikit_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:40:03.000000 scikit-query-0.2/scikit_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:40:03.000000 scikit-query-0.2/scikit_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-06 11:40:03.000000 scikit-query-0.2/scikit_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 11:40:03.000000 scikit-query-0.2/scikit_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:40:03.462624 scikit-query-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-06 11:39:21.000000 scikit-query-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:40:03.462624 scikit-query-0.2/skquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:40:03.462624 scikit-query-0.2/skquery/oracle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/oracle/MLCLOracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/oracle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:40:03.462624 scikit-query-0.2/skquery/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/pairwise/AIPC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/pairwise/FFQS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/pairwise/MinMax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/pairwise/NPU.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/pairwise/Pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/pairwise/RandomMLCL.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/pairwise/SASC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:40:03.462624 scikit-query-0.2/skquery/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:40:03.462624 scikit-query-0.2/skquery/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/utils/BaseSVDD.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 11:39:21.000000 scikit-query-0.2/skquery/utils/__init__.py
```

### Comparing `scikit-query-0.1.1/LICENSE` & `scikit-query-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-query-0.1.1/PKG-INFO` & `scikit-query-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-query
-Version: 0.1.1
+Version: 0.2
 Summary: scikit-query is a Python library for active query strategies in constrained clustering on top of SciPy and scikit-learn.
 Home-page: https://github.com/aymericb213/scikit-query
 Author: Aymeric Beauchamp
 Author-email: aymeric.beauchamp@univ-orleans.fr
 License: BSD 3-Clause License
 Keywords: active clustering,semi-supervised clustering,constrained clustering,pattern recognition,machine learning,artificial intelligence
 Classifier: Intended Audience :: Science/Research
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/scikit-query/badge/?version=latest)](https://scikit-query.readthedocs.io/en/latest/?badge=latest)
 [![version](https://img.shields.io/pypi/v/scikit-query)](https://pypi.org/project/scikit-query)
 [![Python](https://img.shields.io/pypi/pyversions/scikit-query)]()
 [![codecov](https://codecov.io/github/aymericb213/scikit-query/branch/main/graph/badge.svg?token=ZU4OEZKSP9)](https://codecov.io/github/aymericb213/scikit-query)
 [![license](https://img.shields.io/pypi/l/scikit-query)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Downloads](https://static.pepy.tech/badge/scikit-query)](https://pepy.tech/project/scikit-query)
 
 # scikit-query
@@ -53,15 +54,15 @@
 constraints = qs.fit(dataset, oracle)
 ```
 
 ## Constraints
 
 **Must-link** and **cannot-link** (ML/CL) constraints, also referred to as pairwise constraints,
 establish a relation between two data points : they must be in the same cluster (must-link)
-or in separate clusters (cannot-link).
+or in separate clusters (cannot-link). These are most widely studied constraints for clustering.
 
 ## Algorithms
 
 | Algorithm       | Description                            | Constraint type | Works in incremental setting ? | Source                                                                                  | Date |
 |-----------------|----------------------------------------|-----------------|--------------------------------|-----------------------------------------------------------------------------------------|------|
 | Random sampling |                                        | ML/CL           | :heavy_check_mark:             |                                                                                         |      |
 | FFQS            | Neighborhood-based                     | ML/CL           | :heavy_check_mark:             | [Basu et al.](https://epubs.siam.org/doi/10.1137/1.9781611972740.31)                    | 2004   |
@@ -80,10 +81,10 @@
 - cvxopt>=1.3.1
 - scikit-fuzzy>=0.4.2
 - scipy>=1.10.1
 - plotly>=5.14.1
 
 ## Contributors
 
-FFQS, MinMax and NPU are based off the original implementation of Jakub Švehla and changed for library consistency. 
+FFQS, MinMax and NPU are based upon Jakub Švehla's implementation. 
 Other algorithms have been implemented by Aymeric Beauchamp or his students from the University of Orléans :
 - Salma Badri, Elis Ishimwe, Brice Jacquesson, Matthéo Pailler (2023)
```

### Comparing `scikit-query-0.1.1/README.md` & `scikit-query-0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,305 +1,315 @@
-00000000: 5b21 5b76 6572 7369 6f6e 5d28 6874 7470  [![version](http
-00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000020: 696f 2f70 7970 692f 762f 7363 696b 6974  io/pypi/v/scikit
-00000030: 2d71 7565 7279 295d 2868 7474 7073 3a2f  -query)](https:/
-00000040: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000050: 742f 7363 696b 6974 2d71 7565 7279 290a  t/scikit-query).
-00000060: 5b21 5b50 7974 686f 6e5d 2868 7474 7073  [![Python](https
-00000070: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000080: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
-00000090: 732f 7363 696b 6974 2d71 7565 7279 295d  s/scikit-query)]
-000000a0: 2829 0a5b 215b 636f 6465 636f 765d 2868  ().[![codecov](h
-000000b0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-000000c0: 6f2f 6769 7468 7562 2f61 796d 6572 6963  o/github/aymeric
-000000d0: 6232 3133 2f73 6369 6b69 742d 7175 6572  b213/scikit-quer
-000000e0: 792f 6272 616e 6368 2f6d 6169 6e2f 6772  y/branch/main/gr
-000000f0: 6170 682f 6261 6467 652e 7376 673f 746f  aph/badge.svg?to
-00000100: 6b65 6e3d 5a55 344f 455a 4b53 5039 295d  ken=ZU4OEZKSP9)]
-00000110: 2868 7474 7073 3a2f 2f63 6f64 6563 6f76  (https://codecov
-00000120: 2e69 6f2f 6769 7468 7562 2f61 796d 6572  .io/github/aymer
-00000130: 6963 6232 3133 2f73 6369 6b69 742d 7175  icb213/scikit-qu
-00000140: 6572 7929 0a5b 215b 6c69 6365 6e73 655d  ery).[![license]
-00000150: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000160: 656c 6473 2e69 6f2f 7079 7069 2f6c 2f73  elds.io/pypi/l/s
-00000170: 6369 6b69 742d 7175 6572 7929 5d28 6874  cikit-query)](ht
-00000180: 7470 733a 2f2f 6368 6f6f 7365 616c 6963  tps://choosealic
-00000190: 656e 7365 2e63 6f6d 2f6c 6963 656e 7365  ense.com/license
-000001a0: 732f 6273 642d 332d 636c 6175 7365 290a  s/bsd-3-clause).
-000001b0: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
-000001c0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
-000001d0: 792e 7465 6368 2f62 6164 6765 2f73 6369  y.tech/badge/sci
-000001e0: 6b69 742d 7175 6572 7929 5d28 6874 7470  kit-query)](http
-000001f0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
-00000200: 6f6a 6563 742f 7363 696b 6974 2d71 7565  oject/scikit-que
-00000210: 7279 290a 0a23 2073 6369 6b69 742d 7175  ry)..# scikit-qu
-00000220: 6572 790a 0a43 6c75 7374 6572 696e 6720  ery..Clustering 
-00000230: 6169 6d73 2074 6f20 6772 6f75 7020 6461  aims to group da
-00000240: 7461 2069 6e74 6f20 636c 7573 7465 7273  ta into clusters
-00000250: 2077 6974 686f 7574 2074 6865 2068 656c   without the hel
-00000260: 7020 6f66 206c 6162 656c 732c 2075 6e6c  p of labels, unl
-00000270: 696b 6520 636c 6173 7369 6669 6361 7469  ike classificati
-00000280: 6f6e 2061 6c67 6f72 6974 686d 732e 200a  on algorithms. .
-00000290: 4120 7765 6c6c 2d6b 6e6f 776e 2073 686f  A well-known sho
-000002a0: 7274 636f 6d69 6e67 206f 6620 636c 7573  rtcoming of clus
-000002b0: 7465 7269 6e67 2061 6c67 6f72 6974 686d  tering algorithm
-000002c0: 7320 6973 2074 6861 7420 7468 6579 2072  s is that they r
-000002d0: 656c 7920 6f6e 2061 6e20 6f62 6a65 6374  ely on an object
-000002e0: 6976 6520 6675 6e63 7469 6f6e 2067 6561  ive function gea
-000002f0: 7265 6420 746f 7761 7264 200a 7370 6563  red toward .spec
-00000300: 6966 6963 2074 7970 6573 206f 6620 636c  ific types of cl
-00000310: 7573 7465 7273 2028 636f 6e76 6578 2c20  usters (convex, 
-00000320: 6465 6e73 652c 2077 656c 6c2d 7365 7061  dense, well-sepa
-00000330: 7261 7465 6429 2c20 616e 6420 6879 7065  rated), and hype
-00000340: 7270 6172 616d 6574 6572 7320 7468 6174  rparameters that
-00000350: 2061 7265 2068 6172 6420 746f 2074 756e   are hard to tun
-00000360: 652e 0a53 656d 692d 7375 7065 7276 6973  e..Semi-supervis
-00000370: 6564 2063 6c75 7374 6572 696e 6720 6d69  ed clustering mi
-00000380: 7469 6761 7465 7320 7468 6573 6520 7072  tigates these pr
-00000390: 6f62 6c65 6d73 2062 7920 696e 6a65 6374  oblems by inject
-000003a0: 696e 6720 6261 636b 6772 6f75 6e64 206b  ing background k
-000003b0: 6e6f 776c 6564 6765 2069 6e20 6f72 6465  nowledge in orde
-000003c0: 7220 746f 2067 7569 6465 2074 6865 2063  r to guide the c
-000003d0: 6c75 7374 6572 696e 672e 0a41 6374 6976  lustering..Activ
-000003e0: 6520 636c 7573 7465 7269 6e67 2061 6c67  e clustering alg
-000003f0: 6f72 6974 686d 7320 616e 616c 797a 6520  orithms analyze 
-00000400: 7468 6520 6461 7461 2074 6f20 7365 6c65  the data to sele
-00000410: 6374 2069 6e74 6572 6573 7469 6e67 2070  ct interesting p
-00000420: 6f69 6e74 7320 746f 2061 736b 2074 6865  oints to ask the
-00000430: 2075 7365 7220 6162 6f75 742c 2067 656e   user about, gen
-00000440: 6572 6174 696e 6720 636f 6e73 7472 6169  erating constrai
-00000450: 6e74 730a 7468 6174 2061 6c6c 6f77 2066  nts.that allow f
-00000460: 6173 7420 636f 6e76 6572 6765 6e63 6520  ast convergence 
-00000470: 746f 7761 7264 7320 6120 7573 6572 2d73  towards a user-s
-00000480: 7065 6369 6669 6564 2070 6172 7469 7469  pecified partiti
-00000490: 6f6e 2e0a 0a2a 2a73 6369 6b69 742d 7175  on...**scikit-qu
-000004a0: 6572 792a 2a20 6973 2061 206c 6962 7261  ery** is a libra
-000004b0: 7279 206f 6620 6163 7469 7665 2071 7565  ry of active que
-000004c0: 7279 2073 7472 6174 6567 6965 7320 666f  ry strategies fo
-000004d0: 7220 636f 6e73 7472 6169 6e65 6420 636c  r constrained cl
-000004e0: 7573 7465 7269 6e67 2069 6e73 7069 7265  ustering inspire
-000004f0: 6420 6279 205b 7363 696b 6974 2d6c 6561  d by [scikit-lea
-00000500: 726e 5d28 6874 7470 733a 2f2f 7363 696b  rn](https://scik
-00000510: 6974 2d6c 6561 726e 2e6f 7267 290a 616e  it-learn.org).an
-00000520: 6420 7468 6520 6e6f 7720 696e 6163 7469  d the now inacti
-00000530: 7665 205b 6163 7469 7665 2d73 656d 692d  ve [active-semi-
-00000540: 7375 7065 7276 6973 6564 2d63 6c75 7374  supervised-clust
-00000550: 6572 696e 675d 2868 7474 7073 3a2f 2f67  ering](https://g
-00000560: 6974 6875 622e 636f 6d2f 6461 7461 6d6f  ithub.com/datamo
-00000570: 6c65 2d61 692f 6163 7469 7665 2d73 656d  le-ai/active-sem
-00000580: 692d 7375 7065 7276 6973 6564 2d63 6c75  i-supervised-clu
-00000590: 7374 6572 696e 6729 206c 6962 7261 7279  stering) library
-000005a0: 2062 7920 4a61 6b75 6220 c5a0 7665 686c   by Jakub ..vehl
-000005b0: 612e 0a0a 4974 2069 7320 666f 6375 7365  a...It is focuse
-000005c0: 6420 6f6e 2061 6c67 6f72 6974 686d 2d61  d on algorithm-a
-000005d0: 676e 6f73 7469 6320 7175 6572 7920 7374  gnostic query st
-000005e0: 7261 7465 6769 6573 2c20 0a69 2e65 2e20  rategies, .i.e. 
-000005f0: 6d65 7468 6f64 7320 7468 6174 2064 6f20  methods that do 
-00000600: 6e6f 7420 7265 6c79 206f 6e20 6120 7061  not rely on a pa
-00000610: 7274 6963 756c 6172 2063 6c75 7374 6572  rticular cluster
-00000620: 696e 6720 616c 676f 7269 7468 6d2e 200a  ing algorithm. .
-00000630: 4672 6f6d 2061 6e20 696e 7075 7420 6461  From an input da
-00000640: 7461 7365 742c 2074 6865 7920 7072 6f64  taset, they prod
-00000650: 7563 6520 6120 7365 7420 6f66 2063 6f6e  uce a set of con
-00000660: 7374 7261 696e 7473 2062 7920 6d61 6b69  straints by maki
-00000670: 6e67 2069 6e73 6967 6874 6675 6c20 7175  ng insightful qu
-00000680: 6572 6965 7320 746f 2061 6e20 6f72 6163  eries to an orac
-00000690: 6c65 2e0a 4120 7661 7269 616e 7420 666f  le..A variant fo
-000006a0: 7220 696e 6372 656d 656e 7461 6c20 636f  r incremental co
-000006b0: 6e73 7472 6169 6e65 6420 636c 7573 7465  nstrained cluste
-000006c0: 7269 6e67 2069 7320 7072 6f76 6964 6564  ring is provided
-000006d0: 2066 6f72 2061 7070 6c69 6361 626c 6520   for applicable 
-000006e0: 616c 676f 7269 7468 6d73 2c0a 7461 6b69  algorithms,.taki
-000006f0: 6e67 2061 2064 6174 6120 7061 7274 6974  ng a data partit
-00000700: 696f 6e20 696e 746f 2061 6363 6f75 6e74  ion into account
-00000710: 2e20 0a0a 496e 2074 7970 6963 616c 202a  . ..In typical *
-00000720: 7363 696b 6974 2a20 7761 792c 2074 6865  scikit* way, the
-00000730: 206c 6962 7261 7279 2069 7320 7573 6564   library is used
-00000740: 2062 7920 696e 7374 616e 6369 6174 696e   by instanciatin
-00000750: 6720 6120 636c 6173 7320 616e 6420 7573  g a class and us
-00000760: 696e 6720 6974 7320 2a66 6974 2a20 6d65  ing its *fit* me
-00000770: 7468 6f64 2e0a 0a60 6060 2070 7974 686f  thod...``` pytho
-00000780: 6e0a 6672 6f6d 2073 6b71 7565 7279 2e70  n.from skquery.p
-00000790: 6169 7277 6973 6520 696d 706f 7274 2041  airwise import A
-000007a0: 4950 430a 6672 6f6d 2073 6b71 7565 7279  IPC.from skquery
-000007b0: 2e6f 7261 636c 6520 696d 706f 7274 204d  .oracle import M
-000007c0: 4c43 4c4f 7261 636c 650a 0a71 7320 3d20  LCLOracle..qs = 
-000007d0: 4149 5043 2829 0a6f 7261 636c 6520 3d20  AIPC().oracle = 
-000007e0: 4d4c 434c 4f72 6163 6c65 2874 7275 7468  MLCLOracle(truth
-000007f0: 3d6c 6162 656c 732c 2062 7564 6765 743d  =labels, budget=
-00000800: 3130 290a 636f 6e73 7472 6169 6e74 7320  10).constraints 
-00000810: 3d20 7173 2e66 6974 2864 6174 6173 6574  = qs.fit(dataset
-00000820: 2c20 6f72 6163 6c65 290a 6060 600a 0a23  , oracle).```..#
-00000830: 2320 436f 6e73 7472 6169 6e74 730a 0a2a  # Constraints..*
-00000840: 2a4d 7573 742d 6c69 6e6b 2a2a 2061 6e64  *Must-link** and
-00000850: 202a 2a63 616e 6e6f 742d 6c69 6e6b 2a2a   **cannot-link**
-00000860: 2028 4d4c 2f43 4c29 2063 6f6e 7374 7261   (ML/CL) constra
-00000870: 696e 7473 2c20 616c 736f 2072 6566 6572  ints, also refer
-00000880: 7265 6420 746f 2061 7320 7061 6972 7769  red to as pairwi
-00000890: 7365 2063 6f6e 7374 7261 696e 7473 2c0a  se constraints,.
-000008a0: 6573 7461 626c 6973 6820 6120 7265 6c61  establish a rela
-000008b0: 7469 6f6e 2062 6574 7765 656e 2074 776f  tion between two
-000008c0: 2064 6174 6120 706f 696e 7473 203a 2074   data points : t
-000008d0: 6865 7920 6d75 7374 2062 6520 696e 2074  hey must be in t
-000008e0: 6865 2073 616d 6520 636c 7573 7465 7220  he same cluster 
-000008f0: 286d 7573 742d 6c69 6e6b 290a 6f72 2069  (must-link).or i
-00000900: 6e20 7365 7061 7261 7465 2063 6c75 7374  n separate clust
-00000910: 6572 7320 2863 616e 6e6f 742d 6c69 6e6b  ers (cannot-link
-00000920: 292e 0a0a 2323 2041 6c67 6f72 6974 686d  )...## Algorithm
-00000930: 730a 0a7c 2041 6c67 6f72 6974 686d 2020  s..| Algorithm  
-00000940: 2020 2020 207c 2044 6573 6372 6970 7469       | Descripti
-00000950: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
-00000960: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000970: 436f 6e73 7472 6169 6e74 2074 7970 6520  Constraint type 
-00000980: 7c20 576f 726b 7320 696e 2069 6e63 7265  | Works in incre
-00000990: 6d65 6e74 616c 2073 6574 7469 6e67 203f  mental setting ?
-000009a0: 207c 2053 6f75 7263 6520 2020 2020 2020   | Source       
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 2020 2020 2020 2020 2020 207c 2044 6174             | Dat
-00000a00: 6520 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  e |.|-----------
-00000a10: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00000a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a50: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-00000a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a70: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
-00000a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
-00000ad0: 2d2d 2d7c 0a7c 2052 616e 646f 6d20 7361  ---|.| Random sa
-00000ae0: 6d70 6c69 6e67 207c 2020 2020 2020 2020  mpling |        
-00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b10: 7c20 4d4c 2f43 4c20 2020 2020 2020 2020  | ML/CL         
-00000b20: 2020 7c20 3a68 6561 7679 5f63 6865 636b    | :heavy_check
-00000b30: 5f6d 6172 6b3a 2020 2020 2020 2020 2020  _mark:          
-00000b40: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00000ba0: 2020 2020 7c0a 7c20 4646 5153 2020 2020      |.| FFQS    
-00000bb0: 2020 2020 2020 2020 7c20 4e65 6967 6862          | Neighb
-00000bc0: 6f72 686f 6f64 2d62 6173 6564 2020 2020  orhood-based    
+00000000: 5b21 5b44 6f63 756d 656e 7461 7469 6f6e  [![Documentation
+00000010: 2053 7461 7475 735d 2868 7474 7073 3a2f   Status](https:/
+00000020: 2f72 6561 6474 6865 646f 6373 2e6f 7267  /readthedocs.org
+00000030: 2f70 726f 6a65 6374 732f 7363 696b 6974  /projects/scikit
+00000040: 2d71 7565 7279 2f62 6164 6765 2f3f 7665  -query/badge/?ve
+00000050: 7273 696f 6e3d 6c61 7465 7374 295d 2868  rsion=latest)](h
+00000060: 7474 7073 3a2f 2f73 6369 6b69 742d 7175  ttps://scikit-qu
+00000070: 6572 792e 7265 6164 7468 6564 6f63 732e  ery.readthedocs.
+00000080: 696f 2f65 6e2f 6c61 7465 7374 2f3f 6261  io/en/latest/?ba
+00000090: 6467 653d 6c61 7465 7374 290a 5b21 5b76  dge=latest).[![v
+000000a0: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
+000000b0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+000000c0: 7970 692f 762f 7363 696b 6974 2d71 7565  ypi/v/scikit-que
+000000d0: 7279 295d 2868 7474 7073 3a2f 2f70 7970  ry)](https://pyp
+000000e0: 692e 6f72 672f 7072 6f6a 6563 742f 7363  i.org/project/sc
+000000f0: 696b 6974 2d71 7565 7279 290a 5b21 5b50  ikit-query).[![P
+00000100: 7974 686f 6e5d 2868 7474 7073 3a2f 2f69  ython](https://i
+00000110: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000120: 7069 2f70 7976 6572 7369 6f6e 732f 7363  pi/pyversions/sc
+00000130: 696b 6974 2d71 7565 7279 295d 2829 0a5b  ikit-query)]().[
+00000140: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
+00000150: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6769  ://codecov.io/gi
+00000160: 7468 7562 2f61 796d 6572 6963 6232 3133  thub/aymericb213
+00000170: 2f73 6369 6b69 742d 7175 6572 792f 6272  /scikit-query/br
+00000180: 616e 6368 2f6d 6169 6e2f 6772 6170 682f  anch/main/graph/
+00000190: 6261 6467 652e 7376 673f 746f 6b65 6e3d  badge.svg?token=
+000001a0: 5a55 344f 455a 4b53 5039 295d 2868 7474  ZU4OEZKSP9)](htt
+000001b0: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
+000001c0: 6769 7468 7562 2f61 796d 6572 6963 6232  github/aymericb2
+000001d0: 3133 2f73 6369 6b69 742d 7175 6572 7929  13/scikit-query)
+000001e0: 0a5b 215b 6c69 6365 6e73 655d 2868 7474  .[![license](htt
+000001f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000200: 2e69 6f2f 7079 7069 2f6c 2f73 6369 6b69  .io/pypi/l/sciki
+00000210: 742d 7175 6572 7929 5d28 6874 7470 733a  t-query)](https:
+00000220: 2f2f 6368 6f6f 7365 616c 6963 656e 7365  //choosealicense
+00000230: 2e63 6f6d 2f6c 6963 656e 7365 732f 6273  .com/licenses/bs
+00000240: 642d 332d 636c 6175 7365 290a 5b21 5b44  d-3-clause).[![D
+00000250: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+00000260: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
+00000270: 6368 2f62 6164 6765 2f73 6369 6b69 742d  ch/badge/scikit-
+00000280: 7175 6572 7929 5d28 6874 7470 733a 2f2f  query)](https://
+00000290: 7065 7079 2e74 6563 682f 7072 6f6a 6563  pepy.tech/projec
+000002a0: 742f 7363 696b 6974 2d71 7565 7279 290a  t/scikit-query).
+000002b0: 0a23 2073 6369 6b69 742d 7175 6572 790a  .# scikit-query.
+000002c0: 0a43 6c75 7374 6572 696e 6720 6169 6d73  .Clustering aims
+000002d0: 2074 6f20 6772 6f75 7020 6461 7461 2069   to group data i
+000002e0: 6e74 6f20 636c 7573 7465 7273 2077 6974  nto clusters wit
+000002f0: 686f 7574 2074 6865 2068 656c 7020 6f66  hout the help of
+00000300: 206c 6162 656c 732c 2075 6e6c 696b 6520   labels, unlike 
+00000310: 636c 6173 7369 6669 6361 7469 6f6e 2061  classification a
+00000320: 6c67 6f72 6974 686d 732e 200a 4120 7765  lgorithms. .A we
+00000330: 6c6c 2d6b 6e6f 776e 2073 686f 7274 636f  ll-known shortco
+00000340: 6d69 6e67 206f 6620 636c 7573 7465 7269  ming of clusteri
+00000350: 6e67 2061 6c67 6f72 6974 686d 7320 6973  ng algorithms is
+00000360: 2074 6861 7420 7468 6579 2072 656c 7920   that they rely 
+00000370: 6f6e 2061 6e20 6f62 6a65 6374 6976 6520  on an objective 
+00000380: 6675 6e63 7469 6f6e 2067 6561 7265 6420  function geared 
+00000390: 746f 7761 7264 200a 7370 6563 6966 6963  toward .specific
+000003a0: 2074 7970 6573 206f 6620 636c 7573 7465   types of cluste
+000003b0: 7273 2028 636f 6e76 6578 2c20 6465 6e73  rs (convex, dens
+000003c0: 652c 2077 656c 6c2d 7365 7061 7261 7465  e, well-separate
+000003d0: 6429 2c20 616e 6420 6879 7065 7270 6172  d), and hyperpar
+000003e0: 616d 6574 6572 7320 7468 6174 2061 7265  ameters that are
+000003f0: 2068 6172 6420 746f 2074 756e 652e 0a53   hard to tune..S
+00000400: 656d 692d 7375 7065 7276 6973 6564 2063  emi-supervised c
+00000410: 6c75 7374 6572 696e 6720 6d69 7469 6761  lustering mitiga
+00000420: 7465 7320 7468 6573 6520 7072 6f62 6c65  tes these proble
+00000430: 6d73 2062 7920 696e 6a65 6374 696e 6720  ms by injecting 
+00000440: 6261 636b 6772 6f75 6e64 206b 6e6f 776c  background knowl
+00000450: 6564 6765 2069 6e20 6f72 6465 7220 746f  edge in order to
+00000460: 2067 7569 6465 2074 6865 2063 6c75 7374   guide the clust
+00000470: 6572 696e 672e 0a41 6374 6976 6520 636c  ering..Active cl
+00000480: 7573 7465 7269 6e67 2061 6c67 6f72 6974  ustering algorit
+00000490: 686d 7320 616e 616c 797a 6520 7468 6520  hms analyze the 
+000004a0: 6461 7461 2074 6f20 7365 6c65 6374 2069  data to select i
+000004b0: 6e74 6572 6573 7469 6e67 2070 6f69 6e74  nteresting point
+000004c0: 7320 746f 2061 736b 2074 6865 2075 7365  s to ask the use
+000004d0: 7220 6162 6f75 742c 2067 656e 6572 6174  r about, generat
+000004e0: 696e 6720 636f 6e73 7472 6169 6e74 730a  ing constraints.
+000004f0: 7468 6174 2061 6c6c 6f77 2066 6173 7420  that allow fast 
+00000500: 636f 6e76 6572 6765 6e63 6520 746f 7761  convergence towa
+00000510: 7264 7320 6120 7573 6572 2d73 7065 6369  rds a user-speci
+00000520: 6669 6564 2070 6172 7469 7469 6f6e 2e0a  fied partition..
+00000530: 0a2a 2a73 6369 6b69 742d 7175 6572 792a  .**scikit-query*
+00000540: 2a20 6973 2061 206c 6962 7261 7279 206f  * is a library o
+00000550: 6620 6163 7469 7665 2071 7565 7279 2073  f active query s
+00000560: 7472 6174 6567 6965 7320 666f 7220 636f  trategies for co
+00000570: 6e73 7472 6169 6e65 6420 636c 7573 7465  nstrained cluste
+00000580: 7269 6e67 2069 6e73 7069 7265 6420 6279  ring inspired by
+00000590: 205b 7363 696b 6974 2d6c 6561 726e 5d28   [scikit-learn](
+000005a0: 6874 7470 733a 2f2f 7363 696b 6974 2d6c  https://scikit-l
+000005b0: 6561 726e 2e6f 7267 290a 616e 6420 7468  earn.org).and th
+000005c0: 6520 6e6f 7720 696e 6163 7469 7665 205b  e now inactive [
+000005d0: 6163 7469 7665 2d73 656d 692d 7375 7065  active-semi-supe
+000005e0: 7276 6973 6564 2d63 6c75 7374 6572 696e  rvised-clusterin
+000005f0: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
+00000600: 622e 636f 6d2f 6461 7461 6d6f 6c65 2d61  b.com/datamole-a
+00000610: 692f 6163 7469 7665 2d73 656d 692d 7375  i/active-semi-su
+00000620: 7065 7276 6973 6564 2d63 6c75 7374 6572  pervised-cluster
+00000630: 696e 6729 206c 6962 7261 7279 2062 7920  ing) library by 
+00000640: 4a61 6b75 6220 c5a0 7665 686c 612e 0a0a  Jakub ..vehla...
+00000650: 4974 2069 7320 666f 6375 7365 6420 6f6e  It is focused on
+00000660: 2061 6c67 6f72 6974 686d 2d61 676e 6f73   algorithm-agnos
+00000670: 7469 6320 7175 6572 7920 7374 7261 7465  tic query strate
+00000680: 6769 6573 2c20 0a69 2e65 2e20 6d65 7468  gies, .i.e. meth
+00000690: 6f64 7320 7468 6174 2064 6f20 6e6f 7420  ods that do not 
+000006a0: 7265 6c79 206f 6e20 6120 7061 7274 6963  rely on a partic
+000006b0: 756c 6172 2063 6c75 7374 6572 696e 6720  ular clustering 
+000006c0: 616c 676f 7269 7468 6d2e 200a 4672 6f6d  algorithm. .From
+000006d0: 2061 6e20 696e 7075 7420 6461 7461 7365   an input datase
+000006e0: 742c 2074 6865 7920 7072 6f64 7563 6520  t, they produce 
+000006f0: 6120 7365 7420 6f66 2063 6f6e 7374 7261  a set of constra
+00000700: 696e 7473 2062 7920 6d61 6b69 6e67 2069  ints by making i
+00000710: 6e73 6967 6874 6675 6c20 7175 6572 6965  nsightful querie
+00000720: 7320 746f 2061 6e20 6f72 6163 6c65 2e0a  s to an oracle..
+00000730: 4120 7661 7269 616e 7420 666f 7220 696e  A variant for in
+00000740: 6372 656d 656e 7461 6c20 636f 6e73 7472  cremental constr
+00000750: 6169 6e65 6420 636c 7573 7465 7269 6e67  ained clustering
+00000760: 2069 7320 7072 6f76 6964 6564 2066 6f72   is provided for
+00000770: 2061 7070 6c69 6361 626c 6520 616c 676f   applicable algo
+00000780: 7269 7468 6d73 2c0a 7461 6b69 6e67 2061  rithms,.taking a
+00000790: 2064 6174 6120 7061 7274 6974 696f 6e20   data partition 
+000007a0: 696e 746f 2061 6363 6f75 6e74 2e20 0a0a  into account. ..
+000007b0: 496e 2074 7970 6963 616c 202a 7363 696b  In typical *scik
+000007c0: 6974 2a20 7761 792c 2074 6865 206c 6962  it* way, the lib
+000007d0: 7261 7279 2069 7320 7573 6564 2062 7920  rary is used by 
+000007e0: 696e 7374 616e 6369 6174 696e 6720 6120  instanciating a 
+000007f0: 636c 6173 7320 616e 6420 7573 696e 6720  class and using 
+00000800: 6974 7320 2a66 6974 2a20 6d65 7468 6f64  its *fit* method
+00000810: 2e0a 0a60 6060 2070 7974 686f 6e0a 6672  ...``` python.fr
+00000820: 6f6d 2073 6b71 7565 7279 2e70 6169 7277  om skquery.pairw
+00000830: 6973 6520 696d 706f 7274 2041 4950 430a  ise import AIPC.
+00000840: 6672 6f6d 2073 6b71 7565 7279 2e6f 7261  from skquery.ora
+00000850: 636c 6520 696d 706f 7274 204d 4c43 4c4f  cle import MLCLO
+00000860: 7261 636c 650a 0a71 7320 3d20 4149 5043  racle..qs = AIPC
+00000870: 2829 0a6f 7261 636c 6520 3d20 4d4c 434c  ().oracle = MLCL
+00000880: 4f72 6163 6c65 2874 7275 7468 3d6c 6162  Oracle(truth=lab
+00000890: 656c 732c 2062 7564 6765 743d 3130 290a  els, budget=10).
+000008a0: 636f 6e73 7472 6169 6e74 7320 3d20 7173  constraints = qs
+000008b0: 2e66 6974 2864 6174 6173 6574 2c20 6f72  .fit(dataset, or
+000008c0: 6163 6c65 290a 6060 600a 0a23 2320 436f  acle).```..## Co
+000008d0: 6e73 7472 6169 6e74 730a 0a2a 2a4d 7573  nstraints..**Mus
+000008e0: 742d 6c69 6e6b 2a2a 2061 6e64 202a 2a63  t-link** and **c
+000008f0: 616e 6e6f 742d 6c69 6e6b 2a2a 2028 4d4c  annot-link** (ML
+00000900: 2f43 4c29 2063 6f6e 7374 7261 696e 7473  /CL) constraints
+00000910: 2c20 616c 736f 2072 6566 6572 7265 6420  , also referred 
+00000920: 746f 2061 7320 7061 6972 7769 7365 2063  to as pairwise c
+00000930: 6f6e 7374 7261 696e 7473 2c0a 6573 7461  onstraints,.esta
+00000940: 626c 6973 6820 6120 7265 6c61 7469 6f6e  blish a relation
+00000950: 2062 6574 7765 656e 2074 776f 2064 6174   between two dat
+00000960: 6120 706f 696e 7473 203a 2074 6865 7920  a points : they 
+00000970: 6d75 7374 2062 6520 696e 2074 6865 2073  must be in the s
+00000980: 616d 6520 636c 7573 7465 7220 286d 7573  ame cluster (mus
+00000990: 742d 6c69 6e6b 290a 6f72 2069 6e20 7365  t-link).or in se
+000009a0: 7061 7261 7465 2063 6c75 7374 6572 7320  parate clusters 
+000009b0: 2863 616e 6e6f 742d 6c69 6e6b 292e 2054  (cannot-link). T
+000009c0: 6865 7365 2061 7265 206d 6f73 7420 7769  hese are most wi
+000009d0: 6465 6c79 2073 7475 6469 6564 2063 6f6e  dely studied con
+000009e0: 7374 7261 696e 7473 2066 6f72 2063 6c75  straints for clu
+000009f0: 7374 6572 696e 672e 0a0a 2323 2041 6c67  stering...## Alg
+00000a00: 6f72 6974 686d 730a 0a7c 2041 6c67 6f72  orithms..| Algor
+00000a10: 6974 686d 2020 2020 2020 207c 2044 6573  ithm       | Des
+00000a20: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
+00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a40: 2020 2020 7c20 436f 6e73 7472 6169 6e74      | Constraint
+00000a50: 2074 7970 6520 7c20 576f 726b 7320 696e   type | Works in
+00000a60: 2069 6e63 7265 6d65 6e74 616c 2073 6574   incremental set
+00000a70: 7469 6e67 203f 207c 2053 6f75 7263 6520  ting ? | Source 
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ad0: 207c 2044 6174 6520 7c0a 7c2d 2d2d 2d2d   | Date |.|-----
+00000ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+00000af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b10: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+00000b20: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00000b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b40: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ba0: 2d2d 7c2d 2d2d 2d2d 2d7c 0a7c 2052 616e  --|------|.| Ran
+00000bb0: 646f 6d20 7361 6d70 6c69 6e67 207c 2020  dom sampling |  
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 207c 204d 4c2f 434c 2020 2020 2020 2020   | ML/CL        
-00000bf0: 2020 207c 203a 6865 6176 795f 6368 6563     | :heavy_chec
-00000c00: 6b5f 6d61 726b 3a20 2020 2020 2020 2020  k_mark:         
-00000c10: 2020 2020 7c20 5b42 6173 7520 6574 2061      | [Basu et a
-00000c20: 6c2e 5d28 6874 7470 733a 2f2f 6570 7562  l.](https://epub
-00000c30: 732e 7369 616d 2e6f 7267 2f64 6f69 2f31  s.siam.org/doi/1
-00000c40: 302e 3131 3337 2f31 2e39 3738 3136 3131  0.1137/1.9781611
-00000c50: 3937 3237 3430 2e33 3129 2020 2020 2020  972740.31)      
-00000c60: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000c70: 3230 3034 2020 207c 0a7c 204d 4d46 4651  2004   |.| MMFFQ
-00000c80: 5320 284d 696e 4d61 7829 207c 204e 6569  S (MinMax) | Nei
-00000c90: 6768 626f 7268 6f6f 642d 6261 7365 642c  ghborhood-based,
-00000ca0: 2073 696d 696c 6172 6974 7920 2020 2020   similarity     
-00000cb0: 2020 2020 7c20 4d4c 2f43 4c20 2020 2020      | ML/CL     
-00000cc0: 2020 2020 2020 7c20 3a68 6561 7679 5f63        | :heavy_c
-00000cd0: 6865 636b 5f6d 6172 6b3a 2020 2020 2020  heck_mark:      
-00000ce0: 2020 2020 2020 207c 205b 4d61 6c6c 6170         | [Mallap
-00000cf0: 7261 6761 6461 2065 7420 616c 2e5d 2868  ragada et al.](h
-00000d00: 7474 7073 3a2f 2f69 6565 6578 706c 6f72  ttps://ieeexplor
-00000d10: 652e 6965 6565 2e6f 7267 2f64 6f63 756d  e.ieee.org/docum
-00000d20: 656e 742f 3437 3631 3739 3229 2020 2020  ent/4761792)    
+00000be0: 2020 2020 2020 7c20 4d4c 2f43 4c20 2020        | ML/CL   
+00000bf0: 2020 2020 2020 2020 7c20 3a68 6561 7679          | :heavy
+00000c00: 5f63 6865 636b 5f6d 6172 6b3a 2020 2020  _check_mark:    
+00000c10: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c70: 2020 207c 2020 2020 2020 7c0a 7c20 4646     |      |.| FF
+00000c80: 5153 2020 2020 2020 2020 2020 2020 7c20  QS            | 
+00000c90: 4e65 6967 6862 6f72 686f 6f64 2d62 6173  Neighborhood-bas
+00000ca0: 6564 2020 2020 2020 2020 2020 2020 2020  ed              
+00000cb0: 2020 2020 2020 207c 204d 4c2f 434c 2020         | ML/CL  
+00000cc0: 2020 2020 2020 2020 207c 203a 6865 6176           | :heav
+00000cd0: 795f 6368 6563 6b5f 6d61 726b 3a20 2020  y_check_mark:   
+00000ce0: 2020 2020 2020 2020 2020 7c20 5b42 6173            | [Bas
+00000cf0: 7520 6574 2061 6c2e 5d28 6874 7470 733a  u et al.](https:
+00000d00: 2f2f 6570 7562 732e 7369 616d 2e6f 7267  //epubs.siam.org
+00000d10: 2f64 6f69 2f31 302e 3131 3337 2f31 2e39  /doi/10.1137/1.9
+00000d20: 3738 3136 3131 3937 3237 3430 2e33 3129  781611972740.31)
 00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d40: 207c 2032 3030 3820 2020 2020 2020 2020   | 2008         
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 2020 2020 7c0a 7c20 4e50 5520          |.| NPU 
-00000d90: 2020 2020 2020 2020 2020 2020 7c20 4e65              | Ne
-00000da0: 6967 6862 6f72 686f 6f64 2d62 6173 6564  ighborhood-based
-00000db0: 2c20 696e 666f 726d 6174 696f 6e20 7468  , information th
-00000dc0: 656f 7279 207c 204d 4c2f 434c 2020 2020  eory | ML/CL    
-00000dd0: 2020 2020 2020 207c 203a 6865 6176 795f         | :heavy_
-00000de0: 6368 6563 6b5f 6d61 726b 3a20 2020 2020  check_mark:     
-00000df0: 2020 2020 2020 2020 7c20 5b58 696f 6e67          | [Xiong
-00000e00: 2065 7420 616c 2e5d 2868 7474 7073 3a2f   et al.](https:/
-00000e10: 2f64 6c2e 6163 6d2e 6f72 672f 646f 692f  /dl.acm.org/doi/
-00000e20: 3130 2e31 3130 392f 544b 4445 2e32 3031  10.1109/TKDE.201
-00000e30: 332e 3232 2920 2020 2020 2020 2020 2020  3.22)           
+00000d40: 2020 2020 7c20 3230 3034 2020 207c 0a7c      | 2004   |.|
+00000d50: 204d 4d46 4651 5320 284d 696e 4d61 7829   MMFFQS (MinMax)
+00000d60: 207c 204e 6569 6768 626f 7268 6f6f 642d   | Neighborhood-
+00000d70: 6261 7365 642c 2073 696d 696c 6172 6974  based, similarit
+00000d80: 7920 2020 2020 2020 2020 7c20 4d4c 2f43  y         | ML/C
+00000d90: 4c20 2020 2020 2020 2020 2020 7c20 3a68  L           | :h
+00000da0: 6561 7679 5f63 6865 636b 5f6d 6172 6b3a  eavy_check_mark:
+00000db0: 2020 2020 2020 2020 2020 2020 207c 205b               | [
+00000dc0: 4d61 6c6c 6170 7261 6761 6461 2065 7420  Mallapragada et 
+00000dd0: 616c 2e5d 2868 7474 7073 3a2f 2f69 6565  al.](https://iee
+00000de0: 6578 706c 6f72 652e 6965 6565 2e6f 7267  explore.ieee.org
+00000df0: 2f64 6f63 756d 656e 742f 3437 3631 3739  /document/476179
+00000e00: 3229 2020 2020 2020 2020 2020 2020 2020  2)              
+00000e10: 2020 2020 2020 207c 2032 3030 3820 2020         | 2008   
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 2020 7c20 3230 3133 2020 2020 2020 2020    | 2013        
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 2020 2020 2020 2020 207c 0a7c 2053 4153           |.| SAS
-00000ea0: 4320 2020 2020 2020 2020 2020 207c 2053  C            | S
-00000eb0: 5644 442c 2067 7265 6564 7920 6170 7072  VDD, greedy appr
-00000ec0: 6f61 6368 2020 2020 2020 2020 2020 2020  oach            
-00000ed0: 2020 2020 2020 7c20 4d4c 2f43 4c20 2020        | ML/CL   
-00000ee0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f00: 2020 2020 2020 2020 207c 205b 4162 696e           | [Abin
-00000f10: 2026 2042 6569 6779 5d28 6874 7470 733a   & Beigy](https:
-00000f20: 2f2f 7777 772e 7363 6965 6e63 6564 6972  //www.sciencedir
-00000f30: 6563 742e 636f 6d2f 7363 6965 6e63 652f  ect.com/science/
-00000f40: 6172 7469 636c 652f 6162 732f 7069 692f  article/abs/pii/
-00000f50: 5330 3033 3133 3230 3331 3330 3034 3036  S003132031300406
-00000f60: 3829 207c 2032 3031 3420 2020 2020 2020  8) | 2014       
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fa0: 2020 2020 2020 2020 2020 7c0a 7c20 4149            |.| AI
-00000fb0: 5043 2020 2020 2020 2020 2020 2020 7c20  PC            | 
-00000fc0: 4675 7a7a 7920 636c 7573 7465 7269 6e67  Fuzzy clustering
-00000fd0: 2c20 696e 666f 726d 6174 696f 6e20 7468  , information th
-00000fe0: 656f 7279 2020 207c 204d 4c2f 434c 2020  eory   | ML/CL  
-00000ff0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 2020 2020 2020 7c20 5b5a 6861            | [Zha
-00001020: 6e67 2065 7420 616c 2e5d 2868 7474 7073  ng et al.](https
-00001030: 3a2f 2f69 6565 6578 706c 6f72 652e 6965  ://ieeexplore.ie
-00001040: 6565 2e6f 7267 2f64 6f63 756d 656e 742f  ee.org/document/
-00001050: 3837 3430 3936 3029 2020 2020 2020 2020  8740960)        
+00000e50: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00000e60: 7c20 4e50 5520 2020 2020 2020 2020 2020  | NPU           
+00000e70: 2020 7c20 4e65 6967 6862 6f72 686f 6f64    | Neighborhood
+00000e80: 2d62 6173 6564 2c20 696e 666f 726d 6174  -based, informat
+00000e90: 696f 6e20 7468 656f 7279 207c 204d 4c2f  ion theory | ML/
+00000ea0: 434c 2020 2020 2020 2020 2020 207c 203a  CL           | :
+00000eb0: 6865 6176 795f 6368 6563 6b5f 6d61 726b  heavy_check_mark
+00000ec0: 3a20 2020 2020 2020 2020 2020 2020 7c20  :             | 
+00000ed0: 5b58 696f 6e67 2065 7420 616c 2e5d 2868  [Xiong et al.](h
+00000ee0: 7474 7073 3a2f 2f64 6c2e 6163 6d2e 6f72  ttps://dl.acm.or
+00000ef0: 672f 646f 692f 3130 2e31 3130 392f 544b  g/doi/10.1109/TK
+00000f00: 4445 2e32 3031 332e 3232 2920 2020 2020  DE.2013.22)     
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f20: 2020 2020 2020 2020 7c20 3230 3133 2020          | 2013  
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f60: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000f70: 0a7c 2053 4153 4320 2020 2020 2020 2020  .| SASC         
+00000f80: 2020 207c 2053 5644 442c 2067 7265 6564     | SVDD, greed
+00000f90: 7920 6170 7072 6f61 6368 2020 2020 2020  y approach      
+00000fa0: 2020 2020 2020 2020 2020 2020 7c20 4d4c              | ML
+00000fb0: 2f43 4c20 2020 2020 2020 2020 2020 7c20  /CL           | 
+00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000fe0: 205b 4162 696e 2026 2042 6569 6779 5d28   [Abin & Beigy](
+00000ff0: 6874 7470 733a 2f2f 7777 772e 7363 6965  https://www.scie
+00001000: 6e63 6564 6972 6563 742e 636f 6d2f 7363  ncedirect.com/sc
+00001010: 6965 6e63 652f 6172 7469 636c 652f 6162  ience/article/ab
+00001020: 732f 7069 692f 5330 3033 3133 3230 3331  s/pii/S003132031
+00001030: 3330 3034 3036 3829 207c 2032 3031 3420  3004068) | 2014 
+00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 2020 2020 7c20 3230 3139 2020 2020 2020      | 2019      
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010c0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-000010d0: 0a23 2320 4465 7065 6e64 656e 6369 6573  .## Dependencies
-000010e0: 0a0a 7363 696b 6974 2d71 7565 7279 2069  ..scikit-query i
-000010f0: 7320 6465 7665 6c6f 7065 6420 6f6e 2050  s developed on P
-00001100: 7974 686f 6e20 3e3d 2033 2e31 302c 2061  ython >= 3.10, a
-00001110: 6e64 2072 6571 7569 7265 7320 7468 6520  nd requires the 
-00001120: 666f 6c6c 6f77 696e 6720 6c69 6272 6172  following librar
-00001130: 6965 7320 3a0a 2d20 7061 6e64 6173 3e3d  ies :.- pandas>=
-00001140: 322e 302e 310a 2d20 6d61 7470 6c6f 746c  2.0.1.- matplotl
-00001150: 6962 3e3d 332e 372e 310a 2d20 6e75 6d70  ib>=3.7.1.- nump
-00001160: 793e 3d31 2e32 342e 330a 2d20 7363 696b  y>=1.24.3.- scik
-00001170: 6974 2d6c 6561 726e 3e3d 312e 322e 320a  it-learn>=1.2.2.
-00001180: 2d20 6376 786f 7074 3e3d 312e 332e 310a  - cvxopt>=1.3.1.
-00001190: 2d20 7363 696b 6974 2d66 757a 7a79 3e3d  - scikit-fuzzy>=
-000011a0: 302e 342e 320a 2d20 7363 6970 793e 3d31  0.4.2.- scipy>=1
-000011b0: 2e31 302e 310a 2d20 706c 6f74 6c79 3e3d  .10.1.- plotly>=
-000011c0: 352e 3134 2e31 0a0a 2323 2043 6f6e 7472  5.14.1..## Contr
-000011d0: 6962 7574 6f72 730a 0a46 4651 532c 204d  ibutors..FFQS, M
-000011e0: 696e 4d61 7820 616e 6420 4e50 5520 6172  inMax and NPU ar
-000011f0: 6520 6261 7365 6420 6f66 6620 7468 6520  e based off the 
-00001200: 6f72 6967 696e 616c 2069 6d70 6c65 6d65  original impleme
-00001210: 6e74 6174 696f 6e20 6f66 204a 616b 7562  ntation of Jakub
-00001220: 20c5 a076 6568 6c61 2061 6e64 2063 6861   ..vehla and cha
-00001230: 6e67 6564 2066 6f72 206c 6962 7261 7279  nged for library
-00001240: 2063 6f6e 7369 7374 656e 6379 2e20 0a4f   consistency. .O
-00001250: 7468 6572 2061 6c67 6f72 6974 686d 7320  ther algorithms 
-00001260: 6861 7665 2062 6565 6e20 696d 706c 656d  have been implem
-00001270: 656e 7465 6420 6279 2041 796d 6572 6963  ented by Aymeric
-00001280: 2042 6561 7563 6861 6d70 206f 7220 6869   Beauchamp or hi
-00001290: 7320 7374 7564 656e 7473 2066 726f 6d20  s students from 
-000012a0: 7468 6520 556e 6976 6572 7369 7479 206f  the University o
-000012b0: 6620 4f72 6cc3 a961 6e73 203a 0a2d 2053  f Orl..ans :.- S
-000012c0: 616c 6d61 2042 6164 7269 2c20 456c 6973  alma Badri, Elis
-000012d0: 2049 7368 696d 7765 2c20 4272 6963 6520   Ishimwe, Brice 
-000012e0: 4a61 6371 7565 7373 6f6e 2c20 4d61 7474  Jacquesson, Matt
-000012f0: 68c3 a96f 2050 6169 6c6c 6572 2028 3230  h..o Pailler (20
-00001300: 3233 29                                  23)
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 7c0a 7c20 4149 5043 2020 2020 2020 2020  |.| AIPC        
+00001090: 2020 2020 7c20 4675 7a7a 7920 636c 7573      | Fuzzy clus
+000010a0: 7465 7269 6e67 2c20 696e 666f 726d 6174  tering, informat
+000010b0: 696f 6e20 7468 656f 7279 2020 207c 204d  ion theory   | M
+000010c0: 4c2f 434c 2020 2020 2020 2020 2020 207c  L/CL           |
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010f0: 7c20 5b5a 6861 6e67 2065 7420 616c 2e5d  | [Zhang et al.]
+00001100: 2868 7474 7073 3a2f 2f69 6565 6578 706c  (https://ieeexpl
+00001110: 6f72 652e 6965 6565 2e6f 7267 2f64 6f63  ore.ieee.org/doc
+00001120: 756d 656e 742f 3837 3430 3936 3029 2020  ument/8740960)  
+00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001140: 2020 2020 2020 2020 2020 7c20 3230 3139            | 2019
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011a0: 2020 2020 7c0a 0a23 2320 4465 7065 6e64      |..## Depend
+000011b0: 656e 6369 6573 0a0a 7363 696b 6974 2d71  encies..scikit-q
+000011c0: 7565 7279 2069 7320 6465 7665 6c6f 7065  uery is develope
+000011d0: 6420 6f6e 2050 7974 686f 6e20 3e3d 2033  d on Python >= 3
+000011e0: 2e31 302c 2061 6e64 2072 6571 7569 7265  .10, and require
+000011f0: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+00001200: 6c69 6272 6172 6965 7320 3a0a 2d20 7061  libraries :.- pa
+00001210: 6e64 6173 3e3d 322e 302e 310a 2d20 6d61  ndas>=2.0.1.- ma
+00001220: 7470 6c6f 746c 6962 3e3d 332e 372e 310a  tplotlib>=3.7.1.
+00001230: 2d20 6e75 6d70 793e 3d31 2e32 342e 330a  - numpy>=1.24.3.
+00001240: 2d20 7363 696b 6974 2d6c 6561 726e 3e3d  - scikit-learn>=
+00001250: 312e 322e 320a 2d20 6376 786f 7074 3e3d  1.2.2.- cvxopt>=
+00001260: 312e 332e 310a 2d20 7363 696b 6974 2d66  1.3.1.- scikit-f
+00001270: 757a 7a79 3e3d 302e 342e 320a 2d20 7363  uzzy>=0.4.2.- sc
+00001280: 6970 793e 3d31 2e31 302e 310a 2d20 706c  ipy>=1.10.1.- pl
+00001290: 6f74 6c79 3e3d 352e 3134 2e31 0a0a 2323  otly>=5.14.1..##
+000012a0: 2043 6f6e 7472 6962 7574 6f72 730a 0a46   Contributors..F
+000012b0: 4651 532c 204d 696e 4d61 7820 616e 6420  FQS, MinMax and 
+000012c0: 4e50 5520 6172 6520 6261 7365 6420 7570  NPU are based up
+000012d0: 6f6e 204a 616b 7562 20c5 a076 6568 6c61  on Jakub ..vehla
+000012e0: 2773 2069 6d70 6c65 6d65 6e74 6174 696f  's implementatio
+000012f0: 6e2e 200a 4f74 6865 7220 616c 676f 7269  n. .Other algori
+00001300: 7468 6d73 2068 6176 6520 6265 656e 2069  thms have been i
+00001310: 6d70 6c65 6d65 6e74 6564 2062 7920 4179  mplemented by Ay
+00001320: 6d65 7269 6320 4265 6175 6368 616d 7020  meric Beauchamp 
+00001330: 6f72 2068 6973 2073 7475 6465 6e74 7320  or his students 
+00001340: 6672 6f6d 2074 6865 2055 6e69 7665 7273  from the Univers
+00001350: 6974 7920 6f66 204f 726c c3a9 616e 7320  ity of Orl..ans 
+00001360: 3a0a 2d20 5361 6c6d 6120 4261 6472 692c  :.- Salma Badri,
+00001370: 2045 6c69 7320 4973 6869 6d77 652c 2042   Elis Ishimwe, B
+00001380: 7269 6365 204a 6163 7175 6573 736f 6e2c  rice Jacquesson,
+00001390: 204d 6174 7468 c3a9 6f20 5061 696c 6c65   Matth..o Paille
+000013a0: 7220 2832 3032 3329                      r (2023)
```

### Comparing `scikit-query-0.1.1/scikit_query.egg-info/PKG-INFO` & `scikit-query-0.2/scikit_query.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-query
-Version: 0.1.1
+Version: 0.2
 Summary: scikit-query is a Python library for active query strategies in constrained clustering on top of SciPy and scikit-learn.
 Home-page: https://github.com/aymericb213/scikit-query
 Author: Aymeric Beauchamp
 Author-email: aymeric.beauchamp@univ-orleans.fr
 License: BSD 3-Clause License
 Keywords: active clustering,semi-supervised clustering,constrained clustering,pattern recognition,machine learning,artificial intelligence
 Classifier: Intended Audience :: Science/Research
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/scikit-query/badge/?version=latest)](https://scikit-query.readthedocs.io/en/latest/?badge=latest)
 [![version](https://img.shields.io/pypi/v/scikit-query)](https://pypi.org/project/scikit-query)
 [![Python](https://img.shields.io/pypi/pyversions/scikit-query)]()
 [![codecov](https://codecov.io/github/aymericb213/scikit-query/branch/main/graph/badge.svg?token=ZU4OEZKSP9)](https://codecov.io/github/aymericb213/scikit-query)
 [![license](https://img.shields.io/pypi/l/scikit-query)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Downloads](https://static.pepy.tech/badge/scikit-query)](https://pepy.tech/project/scikit-query)
 
 # scikit-query
@@ -53,15 +54,15 @@
 constraints = qs.fit(dataset, oracle)
 ```
 
 ## Constraints
 
 **Must-link** and **cannot-link** (ML/CL) constraints, also referred to as pairwise constraints,
 establish a relation between two data points : they must be in the same cluster (must-link)
-or in separate clusters (cannot-link).
+or in separate clusters (cannot-link). These are most widely studied constraints for clustering.
 
 ## Algorithms
 
 | Algorithm       | Description                            | Constraint type | Works in incremental setting ? | Source                                                                                  | Date |
 |-----------------|----------------------------------------|-----------------|--------------------------------|-----------------------------------------------------------------------------------------|------|
 | Random sampling |                                        | ML/CL           | :heavy_check_mark:             |                                                                                         |      |
 | FFQS            | Neighborhood-based                     | ML/CL           | :heavy_check_mark:             | [Basu et al.](https://epubs.siam.org/doi/10.1137/1.9781611972740.31)                    | 2004   |
@@ -80,10 +81,10 @@
 - cvxopt>=1.3.1
 - scikit-fuzzy>=0.4.2
 - scipy>=1.10.1
 - plotly>=5.14.1
 
 ## Contributors
 
-FFQS, MinMax and NPU are based off the original implementation of Jakub Švehla and changed for library consistency. 
+FFQS, MinMax and NPU are based upon Jakub Švehla's implementation. 
 Other algorithms have been implemented by Aymeric Beauchamp or his students from the University of Orléans :
 - Salma Badri, Elis Ishimwe, Brice Jacquesson, Matthéo Pailler (2023)
```

### Comparing `scikit-query-0.1.1/scikit_query.egg-info/SOURCES.txt` & `scikit-query-0.2/scikit_query.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,9 +19,8 @@
 skquery/pairwise/Pairwise.py
 skquery/pairwise/RandomMLCL.py
 skquery/pairwise/SASC.py
 skquery/pairwise/__init__.py
 skquery/tests/__init__.py
 skquery/tests/test_query.py
 skquery/utils/BaseSVDD.py
-skquery/utils/__init__.py
-skquery/utils/line_intercept.py
+skquery/utils/__init__.py
```

### Comparing `scikit-query-0.1.1/setup.py` & `scikit-query-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-query-0.1.1/skquery/pairwise/Pairwise.py` & `scikit-query-0.2/skquery/pairwise/Pairwise.py`

 * *Files identical despite different names*

### Comparing `scikit-query-0.1.1/skquery/tests/test_query.py` & `scikit-query-0.2/skquery/tests/test_query.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,99 +7,131 @@
 00000060: 7175 6572 792e 6f72 6163 6c65 2069 6d70  query.oracle imp
 00000070: 6f72 7420 4d4c 434c 4f72 6163 6c65 0a66  ort MLCLOracle.f
 00000080: 726f 6d20 6163 7469 7665 5f73 656d 695f  rom active_semi_
 00000090: 636c 7573 7465 7269 6e67 2069 6d70 6f72  clustering impor
 000000a0: 7420 434f 504b 4d65 616e 730a 6672 6f6d  t COPKMeans.from
 000000b0: 2074 696d 6520 696d 706f 7274 2074 696d   time import tim
 000000c0: 650a 6672 6f6d 2074 7164 6d20 696d 706f  e.from tqdm impo
-000000d0: 7274 2074 7164 6d0a 7472 793a 0a20 2020  rt tqdm.try:.   
-000000e0: 2066 726f 6d20 736b 6c65 6172 6e65 7820   from sklearnex 
-000000f0: 696d 706f 7274 2070 6174 6368 5f73 6b6c  import patch_skl
-00000100: 6561 726e 0a20 2020 2070 6174 6368 5f73  earn.    patch_s
-00000110: 6b6c 6561 726e 2829 0a65 7863 6570 7420  klearn().except 
-00000120: 4d6f 6475 6c65 4e6f 7446 6f75 6e64 4572  ModuleNotFoundEr
-00000130: 726f 723a 0a20 2020 2070 6173 730a 6672  ror:.    pass.fr
-00000140: 6f6d 2073 6b6c 6561 726e 2e63 6c75 7374  om sklearn.clust
-00000150: 6572 2069 6d70 6f72 7420 4b4d 6561 6e73  er import KMeans
-00000160: 0a0a 0a64 6566 2074 6573 745f 7175 6572  ...def test_quer
-00000170: 7928 293a 0a20 2020 2064 6174 6173 6574  y():.    dataset
-00000180: 203d 2063 6c75 7374 6265 6e63 682e 6c6f   = clustbench.lo
-00000190: 6164 5f64 6174 6173 6574 2822 6663 7073  ad_dataset("fcps
-000001a0: 222c 2022 6c73 756e 222c 2070 6174 683d  ", "lsun", path=
-000001b0: 2263 6c75 7374 6572 696e 672d 6461 7461  "clustering-data
-000001c0: 2d76 3122 290a 2020 2020 6c61 6265 6c73  -v1").    labels
-000001d0: 203d 2064 6174 6173 6574 2e6c 6162 656c   = dataset.label
-000001e0: 735b 305d 202d 2031 2020 2320 636f 7272  s[0] - 1  # corr
-000001f0: 6573 706f 6e64 616e 6365 2062 6574 7765  espondance betwe
-00000200: 656e 2063 6c75 7374 6265 6e63 6820 616e  en clustbench an
-00000210: 6420 5079 7468 6f6e 2069 6e64 6578 696e  d Python indexin
-00000220: 670a 0a20 2020 2023 2054 6573 7420 616c  g..    # Test al
-00000230: 6c20 696d 706c 656d 656e 7465 6420 616c  l implemented al
-00000240: 676f 7269 7468 6d73 0a20 2020 2066 6f72  gorithms.    for
-00000250: 2073 7472 6174 2069 6e20 7471 646d 285b   strat in tqdm([
-00000260: 5261 6e64 6f6d 4d4c 434c 2c20 4646 5153  RandomMLCL, FFQS
-00000270: 2c20 4d69 6e4d 6178 2c20 4e50 552c 2041  , MinMax, NPU, A
-00000280: 4950 432c 2053 4153 435d 293a 0a20 2020  IPC, SASC]):.   
-00000290: 2020 2020 2071 7320 3d20 7374 7261 7428       qs = strat(
-000002a0: 290a 2020 2020 2020 2020 6966 2073 7472  ).        if str
-000002b0: 6174 203d 3d20 4e50 553a 0a20 2020 2020  at == NPU:.     
-000002c0: 2020 2020 2020 2071 7320 3d20 7374 7261         qs = stra
-000002d0: 7428 636c 7573 7465 7265 723d 434f 504b  t(clusterer=COPK
-000002e0: 4d65 616e 7328 6e5f 636c 7573 7465 7273  Means(n_clusters
-000002f0: 3d64 6174 6173 6574 2e6e 5f63 6c75 7374  =dataset.n_clust
-00000300: 6572 735b 305d 2929 0a20 2020 2020 2020  ers[0])).       
-00000310: 2074 3120 3d20 7469 6d65 2829 0a20 2020   t1 = time().   
-00000320: 2020 2020 2063 6f6e 7374 7261 696e 7473       constraints
-00000330: 203d 2071 732e 6669 7428 6461 7461 7365   = qs.fit(datase
-00000340: 742e 6461 7461 2c20 4d4c 434c 4f72 6163  t.data, MLCLOrac
-00000350: 6c65 2874 7275 7468 3d6c 6162 656c 7329  le(truth=labels)
-00000360: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000370: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00000380: 5f63 6c75 7374 6572 733d 6461 7461 7365  _clusters=datase
-00000390: 742e 6e5f 636c 7573 7465 7273 5b30 5d29  t.n_clusters[0])
-000003a0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-000003b0: 225c 6e7b 7374 7261 742e 5f5f 6e61 6d65  "\n{strat.__name
-000003c0: 5f5f 7d20 3a20 7b74 696d 6528 2920 2d20  __} : {time() - 
-000003d0: 7431 7d20 7322 290a 2020 2020 2020 2020  t1} s").        
-000003e0: 6173 7365 7274 206c 656e 2863 6f6e 7374  assert len(const
-000003f0: 7261 696e 7473 2920 3e20 300a 0a20 2020  raints) > 0..   
-00000400: 2023 2054 6573 7420 616c 6c20 696d 706c   # Test all impl
-00000410: 656d 656e 7465 6420 616c 676f 7269 7468  emented algorith
-00000420: 6d73 0a20 2020 2066 6f72 2073 7472 6174  ms.    for strat
-00000430: 2069 6e20 7471 646d 285b 4646 5153 2c20   in tqdm([FFQS, 
-00000440: 4d69 6e4d 6178 2c20 4e50 555d 293a 0a20  MinMax, NPU]):. 
-00000450: 2020 2020 2020 2063 6f6e 7374 7261 696e         constrain
-00000460: 7473 203d 207b 226d 6c22 3a20 5b5d 2c20  ts = {"ml": [], 
-00000470: 2263 6c22 3a20 5b5d 7d0a 2020 2020 2020  "cl": []}.      
-00000480: 2020 6e62 6864 7320 3d20 4e6f 6e65 0a20    nbhds = None. 
-00000490: 2020 2020 2020 2074 3120 3d20 7469 6d65         t1 = time
-000004a0: 2829 0a20 2020 2020 2020 2066 6f72 2069  ().        for i
-000004b0: 2069 6e20 7261 6e67 6528 3229 3a0a 2020   in range(2):.  
-000004c0: 2020 2020 2020 2020 2020 616c 676f 203d            algo =
-000004d0: 2043 4f50 4b4d 6561 6e73 286e 5f63 6c75   COPKMeans(n_clu
-000004e0: 7374 6572 733d 6461 7461 7365 742e 6e5f  sters=dataset.n_
-000004f0: 636c 7573 7465 7273 5b30 5d29 0a20 2020  clusters[0]).   
-00000500: 2020 2020 2020 2020 2061 6c67 6f2e 6669           algo.fi
-00000510: 7428 6461 7461 7365 742e 6461 7461 2c20  t(dataset.data, 
-00000520: 6d6c 3d63 6f6e 7374 7261 696e 7473 5b22  ml=constraints["
-00000530: 6d6c 225d 2c20 636c 3d63 6f6e 7374 7261  ml"], cl=constra
-00000540: 696e 7473 5b22 636c 225d 290a 0a20 2020  ints["cl"])..   
-00000550: 2020 2020 2020 2020 2071 7320 3d20 7374           qs = st
-00000560: 7261 7428 6e65 6967 6862 6f72 686f 6f64  rat(neighborhood
-00000570: 733d 6e62 6864 7329 0a0a 2020 2020 2020  s=nbhds)..      
-00000580: 2020 2020 2020 636f 6e73 7472 6169 6e74        constraint
-00000590: 7320 3d20 7173 2e66 6974 2864 6174 6173  s = qs.fit(datas
-000005a0: 6574 2e64 6174 612c 204d 4c43 4c4f 7261  et.data, MLCLOra
-000005b0: 636c 6528 7472 7574 683d 6c61 6265 6c73  cle(truth=labels
-000005c0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 2020 2020 7061 7274 6974 696f 6e3d 616c      partition=al
-000005f0: 676f 2e6c 6162 656c 735f 290a 2020 2020  go.labels_).    
-00000600: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
-00000610: 656e 2863 6f6e 7374 7261 696e 7473 2920  en(constraints) 
-00000620: 3e20 300a 2020 2020 2020 2020 2020 2020  > 0.            
-00000630: 6e62 6864 7320 3d20 7173 2e6e 6569 6768  nbhds = qs.neigh
-00000640: 626f 7268 6f6f 6473 0a20 2020 2020 2020  borhoods.       
-00000650: 2070 7269 6e74 2866 225c 6e7b 7374 7261   print(f"\n{stra
-00000660: 742e 5f5f 6e61 6d65 5f5f 7d20 696e 6372  t.__name__} incr
-00000670: 656d 656e 7461 6c20 3a20 7b74 696d 6528  emental : {time(
-00000680: 2920 2d20 7431 7d20 7322 290a            ) - t1} s").
+000000d0: 7274 2074 7164 6d0a 0a0a 6465 6620 7465  rt tqdm...def te
+000000e0: 7374 5f71 7565 7279 2829 3a0a 2020 2020  st_query():.    
+000000f0: 616c 676f 7269 7468 6d73 203d 205b 5261  algorithms = [Ra
+00000100: 6e64 6f6d 4d4c 434c 2c20 4646 5153 2c20  ndomMLCL, FFQS, 
+00000110: 4d69 6e4d 6178 2c20 4e50 552c 2041 4950  MinMax, NPU, AIP
+00000120: 432c 2053 4153 435d 0a20 2020 2069 6e63  C, SASC].    inc
+00000130: 725f 616c 676f 7320 3d20 5b52 616e 646f  r_algos = [Rando
+00000140: 6d4d 4c43 4c2c 2046 4651 532c 204d 696e  mMLCL, FFQS, Min
+00000150: 4d61 782c 204e 5055 5d0a 0a20 2020 2064  Max, NPU]..    d
+00000160: 6174 6173 6574 203d 2063 6c75 7374 6265  ataset = clustbe
+00000170: 6e63 682e 6c6f 6164 5f64 6174 6173 6574  nch.load_dataset
+00000180: 2822 6f74 6865 7222 2c20 2269 7269 7322  ("other", "iris"
+00000190: 2c20 7061 7468 3d22 636c 7573 7465 7269  , path="clusteri
+000001a0: 6e67 2d64 6174 612d 7631 2229 0a20 2020  ng-data-v1").   
+000001b0: 206c 6162 656c 7320 3d20 6461 7461 7365   labels = datase
+000001c0: 742e 6c61 6265 6c73 5b30 5d20 2d20 3120  t.labels[0] - 1 
+000001d0: 2023 2063 6f72 7265 7370 6f6e 6461 6e63   # correspondanc
+000001e0: 6520 6265 7477 6565 6e20 636c 7573 7462  e between clustb
+000001f0: 656e 6368 2061 6e64 2050 7974 686f 6e20  ench and Python 
+00000200: 696e 6465 7869 6e67 0a0a 2020 2020 6275  indexing..    bu
+00000210: 6467 6574 203d 2031 300a 2020 2020 2320  dget = 10.    # 
+00000220: 5465 7374 2061 6c6c 2069 6d70 6c65 6d65  Test all impleme
+00000230: 6e74 6564 2061 6c67 6f72 6974 686d 730a  nted algorithms.
+00000240: 2020 2020 666f 7220 7374 7261 7420 696e      for strat in
+00000250: 2074 7164 6d28 616c 676f 7269 7468 6d73   tqdm(algorithms
+00000260: 293a 0a20 2020 2020 2020 2071 7320 3d20  ):.        qs = 
+00000270: 7374 7261 7428 290a 2020 2020 2020 2020  strat().        
+00000280: 6966 2073 7472 6174 203d 3d20 4e50 553a  if strat == NPU:
+00000290: 0a20 2020 2020 2020 2020 2020 2071 7320  .            qs 
+000002a0: 3d20 7374 7261 7428 6363 5f61 6c67 3d43  = strat(cc_alg=C
+000002b0: 4f50 4b4d 6561 6e73 286e 5f63 6c75 7374  OPKMeans(n_clust
+000002c0: 6572 733d 6461 7461 7365 742e 6e5f 636c  ers=dataset.n_cl
+000002d0: 7573 7465 7273 5b30 5d29 290a 2020 2020  usters[0])).    
+000002e0: 2020 2020 7431 203d 2074 696d 6528 290a      t1 = time().
+000002f0: 2020 2020 2020 2020 636f 6e73 7472 6169          constrai
+00000300: 6e74 7320 3d20 7173 2e66 6974 2864 6174  nts = qs.fit(dat
+00000310: 6173 6574 2e64 6174 612c 204d 4c43 4c4f  aset.data, MLCLO
+00000320: 7261 636c 6528 7472 7574 683d 6c61 6265  racle(truth=labe
+00000330: 6c73 2c20 6275 6467 6574 3d62 7564 6765  ls, budget=budge
+00000340: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+00000350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000360: 206e 5f63 6c75 7374 6572 733d 6461 7461   n_clusters=data
+00000370: 7365 742e 6e5f 636c 7573 7465 7273 5b30  set.n_clusters[0
+00000380: 5d29 0a20 2020 2020 2020 2023 7173 2e63  ]).        #qs.c
+00000390: 7374 735f 746f 5f66 696c 6528 636f 6e73  sts_to_file(cons
+000003a0: 7472 6169 6e74 7329 0a20 2020 2020 2020  traints).       
+000003b0: 2070 7269 6e74 2866 225c 6e7b 7374 7261   print(f"\n{stra
+000003c0: 742e 5f5f 6e61 6d65 5f5f 7d20 3a20 7b74  t.__name__} : {t
+000003d0: 696d 6528 2920 2d20 7431 7d20 7322 290a  ime() - t1} s").
+000003e0: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+000003f0: 656e 2863 6f6e 7374 7261 696e 7473 2920  en(constraints) 
+00000400: 3e20 300a 0a20 2020 2023 2054 6573 7473  > 0..    # Tests
+00000410: 2069 6e20 696e 6372 656d 656e 7461 6c20   in incremental 
+00000420: 7365 7474 696e 670a 2020 2020 6e5f 6974  setting.    n_it
+00000430: 6572 203d 2032 0a20 2020 2066 6f72 2073  er = 2.    for s
+00000440: 7472 6174 2069 6e20 7471 646d 2869 6e63  trat in tqdm(inc
+00000450: 725f 616c 676f 7329 3a0a 2020 2020 2020  r_algos):.      
+00000460: 2020 636f 6e73 7472 6169 6e74 7320 3d20    constraints = 
+00000470: 7b22 6d6c 223a 205b 5d2c 2022 636c 223a  {"ml": [], "cl":
+00000480: 205b 5d7d 0a20 2020 2020 2020 206e 6268   []}.        nbh
+00000490: 6473 203d 204e 6f6e 650a 2020 2020 2020  ds = None.      
+000004a0: 2020 7064 6973 7473 203d 204e 6f6e 650a    pdists = None.
+000004b0: 2020 2020 2020 2020 745f 7173 203d 205b          t_qs = [
+000004c0: 5d0a 2020 2020 2020 2020 666f 7220 6920  ].        for i 
+000004d0: 696e 2072 616e 6765 286e 5f69 7465 7229  in range(n_iter)
+000004e0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
+000004f0: 676f 203d 2043 4f50 4b4d 6561 6e73 286e  go = COPKMeans(n
+00000500: 5f63 6c75 7374 6572 733d 6461 7461 7365  _clusters=datase
+00000510: 742e 6e5f 636c 7573 7465 7273 5b30 5d29  t.n_clusters[0])
+00000520: 0a20 2020 2020 2020 2020 2020 2061 6c67  .            alg
+00000530: 6f2e 6669 7428 6461 7461 7365 742e 6461  o.fit(dataset.da
+00000540: 7461 2c20 6d6c 3d63 6f6e 7374 7261 696e  ta, ml=constrain
+00000550: 7473 5b22 6d6c 225d 2c20 636c 3d63 6f6e  ts["ml"], cl=con
+00000560: 7374 7261 696e 7473 5b22 636c 225d 290a  straints["cl"]).
+00000570: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000580: 7374 7261 7420 3d3d 2052 616e 646f 6d4d  strat == RandomM
+00000590: 4c43 4c3a 0a20 2020 2020 2020 2020 2020  LCL:.           
+000005a0: 2020 2020 2071 7320 3d20 7374 7261 7428       qs = strat(
+000005b0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+000005c0: 6966 2073 7472 6174 2069 6e20 5b46 4651  if strat in [FFQ
+000005d0: 532c 204d 696e 4d61 785d 3a0a 2020 2020  S, MinMax]:.    
+000005e0: 2020 2020 2020 2020 2020 2020 7173 203d              qs =
+000005f0: 2073 7472 6174 286e 6569 6768 626f 7268   strat(neighborh
+00000600: 6f6f 6473 3d6e 6268 6473 2c20 6469 7374  oods=nbhds, dist
+00000610: 616e 6365 733d 7064 6973 7473 290a 2020  ances=pdists).  
+00000620: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000640: 7173 203d 2073 7472 6174 286e 6569 6768  qs = strat(neigh
+00000650: 626f 7268 6f6f 6473 3d6e 6268 6473 290a  borhoods=nbhds).
+00000660: 2020 2020 2020 2020 2020 2020 7431 203d              t1 =
+00000670: 2074 696d 6528 290a 2020 2020 2020 2020   time().        
+00000680: 2020 2020 636f 6e73 7472 6169 6e74 7320      constraints 
+00000690: 3d20 7173 2e66 6974 2864 6174 6173 6574  = qs.fit(dataset
+000006a0: 2e64 6174 612c 204d 4c43 4c4f 7261 636c  .data, MLCLOracl
+000006b0: 6528 7472 7574 683d 6c61 6265 6c73 2c20  e(truth=labels, 
+000006c0: 6275 6467 6574 3d62 7564 6765 7429 2c0a  budget=budget),.
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006f0: 2070 6172 7469 7469 6f6e 3d61 6c67 6f2e   partition=algo.
+00000700: 6c61 6265 6c73 5f29 0a20 2020 2020 2020  labels_).       
+00000710: 2020 2020 2074 5f71 732e 6170 7065 6e64       t_qs.append
+00000720: 2874 696d 6528 2920 2d20 7431 290a 0a20  (time() - t1).. 
+00000730: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00000740: 7420 6c65 6e28 636f 6e73 7472 6169 6e74  t len(constraint
+00000750: 7329 203e 2030 0a20 2020 2020 2020 2020  s) > 0.         
+00000760: 2020 2069 6620 7374 7261 7420 696e 205b     if strat in [
+00000770: 4646 5153 2c20 4d69 6e4d 6178 2c20 4e50  FFQS, MinMax, NP
+00000780: 555d 3a0a 2020 2020 2020 2020 2020 2020  U]:.            
+00000790: 2020 2020 6e62 6864 7320 3d20 7173 2e6e      nbhds = qs.n
+000007a0: 6569 6768 626f 7268 6f6f 6473 0a20 2020  eighborhoods.   
+000007b0: 2020 2020 2020 2020 2069 6620 7374 7261           if stra
+000007c0: 7420 696e 205b 4646 5153 2c20 4d69 6e4d  t in [FFQS, MinM
+000007d0: 6178 5d3a 0a20 2020 2020 2020 2020 2020  ax]:.           
+000007e0: 2020 2020 2070 6469 7374 7320 3d20 7173       pdists = qs
+000007f0: 2e70 5f64 6973 7473 0a20 2020 2020 2020  .p_dists.       
+00000800: 2023 544f 444f 3a20 746f 6f20 6d75 6368   #TODO: too much
+00000810: 2063 6c75 7474 6572 2c20 6d61 6b65 2074   clutter, make t
+00000820: 6573 7473 2066 6f72 2065 6163 6820 616c  ests for each al
+00000830: 670a 2020 2020 2020 2020 7072 696e 7428  g.        print(
+00000840: 6622 5c6e 7b73 7472 6174 2e5f 5f6e 616d  f"\n{strat.__nam
+00000850: 655f 5f7d 2069 6e63 7265 6d65 6e74 616c  e__} incremental
+00000860: 203a 207b 7375 6d28 745f 7173 297d 2073   : {sum(t_qs)} s
+00000870: 2028 6272 6561 6b64 6f77 6e3a 207b 745f   (breakdown: {t_
+00000880: 7173 7d29 2229 0a                        qs})").
```

### Comparing `scikit-query-0.1.1/skquery/utils/BaseSVDD.py` & `scikit-query-0.2/skquery/utils/BaseSVDD.py`

 * *Files identical despite different names*

