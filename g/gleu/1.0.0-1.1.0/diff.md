# Comparing `tmp/gleu-1.0.0.tar.gz` & `tmp/gleu-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gleu-1.0.0.tar", last modified: Mon Jun 12 00:13:14 2023, max compression
+gzip compressed data, was "gleu-1.1.0.tar", last modified: Thu Jul  6 14:08:16 2023, max compression
```

## Comparing `gleu-1.0.0.tar` & `gleu-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 koyama.s  (1028) koyama.s  (1030)        0 2023-06-12 00:13:14.363696 gleu-1.0.0/
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1069 2023-06-11 23:36:14.000000 gleu-1.0.0/LICENSE
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      390 2023-06-12 00:13:14.363696 gleu-1.0.0/PKG-INFO
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     6757 2023-06-11 23:16:22.000000 gleu-1.0.0/README.md
-drwxrwxr-x   0 koyama.s  (1028) koyama.s  (1030)        0 2023-06-12 00:13:14.351696 gleu-1.0.0/gleu/
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)        0 2023-06-11 23:46:38.000000 gleu-1.0.0/gleu/__init__.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1239 2023-06-11 13:21:51.000000 gleu-1.0.0/gleu/accum.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1292 2023-06-11 13:22:03.000000 gleu-1.0.0/gleu/aggreg.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     2285 2023-06-11 13:19:25.000000 gleu-1.0.0/gleu/corpus_main.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      844 2023-06-11 11:09:18.000000 gleu-1.0.0/gleu/count.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1138 2023-06-11 11:09:52.000000 gleu-1.0.0/gleu/load.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     2077 2023-06-11 12:51:08.000000 gleu-1.0.0/gleu/main.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      523 2023-06-11 10:11:03.000000 gleu-1.0.0/gleu/ngram.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      593 2023-06-11 02:19:52.000000 gleu-1.0.0/gleu/result.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1953 2023-06-11 13:19:17.000000 gleu-1.0.0/gleu/score.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     2125 2023-06-11 13:20:06.000000 gleu-1.0.0/gleu/sent_main.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      858 2023-06-11 13:26:11.000000 gleu-1.0.0/gleu/util.py
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     2951 2023-06-11 13:19:03.000000 gleu-1.0.0/gleu/verbose.py
-drwxrwxr-x   0 koyama.s  (1028) koyama.s  (1030)        0 2023-06-12 00:13:14.363696 gleu-1.0.0/gleu.egg-info/
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      390 2023-06-12 00:13:14.000000 gleu-1.0.0/gleu.egg-info/PKG-INFO
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      392 2023-06-12 00:13:14.000000 gleu-1.0.0/gleu.egg-info/SOURCES.txt
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)        1 2023-06-12 00:13:14.000000 gleu-1.0.0/gleu.egg-info/dependency_links.txt
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)       40 2023-06-12 00:13:14.000000 gleu-1.0.0/gleu.egg-info/entry_points.txt
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)       18 2023-06-12 00:13:14.000000 gleu-1.0.0/gleu.egg-info/requires.txt
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)        5 2023-06-12 00:13:14.000000 gleu-1.0.0/gleu.egg-info/top_level.txt
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)       38 2023-06-12 00:13:14.363696 gleu-1.0.0/setup.cfg
--rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      824 2023-06-12 00:10:31.000000 gleu-1.0.0/setup.py
+drwxrwxr-x   0 koyama.s  (1028) koyama.s  (1030)        0 2023-07-06 14:08:16.393178 gleu-1.1.0/
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1069 2023-06-11 23:36:14.000000 gleu-1.1.0/LICENSE
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      390 2023-07-06 14:08:16.393178 gleu-1.1.0/PKG-INFO
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     7156 2023-07-06 13:20:53.000000 gleu-1.1.0/README.md
+drwxrwxr-x   0 koyama.s  (1028) koyama.s  (1030)        0 2023-07-06 14:08:16.377177 gleu-1.1.0/gleu/
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)        0 2023-06-11 23:46:38.000000 gleu-1.1.0/gleu/__init__.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      660 2023-06-13 05:40:12.000000 gleu-1.1.0/gleu/accum.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1229 2023-06-13 02:02:03.000000 gleu-1.1.0/gleu/aggreg.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     2251 2023-06-13 01:55:51.000000 gleu-1.1.0/gleu/corpus_main.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      844 2023-06-11 11:09:18.000000 gleu-1.1.0/gleu/count.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1118 2023-06-13 02:01:31.000000 gleu-1.1.0/gleu/load.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1909 2023-07-04 16:16:30.000000 gleu-1.1.0/gleu/main.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      681 2023-06-16 09:09:27.000000 gleu-1.1.0/gleu/ngram.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      593 2023-06-11 02:19:52.000000 gleu-1.1.0/gleu/result.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1885 2023-06-13 05:40:08.000000 gleu-1.1.0/gleu/score.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     2117 2023-06-13 01:55:25.000000 gleu-1.1.0/gleu/sent_main.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      858 2023-06-11 13:26:11.000000 gleu-1.1.0/gleu/util.py
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)     1879 2023-06-16 04:21:55.000000 gleu-1.1.0/gleu/verbose.py
+drwxrwxr-x   0 koyama.s  (1028) koyama.s  (1030)        0 2023-07-06 14:08:16.393178 gleu-1.1.0/gleu.egg-info/
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      390 2023-07-06 14:08:15.000000 gleu-1.1.0/gleu.egg-info/PKG-INFO
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      392 2023-07-06 14:08:15.000000 gleu-1.1.0/gleu.egg-info/SOURCES.txt
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)        1 2023-07-06 14:08:15.000000 gleu-1.1.0/gleu.egg-info/dependency_links.txt
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)       88 2023-07-06 14:08:15.000000 gleu-1.1.0/gleu.egg-info/entry_points.txt
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)       18 2023-07-06 14:08:15.000000 gleu-1.1.0/gleu.egg-info/requires.txt
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)        5 2023-07-06 14:08:15.000000 gleu-1.1.0/gleu.egg-info/top_level.txt
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)       38 2023-07-06 14:08:16.393178 gleu-1.1.0/setup.cfg
+-rw-rw-r--   0 koyama.s  (1028) koyama.s  (1030)      940 2023-07-06 13:21:20.000000 gleu-1.1.0/setup.py
```

### Comparing `gleu-1.0.0/LICENSE` & `gleu-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gleu-1.0.0/README.md` & `gleu-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -32,24 +32,28 @@
 
 $$ p_n = \cfrac{ \displaystyle \sum_i^{|D|} \max(0,  \sum_{g_n \in h_i} \min(\rho_{i,g_n}, \eta_{i, g_n}) - \min(\sigma_{i, g_n}^{\mathrm{diff}}, \eta_{i, g_n})) } {\displaystyle \sum_i^{|D|} \sum_{g_n \in h_i} \eta_{i, g_n} } $$
 
 https://github.com/shotakoyama/gleu/blob/d20b995be142ff40a7e342cfe8e866a1fce09073/ref/gleu.py#L95-L105
 
 These two formulae are not equivalent because the penalty terms differ. For example, let $(\sigma, \rho, \eta) = (2, 1, 3)$, $\max(0, \min(\sigma, \eta) - \min(\rho, \eta)) = 1$, while $\min(\sigma^{\mathrm{diff}}, \eta) = 0$.
 
+Furthermore, the equation above equals to the next equation. In our implementation, we adopted this.
+
+$$ p_n = \cfrac{ \displaystyle \sum_i^{|D|} \sum_{g_n \in h_i} \min(\rho_{i,g_n}, \eta_{i, g_n}) - \sum_i^{|D|} \min( \sum_{g_n \in h_i} \min(\sigma_{i, g_n}^{\mathrm{diff}}, \eta_{i,g_n}), \sum_{g_n \in h_i} \min(\rho_{i,g_n}, \eta_{i, g_n}) ) } {\displaystyle \sum_i^{|D|} \sum_{g_n \in h_i} \eta_{i, g_n} } $$
+
 # Usage
 
-You can install the code by running `pip install -e .` under the directry with `setup.py`.
+You can install the code by running `pip install -e .` under the directry with `setup.py`. `pip install gleu` is also OK.
 
 ## corpus-level GLEU
 
 Run the code below to get the same result as the original implementation. `-d` or `--digit` specifies the number of digits of decimal places. `-f` or `--fix-seed` is required to reproduce the original result.
 
 ```
-$ gleu corpus -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -d 4 -f
+$ gleu -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -d 4 -f
 AMU     58.3256
 CAMB    59.2553
 INPUT   56.6048
 REF0    81.8462
 ```
 
 This result equals to the original GLEU+ output.
@@ -61,31 +65,31 @@
 INPUT 0.566048
 REF0 0.818462
 ```
 
 `-p` is the number of process (default: 1). In my environment, `-p 8` is the fastest. `-n` is the number of the max size of n-gram (default: 4). `-i` is the number of iterations of reference sampling. `-t` specifies tokenization method (choices: `word` or `char`, default: `word`).
 
 ```
-$ gleu corpus -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -p 8 -n 6 -i 1000 -t char
+$ gleu -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -p 8 -n 6 -i 1000 -t char
 AMU     83.06
 CAMB    83.41
 INPUT   83.30
 REF0    92.22
 ```
 
 Although default mode samples from multiple refereces, max mode (`-m`) uses the best reference for each sentence.
 
 ```
-$ gleu corpus -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -p 8 -m
+$ gleu -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -p 8 -m
 AMU     68.81
 CAMB    68.55
 INPUT   68.34
 REF0    100.00
 
-$ gleu corpus -s INPUT -r REF0 REF1 -o AMU CAMB -p 8 -mv
+$ gleu -s INPUT -r REF0 REF1 -o AMU CAMB -p 8 -mv
 AMU
 +-------+-------+--------+-------+--------+-------+
 |       | numer | denom  |   p   |   bp   |  gleu |
 +-------+-------+--------+-------+--------+-------+
 |   1   | 26538 | 30362  | 87.41 | 100.00 | 87.41 |
 |   2   | 21521 | 29050  | 74.08 | 100.00 | 74.08 |
 |   3   | 17600 | 27739  | 63.45 | 100.00 | 63.45 |
@@ -103,44 +107,44 @@
 | total | 78864 | 111567 | 69.00 | 99.36 | 68.55 |
 +-------+-------+--------+-------+-------+-------+
 ```
 
 ## sentence-level GLEU
 
 ```
-$ gleu sent -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0
+$ sgleu -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0
 100.00  100.00  100.00  100.00
 100.00  0.00    100.00  100.00
 53.34   0.00    53.34   100.00
 0.00    67.53   0.00    100.00
 84.92   56.30   100.00  100.00
 100.00  80.96   100.00  100.00
 100.00  0.00    100.00  100.00
 92.93   92.93   92.93   92.93
 86.35   72.42   86.35   100.00
 26.93   0.00    0.00    69.62
 ...
 ```
 
 ```
-$ gleu sent -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -m
+$ sgleu -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -m
 100.00  100.00  100.00  100.00
 100.00  0.00    100.00  100.00
 53.34   0.00    53.34   100.00
 0.00    67.53   0.00    100.00
 84.92   56.30   100.00  100.00
 100.00  80.96   100.00  100.00
 100.00  0.00    100.00  100.00
 100.00  100.00  100.00  100.00
 86.35   72.42   86.35   100.00
 ...
 ```
 
 ```
-$ gleu sent -s INPUT -r REF0 REF1 -o AMU -v
+$ sgleu -s INPUT -r REF0 REF1 -o AMU -v
 S-1     Keeping the Secret of Genetic Testing
 H-1-1   Keeping the Secret of Genetic Testing
 R-1-1*  Keeping the Secret of Genetic Testing
 +-------+-------+-------+-------+-------+--------+--------+--------+
 |       | match | penal | numer | denom |   p    |   bp   |  gleu  |
 +-------+-------+-------+-------+-------+--------+--------+--------+
 |   1   |   6   |   0   |   6   |   6   | 100.00 | 100.00 | 100.00 |
@@ -161,20 +165,20 @@
 |   4   |   3   |   0   |   3   |   3   | 100.00 | 100.00 | 100.00 |
 | total |   18  |   0   |   18  |   18  | 100.00 | 100.00 | 100.00 |
 +-------+-------+-------+-------+-------+--------+--------+--------+
 ...
 ```
 
 ```
- $ gleu mean -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0
+ $ mgleu -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0
 AMU     54.12
 CAMB    54.33
 INPUT   50.67
 REF0    79.63
 
-$ gleu mean -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -m
+$ mgleu -s INPUT -r REF0 REF1 -o AMU CAMB INPUT REF0 -m
 AMU     66.70
 CAMB    65.55
 INPUT   64.53
 REF0    100.00
 ```
```

### Comparing `gleu-1.0.0/gleu/corpus_main.py` & `gleu-1.1.0/gleu/corpus_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 import numpy as np
 import random
 from multiprocessing import Pool
 from .load import load_hdrn_data
 from .score import (
-        drn_sent_accum_to_d_rmax,
-        drn_sent_accum_to_n_data_accum,
+        drn_accum_to_d_rmax,
+        drn_accum_to_n_accum,
         rindex_to_rhlen,
         n_accum_to_gleu)
 from .util import make_id_rindex
-from .verbose import CorpusNVerbose
+from .verbose import NVerbose
 from .result import simple_result, table_result
 
 
 def corpus_main(args):
     if args.max:
         corpus_max(args)
     else:
         corpus_sampling(args)
 
 
 def corpus_max(args):
-    _, _, _, dr_rlen, dh_hlen, hdrn_sacc = load_hdrn_data(args)
+    _, _, _, dr_rlen, dh_hlen, hdrn_accum = load_hdrn_data(args)
 
-    for h, drn_sacc in enumerate(hdrn_sacc):
+    for h, drn_accum in enumerate(hdrn_accum):
         d_hlen = dh_hlen[:, h]
-        d_rmax = drn_sent_accum_to_d_rmax(drn_sacc, dr_rlen, d_hlen)
-        n_dacc = drn_sent_accum_to_n_data_accum(drn_sacc, d_rmax)
+        d_rmax = drn_accum_to_d_rmax(drn_accum, dr_rlen, d_hlen)
+        n_accum = drn_accum_to_n_accum(drn_accum, d_rmax)
         rlen, hlen = rindex_to_rhlen(dr_rlen, d_hlen, d_rmax)
 
         if args.verbose:
-            cnvb = CorpusNVerbose(n_dacc, rlen, hlen)
-            table = table_result(cnvb, args.digit)
+            nvb = NVerbose(n_accum, rlen, hlen)
+            table = table_result(nvb, args.digit)
             print(args.hyp_path_list[h])
             print(table)
         else:
-            gleu = n_accum_to_gleu(n_dacc, rlen, hlen)
+            gleu = n_accum_to_gleu(n_accum, rlen, hlen)
             line = simple_result(gleu, args.digit)
             print(args.hyp_path_list[h] + '\t' + line)
 
 
 def corpus_sampling(args):
-    _, _, _, dr_rlen, dh_hlen, hdrn_sacc = load_hdrn_data(args)
+    _, _, _, dr_rlen, dh_hlen, hdrn_accum = load_hdrn_data(args)
     id_rindex = make_id_rindex(args.iter, len(dr_rlen), len(args.ref_path_list), args.fix_seed)
 
-    for h, drn_sacc in enumerate(hdrn_sacc):
+    for h, drn_accum in enumerate(hdrn_accum):
         d_hlen = dh_hlen[:, h]
 
         if args.proc > 1:
             gleu_args = [
-                (drn_sacc, d_rindex, dr_rlen, d_hlen)
+                (drn_accum, d_rindex, dr_rlen, d_hlen)
                 for d_rindex
                 in id_rindex]
             with Pool(args.proc) as pool:
-                gleus = pool.starmap(drn_sacc_to_gleu, gleu_args)
+                gleus = pool.starmap(drn_accum_to_gleu, gleu_args)
         else:
             gleus = [
-                drn_sacc_to_gleu(drn_sacc, d_rindex, dr_rlen, d_hlen)
+                drn_accum_to_gleu(drn_accum, d_rindex, dr_rlen, d_hlen)
                 for d_rindex
                 in id_rindex]
 
         gleu = np.mean(gleus)
         line = simple_result(gleu, args.digit)
         print(args.hyp_path_list[h] + '\t' + line)
 
 
-def drn_sacc_to_gleu(drn_sacc, d_rindex, dr_rlen, d_hlen):
-    n_dacc = drn_sent_accum_to_n_data_accum(drn_sacc, d_rindex)
+def drn_accum_to_gleu(drn_accum, d_rindex, dr_rlen, d_hlen):
+    n_accum = drn_accum_to_n_accum(drn_accum, d_rindex)
     rlen, hlen = rindex_to_rhlen(dr_rlen, d_hlen, d_rindex)
-    gleu = n_accum_to_gleu(n_dacc, rlen, hlen)
+    gleu = n_accum_to_gleu(n_accum, rlen, hlen)
     return gleu
```

### Comparing `gleu-1.0.0/gleu/count.py` & `gleu-1.1.0/gleu/count.py`

 * *Files identical despite different names*

### Comparing `gleu-1.0.0/gleu/load.py` & `gleu-1.1.0/gleu/load.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .aggreg import make_dhrn_sent_accum, make_hdrn_sent_accum
+from .aggreg import make_dhrn_accum, make_hdrn_accum
 from .count import make_dx_xlen
 
 
 def load_corpora(args):
     s_dat = load_text(args.source_path)
     rs_dat = load_paired_texts(args.ref_path_list)
     hs_dat = load_paired_texts(args.hyp_path_list)
@@ -22,16 +22,16 @@
     data = [load_text(path) for path in path_list]
     return list(zip(*data))
 
 
 def load_hdrn_data(args):
     s_dat, rs_dat, hs_dat, dr_rlen, dh_hlen = load_corpora(args)
     h_dats = list(zip(*hs_dat))
-    hrnd_sacc = make_hdrn_sent_accum(args.n, s_dat, rs_dat, h_dats)
+    hrnd_sacc = make_hdrn_accum(args.n, s_dat, rs_dat, h_dats)
     return s_dat, rs_dat, hs_dat, dr_rlen, dh_hlen, hrnd_sacc
 
 
 def load_dhrn_data(args):
     s_dat, rs_dat, hs_dat, dr_rlen, dh_hlen = load_corpora(args)
-    dhrn_sacc = make_dhrn_sent_accum(args.n, s_dat, rs_dat, hs_dat)
+    dhrn_sacc = make_dhrn_accum(args.n, s_dat, rs_dat, hs_dat)
     return s_dat, rs_dat, hs_dat, dr_rlen, dh_hlen, dhrn_sacc
```

### Comparing `gleu-1.0.0/gleu/main.py` & `gleu-1.1.0/gleu/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from argparse import ArgumentParser
 from .sent_main import sent_main, mean_main
 from .corpus_main import corpus_main
 from .count import set_tokenization
 
 
-def main():
-    args = parse_args()
-    set_tokenization(args.token)
-    args.handler(args)
+def gleu():
+    main(corpus_main)
 
 
-def parse_args():
-    parser = ArgumentParser()
-    first = parser.add_subparsers()
-    set_method(first, 'sent', sent_main)
-    set_method(first, 'mean', mean_main)
-    set_method(first, 'corpus', corpus_main)
-    return parser.parse_args()
+def sgleu():
+    main(sent_main)
+
 
+def mgleu():
+    main(mean_main)
 
-def set_method(first, arg, handler):
-    parser = first.add_parser(arg)
+
+def main(handler):
+    parser = ArgumentParser()
     add_args(parser)
     parser.set_defaults(handler = handler)
+    args = parser.parse_args()
+    set_tokenization(args.token)
+    args.handler(args)
 
 
 def add_args(parser):
     parser.add_argument(
             '-n', type = int, default = 4,
             help = 'maximum n for n-gram')
     parser.add_argument(
```

### Comparing `gleu-1.0.0/gleu/result.py` & `gleu-1.1.0/gleu/result.py`

 * *Files identical despite different names*

### Comparing `gleu-1.0.0/gleu/sent_main.py` & `gleu-1.1.0/gleu/sent_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 import numpy as np
 from .load import load_dhrn_data, load_hdrn_data
-from .score import rn_sent_accum_to_gleu
+from .score import rn_accum_to_gleu
 from .util import argmax
-from .verbose import SentNVerbose
+from .verbose import NVerbose
 from .result import simple_result, table_result
 
 
 def sent_main(args):
     if args.verbose:
         sent_verbose(args)
     else:
         sent_simple(args)
 
 
 def sent_simple(args):
-    _, _, _, dr_rlen, dh_hlen, dhrn_sacc = load_dhrn_data(args)
+    _, _, _, dr_rlen, dh_hlen, dhrn_accum = load_dhrn_data(args)
 
-    for d, hrn_sacc in enumerate(dhrn_sacc):
+    for d, hrn_accum in enumerate(dhrn_accum):
         h_score = [
-            rn_sent_accum_to_gleu(
-                rn_sacc,
+            rn_accum_to_gleu(
+                rn_accum,
                 dr_rlen[d],
                 dh_hlen[d, h],
                 args.max)
-            for h, rn_sacc
-            in enumerate(hrn_sacc)]
+            for h, rn_accum
+            in enumerate(hrn_accum)]
         results = [
             simple_result(score, args.digit)
             for score
             in h_score]
         line = '\t'.join(results)
         print(line)
 
 
 def sent_verbose(args):
-    s_dat, rs_dat, hs_dat, dr_rlen, dh_hlen, dhrn_sacc = load_dhrn_data(args)
+    s_dat, rs_dat, hs_dat, dr_rlen, dh_hlen, dhrn_accum = load_dhrn_data(args)
 
-    for d, hrn_sacc in enumerate(dhrn_sacc):
-        for h, rn_sacc in enumerate(hrn_sacc):
-            r_snvb = [
-                SentNVerbose(
-                    n_sacc,
+    for d, hrn_accum in enumerate(dhrn_accum):
+        for h, rn_accum in enumerate(hrn_accum):
+            r_nvb = [
+                NVerbose(
+                    n_accum,
                     dr_rlen[d, r],
                     dh_hlen[d, h])
-                for r, n_sacc
-                in enumerate(rn_sacc)]
-            rmax = argmax(r_snvb)
-            for r, snvb in enumerate(r_snvb):
-                table = table_result(snvb, args.digit)
+                for r, n_accum
+                in enumerate(rn_accum)]
+            rmax = argmax(r_nvb)
+            for r, nvb in enumerate(r_nvb):
+                table = table_result(nvb, args.digit)
                 chosen = '*' if r == rmax else ' '
                 print(f'S-{d+1}   \t{s_dat[d]}')
                 print(f'H-{d+1}-{h+1} \t{hs_dat[d][h]}')
                 print(f'R-{d+1}-{r+1}{chosen}\t{rs_dat[d][r]}')
                 print(table)
 
 
 def mean_main(args):
-    _, _, _, dr_rlen, dh_hlen, hdrn_sacc = load_hdrn_data(args)
+    _, _, _, dr_rlen, dh_hlen, hdrn_accum = load_hdrn_data(args)
 
-    for h, drn_sacc in enumerate(hdrn_sacc):
+    for h, drn_accum in enumerate(hdrn_accum):
         d_score = [
-            rn_sent_accum_to_gleu(
-                rn_sacc,
+            rn_accum_to_gleu(
+                rn_accum,
                 dr_rlen[d],
                 dh_hlen[d, h],
                 args.max)
-            for d, rn_sacc
-            in enumerate(drn_sacc)]
+            for d, rn_accum
+            in enumerate(drn_accum)]
         line = simple_result(np.mean(d_score), args.digit)
         print(args.hyp_path_list[h] + '\t' + line)
```

### Comparing `gleu-1.0.0/gleu/util.py` & `gleu-1.1.0/gleu/util.py`

 * *Files identical despite different names*

