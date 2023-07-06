# Comparing `tmp/pychadwick-0.5.0.tar.gz` & `tmp/pychadwick-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychadwick-0.5.0.tar", last modified: Sat Feb  6 13:35:46 2021, max compression
+gzip compressed data, was "pychadwick-0.6.1.tar", last modified: Thu Jul  6 12:31:08 2023, max compression
```

## Comparing `pychadwick-0.5.0.tar` & `pychadwick-0.6.1.tar`

### file list

```diff
@@ -1,66 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:46.020051 pychadwick-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (116)      432 2021-02-06 13:35:33.000000 pychadwick-0.5.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (116)    18092 2021-02-06 13:35:33.000000 pychadwick-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      293 2021-02-06 13:35:33.000000 pychadwick-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      527 2021-02-06 13:35:33.000000 pychadwick-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     9592 2021-02-06 13:35:46.020051 pychadwick-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7627 2021-02-06 13:35:33.000000 pychadwick-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:46.012050 pychadwick-0.5.0/pychadwick/
--rw-r--r--   0 runner    (1001) docker     (116)     4797 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      513 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/book.py
--rw-r--r--   0 runner    (1001) docker     (116)     3863 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/box.py
--rw-r--r--   0 runner    (1001) docker     (116)     9817 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/chadwick.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:46.012050 pychadwick-0.5.0/pychadwick/cli/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2003 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/cli/pycwevent.py
--rw-r--r--   0 runner    (1001) docker     (116)     1094 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/experiments.py
--rw-r--r--   0 runner    (1001) docker     (116)     2292 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/game.py
--rw-r--r--   0 runner    (1001) docker     (116)     1513 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/gameiter.py
--rw-r--r--   0 runner    (1001) docker     (116)      212 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/league.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:46.016050 pychadwick-0.5.0/pychadwick/libutils/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/libutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      527 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/libutils/cwlib.py
--rw-r--r--   0 runner    (1001) docker     (116)     2996 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/parse.py
--rw-r--r--   0 runner    (1001) docker     (116)      637 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/roster.py
--rw-r--r--   0 runner    (1001) docker     (116)      467 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pychadwick/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)       70 2021-02-06 13:35:33.000000 pychadwick-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       60 2021-02-06 13:35:33.000000 pychadwick-0.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-06 13:35:33.000000 pychadwick-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       70 2021-02-06 13:35:33.000000 pychadwick-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1128 2021-02-06 13:35:33.000000 pychadwick-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:46.016050 pychadwick-0.5.0/src/
--rw-r--r--   0 runner    (1001) docker     (116)       56 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:46.016050 pychadwick-0.5.0/src/pychadwicklib/
--rw-r--r--   0 runner    (1001) docker     (116)    18092 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      113 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:46.016050 pychadwick-0.5.0/src/pychadwicklib/cwlib/
--rw-r--r--   0 runner    (1001) docker     (116)     6885 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/book.c
--rw-r--r--   0 runner    (1001) docker     (116)     3928 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/book.h
--rw-r--r--   0 runner    (1001) docker     (116)    49730 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/box.c
--rw-r--r--   0 runner    (1001) docker     (116)     5727 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/box.h
--rw-r--r--   0 runner    (1001) docker     (116)     1433 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/chadwick.h
--rw-r--r--   0 runner    (1001) docker     (116)     5105 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/file.c
--rw-r--r--   0 runner    (1001) docker     (116)     1894 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/file.h
--rw-r--r--   0 runner    (1001) docker     (116)    27663 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/game.c
--rw-r--r--   0 runner    (1001) docker     (116)     6729 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/game.h
--rw-r--r--   0 runner    (1001) docker     (116)    29908 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/gameiter.c
--rw-r--r--   0 runner    (1001) docker     (116)     5340 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/gameiter.h
--rw-r--r--   0 runner    (1001) docker     (116)     3978 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/league.c
--rw-r--r--   0 runner    (1001) docker     (116)     2593 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/league.h
--rw-r--r--   0 runner    (1001) docker     (116)     5066 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/lint.c
--rw-r--r--   0 runner    (1001) docker     (116)    60924 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/parse.c
--rw-r--r--   0 runner    (1001) docker     (116)     4485 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/parse.h
--rw-r--r--   0 runner    (1001) docker     (116)     7623 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/roster.c
--rw-r--r--   0 runner    (1001) docker     (116)     4332 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwlib/roster.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 13:35:46.020051 pychadwick-0.5.0/src/pychadwicklib/cwtools/
--rw-r--r--   0 runner    (1001) docker     (116)    24390 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwbox.c
--rw-r--r--   0 runner    (1001) docker     (116)    52983 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwboxsml.c
--rw-r--r--   0 runner    (1001) docker     (116)    15108 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwboxxml.c
--rw-r--r--   0 runner    (1001) docker     (116)     7209 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwcomment.c
--rw-r--r--   0 runner    (1001) docker     (116)    30812 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwdaily.c
--rw-r--r--   0 runner    (1001) docker     (116)    62661 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwevent.c
--rw-r--r--   0 runner    (1001) docker     (116)    60531 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwgame.c
--rw-r--r--   0 runner    (1001) docker     (116)     9665 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwsub.c
--rw-r--r--   0 runner    (1001) docker     (116)    10333 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/cwtools.c
--rw-r--r--   0 runner    (1001) docker     (116)     4532 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/xmlwrite.c
--rw-r--r--   0 runner    (1001) docker     (116)     4971 2021-02-06 13:35:33.000000 pychadwick-0.5.0/src/pychadwicklib/cwtools/xmlwrite.h
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.245691 pychadwick-0.6.1/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      432 2020-09-04 22:13:41.000000 pychadwick-0.6.1/CMakeLists.txt
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    18092 2020-09-04 22:13:41.000000 pychadwick-0.6.1/LICENSE
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      293 2020-09-04 22:13:41.000000 pychadwick-0.6.1/MANIFEST.in
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      527 2021-02-06 12:51:53.000000 pychadwick-0.6.1/Makefile
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     8147 2023-07-06 12:31:08.245691 pychadwick-0.6.1/PKG-INFO
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     7627 2020-09-04 22:13:41.000000 pychadwick-0.6.1/README.md
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.241691 pychadwick-0.6.1/pychadwick/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     4797 2023-07-06 12:20:13.000000 pychadwick-0.6.1/pychadwick/__init__.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      513 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/book.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     3863 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/box.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    10753 2023-07-06 11:37:59.000000 pychadwick-0.6.1/pychadwick/chadwick.py
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.241691 pychadwick-0.6.1/pychadwick/cli/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)        0 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/cli/__init__.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     2003 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/cli/pycwevent.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     1094 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/experiments.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     2292 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/game.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     1513 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/gameiter.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      212 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/league.py
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.241691 pychadwick-0.6.1/pychadwick/libutils/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)       74 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/libutils/__init__.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      529 2023-07-06 11:37:59.000000 pychadwick-0.6.1/pychadwick/libutils/cwlib.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     2996 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/parse.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      637 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/roster.py
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      467 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pychadwick/utils.py
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.241691 pychadwick-0.6.1/pychadwick.egg-info/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     8147 2023-07-06 12:31:08.000000 pychadwick-0.6.1/pychadwick.egg-info/PKG-INFO
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     1721 2023-07-06 12:31:08.000000 pychadwick-0.6.1/pychadwick.egg-info/SOURCES.txt
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)        1 2023-07-06 12:31:08.000000 pychadwick-0.6.1/pychadwick.egg-info/dependency_links.txt
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)       61 2023-07-06 12:31:08.000000 pychadwick-0.6.1/pychadwick.egg-info/entry_points.txt
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)       65 2023-07-06 12:31:08.000000 pychadwick-0.6.1/pychadwick.egg-info/requires.txt
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)       11 2023-07-06 12:31:08.000000 pychadwick-0.6.1/pychadwick.egg-info/top_level.txt
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)       70 2020-09-04 22:13:41.000000 pychadwick-0.6.1/pyproject.toml
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)       29 2023-07-06 11:37:59.000000 pychadwick-0.6.1/requirements-dev.txt
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)       40 2023-07-06 11:37:59.000000 pychadwick-0.6.1/requirements.txt
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      109 2023-07-06 12:31:08.249691 pychadwick-0.6.1/setup.cfg
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     1128 2023-07-06 12:20:11.000000 pychadwick-0.6.1/setup.py
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.241691 pychadwick-0.6.1/src/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)       56 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/Makefile
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.241691 pychadwick-0.6.1/src/pychadwicklib/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    18092 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/LICENSE
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)      113 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/Makefile
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.245691 pychadwick-0.6.1/src/pychadwicklib/cwlib/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     6885 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/book.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     3928 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/book.h
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    49730 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/box.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     5727 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/box.h
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     1433 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/chadwick.h
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     5105 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/file.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     1894 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/file.h
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    27663 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/game.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     6729 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/game.h
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    29908 2020-10-04 16:19:06.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/gameiter.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     5340 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/gameiter.h
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     3978 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/league.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     2593 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/league.h
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     5066 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/lint.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    60924 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/parse.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     4485 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/parse.h
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     7623 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/roster.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     4332 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwlib/roster.h
+drwxrwxr-x   0 bdilday   (1000) bdilday   (1000)        0 2023-07-06 12:31:08.245691 pychadwick-0.6.1/src/pychadwicklib/cwtools/
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    24390 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwbox.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    52983 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwboxsml.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    15108 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwboxxml.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     7209 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwcomment.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    30812 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwdaily.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    62661 2020-10-04 16:19:06.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwevent.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    60531 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwgame.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     9665 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwsub.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)    10333 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/cwtools.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     4532 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/xmlwrite.c
+-rw-rw-r--   0 bdilday   (1000) bdilday   (1000)     4971 2020-09-04 22:13:41.000000 pychadwick-0.6.1/src/pychadwicklib/cwtools/xmlwrite.h
```

### Comparing `pychadwick-0.5.0/LICENSE` & `pychadwick-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/Makefile` & `pychadwick-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/README.md` & `pychadwick-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/pychadwick/__init__.py` & `pychadwick-0.6.1/pychadwick/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pandas import Int32Dtype
 from pychadwick.libutils import ChadwickLibrary
 
 
-_version = "0.5.0"
+_version = "0.6.1"
 
 __all__ = ["ChadwickLibrary"]
 
 nullable_int = Int32Dtype()
 
 EVENT_DATA_TYPES = {
     "GAME_ID": str,
```

### Comparing `pychadwick-0.5.0/pychadwick/book.py` & `pychadwick-0.6.1/pychadwick/book.py`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/pychadwick/box.py` & `pychadwick-0.6.1/pychadwick/box.py`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/pychadwick/chadwick.py` & `pychadwick-0.6.1/pychadwick/chadwick.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from pychadwick.league import CWLeague
 from pychadwick.game import CWGame
 from pychadwick.gameiter import CWGameIterator
 from pychadwick.roster import CWRoster
 from pychadwick.utils import CWEventFieldStruct
 from pychadwick import EVENT_DATA_TYPES, ChadwickLibrary
 
+logger = logging.getLogger(__name__)
+
 
 class Chadwick:
     FIELDS_COUNT = 96
     EXT_FIELDS_COUNT = 63
 
     def __init__(self, *args, **kwargs):
         self.libchadwick = ChadwickLibrary.libchadwick
@@ -224,45 +226,66 @@
     def cw_gameiter_create(self, game_ptr):
         func = self.libchadwick.cw_gameiter_create
         func.restype = POINTER(CWGameIterator)
         func.argtypes = (POINTER(CWGame),)
         return func(game_ptr)
 
     @staticmethod
+    def _convert_int32(ser: pd.Series, data_type_conversion):
+        """
+        workaround for pandas < 2 where a string like "1" cannot be converted
+        directly to a Int32
+        """
+        try:
+            converted_values = ser.astype(data_type_conversion)
+        except TypeError:
+            converted_values = ser.astype(int).astype(data_type_conversion)
+
+        return converted_values
+
+    @staticmethod
     def convert_data_frame_types(df, data_type_mapping):
         for column_name, data_type_conversion in data_type_mapping.items():
             if column_name in df:
                 try:
-                    df.loc[:, column_name] = df.loc[:, column_name].astype(
-                        data_type_conversion
+                    converted_values = (
+                        Chadwick._convert_int32(
+                            df.loc[:, column_name], data_type_conversion
+                        )
+                        if str(data_type_conversion).startswith("Int")
+                        else df.loc[:, column_name].astype(data_type_conversion)
                     )
+                    df.loc[:, column_name] = converted_values
                 except TypeError:
-                    print(f"Cannot convert column {column_name}")
-                    print(df.loc[:column_name])
+                    logger.error(
+                        f"Cannot convert column {column_name} to data_type {data_type_conversion}"
+                    )
+                    logger.error(df.loc[:, column_name].describe())
                     raise TypeError
         return df
 
     def games_to_dataframe(self, games, data_type_mapping=None):
         if data_type_mapping is None:
             data_type_mapping = EVENT_DATA_TYPES
-        dfs = [
-            pd.DataFrame(list(self.process_game(game_ptr)), dtype="f8")
-            for game_ptr in games
-        ]
+        try:
+            dfs = [
+                pd.DataFrame(list(self.process_game(game_ptr)), dtype=None)
+                for game_ptr in games
+            ]
+        except TypeError:  # pandas < 2 compatibility
+            dfs = [
+                pd.DataFrame(list(self.process_game(game_ptr)), dtype="f8")
+                for game_ptr in games
+            ]
         return self.convert_data_frame_types(
             pd.concat(dfs, axis=0, ignore_index=True), data_type_mapping
         )
 
     def game_to_dataframe(self, game_ptr, data_type_mapping=None):
-        if data_type_mapping is None:
-            data_type_mapping = EVENT_DATA_TYPES
-        return self.convert_data_frame_types(
-            pd.DataFrame(list(self.process_game(game_ptr)), dtype="f8"),
-            data_type_mapping,
-        )
+        return self.games_to_dataframe([game_ptr], data_type_mapping=data_type_mapping)
 
     def event_file_to_dataframe(self, event_file, data_type_mapping=None):
         if data_type_mapping is None:
             data_type_mapping = EVENT_DATA_TYPES
         return self.games_to_dataframe(self.games(event_file), data_type_mapping)
 
     def event_files_to_dataframe(self, event_files, data_type_mapping=None):
@@ -270,15 +293,16 @@
             data_type_mapping = EVENT_DATA_TYPES
         data = []
         for event_file in event_files:
             games = self.games(event_file)
             for game in games:
                 data += list(self.process_game(game))
         return self.convert_data_frame_types(
-            pd.DataFrame(data, dtype="f8"), data_type_mapping,
+            pd.DataFrame(data, dtype="f8"),
+            data_type_mapping,
         )
 
     def register_function(self, func_name, func_arg_types, func_res_type):
         func = self.libchadwick.__getattr__(func_name)
         func.argtypes = func_arg_types
         func.restype = func_res_type
         self.__dict__[func_name] = func
```

### Comparing `pychadwick-0.5.0/pychadwick/cli/pycwevent.py` & `pychadwick-0.6.1/pychadwick/cli/pycwevent.py`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/pychadwick/experiments.py` & `pychadwick-0.6.1/pychadwick/experiments.py`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/pychadwick/game.py` & `pychadwick-0.6.1/pychadwick/game.py`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/pychadwick/gameiter.py` & `pychadwick-0.6.1/pychadwick/gameiter.py`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/pychadwick/libutils/cwlib.py` & `pychadwick-0.6.1/pychadwick/libutils/cwlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import ctypes
 import pathlib
 import sys
 
 FILE_EXTENSION = {"darwin": "dylib", "linux": "so", "windows": "dll"}
+
+
 class _ChadwickLibrary:
     library_path = (
         pathlib.Path(__file__).absolute().parent.parent
         / "lib"
         / "cwevent"
         / f"libcwevent.{FILE_EXTENSION.get(sys.platform)}"
     )
```

### Comparing `pychadwick-0.5.0/pychadwick/parse.py` & `pychadwick-0.6.1/pychadwick/parse.py`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/pychadwick/roster.py` & `pychadwick-0.6.1/pychadwick/roster.py`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/setup.py` & `pychadwick-0.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(
     name="pychadwick",
-    version="0.5.0",
+    version="0.6.1",
     author="Ben Dilday",
     author_email="ben.dilday.phd@gmail.com",
     description="Python bindings to the Chadwick library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bdilday/pychadwick",
     packages=find_packages(),
```

### Comparing `pychadwick-0.5.0/src/pychadwicklib/LICENSE` & `pychadwick-0.6.1/src/pychadwicklib/LICENSE`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/book.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/book.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/book.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/book.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/box.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/box.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/box.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/box.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/chadwick.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/chadwick.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/file.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/file.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/file.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/file.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/game.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/game.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/game.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/game.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/gameiter.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/gameiter.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/gameiter.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/gameiter.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/league.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/league.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/league.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/league.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/lint.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/lint.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/parse.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/parse.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/parse.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/parse.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/roster.c` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/roster.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwlib/roster.h` & `pychadwick-0.6.1/src/pychadwicklib/cwlib/roster.h`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwbox.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwbox.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwboxsml.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwboxsml.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwboxxml.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwboxxml.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwcomment.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwcomment.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwdaily.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwdaily.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwevent.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwevent.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwgame.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwgame.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwsub.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwsub.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/cwtools.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/cwtools.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/xmlwrite.c` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/xmlwrite.c`

 * *Files identical despite different names*

### Comparing `pychadwick-0.5.0/src/pychadwicklib/cwtools/xmlwrite.h` & `pychadwick-0.6.1/src/pychadwicklib/cwtools/xmlwrite.h`

 * *Files identical despite different names*

