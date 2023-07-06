# Comparing `tmp/easy_sudoku_solver-0.1.3.tar.gz` & `tmp/easy_sudoku_solver-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_sudoku_solver-0.1.3.tar", max compression
+gzip compressed data, was "easy_sudoku_solver-0.1.4.tar", max compression
```

## Comparing `easy_sudoku_solver-0.1.3.tar` & `easy_sudoku_solver-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      446 2023-07-06 18:44:19.464262 easy_sudoku_solver-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      396 2023-07-06 18:44:13.922291 easy_sudoku_solver-0.1.3/README.md
--rw-r--r--   0        0        0       52 2023-07-06 18:32:55.198984 easy_sudoku_solver-0.1.3/sudoku_solver/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-03 19:05:41.198312 easy_sudoku_solver-0.1.3/sudoku_solver/board.py
--rw-r--r--   0        0        0     2156 2023-07-06 17:59:52.485460 easy_sudoku_solver-0.1.3/sudoku_solver/sudoku_solver.py
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 easy_sudoku_solver-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      494 2023-07-06 18:49:05.773367 easy_sudoku_solver-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      396 2023-07-06 18:44:13.922291 easy_sudoku_solver-0.1.4/README.md
+-rw-r--r--   0        0        0       52 2023-07-06 18:32:55.198984 easy_sudoku_solver-0.1.4/sudoku_solver/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-03 19:05:41.198312 easy_sudoku_solver-0.1.4/sudoku_solver/board.py
+-rw-r--r--   0        0        0     2156 2023-07-06 17:59:52.485460 easy_sudoku_solver-0.1.4/sudoku_solver/sudoku_solver.py
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 easy_sudoku_solver-0.1.4/PKG-INFO
```

### Comparing `easy_sudoku_solver-0.1.3/sudoku_solver/board.py` & `easy_sudoku_solver-0.1.4/sudoku_solver/board.py`

 * *Files identical despite different names*

### Comparing `easy_sudoku_solver-0.1.3/sudoku_solver/sudoku_solver.py` & `easy_sudoku_solver-0.1.4/sudoku_solver/sudoku_solver.py`

 * *Files identical despite different names*

### Comparing `easy_sudoku_solver-0.1.3/PKG-INFO` & `easy_sudoku_solver-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-sudoku-solver
-Version: 0.1.3
+Version: 0.1.4
 Summary: sudoku solver
 Author: Gustaw Filipek
 Author-email: guciofilipek@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

