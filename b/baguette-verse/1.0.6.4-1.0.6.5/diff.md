# Comparing `tmp/baguette_verse-1.0.6.4.tar.gz` & `tmp/baguette_verse-1.0.6.5.tar.gz`

## Comparing `baguette_verse-1.0.6.4.tar` & `baguette_verse-1.0.6.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/baguette.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/logger.py
--rw-r--r--   0        0        0    17676 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/rack.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/__init__.py
--rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/bake.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/compiler.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    33988 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/utils.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/__proc__.py
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/entities.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/integration.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/relations.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/data/utils.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/__proc__.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/entities.py
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/integration.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/relations.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/utils.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/__proc__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/entities.py
--rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/integration.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/relations.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/__proc__.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/entities.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/integration.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/relations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/__proc__.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/entities.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/integration.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/network/relations.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/__proc__.py
--rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/entities.py
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/integration.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/relations.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/extractor.py
--rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/toast.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/source/evaluator.py
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/tutorial/data.zip
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/tutorial/scripts.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/tutorial/state.txt
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/baguette/tutorial/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/LICENSE
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/README.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/pyproject.toml
--rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/baguette.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/logger.py
+-rw-r--r--   0        0        0    17676 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/rack.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/bake.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    34843 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/toast.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/source/evaluator.py
+-rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/tutorial/data.zip
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/tutorial/scripts.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/tutorial/state.txt
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/baguette/tutorial/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/LICENSE
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.5/PKG-INFO
```

### Comparing `baguette_verse-1.0.6.4/baguette/baguette.py` & `baguette_verse-1.0.6.5/baguette/baguette.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/logger.py` & `baguette_verse-1.0.6.5/baguette/logger.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/rack.py` & `baguette_verse-1.0.6.5/baguette/rack.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/bake.py` & `baguette_verse-1.0.6.5/baguette/bakery/bake.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/compiler.py` & `baguette_verse-1.0.6.5/baguette/bakery/compiler.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/build.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/build.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/colors.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/colors.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/config.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/config.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/event.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/event.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/filters.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/filters.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/graph.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This module defines all graph-related base classes.
 Look at the classes Vertex, Edge, Arrow and Graph.
 Vertex, Edge and Arrow classes are heavily subclasses in BAGUETTE. Look at package 'baguette.bakery.source.types' to know more.
 """
 
 from threading import RLock, Thread
 from typing import Any, Callable, Iterable, Iterator, Optional, TypeVar, Union
+from weakref import WeakKeyDictionary
 from .colors import Color
 from .config import ColorSetting, SizeSetting, SwitchSetting, WeightSetting
 from Viper.meta.iterable import InstanceReferencingClass
 
 __all__ = ["Vertex", "UniqueVertex", "Edge", "Arrow", "Graph", "find_or_create"]
 
 
@@ -564,46 +565,56 @@
 
     __slots__ = {
         "vertices" : "The set of vertices in this graph",
         "edges" : "The set of edges in this graph",
         "data" : "A dictionary holding additional data for this graph"
     }
 
-    __active_graphs : dict[Thread, list["Graph"]] = {}
+    __active_graphs : WeakKeyDictionary[Thread, dict["Graph", bool]] = WeakKeyDictionary()
 
     def __init__(self) -> None:
         from typing import Any
         self.vertices : set[Vertex] = set()
         self.edges : set[Edge] = set()
         self.data : dict[str, Any] = {}
     
     def __enter__(self):
         """
         Implements with self.
         """
         from threading import current_thread
         if current_thread() not in Graph.__active_graphs:
-            Graph.__active_graphs[current_thread()] = []
-        Graph.__active_graphs[current_thread()].append(self)
+            Graph.__active_graphs[current_thread()] = {}
+        Graph.__active_graphs[current_thread()][self] = True
     
     def __exit__(self, exc_type, exc_value, traceback):
         """
         Implements with self.
         """
         from threading import current_thread
-        Graph.__active_graphs[current_thread()].remove(self)
+        Graph.__active_graphs[current_thread()].pop(self)
     
     @staticmethod
     def active_graphs() -> list["Graph"]:
         """
         Returns the list of all the active Graphs in the current thread.
         """
         from threading import current_thread
         if current_thread() not in Graph.__active_graphs:
             return []
+        return [g for g, inserting in Graph.__active_graphs[current_thread()].items() if inserting]
+    
+    @staticmethod
+    def graphs_status() -> dict["Graph", bool]:
+        """
+        More advanced version of active_graphs. Returns a dictionary of Graphs that indicates if they are in auto_write mode.
+        """
+        from threading import current_thread
+        if current_thread() not in Graph.__active_graphs:
+            return {}
         return Graph.__active_graphs[current_thread()].copy()
 
     def add_vertex(self, v : Vertex, explore : bool = True) -> None:
         """
         Adds a vertex to the graph and explores from this vertex.
         """
         if not isinstance(v, Vertex):
@@ -768,20 +779,26 @@
             "data" : self.data
         }
 
     def __setstate__(self, state : dict[str, Any]):
         """
         Implements loading of self.
         """
-        for name, value in state.items():
-            setattr(self, name, value)
-        for v in self.vertices:
-            v.graph = self
-        for e in self.edges:
-            e.write()
+        from threading import current_thread
+        thread_dict = self.__active_graphs.get(current_thread(), default={})
+        thread_dict[self] = False       # This is a weak graph activation. It does not trigger auto_insertion.
+        try:
+            for name, value in state.items():
+                setattr(self, name, value)
+            for v in self.vertices:
+                v.graph = self
+            for e in self.edges:
+                e.write()
+        finally:
+            thread_dict.pop(self)
    
     # def __copy__(self) -> "graph":
     #     """
     #     Implements copy of self
     #     """
     #     from copy import copy
     #     translation = {u : copy(u) for u in self.vertices}
```

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/record.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/record.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/utils.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,19 @@
 def path_factory(path : str) -> pathlib.PurePath:
     """
     Returns the correct path factory class for the given graph (either WindowsPurePath or PosixPurePath).
     """
     from pathlib import PurePosixPath, PureWindowsPath
 
     from .graph import Graph
-    platform = Graph.active_graphs()[-1].data["platform"].lower() if Graph.active_graphs() else "windows"
+    platform = "windows"
+    for g in Graph.graphs_status():
+        if "platform" in g.data:
+            platform = g.data["platform"].lower()
+            break
     if "windows" in platform:
         return PureWindowsPath(path)
     else:
         return PurePosixPath(path)
 
 
 def is_path(s : str) -> bool:
@@ -89,15 +93,15 @@
     """
     Parses command line with the syntax of the current platform's shell. Returns the argument vector.
     """
     import re
 
     from .graph import Graph
 
-    platform = Graph.active_graphs()[-1].data["platform"].lower() if Graph.active_graphs() else "windows"
+    platform = Graph.active_graphs()[-1].data["platform"].lower() if Graph.active_graphs() and "platform" in Graph.active_graphs()[-1].data else "windows"
     if "windows" not in platform:
         RE_CMD_LEX = r'''"((?:\\["\\]|[^"])*)"|'([^']*)'|(\\.)|(&&?|\|\|?|\d?\>|[<])|([^\s'"\\&|<>]+)|(\s+)|(.)'''
     else:
         RE_CMD_LEX = r'''"((?:""|\\["\\]|[^"])*)"?()|(\\\\(?=\\*")|\\")|(&&?|\|\|?|\d?>|[<])|([^\s"&|<>]+)|(\s+)|(.)'''
 
     args : list[str] = []
     accu = None   # collects pieces of one arg
```

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/__init__.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/utils.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/data/entities.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/data/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/data/integration.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/data/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/data/relations.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/data/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/data/utils.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/data/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/entities.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/integration.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/relations.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/execution/utils.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/execution/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/entities.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/filesystem/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/integration.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/filesystem/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/filesystem/relations.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/filesystem/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/entities.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/imports/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/integration.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/imports/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/imports/relations.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/imports/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/network/entities.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/network/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/network/integration.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/network/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/network/relations.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/network/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/entities.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/registry/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/integration.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/registry/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/bakery/source/types/registry/relations.py` & `baguette_verse-1.0.6.5/baguette/bakery/source/types/registry/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/croutons/extractor.py` & `baguette_verse-1.0.6.5/baguette/croutons/extractor.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/croutons/toast.py` & `baguette_verse-1.0.6.5/baguette/croutons/toast.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/croutons/metalib/__init__.py` & `baguette_verse-1.0.6.5/baguette/croutons/metalib/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/croutons/metalib/interact.py` & `baguette_verse-1.0.6.5/baguette/croutons/metalib/interact.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/croutons/metalib/utils.py` & `baguette_verse-1.0.6.5/baguette/croutons/metalib/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/croutons/source/evaluator.py` & `baguette_verse-1.0.6.5/baguette/croutons/source/evaluator.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/croutons/source/metagraph.py` & `baguette_verse-1.0.6.5/baguette/croutons/source/metagraph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/croutons/source/utils.py` & `baguette_verse-1.0.6.5/baguette/croutons/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/tutorial/data.zip` & `baguette_verse-1.0.6.5/baguette/tutorial/data.zip`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/tutorial/scripts.py` & `baguette_verse-1.0.6.5/baguette/tutorial/scripts.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/baguette/tutorial/utils.py` & `baguette_verse-1.0.6.5/baguette/tutorial/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/.gitignore` & `baguette_verse-1.0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/LICENSE` & `baguette_verse-1.0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/README.md` & `baguette_verse-1.0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.4/pyproject.toml` & `baguette_verse-1.0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baguette-verse"
-version = "1.0.6.4"
+version = "1.0.6.5"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin@inria.fr" },
 ]
 description = "A malware behavioral analysis framework centered around BAGUETTE!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `baguette_verse-1.0.6.4/PKG-INFO` & `baguette_verse-1.0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 1.0.6.4
+Version: 1.0.6.5
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

