# Comparing `tmp/svbench-0.7.1.tar.gz` & `tmp/svbench-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svbench-0.7.1.tar", last modified: Tue Jul  4 13:57:27 2023, max compression
+gzip compressed data, was "svbench-0.7.2.tar", last modified: Thu Jul  6 15:13:31 2023, max compression
```

## Comparing `svbench-0.7.1.tar` & `svbench-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-04 13:57:26.998912 svbench-0.7.1/
--rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.1/LICENSE.md
--rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.1/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-04 13:57:26.998572 svbench-0.7.1/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.1/README.rst
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-04 13:57:26.999004 svbench-0.7.1/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-07-04 13:52:52.000000 svbench-0.7.1/setup.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-04 13:57:26.986272 svbench-0.7.1/svbench/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.1/svbench/.DS_Store
--rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.1/svbench/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     1158 2023-05-26 13:39:20.000000 svbench-0.7.1/svbench/cli.py
--rw-r--r--   0 kezcleal   (501) staff       (20)    69121 2023-07-04 13:56:22.000000 svbench-0.7.1/svbench/io_tools.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.1/svbench/loaders.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-04 13:57:26.998266 svbench-0.7.1/svbench/models/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.1/svbench/models/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.1/svbench/quant_tools.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-04 13:57:26.997865 svbench-0.7.1/svbench.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/entry_points.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/top_level.txt
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-06 15:13:31.856224 svbench-0.7.2/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.2/LICENSE.md
+-rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.2/MANIFEST.in
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-06 15:13:31.855849 svbench-0.7.2/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.2/README.rst
+-rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-06 15:13:31.856321 svbench-0.7.2/setup.cfg
+-rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-07-06 15:13:27.000000 svbench-0.7.2/setup.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-06 15:13:31.852742 svbench-0.7.2/svbench/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.2/svbench/.DS_Store
+-rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.2/svbench/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1357 2023-07-06 15:05:30.000000 svbench-0.7.2/svbench/cli.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)    69878 2023-07-06 15:05:30.000000 svbench-0.7.2/svbench/io_tools.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.2/svbench/loaders.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-06 15:13:31.855534 svbench-0.7.2/svbench/models/
+-rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.2/svbench/models/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.2/svbench/quant_tools.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-06 15:13:31.855101 svbench-0.7.2/svbench.egg-info/
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/SOURCES.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/dependency_links.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/entry_points.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/requires.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/top_level.txt
```

### Comparing `svbench-0.7.1/LICENSE.md` & `svbench-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `svbench-0.7.1/README.rst` & `svbench-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `svbench-0.7.1/svbench/.DS_Store` & `svbench-0.7.2/svbench/.DS_Store`

 * *Files identical despite different names*

### Comparing `svbench-0.7.1/svbench/cli.py` & `svbench-0.7.2/svbench/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import click
 import svbench as svb
 from svbench import CallSet
+import pkg_resources
+
+version = pkg_resources.require("svbench")[0].version
 
 
 @click.command()
 @click.argument('reference_vcf', required=True, type=click.Path())
 @click.argument('query_vcfs', required=True, type=click.Path(), nargs=-1)
 @click.option("--pass-only", help="Assess only PASS variants", is_flag=True, flag_value=True, show_default=False, default=False)
 @click.option("--slop", help="Add intervals +/- slop around breakpoints", default=250, type=int, show_default=True)
 @click.option("--min-size", help="Min SV length", default=20, type=int, show_default=True)
+@click.version_option()
 def main(reference_vcf, query_vcfs, pass_only, slop, min_size):
     keep = [svb.Col("FILTER", op="eq", thresh=None)] if pass_only else []
-    ref = CallSet(dataset="REFERENCE").\
+    ref = CallSet(dataset="REFERENCE", no_translocations=False).\
         load_vcf(reference_vcf, other_cols=["FILTER"], keep=keep). \
-        filter_by_size(min_size, None)
-
+        filter_by_size(min_size, None, keep_translocations=True)
     ref.add_intervals(slop)
-
-    query = [CallSet(dataset="REFERENCE", caller=path.split("/")[-1]).
+    query = [CallSet(dataset="REFERENCE", caller=path.split("/")[-1], no_translocations=False).
              load_vcf(path, other_cols=["FILTER"], keep=keep).
-             filter_by_size(min_size, None)
+             filter_by_size(min_size, None, keep_translocations=True)
              for path in query_vcfs]
-
     svb.score(ref, query)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `svbench-0.7.1/svbench/io_tools.py` & `svbench-0.7.2/svbench/io_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -630,15 +630,15 @@
         else:
             max_s = max_size
 
         l_before = len(cs.breaks_df)
         df = cs.breaks_df
 
         if keep_translocations:
-            size_filter = ((df["svlen"] >= min_s) & (df["svlen"] < max_s)) | (df["chrom1"] != df["chrom2"])
+            size_filter = ((df["svlen"] >= min_s) & (df["svlen"] < max_s)) | (df["chrom"] != df["chrom2"])
         else:
             size_filter = (df["svlen"] >= min_s) & (df["svlen"] < max_s)
 
         df["size_filter_pass"] = size_filter
         if not soft:
             df = df[size_filter]
         print("Filtered by min_size={}, max_size={}, caller={}, dataset={} rows before {}, after {}".format(
@@ -738,25 +738,24 @@
                 else:
                     c.append(Col(k))
             return c
         else:
             return cols
 
     def load_vcf(self, path, weight_field=None,
-                 no_translocations=True, allowed_svtypes=None, keep=None, stratify=None, allowed_chroms=None,
+                 allowed_svtypes=None, keep=None, stratify=None, allowed_chroms=None,
                  min_size=None, max_size=None, soft_size_filter=False,
                  other_cols=None, include_bed=None, include_if="both", load_genotype=True):
         """Load variants from the vcf file path.
 
         :param path: The path to the vcf input file
         :type path: str
         :param weight_field: The field used to weight a variant, useful for breaking ties between similar variants when \
         benchmarking
         :type weight_field: svbench.Col
-        :param no_translocations: Ignore translocations when loading file
         :type no_translocations: bool
         :param allowed_svtypes: The types of SVs allowed, comma seperated string e.g. "DEL", or "DEL,DUP,INV" etc
         :type allowed_svtypes: str
         :param keep: A list of filtering operations to perform on input data. e.g. keep=[Col("INFO", "SU", "ge" 3)] \
         would keep variants if the value found in INFO --> SU was greater than or equal to 3
         :type keep: list
         :param stratify:
@@ -913,37 +912,44 @@
                 except AttributeError:
                     print("Error parsing", r, file=stderr)
                     continue
                 if end is None:
                     end = start + 1
                 else:
                     end = int(r.ALT[0].pos)
-
+                if chrom.startswith("chr") and not chrom2.startswith("chr"):
+                    chrom2 = "chr" + chrom2
             else:
                 chrom2 = chrom
                 if "CHR2" in r.INFO:
                     chrom2 = r.INFO["CHR2"]
                     if chrom2[0] != "c":
                         chrom2 = "chr" + chrom2
 
                 done = False
-                if "END" in r.INFO:
-                    end = r.INFO["END"]
-                    if isinstance(end, list):
-                        end = end[0]
-                    end = int(end)
-                    done = True
+                if "END" in r.INFO or "CHR2_POS" in r.INFO:
+                    if "CHR2_POS" in r.INFO:
+                        end = r.INFO["CHR2_POS"]
+                        if isinstance(end, list):
+                            end = end[0]
+                        end = int(end)
+                        done = True
+                    else:
+                        end = r.INFO["END"]
+                        if isinstance(end, list):
+                            end = end[0]
+                        end = int(end)
+                        done = True
                 elif svtype in ("DEL", "DUP", "INV") and "SVLEN" in r.INFO:
                     svlen = r.INFO["SVLEN"]
                     if isinstance(svlen, list):
                         svlen = svlen[0]
                     end = start + svlen
                     done = True
                 else:  # Try and use ALT / REF lengths
-
                     if r.INFO["SVTYPE"] == "DEL" or (isinstance(r.INFO["SVTYPE"], list) and r.INFO["SVTYPE"][0] == "DEL"):
                         svlen = len(r.REF) if r.ALT is not isinstance(r.REF, list) else r.REF[0]
                         end = r.POS + svlen
                         done = True
                     elif r.INFO["SVTYPE"] == "INS" or (isinstance(r.INFO["SVTYPE"], list) and r.INFO["SVTYPE"][0] == "INS"):
                         svlen = len(r.ALT) if r.ALT is not isinstance(r.ALT, list) else r.ALT[0]
                         end = r.POS + svlen
@@ -1054,15 +1060,14 @@
 
         # Normalize new columns, might be more than one column added per Col
         if other_cols is not None and other_cols != "all":
             item_key = {(k.col, k.key): k for k in other_cols if k.norm is not None}
             for k, v in item_key.items():
                 for ec in new_cols:
                     ecs = ec.split(":")
-
                     if ecs[0] == k or (ecs[0], ecs[1]) == k:
                         df[ec] = v.norm(df[ec], self.kwargs)
 
         # Order df
         base_cols = ["chrom", "start", "chrom2", "end", "svtype", "w", "strata", "id", "size_filter_pass", "svlen", "filter"]
         if load_genotype:
             base_cols.append("GT")
@@ -1191,15 +1196,14 @@
             else:
                 df[n] = df_in[col]
 
         if id_field is not None:
             df["id"] = df_in[id_field]
         else:
             df["id"] = df.index
-        print(df.head(), file=stderr)
 
         if allowed_chroms:
             if not isinstance(allowed_chroms, set):
                 allowed_chroms = set(allowed_chroms)
             df = df[df["chrom"].isin(allowed_chroms) & df["chrom2"].isin(allowed_chroms)]
 
         if no_translocations:
@@ -1506,183 +1510,159 @@
         data.scores = pd.DataFrame.from_records(ts)[["T >=", "Ref", "Total", "TP", "FP", "DTP", "FN", "Duplication", "Precision",
                                                      "Recall", "F1"]]
         data.false_negative_indexes = ref_bedpe.index
         return
 
     for query_idx, chrom, start, chrom2, end, svtype, w in zip(dta.index, dta["chrom"], dta["start"], dta["chrom2"], dta["end"],
                                                        dta["svtype"], dta["w"]):
-
         if chrom == chrom2 and start == end:
             end += 1  # prevent 0 width interval
         chrom, start, chrom2, end = sv_key(chrom, start, chrom2, end)
 
         ol_start = intersecter(tree, chrom, start, start + 1)
         if not ol_start:
+            # print("FALSE1", chrom, start, chrom2, end, svtype, file=stderr)
             continue
 
         ol_end = intersecter(tree, chrom2, end, end + 1)
         if not ol_end:
+            # print("FALSE2", chrom, start, chrom2, end, svtype, file=stderr)
             continue
 
         # if start == 57861455:
         #     print(ol_start)
         #     print(ol_end)
 
         # Get the ref_data index
         common_idxs = set([i[2] for i in ol_start]).intersection([i[2] for i in ol_end])
         if len(common_idxs) == 0:
             continue
 
         # Choose an index by highest weight/lowest total distance, meeting reciprocal_overlap threshold
         min_d = 1e12
         chosen_index = None
-
+        ref_chrom, ref_start, ref_chrom2, ref_end = None, None, None, None
         for index in common_idxs:
-
             try:
                 ref_row = ref_bedpe.loc[index]
             except IndexError:
                 raise ("Index error", index, " Try re-setting intervals")
-
             ref_chrom, ref_start, ref_chrom2, ref_end = sv_key(ref_row["chrom"], ref_row["start"],
                                                                ref_row["chrom2"], ref_row["end"])
-
             # Make sure chromosomes match
             if chrom != ref_chrom or chrom2 != ref_chrom2:
                 continue
-
             if not ignore_svtype and ref_row["svtype"] != svtype:
                 if dups_and_ins_equivalent and svtype in ("DUP", "INS") and ref_row["svtype"] in ("DUP", "INS"):
                     pass
+                if svtype == "BND" or ref_row["svtype"] == "BND":  # lenient match
+                    pass
                 else:
                     continue
-
             # If intra-chromosomal, check reciprocal overlap
             if chrom == chrom2:
-
                 if "svlen" in ref_row:
                     ref_size = ref_row["svlen"] + 1e-6
                 else:
                     ref_size = ref_end - ref_start + 1e-3
-
                 if min_ref_size is not None:
                     if ref_size < min_ref_size:
                         continue
-
                 if max_ref_size is not None:
                     if ref_size >= max_ref_size:
                         continue
-
                 if "svlen" in dta:
                     query_size = dta["svlen"].loc[query_idx] + 1e-6
                 else:
                     query_size = end - start + 1e-6
-
                 ol = float(max(0, min(end, ref_end) - max(start, ref_start)))
-
                 if pct_size > 0:
                     pct = min(ref_size, query_size) / max(ref_size, query_size)
                     if pct < pct_size:
                         continue
-
                 if reciprocal_overlap > 0:
                     if (ol / query_size < reciprocal_overlap) and (ol / ref_size < reciprocal_overlap):
                         continue
-
                 if force_intersection and ol == 0:
                     continue
-
             dis = abs(ref_start - start) + abs(ref_end - end)
             if dis < min_d:
                 min_d = dis
                 chosen_index = index
 
         if chosen_index is not None:
             G.add_edge(('t', chosen_index), ('q', query_idx), dis=min_d, weight=w)
+            # print(chosen_index, query_idx, (ref_chrom, ref_start), (ref_chrom2, ref_end), chrom, start, chrom2, end, svtype, file=stderr)
 
         # if start == 57861455:
         #     print(common_idxs)
         #     print(chosen_index)
         #     print(chrom, ref_chrom, chrom2, ref_chrom2, dis < min_d, index)
         #     quit()
 
     good_idxs = {}
     duplicate_idxs = {}
     # Make partitions bipartite-matching i.e. one reference call matched to one query call
     for sub in nx.connected_components(G):
         sub = list(sub)
-
         if len(sub) == 2:  # One ref matches one query, easy case
-
             if sub[0][0] == "q":
                 good_idxs[sub[0][1]] = sub[1][1]
             else:  # t first
                 good_idxs[sub[1][1]] = sub[0][1]
             continue
-
         else:
             bi_count = Counter([i[0] for i in sub])
-
             if bi_count["t"] == 1 or bi_count["q"] == 1:  # Choose best edge
                 ref_node = [i for i in sub if i[0] == "t"][0]
                 out_edges = list(G.edges(ref_node, data=True))
                 found, others = best_index(out_edges, key="q")
                 good_idxs.update(found)
                 duplicate_idxs.update(others)
-
             else:  # Do multi with the maximum-bipartite-matching
                 print("Maximum bipartite matching not implemented", file=stderr)
                 quit()
         continue
-
     df = data.breaks_df
     index = df.index  # Use the original IDs?
-
     if good_indexes_only:
         return [i in good_idxs for i in index]
 
     missing_ref_indexes = set(ref_bedpe.index).difference(set(good_idxs.values()))
     if allow_duplicate_tp:
         duplicate_idxs = {k: v for k, v in duplicate_idxs.items() if k not in good_idxs}
     else:
         duplicate_idxs = {}
 
     df["TP"] = [i in good_idxs for i in index]
     df["DTP"] = [i in duplicate_idxs for i in index]
-
     df["ref_index"] = [good_idxs[i] if i in good_idxs else duplicate_idxs[i] if i in duplicate_idxs
                                   else None for i in index]
     df["FP"] = [not i and not j for i, j in zip(df["DTP"], df["TP"])]
-
     if "svlen" in ref_bedpe:
         df["ref_size"] = [abs(ref_bedpe["svlen"].loc[good_idxs[i]]) if
                           (i in good_idxs and dta.loc[i]["chrom"] == dta.loc[i]["chrom2"]) else None
                           for i in index]
 
     else:
         df["ref_size"] = [abs(ref_bedpe["end"].loc[good_idxs[i]] - ref_bedpe["start"].loc[good_idxs[i]]) if
                                       (i in good_idxs and dta.loc[i]["chrom"] == dta.loc[i]["chrom2"]) else None
                                       for i in index]
 
     n_in_ref = len(ref_bedpe)
-
     if stratify and data.stratify_range is not None:
         rng = data.stratify_range
     else:
         rng = [None]
 
     data.breaks_df = df
     dta = df
-
     ts = []
-
     for threshold in rng:
-
         if threshold is None or len(dta) == 0:
-
             t = {"Total": len(dta),
                  "Ref": n_in_ref,
                  "DTP": np.sum(np.in1d(dta["DTP"], True)),
                  "TP": np.sum(np.in1d(dta["TP"], True)),
                  "FP": np.sum(np.in1d(dta["FP"], True)),
                  "FN": len(missing_ref_indexes),
                  "T >=": None,
@@ -1702,43 +1682,40 @@
                           "Recall": round(float(t["TP"]) / t["Ref"], 4)})
                 if (t["Precision"] + t["Recall"]) > 0:
                     t.update({"F1": round(2 * ((t["Precision"] * t["Recall"]) / (t["Precision"] + t["Recall"])), 4)})
                 else:
                     t["F1"] = None
             else:
                 t.update({"F1": None, "Precision": None, "Recall": None})
-
             ts.append(t)
 
         else:
             df = dta[dta["strata"] >= threshold]
             if len(df) > 0:
                 t = {"Total": len(df),
                      "Ref": n_in_ref,
                      "DTP": np.sum(np.in1d(df["DTP"], True)),
                      "TP": np.sum(np.in1d(df["TP"], True)),
                      "FP": np.sum(np.in1d(df["FP"], True)),
                      "T >=": threshold,
                      "Caller": data.caller,
                      }
                 t["FN"] = n_in_ref - t["TP"]
-
                 if len(good_idxs) > 0:
                     t["Duplication"] = t["DTP"] / len(good_idxs)
                 else:
                     t["Duplication"] = 0
                 if allow_duplicate_tp:
                     sub_total = t["Total"] - t["DTP"]
                 else:
                     sub_total = t["Total"]
                 if sub_total > 0:
                     t.update({"Precision": round(float(t["TP"]) / sub_total, 4),
                               "Recall": round(float(t["TP"]) / t["Ref"], 4)})
                     t.update({"F1": round(2 * ((t["Precision"] * t["Recall"]) / (t["Precision"] + t["Recall"] + 1e-6)), 4)})
-
                 ts.append(t)
 
     if len(ts) == 0:
         print("Warning: precision/recall could not be determined", file=stderr)
         ts = [{"Total": None, "Ref": len(ref_bedpe), "DTP": None, "TP": None, "FP": None, "FN": None, "T >=": None,
                "Duplication": None, "Precision": None, "Recall": None, "F1": None, "strata": None}]
         data.false_negative_indexes = ref_bedpe.index
```

### Comparing `svbench-0.7.1/svbench/loaders.py` & `svbench-0.7.2/svbench/loaders.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.1/svbench/quant_tools.py` & `svbench-0.7.2/svbench/quant_tools.py`

 * *Files identical despite different names*

