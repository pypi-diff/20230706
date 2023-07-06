# Comparing `tmp/hostile-0.0.1.tar.gz` & `tmp/hostile-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostile-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hostile-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hostile-0.0.1.tar` & `hostile-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,34 @@
--rw-r--r--   0        0        0      682 2023-06-20 13:27:05.656599 hostile-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1963 2023-06-20 13:40:01.254289 hostile-0.0.1/.gitignore
--rw-r--r--   0        0        0      260 2023-05-31 15:56:25.388315 hostile-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1086 2023-05-23 13:13:09.919197 hostile-0.0.1/LICENSE
--rw-r--r--   0        0        0     2987 2023-06-20 13:33:34.090656 hostile-0.0.1/README.md
--rw-r--r--   0        0        0      152 2023-06-20 12:34:36.740394 hostile-0.0.1/environment.yml
--rw-r--r--   0        0        0      647 2023-06-20 13:38:38.854302 hostile-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       55 2023-06-20 13:29:11.970157 hostile-0.0.1/src/hostile/__init__.py
--rw-r--r--   0        0        0     3807 2023-06-20 12:32:16.861655 hostile-0.0.1/src/hostile/aligner.py
--rw-r--r--   0        0        0     2125 2023-06-20 11:56:33.635211 hostile-0.0.1/src/hostile/cli.py
--rw-r--r--   0        0        0     4629 2023-06-20 12:09:32.801204 hostile-0.0.1/src/hostile/lib.py
--rw-r--r--   0        0        0     2461 2023-06-20 12:32:41.355593 hostile-0.0.1/src/hostile/util.py
--rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.881250 hostile-0.0.1/tests/data/MN908947/MN908947.1.bt2
--rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.881240 hostile-0.0.1/tests/data/MN908947/MN908947.2.bt2
--rw-r--r--   0        0        0       17 2023-06-02 16:28:46.850838 hostile-0.0.1/tests/data/MN908947/MN908947.3.bt2
--rw-r--r--   0        0        0     7476 2023-06-02 16:28:46.850709 hostile-0.0.1/tests/data/MN908947/MN908947.4.bt2
--rw-r--r--   0        0        0     9458 2022-07-08 10:03:05.588963 hostile-0.0.1/tests/data/MN908947/MN908947.fasta.gz
--rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.913064 hostile-0.0.1/tests/data/MN908947/MN908947.rev.1.bt2
--rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.913055 hostile-0.0.1/tests/data/MN908947/MN908947.rev.2.bt2
--rw-r--r--   0        0        0     1508 2023-05-25 19:01:02.910477 hostile-0.0.1/tests/data/h37rv_10.r1.fastq.gz
--rw-r--r--   0        0        0     1501 2023-05-25 19:01:13.127122 hostile-0.0.1/tests/data/h37rv_10.r2.fastq.gz
--rw-r--r--   0        0        0    19004 2023-05-31 15:32:30.691759 hostile-0.0.1/tests/data/human.1k.fa.gz
--rw-r--r--   0        0        0      813 2023-06-20 13:24:36.646409 hostile-0.0.1/tests/test_all.py
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 hostile-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-06-23 11:14:47.624384 hostile-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1971 2023-07-06 18:18:11.923048 hostile-0.0.2/.gitignore
+-rw-r--r--   0        0        0      260 2023-05-31 15:56:25.388315 hostile-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1086 2023-05-23 13:13:09.919197 hostile-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3584 2023-07-06 18:18:11.923306 hostile-0.0.2/README.md
+-rw-r--r--   0        0        0      178 2023-06-21 13:48:03.074531 hostile-0.0.2/environment.yml
+-rw-r--r--   0        0        0     5403 2023-07-06 18:18:11.923619 hostile-0.0.2/paper/supplementary-table-1.tsv
+-rw-r--r--   0        0        0    39955 2023-07-06 18:18:11.923951 hostile-0.0.2/paper/supplementary-table-2.tsv
+-rw-r--r--   0        0        0      647 2023-06-20 13:38:38.854302 hostile-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-07-06 18:20:24.201153 hostile-0.0.2/src/hostile/__init__.py
+-rw-r--r--   0        0        0     6139 2023-07-06 18:18:11.924322 hostile-0.0.2/src/hostile/aligner.py
+-rw-r--r--   0        0        0     2664 2023-06-28 16:38:34.717809 hostile-0.0.2/src/hostile/cli.py
+-rw-r--r--   0        0        0     7625 2023-07-06 18:18:11.924493 hostile-0.0.2/src/hostile/lib.py
+-rw-r--r--   0        0        0     2809 2023-06-28 17:00:15.389198 hostile-0.0.2/src/hostile/util.py
+-rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.881250 hostile-0.0.2/tests/data/MN908947/MN908947.1.bt2
+-rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.881240 hostile-0.0.2/tests/data/MN908947/MN908947.2.bt2
+-rw-r--r--   0        0        0       17 2023-06-02 16:28:46.850838 hostile-0.0.2/tests/data/MN908947/MN908947.3.bt2
+-rw-r--r--   0        0        0     7476 2023-06-02 16:28:46.850709 hostile-0.0.2/tests/data/MN908947/MN908947.4.bt2
+-rw-r--r--   0        0        0     9458 2022-07-08 10:03:05.588963 hostile-0.0.2/tests/data/MN908947/MN908947.fasta.gz
+-rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.913064 hostile-0.0.2/tests/data/MN908947/MN908947.rev.1.bt2
+-rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.913055 hostile-0.0.2/tests/data/MN908947/MN908947.rev.2.bt2
+-rw-r--r--   0        0        0     3562 2023-05-25 19:01:02.910477 hostile-0.0.2/tests/data/h37rv_10.r1.fastq
+-rw-r--r--   0        0        0     1508 2023-05-25 19:01:02.910477 hostile-0.0.2/tests/data/h37rv_10.r1.fastq.gz
+-rw-r--r--   0        0        0     3562 2023-05-25 19:01:13.127122 hostile-0.0.2/tests/data/h37rv_10.r2.fastq
+-rw-r--r--   0        0        0     1501 2023-05-25 19:01:13.127122 hostile-0.0.2/tests/data/h37rv_10.r2.fastq.gz
+-rw-r--r--   0        0        0    19004 2023-05-31 15:32:30.691759 hostile-0.0.2/tests/data/human.1k.fa.gz
+-rw-r--r--   0        0        0      164 2023-07-06 18:18:11.924762 hostile-0.0.2/tests/data/human_1_1.fastq.gz
+-rw-r--r--   0        0        0      178 2023-07-06 18:18:11.925005 hostile-0.0.2/tests/data/human_1_2.fastq.gz
+-rw-r--r--   0        0        0     3497 2023-07-06 18:18:11.925318 hostile-0.0.2/tests/data/mixed_human_100_1.fastq.gz
+-rw-r--r--   0        0        0     3798 2023-07-06 18:18:11.925658 hostile-0.0.2/tests/data/mixed_human_100_2.fastq.gz
+-rw-r--r--   0        0        0      239 2023-07-06 18:18:11.925871 hostile-0.0.2/tests/data/tuberculosis_1_1.fastq.gz
+-rw-r--r--   0        0        0      232 2023-07-06 18:18:11.926049 hostile-0.0.2/tests/data/tuberculosis_1_2.fastq.gz
+-rw-r--r--   0        0        0     1799 2023-06-28 15:12:22.450633 hostile-0.0.2/tests/test_all.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 hostile-0.0.2/PKG-INFO
```

### Comparing `hostile-0.0.1/.github/workflows/test.yml` & `hostile-0.0.2/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-22.04, macos-11, macos-12]
+        os: [ubuntu-22.04, macos-12]
         python-version: ['3.10']
     name: Python ${{ matrix.python-version }} (${{ matrix.os }})
     steps:
       - uses: actions/checkout@v2
       - name: Setup conda
         uses: s-weigand/setup-conda@v1
         with:
```

### Comparing `hostile-0.0.1/.gitignore` & `hostile-0.0.2/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -132,9 +132,9 @@
 
 .vscode
 
 test.sam
 tests/data/h37rv_10_2.r1.fastq.gz
 tests/data/h37rv_10_2.r2.fastq.gz
 tests/data/human-index
-tests/data/human.fa.gz
+tests/data/human-t2t-hla.fa.gz
 tests/data/mtb-jeff
```

### Comparing `hostile-0.0.1/LICENSE` & `hostile-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/pyproject.toml` & `hostile-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/MN908947/MN908947.1.bt2` & `hostile-0.0.2/tests/data/MN908947/MN908947.1.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/MN908947/MN908947.2.bt2` & `hostile-0.0.2/tests/data/MN908947/MN908947.2.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/MN908947/MN908947.4.bt2` & `hostile-0.0.2/tests/data/MN908947/MN908947.4.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/MN908947/MN908947.fasta.gz` & `hostile-0.0.2/tests/data/MN908947/MN908947.fasta.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/MN908947/MN908947.rev.1.bt2` & `hostile-0.0.2/tests/data/MN908947/MN908947.rev.1.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/MN908947/MN908947.rev.2.bt2` & `hostile-0.0.2/tests/data/MN908947/MN908947.rev.2.bt2`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/h37rv_10.r1.fastq.gz` & `hostile-0.0.2/tests/data/h37rv_10.r1.fastq.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/h37rv_10.r2.fastq.gz` & `hostile-0.0.2/tests/data/h37rv_10.r2.fastq.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/data/human.1k.fa.gz` & `hostile-0.0.2/tests/data/human.1k.fa.gz`

 * *Files identical despite different names*

### Comparing `hostile-0.0.1/tests/test_all.py` & `hostile-0.0.2/tests/test_all.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,20 +13,52 @@
     )
 
 
 def test_version_cli():
     run("hostile --version")
 
 
-# def test_minimal_fastqs():
-#     lib.dehost_paired_fastqs(
-#         fastqs=[(data_dir / "h37rv_10.r1.fastq.gz", data_dir / "h37rv_10.r2.fastq.gz")],
-#         out_dir=Path("test_minimal_fastqs"),
-#     )
-#     shutil.rmtree("test_minimal_fastqs")
+def test_minimal_fastq():
+    lib.clean_fastqs(
+        fastqs=[data_dir / "h37rv_10.r1.fastq.gz"],
+        out_dir=Path("test_minimal_fastq"),
+    )
+    shutil.rmtree("test_minimal_fastq")
+
+
+def test_minimal_paired_fastqs():
+    lib.clean_paired_fastqs(
+        fastqs=[(data_dir / "h37rv_10.r1.fastq.gz", data_dir / "h37rv_10.r2.fastq.gz")],
+        out_dir=Path("test_minimal_fastqs"),
+    )
+    shutil.rmtree("test_minimal_fastqs")
+
+
+def test_minimal_uncompressed_paired_fastqs():
+    lib.clean_paired_fastqs(
+        fastqs=[(data_dir / "h37rv_10.r1.fastq", data_dir / "h37rv_10.r2.fastq")],
+        out_dir=Path("test_minimal_fastqs"),
+    )
+    shutil.rmtree("test_minimal_fastqs")
 
 
-# def test_minimal_fastqs_cli():
-#     run(
-#         f"hostile dehost --fastq1 h37rv_10.r1.fastq.gz --fastq2 h37rv_10.r2.fastq.gz --out-dir test_minimal_fastqs"
-#     )
-#     shutil.rmtree(f"{data_dir}/test_minimal_fastqs")
+def test_minimal_paired_fastqs_cli():
+    run(
+        f"hostile clean --fastq1 h37rv_10.r1.fastq.gz --fastq2 h37rv_10.r2.fastq.gz --out-dir test_minimal_fastqs"
+    )
+    shutil.rmtree(f"{data_dir}/test_minimal_fastqs")
+
+
+def test_many_minimal_paired_fastqs_cli():
+    run(
+        f"hostile clean-many h37rv_10.r1.fastq.gz,h37rv_10.r2.fastq.gz h37rv_10_2.r1.fastq.gz,h37rv_10_2.r2.fastq.gz --out-dir test_minimal_fastqs"
+    )
+    shutil.rmtree(f"{data_dir}/test_minimal_fastqs")
+
+
+def test_custom_index():
+    lib.clean_paired_fastqs(
+        fastqs=[(data_dir / "h37rv_10.r1.fastq.gz", data_dir / "h37rv_10.r2.fastq.gz")],
+        custom_index="tests/data/MN908947/MN908947",
+        out_dir=Path("test_minimal_fastqs"),
+    )
+    shutil.rmtree("test_minimal_fastqs")
```

### Comparing `hostile-0.0.1/PKG-INFO` & `hostile-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hostile
-Version: 0.0.1
-Summary: Hostile: host read removal
+Version: 0.0.2
+Summary: Host read removal
 Author-email: Bede Constantinides <bedeabc@gmail.com>
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: defopt>=6.4.0
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: platformdirs>=3.5.1
 Requires-Dist: tqdm>=4.65.0
```

