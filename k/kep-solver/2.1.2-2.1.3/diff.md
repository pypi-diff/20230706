# Comparing `tmp/kep_solver-2.1.2.tar.gz` & `tmp/kep_solver-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kep_solver-2.1.2.tar", last modified: Thu Apr 20 14:39:08 2023, max compression
+gzip compressed data, was "kep_solver-2.1.3.tar", last modified: Thu Jul  6 14:01:38 2023, max compression
```

## Comparing `kep_solver-2.1.2.tar` & `kep_solver-2.1.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.156268 kep_solver-2.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-20 14:38:57.000000 kep_solver-2.1.2/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-20 14:38:57.000000 kep_solver-2.1.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1252 2023-04-20 14:38:57.000000 kep_solver-2.1.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-04-20 14:38:57.000000 kep_solver-2.1.2/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-04-20 14:38:57.000000 kep_solver-2.1.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     8779 2023-04-20 14:38:57.000000 kep_solver-2.1.2/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    34462 2023-04-20 14:38:57.000000 kep_solver-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5294 2023-04-20 14:39:08.156268 kep_solver-2.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4482 2023-04-20 14:38:57.000000 kep_solver-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.122262 kep_solver-2.1.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2717 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.122262 kep_solver-2.1.2/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)    11079 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/source/formats.rst
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/source/terms.rst
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-04-20 14:38:57.000000 kep_solver-2.1.2/docs/source/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.125265 kep_solver-2.1.2/kep_solver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19271 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     9106 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/fileio.py
--rw-rw-rw-   0 root         (0) root         (0)    35842 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/generation.py
--rw-rw-rw-   0 root         (0) root         (0)    23791 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    19222 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7152 2023-04-20 14:38:57.000000 kep_solver-2.1.2/kep_solver/pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.126265 kep_solver-2.1.2/kep_solver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5294 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2815 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-20 14:39:08.000000 kep_solver-2.1.2/kep_solver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-20 14:38:57.000000 kep_solver-2.1.2/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.127265 kep_solver-2.1.2/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)     6159 2023-04-20 14:38:57.000000 kep_solver-2.1.2/notebooks/Match Run.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1485 2023-04-20 14:38:57.000000 kep_solver-2.1.2/notebooks/README.md
--rw-rw-rw-   0 root         (0) root         (0)    23889 2023-04-20 14:38:57.000000 kep_solver-2.1.2/notebooks/Statistical Analysis.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.128265 kep_solver-2.1.2/paper/
--rw-rw-rw-   0 root         (0) root         (0)     2848 2023-04-20 14:38:57.000000 kep_solver-2.1.2/paper/paper.bib
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-04-20 14:38:57.000000 kep_solver-2.1.2/paper/paper.md
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-20 14:38:57.000000 kep_solver-2.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-20 14:38:57.000000 kep_solver-2.1.2/runtime.txt
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-20 14:39:08.157268 kep_solver-2.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-04-20 14:38:57.000000 kep_solver-2.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.130266 kep_solver-2.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4581 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_fileio.py
--rw-rw-rw-   0 root         (0) root         (0)    21574 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    16083 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 14:39:08.156268 kep_solver-2.1.2/tests/test_instances/
--rw-rw-rw-   0 root         (0) root         (0)   514090 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-1.json
--rw-rw-rw-   0 root         (0) root         (0)   590458 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-10.json
--rw-rw-rw-   0 root         (0) root         (0)   610079 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-2.json
--rw-rw-rw-   0 root         (0) root         (0)   590792 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-3.json
--rw-rw-rw-   0 root         (0) root         (0)   550366 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-4.json
--rw-rw-rw-   0 root         (0) root         (0)   575193 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-5.json
--rw-rw-rw-   0 root         (0) root         (0)   660843 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-6.json
--rw-rw-rw-   0 root         (0) root         (0)   665457 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-7.json
--rw-rw-rw-   0 root         (0) root         (0)   684308 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-8.json
--rw-rw-rw-   0 root         (0) root         (0)   686677 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/large-9.json
--rw-rw-rw-   0 root         (0) root         (0)    40468 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-1.json
--rw-rw-rw-   0 root         (0) root         (0)    32770 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-10.json
--rw-rw-rw-   0 root         (0) root         (0)    43595 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-2.json
--rw-rw-rw-   0 root         (0) root         (0)    33837 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-3.json
--rw-rw-rw-   0 root         (0) root         (0)    34664 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-4.json
--rw-rw-rw-   0 root         (0) root         (0)    38406 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-5.json
--rw-rw-rw-   0 root         (0) root         (0)    33991 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-6.json
--rw-rw-rw-   0 root         (0) root         (0)    35438 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-7.json
--rw-rw-rw-   0 root         (0) root         (0)    37158 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-8.json
--rw-rw-rw-   0 root         (0) root         (0)    46046 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/medium-9.json
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test1.json
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test1.txt
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test1.xml
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test10.json
--rw-rw-rw-   0 root         (0) root         (0)     2598 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test10_output.json
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test1_output.json
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test2.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test2.txt
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test2.xml
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3.json
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3.txt
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3.xml
--rw-rw-rw-   0 root         (0) root         (0)     1031 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3b.json
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3b.txt
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test3b.xml
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test4.json
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test4.txt
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test4.xml
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5.json
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5.txt
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5.xml
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5b.json
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test5b.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6.txt
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6a.json
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6a.xml
--rw-rw-rw-   0 root         (0) root         (0)      691 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6b.json
--rw-rw-rw-   0 root         (0) root         (0)      950 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test6b.xml
--rw-rw-rw-   0 root         (0) root         (0)   116023 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test7.json
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test7.txt
--rw-rw-rw-   0 root         (0) root         (0)      691 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test8.json
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test8.txt
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test8b.json
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test8b.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test9.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test9_output.json
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test_simple_chains.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_instances/test_simple_chains.txt
--rw-rw-rw-   0 root         (0) root         (0)    10969 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_output.py
--rw-rw-rw-   0 root         (0) root         (0)     8826 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     4097 2023-04-20 14:38:57.000000 kep_solver-2.1.2/tests/test_statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.759134 kep_solver-2.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-06 14:01:29.000000 kep_solver-2.1.3/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-06 14:01:29.000000 kep_solver-2.1.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-07-06 14:01:29.000000 kep_solver-2.1.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-06 14:01:29.000000 kep_solver-2.1.3/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     5003 2023-07-06 14:01:29.000000 kep_solver-2.1.3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     8779 2023-07-06 14:01:29.000000 kep_solver-2.1.3/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    34462 2023-07-06 14:01:29.000000 kep_solver-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-07-06 14:01:38.760134 kep_solver-2.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4482 2023-07-06 14:01:29.000000 kep_solver-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.741134 kep_solver-2.1.3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-06 14:01:29.000000 kep_solver-2.1.3/docs/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-06 14:01:29.000000 kep_solver-2.1.3/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-07-06 14:01:29.000000 kep_solver-2.1.3/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-06 14:01:29.000000 kep_solver-2.1.3/docs/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.742134 kep_solver-2.1.3/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)    11079 2023-07-06 14:01:29.000000 kep_solver-2.1.3/docs/source/formats.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-07-06 14:01:29.000000 kep_solver-2.1.3/docs/source/terms.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-06 14:01:29.000000 kep_solver-2.1.3/docs/source/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.743134 kep_solver-2.1.3/kep_solver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 14:01:30.000000 kep_solver-2.1.3/kep_solver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21630 2023-07-06 14:01:29.000000 kep_solver-2.1.3/kep_solver/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     9106 2023-07-06 14:01:29.000000 kep_solver-2.1.3/kep_solver/fileio.py
+-rw-rw-rw-   0 root         (0) root         (0)    35880 2023-07-06 14:01:29.000000 kep_solver-2.1.3/kep_solver/generation.py
+-rw-rw-rw-   0 root         (0) root         (0)    23791 2023-07-06 14:01:29.000000 kep_solver-2.1.3/kep_solver/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    19222 2023-07-06 14:01:29.000000 kep_solver-2.1.3/kep_solver/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7152 2023-07-06 14:01:29.000000 kep_solver-2.1.3/kep_solver/pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.744134 kep_solver-2.1.3/kep_solver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-07-06 14:01:38.000000 kep_solver-2.1.3/kep_solver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-07-06 14:01:38.000000 kep_solver-2.1.3/kep_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:01:38.000000 kep_solver-2.1.3/kep_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-06 14:01:38.000000 kep_solver-2.1.3/kep_solver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-06 14:01:38.000000 kep_solver-2.1.3/kep_solver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-06 14:01:29.000000 kep_solver-2.1.3/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.744134 kep_solver-2.1.3/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)     6159 2023-07-06 14:01:29.000000 kep_solver-2.1.3/notebooks/Match Run.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2023-07-06 14:01:29.000000 kep_solver-2.1.3/notebooks/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    23889 2023-07-06 14:01:29.000000 kep_solver-2.1.3/notebooks/Statistical Analysis.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.745134 kep_solver-2.1.3/paper/
+-rw-rw-rw-   0 root         (0) root         (0)     2848 2023-07-06 14:01:29.000000 kep_solver-2.1.3/paper/paper.bib
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-07-06 14:01:29.000000 kep_solver-2.1.3/paper/paper.md
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-06 14:01:29.000000 kep_solver-2.1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-06 14:01:29.000000 kep_solver-2.1.3/runtime.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-07-06 14:01:38.760134 kep_solver-2.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-06 14:01:29.000000 kep_solver-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.746134 kep_solver-2.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5344 2023-07-06 14:01:29.000000 kep_solver-2.1.3/tests/test_fileio.py
+-rw-rw-rw-   0 root         (0) root         (0)    22082 2023-07-06 14:01:29.000000 kep_solver-2.1.3/tests/test_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    16083 2023-07-06 14:01:29.000000 kep_solver-2.1.3/tests/test_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:01:38.759134 kep_solver-2.1.3/tests/test_instances/
+-rw-rw-rw-   0 root         (0) root         (0)   514090 2023-07-06 14:01:29.000000 kep_solver-2.1.3/tests/test_instances/large-1.json
+-rw-rw-rw-   0 root         (0) root         (0)   590458 2023-07-06 14:01:29.000000 kep_solver-2.1.3/tests/test_instances/large-10.json
+-rw-rw-rw-   0 root         (0) root         (0)   610079 2023-07-06 14:01:29.000000 kep_solver-2.1.3/tests/test_instances/large-2.json
+-rw-rw-rw-   0 root         (0) root         (0)   590792 2023-07-06 14:01:29.000000 kep_solver-2.1.3/tests/test_instances/large-3.json
+-rw-rw-rw-   0 root         (0) root         (0)   550366 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/large-4.json
+-rw-rw-rw-   0 root         (0) root         (0)   575193 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/large-5.json
+-rw-rw-rw-   0 root         (0) root         (0)   660843 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/large-6.json
+-rw-rw-rw-   0 root         (0) root         (0)   665457 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/large-7.json
+-rw-rw-rw-   0 root         (0) root         (0)   684308 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/large-8.json
+-rw-rw-rw-   0 root         (0) root         (0)   686677 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/large-9.json
+-rw-rw-rw-   0 root         (0) root         (0)    40468 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-1.json
+-rw-rw-rw-   0 root         (0) root         (0)    32770 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-10.json
+-rw-rw-rw-   0 root         (0) root         (0)    43595 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-2.json
+-rw-rw-rw-   0 root         (0) root         (0)    33837 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-3.json
+-rw-rw-rw-   0 root         (0) root         (0)    34664 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-4.json
+-rw-rw-rw-   0 root         (0) root         (0)    38406 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-5.json
+-rw-rw-rw-   0 root         (0) root         (0)    33991 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-6.json
+-rw-rw-rw-   0 root         (0) root         (0)    35438 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-7.json
+-rw-rw-rw-   0 root         (0) root         (0)    37158 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-8.json
+-rw-rw-rw-   0 root         (0) root         (0)    46046 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/medium-9.json
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test1.json
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test1.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test1.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test10.json
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test10_output.json
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test1_output.json
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test2.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test2.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test2.xml
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test3.json
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test3.txt
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test3.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test3b.json
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test3b.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test3b.xml
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test4.json
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test4.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test4.xml
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test5.json
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test5.txt
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test5.xml
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test5b.json
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test5b.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test6.txt
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test6a.json
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test6a.xml
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test6b.json
+-rw-rw-rw-   0 root         (0) root         (0)      950 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test6b.xml
+-rw-rw-rw-   0 root         (0) root         (0)   116023 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test7.json
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test7.txt
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test8.json
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test8.txt
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test8b.json
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test8b.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test9.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test9_output.json
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test_simple_chains.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_instances/test_simple_chains.txt
+-rw-rw-rw-   0 root         (0) root         (0)    10969 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     8826 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2023-07-06 14:01:30.000000 kep_solver-2.1.3/tests/test_statistics.py
```

### Comparing `kep_solver-2.1.2/.gitlab-ci.yml` & `kep_solver-2.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/CHANGELOG.md` & `kep_solver-2.1.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 ## [Unreleased]
 
+## [2.1.3]
+
+- Add Instance.writeFile() and Instance.writeFileJson() methods for writing
+	instances to files. So far only the NHSBT JSON format is supported.
+- Fix DonorCountGenerator to not expect integers as keys in JSON. JSON doesn't
+	allow integers as keys, so expect the keys to be string representations of
+	integers instead.
+- Fix reading of FloatGenerator from JSON when a single floating point number
+	has a chance of occuring.
+
 ## [2.1.2]
 
 - RecipientGenerator now links a donor to their recipient correctly
 - CompatibilityGraph.findCycles() speed-ups
 - CompatibilityGraph.findChains() speed-ups
 - Cache Vertex.adjacent() list and hash(Exchange)
 - Update python version for notebooks
```

### Comparing `kep_solver-2.1.2/CONTRIBUTING.md` & `kep_solver-2.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/LICENSE` & `kep_solver-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/PKG-INFO` & `kep_solver-2.1.3/kep_solver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kep_solver
-Version: 2.1.2
+Name: kep-solver
+Version: 2.1.3
 Summary: A Python package for reading and solving single instances of kidney exchange problems.
 Home-page: https://gitlab.com/wpettersson/kep_solver
 Author: William Pettersson
 Author-email: william@ewpettersson.se
 License: AGPLv3
 Keywords: kidney kidney_exchange
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kep_solver-2.1.2/README.md` & `kep_solver-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/docs/Makefile` & `kep_solver-2.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/docs/conf.py` & `kep_solver-2.1.3/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('..'))
 
 
 # -- Project information ----------------------------------------------
 
 project = 'kep_solver'
-copyright = '2021, William Pettersson'
+copyright = '2023, William Pettersson'
 author = 'William Pettersson'
 
 
 # -- General configuration --------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -41,14 +41,19 @@
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 source_suffix = [".rst", ".md"]
 
+autodoc_default_options = {
+    'members': True,
+    'member-order': 'bysource',
+    'special-members': '__init__'
+}
 
 def run_apidoc(_):
     from sphinx.ext.apidoc import main
     import os
     import sys
     sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
     cur_dir = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `kep_solver-2.1.2/docs/source/formats.rst` & `kep_solver-2.1.3/docs/source/formats.rst`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/docs/source/terms.rst` & `kep_solver-2.1.3/docs/source/terms.rst`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/docs/source/usage.rst` & `kep_solver-2.1.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/kep_solver/entities.py` & `kep_solver-2.1.3/kep_solver/entities.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from __future__ import annotations
 
 from collections import defaultdict
 from collections.abc import ValuesView
 from enum import Enum
+import json
 from typing import Optional, Union
 
 import pandas  # type: ignore
 
 # We need numpy for NaN, as pandas won't allow None as a categorical data type,
 # but will allow NaN
 import numpy  # type: ignore
@@ -364,14 +365,18 @@
         return self._recipient
 
     @property
     def weight(self) -> float:
         return self._weight
 
 
+class OutputFormat(Enum):
+    JSON = 1
+
+
 class Instance:
     """A KEP instance."""
 
     def __init__(self) -> None:
         """Create a new KEP instance."""
         self._donors: dict[str, Donor] = {}
         self._recips: dict[str, Recipient] = {}
@@ -453,14 +458,75 @@
         :return: the donor
         """
         return self._donors[id]
 
     def transplants(self) -> list[Transplant]:
         return self._transplants
 
+    def writeFile(self, filename: str, file_format: OutputFormat) -> None:
+        """Write the instance to a file of the given format.
+
+        :param filename: The name of the file to write
+        :param file_format: The file format to use. Currenly only JSON is
+            supported
+        """
+        if file_format == OutputFormat.JSON:
+            self.writeFileJson(filename)
+
+    def writeFileJson(self, filename: str, write_recipients: bool = False) -> None:
+        """Write the instance to a JSON file, where recipient data (e.g., blood
+        types and cPRA of recipients) are included only if the parameter
+        write_recipients is True
+
+        :param filename: The name of the file to write
+        :param write_recipients: If True, also write the recipient data to the file
+        """
+
+        def mkdonor(donor: Donor):
+            result = {
+                "sources": [int(donor.recipient.id)],
+                "dage": donor.age,
+                "matches": [
+                    {"recipient": int(t.recipient.id), "score": t.weight}
+                    for t in donor.transplants()
+                ],
+            }
+            try:
+                result["bloodtype"] = str(donor.bloodGroup)
+            except KEPDataValidationException:
+                # If blood group is not known, don't try to write it
+                pass
+            return result
+
+        data = {str(donor.id): mkdonor(donor) for donor in self.donors()}
+        output = {"data": data}
+
+        def mkrecipient(recipient: Recipient):
+            result: dict[str, Union[str, float]] = {}
+            try:
+                result["pra"] = recipient.cPRA
+            except KEPDataValidationException:
+                # If cPRA is not known, don't try to write it
+                pass
+            try:
+                result["bloodgroup"] = str(recipient.bloodGroup)
+            except KEPDataValidationException:
+                # If blood group is not known, don't try to write it
+                pass
+            return result
+
+        if write_recipients:
+            output["recipients"] = {
+                str(recipient.id): mkrecipient(recipient)
+                for recipient in self.recipients()
+            }
+
+        with open(filename, "w") as outfile:
+            json.dump(output, outfile)
+
 
 class InstanceSet:
     """A set of instances that can be analysed for statistical properties."""
 
     def __init__(self, instances: list[Instance]):
         """Constructor for InstanceSet.
```

### Comparing `kep_solver-2.1.2/kep_solver/fileio.py` & `kep_solver-2.1.3/kep_solver/fileio.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/kep_solver/generation.py` & `kep_solver-2.1.3/kep_solver/generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,16 @@
         """Create a DonorCountGenerator from a JSON object. The JSON
         object should be a dictionary of key, value pairs where each key is a
         is an integer, and the corresponding value is the proportion of recipients
         with that number of donors.
         """
         num = 1
         dists = {}
-        while num in json_obj:
-            dists[num] = json_obj[num]
+        while str(num) in json_obj:
+            dists[num] = json_obj[str(num)]
             num += 1
         if not dists:
             raise Exception(
                 f"Parsing JSON for DonorCountGenerator failed: No donor counts found."
             )
         return cls(dists)
 
@@ -347,15 +347,16 @@
         """
         bands = {}
         for band in json_obj:
             entry, chance = band
             try:
                 low, high = entry
             except (
-                ValueError
+                ValueError,
+                TypeError,
             ):  # Only one value in list, must be both low and high value
                 low = entry
                 high = entry
             bands[(low, high)] = chance
         return cls(bands=bands)
```

### Comparing `kep_solver-2.1.2/kep_solver/graph.py` & `kep_solver-2.1.3/kep_solver/graph.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/kep_solver/model.py` & `kep_solver-2.1.3/kep_solver/model.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/kep_solver/pool.py` & `kep_solver-2.1.3/kep_solver/pool.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/kep_solver.egg-info/PKG-INFO` & `kep_solver-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kep-solver
-Version: 2.1.2
+Name: kep_solver
+Version: 2.1.3
 Summary: A Python package for reading and solving single instances of kidney exchange problems.
 Home-page: https://gitlab.com/wpettersson/kep_solver
 Author: William Pettersson
 Author-email: william@ewpettersson.se
 License: AGPLv3
 Keywords: kidney kidney_exchange
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kep_solver-2.1.2/kep_solver.egg-info/SOURCES.txt` & `kep_solver-2.1.3/kep_solver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/notebooks/Match Run.ipynb` & `kep_solver-2.1.3/notebooks/Match Run.ipynb`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/notebooks/README.md` & `kep_solver-2.1.3/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/notebooks/Statistical Analysis.ipynb` & `kep_solver-2.1.3/notebooks/Statistical Analysis.ipynb`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/paper/paper.bib` & `kep_solver-2.1.3/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/paper/paper.md` & `kep_solver-2.1.3/paper/paper.md`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/setup.cfg` & `kep_solver-2.1.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 [options.extras_require]
 test = 
 	pytest
 	mypy>=0.800
 	black
 	pytest-cov
 docs = 
-	sphinx_rtd_theme
+	Sphinx<7
+	sphinx_rtd_theme==1.2.0
 	sphinx_autodoc_typehints
 	m2r2
 
 [options.packages.find]
 exclude = 
 	*test*
```

### Comparing `kep_solver-2.1.2/tests/test_generator.py` & `kep_solver-2.1.3/tests/test_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     numDonors = gen.draw()
     assert numDonors == 1
     numDonors = gen.draw()
     assert numDonors == 3
 
 
 def test_donor_count_gen_from_json():
-    dist = {1: 0.67, 2: 0.22, 3: 0.10, 4: 0.01}
+    dist = {"1": 0.67, "2": 0.22, "3": 0.10, "4": 0.01}
     gen = generation.DonorCountGenerator.from_json(dist)
     # With the forced seed, we test a bunch of draws until we at least see a 3.
     random.seed(SEED)
     numDonors = gen.draw()
     assert numDonors == 1
     numDonors = gen.draw()
     assert numDonors == 1
@@ -393,14 +393,31 @@
     ]
     float_bands = generation.FloatGenerator.from_json(json)
     # With the forced seed, we test a bunch of draws until we see all 4 values.
     random.seed(SEED)
     assert float_bands.draw() == 0.5
     assert float_bands.draw() == 1.0
     assert float_bands.draw() == 0.5
+    assert float_bands.draw() == 0.9
+    assert float_bands.draw() == 0.0
+
+
+def test_float_band_gen_from_json_single_value():
+    json = [
+        [0, 0.25],
+        [0.5, 0.25],
+        [0.9, 0.25],
+        [1.0, 0.25],
+    ]
+    float_bands = generation.FloatGenerator.from_json(json)
+    # With the forced seed, we test a bunch of draws until we see all 4 values.
+    random.seed(SEED)
+    assert float_bands.draw() == 0.5
+    assert float_bands.draw() == 1.0
+    assert float_bands.draw() == 0.5
     assert float_bands.draw() == 0.9
     assert float_bands.draw() == 0.0
 
 
 def test_float_band_gen_config():
     in_string = "0.25 0\n0.25 0.5\n0.25 0.9\n0.25 1\n"
     float_bands = generation.FloatGenerator(bandString=in_string)
```

### Comparing `kep_solver-2.1.2/tests/test_graph.py` & `kep_solver-2.1.3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-1.json` & `kep_solver-2.1.3/tests/test_instances/large-1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-10.json` & `kep_solver-2.1.3/tests/test_instances/large-10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-2.json` & `kep_solver-2.1.3/tests/test_instances/large-2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-3.json` & `kep_solver-2.1.3/tests/test_instances/large-3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-4.json` & `kep_solver-2.1.3/tests/test_instances/large-4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-5.json` & `kep_solver-2.1.3/tests/test_instances/large-5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-6.json` & `kep_solver-2.1.3/tests/test_instances/large-6.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-7.json` & `kep_solver-2.1.3/tests/test_instances/large-7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-8.json` & `kep_solver-2.1.3/tests/test_instances/large-8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/large-9.json` & `kep_solver-2.1.3/tests/test_instances/large-9.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-1.json` & `kep_solver-2.1.3/tests/test_instances/medium-1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-10.json` & `kep_solver-2.1.3/tests/test_instances/medium-10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-2.json` & `kep_solver-2.1.3/tests/test_instances/medium-2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-3.json` & `kep_solver-2.1.3/tests/test_instances/medium-3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-4.json` & `kep_solver-2.1.3/tests/test_instances/medium-4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-5.json` & `kep_solver-2.1.3/tests/test_instances/medium-5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-6.json` & `kep_solver-2.1.3/tests/test_instances/medium-6.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-7.json` & `kep_solver-2.1.3/tests/test_instances/medium-7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-8.json` & `kep_solver-2.1.3/tests/test_instances/medium-8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/medium-9.json` & `kep_solver-2.1.3/tests/test_instances/medium-9.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test1.json` & `kep_solver-2.1.3/tests/test_instances/test1.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test1.xml` & `kep_solver-2.1.3/tests/test_instances/test1.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test10.json` & `kep_solver-2.1.3/tests/test_instances/test10.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test10_output.json` & `kep_solver-2.1.3/tests/test_instances/test10_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test1_output.json` & `kep_solver-2.1.3/tests/test_instances/test1_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test2.json` & `kep_solver-2.1.3/tests/test_instances/test2.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test2.xml` & `kep_solver-2.1.3/tests/test_instances/test2.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test3.json` & `kep_solver-2.1.3/tests/test_instances/test3.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test3.xml` & `kep_solver-2.1.3/tests/test_instances/test3.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test3b.json` & `kep_solver-2.1.3/tests/test_instances/test3b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test3b.xml` & `kep_solver-2.1.3/tests/test_instances/test3b.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test4.json` & `kep_solver-2.1.3/tests/test_instances/test4.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test4.xml` & `kep_solver-2.1.3/tests/test_instances/test4.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test5.json` & `kep_solver-2.1.3/tests/test_instances/test5.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test5.xml` & `kep_solver-2.1.3/tests/test_instances/test5.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test6a.json` & `kep_solver-2.1.3/tests/test_instances/test6a.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test6a.xml` & `kep_solver-2.1.3/tests/test_instances/test6a.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test6b.json` & `kep_solver-2.1.3/tests/test_instances/test6b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test6b.xml` & `kep_solver-2.1.3/tests/test_instances/test6b.xml`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test7.json` & `kep_solver-2.1.3/tests/test_instances/test7.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test8.json` & `kep_solver-2.1.3/tests/test_instances/test8.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test8b.json` & `kep_solver-2.1.3/tests/test_instances/test8b.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_instances/test9_output.json` & `kep_solver-2.1.3/tests/test_instances/test9_output.json`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_model.py` & `kep_solver-2.1.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_output.py` & `kep_solver-2.1.3/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_pool.py` & `kep_solver-2.1.3/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `kep_solver-2.1.2/tests/test_statistics.py` & `kep_solver-2.1.3/tests/test_statistics.py`

 * *Files identical despite different names*

