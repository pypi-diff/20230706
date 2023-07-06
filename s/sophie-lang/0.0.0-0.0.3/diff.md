# Comparing `tmp/sophie-lang-0.0.0.tar.gz` & `tmp/sophie-lang-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sophie-lang-0.0.0.tar", last modified: Thu Jun 15 04:28:24 2023, max compression
+gzip compressed data, was "sophie-lang-0.0.3.tar", last modified: Thu Jul  6 04:27:40 2023, max compression
```

## Comparing `sophie-lang-0.0.0.tar` & `sophie-lang-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 04:28:24.629052 sophie-lang-0.0.0/
--rw-rw-rw-   0        0        0     1086 2022-10-16 03:53:26.000000 sophie-lang-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     4704 2023-06-15 04:28:24.629052 sophie-lang-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3855 2023-05-18 05:11:14.000000 sophie-lang-0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 04:28:24.629052 sophie-lang-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1319 2023-06-15 04:27:34.000000 sophie-lang-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:28:24.619178 sophie-lang-0.0.0/sophie/
--rw-rw-rw-   0        0        0    17199 2023-06-13 04:39:22.000000 sophie-lang-0.0.0/sophie/Sophie.automaton
--rw-rw-rw-   0        0        0        0 2022-10-09 04:11:54.000000 sophie-lang-0.0.0/sophie/__init__.py
--rw-rw-rw-   0        0        0     1621 2023-05-07 05:56:11.000000 sophie-lang-0.0.0/sophie/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:28:24.619178 sophie-lang-0.0.0/sophie/adapters/
--rw-rw-rw-   0        0        0        0 2023-05-08 04:47:45.000000 sophie-lang-0.0.0/sophie/adapters/__init__.py
--rw-rw-rw-   0        0        0     1024 2023-06-14 04:52:15.000000 sophie-lang-0.0.0/sophie/adapters/game_adapter.py
--rw-rw-rw-   0        0        0      728 2023-06-14 04:48:54.000000 sophie-lang-0.0.0/sophie/adapters/teletype_adapter.py
--rw-rw-rw-   0        0        0     1120 2023-06-14 04:52:15.000000 sophie-lang-0.0.0/sophie/adapters/turtle_adapter.py
--rw-rw-rw-   0        0        0      493 2023-05-13 05:50:12.000000 sophie-lang-0.0.0/sophie/adapters/yarn.py
--rw-rw-rw-   0        0        0     9026 2023-06-13 22:24:27.000000 sophie-lang-0.0.0/sophie/calculus.py
--rw-rw-rw-   0        0        0     4594 2023-06-14 04:58:39.000000 sophie-lang-0.0.0/sophie/diagnostics.py
--rw-rw-rw-   0        0        0     5431 2023-06-07 07:25:47.000000 sophie-lang-0.0.0/sophie/front_end.py
--rw-rw-rw-   0        0        0     5141 2023-06-13 04:29:01.000000 sophie-lang-0.0.0/sophie/modularity.py
--rw-rw-rw-   0        0        0     1758 2023-06-13 22:24:39.000000 sophie-lang-0.0.0/sophie/ontology.py
--rw-rw-rw-   0        0        0     1976 2023-05-05 02:32:33.000000 sophie-lang-0.0.0/sophie/primitive.py
--rw-rw-rw-   0        0        0    20664 2023-05-29 06:51:12.000000 sophie-lang-0.0.0/sophie/resolution.py
--rw-rw-rw-   0        0        0     9677 2023-06-14 04:47:56.000000 sophie-lang-0.0.0/sophie/simple_evaluator.py
--rw-rw-rw-   0        0        0     1221 2023-06-14 04:26:06.000000 sophie-lang-0.0.0/sophie/stacking.py
--rw-rw-rw-   0        0        0    13457 2023-06-13 04:30:18.000000 sophie-lang-0.0.0/sophie/syntax.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:28:24.619178 sophie-lang-0.0.0/sophie/sys/
--rw-rw-rw-   0        0        0     1293 2023-06-13 03:48:23.000000 sophie-lang-0.0.0/sophie/sys/game.sg
--rw-rw-rw-   0        0        0     3565 2023-06-10 20:44:12.000000 sophie-lang-0.0.0/sophie/sys/preamble.sg
--rw-rw-rw-   0        0        0      476 2023-05-14 23:47:52.000000 sophie-lang-0.0.0/sophie/sys/teletype.sg
--rw-rw-rw-   0        0        0      524 2023-05-08 05:20:15.000000 sophie-lang-0.0.0/sophie/sys/turtle.sg
--rw-rw-rw-   0        0        0    20037 2023-06-14 04:37:53.000000 sophie-lang-0.0.0/sophie/type_evaluator.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:28:24.629052 sophie-lang-0.0.0/sophie_lang.egg-info/
--rw-rw-rw-   0        0        0     4704 2023-06-15 04:28:24.000000 sophie-lang-0.0.0/sophie_lang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      732 2023-06-15 04:28:24.000000 sophie-lang-0.0.0/sophie_lang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 04:28:24.000000 sophie-lang-0.0.0/sophie_lang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-15 04:28:24.000000 sophie-lang-0.0.0/sophie_lang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 04:28:24.000000 sophie-lang-0.0.0/sophie_lang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 04:27:40.231632 sophie-lang-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2022-10-16 03:53:26.000000 sophie-lang-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4712 2023-07-06 04:27:40.231632 sophie-lang-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3863 2023-07-03 23:37:35.000000 sophie-lang-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 04:27:40.231632 sophie-lang-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2023-07-06 04:26:41.000000 sophie-lang-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:27:40.210497 sophie-lang-0.0.3/sophie/
+-rw-rw-rw-   0        0        0    18045 2023-07-04 03:07:10.000000 sophie-lang-0.0.3/sophie/Sophie.automaton
+-rw-rw-rw-   0        0        0        0 2022-10-09 04:11:54.000000 sophie-lang-0.0.3/sophie/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-07-01 03:52:18.000000 sophie-lang-0.0.3/sophie/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:27:40.210497 sophie-lang-0.0.3/sophie/adapters/
+-rw-rw-rw-   0        0        0        0 2023-05-08 04:47:45.000000 sophie-lang-0.0.3/sophie/adapters/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-06-24 07:19:44.000000 sophie-lang-0.0.3/sophie/adapters/game_adapter.py
+-rw-rw-rw-   0        0        0      638 2023-07-01 05:59:40.000000 sophie-lang-0.0.3/sophie/adapters/teletype_adapter.py
+-rw-rw-rw-   0        0        0     1031 2023-06-24 07:19:44.000000 sophie-lang-0.0.3/sophie/adapters/turtle_adapter.py
+-rw-rw-rw-   0        0        0      493 2023-05-13 05:50:12.000000 sophie-lang-0.0.3/sophie/adapters/yarn.py
+-rw-rw-rw-   0        0        0     9275 2023-07-05 03:51:48.000000 sophie-lang-0.0.3/sophie/calculus.py
+-rw-rw-rw-   0        0        0     1660 2023-07-05 02:48:28.000000 sophie-lang-0.0.3/sophie/cmdline.py
+-rw-rw-rw-   0        0        0    11831 2023-07-05 04:39:51.000000 sophie-lang-0.0.3/sophie/diagnostics.py
+-rw-rw-rw-   0        0        0     3745 2023-07-02 23:17:57.000000 sophie-lang-0.0.3/sophie/executive.py
+-rw-rw-rw-   0        0        0     5140 2023-07-03 02:53:12.000000 sophie-lang-0.0.3/sophie/front_end.py
+-rw-rw-rw-   0        0        0     3353 2023-07-05 02:18:16.000000 sophie-lang-0.0.3/sophie/modularity.py
+-rw-rw-rw-   0        0        0     1602 2023-07-01 07:03:35.000000 sophie-lang-0.0.3/sophie/ontology.py
+-rw-rw-rw-   0        0        0     2015 2023-07-04 20:34:34.000000 sophie-lang-0.0.3/sophie/primitive.py
+-rw-rw-rw-   0        0        0    19107 2023-07-05 02:20:43.000000 sophie-lang-0.0.3/sophie/resolution.py
+-rw-rw-rw-   0        0        0    11034 2023-07-02 23:17:57.000000 sophie-lang-0.0.3/sophie/runtime.py
+-rw-rw-rw-   0        0        0     2943 2023-07-05 03:38:18.000000 sophie-lang-0.0.3/sophie/stacking.py
+-rw-rw-rw-   0        0        0    13577 2023-07-05 03:39:57.000000 sophie-lang-0.0.3/sophie/syntax.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:27:40.216006 sophie-lang-0.0.3/sophie/sys/
+-rw-rw-rw-   0        0        0     1290 2023-06-24 06:54:22.000000 sophie-lang-0.0.3/sophie/sys/game.sg
+-rw-rw-rw-   0        0        0     3565 2023-06-25 20:09:27.000000 sophie-lang-0.0.3/sophie/sys/preamble.sg
+-rw-rw-rw-   0        0        0      473 2023-06-24 08:56:28.000000 sophie-lang-0.0.3/sophie/sys/teletype.sg
+-rw-rw-rw-   0        0        0      519 2023-06-24 06:27:18.000000 sophie-lang-0.0.3/sophie/sys/turtle.sg
+-rw-rw-rw-   0        0        0    26812 2023-07-05 06:12:44.000000 sophie-lang-0.0.3/sophie/type_evaluator.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:27:40.231632 sophie-lang-0.0.3/sophie_lang.egg-info/
+-rw-rw-rw-   0        0        0     4712 2023-07-06 04:27:40.000000 sophie-lang-0.0.3/sophie_lang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-07-06 04:27:40.000000 sophie-lang-0.0.3/sophie_lang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 04:27:40.000000 sophie-lang-0.0.3/sophie_lang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-06 04:27:40.000000 sophie-lang-0.0.3/sophie_lang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2023-07-06 04:27:40.000000 sophie-lang-0.0.3/sophie_lang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 04:27:40.000000 sophie-lang-0.0.3/sophie_lang.egg-info/top_level.txt
```

### Comparing `sophie-lang-0.0.0/LICENSE` & `sophie-lang-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sophie-lang-0.0.0/PKG-INFO` & `sophie-lang-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophie-lang
-Version: 0.0.0
+Version: 0.0.3
 Summary: A call-by-need strong-inferred-type language named for French mathematician Sophie Germain
 Home-page: https://github.com/kjosib/sophie
 Author: Ian Kjos
 Author-email: kjosib@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -42,23 +42,14 @@
 this should not break too many brains. However, Sophie is an expression-oriented call-by-need language,
 so some things are bound look a bit more like SQL or Haskell.
 
 It may seem a small thing, but algebra-style parentheses are much more clear to me than Lisp or Haskell style.
 I think that's also true for most of the world's programmers.
 Things are better when the notation does not interfere with understanding.
 
-## Install/Run
-
-1. `pip install --upgrade booze-tools`
-2. Clone or download the repository.
-3. `py -m sophie examples/turtle.sg`
-
-Yes, it's implemented atop Python. For now. That's a key enabler, actually.
-Python pays the bills right now. C'est la vie.
-
 ## How do I Learn Sophie?
 
 1. [Read the docs](https://sophie.readthedocs.io)
 2. Poke around the [examples](https://github.com/kjosib/sophie/tree/main/examples) and [grammar](https://github.com/kjosib/sophie/blob/main/sophie/Sophie.md)
 3. Contribute to the docs in the usual way.
 
 It sure might be nice to have a *Learn computer science with Sophie*
@@ -73,15 +64,22 @@
 * Sophie has Turtle-graphics! (See [here](https://github.com/kjosib/sophie/blob/main/examples/turtle.sg) for examples.)
 * Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/guess_the_number.sg) as an example.
 * The new type-checker gives excellent feedback and cannot be fooled. Through abstract interpretation it completely rules out *type* errors.
   (Domain errors, such as division by zero, are still possible.)
 * The module system got an upgrade: there is now a notion of a system-package and the beginnings of a standard library.
 * The FFI (into Python): Sophie can call Python; Python can call Sophie; and Python can install I/O drivers into Sophie.
 * Error display is improved in various ways. There is also now an easy way to install helpful messages for parse errors.
-  This works; there just aren't many good messages yet.
+  This works surprisingly well now.
+
+*Caveat:* Type-checking is presently out of commission in HEAD, but the release has it working.
+
+Some things are in progress:
+
+* I'm in progress to add asynchronous message-passing, with an eye towards a safe concurrency model.
+  (That's why type-checking is temporarily turned off)
 
 Certain things are not started yet:
 
 * Variable-Arity Functions.
 * Ad-hoc polymorphic multi-methods.
 * List comprehension (expressions like `[expr FOR name IN expr]`) are removed from the syntax for now.
 * Asynchrony.
```

### Comparing `sophie-lang-0.0.0/README.md` & `sophie-lang-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,14 @@
 this should not break too many brains. However, Sophie is an expression-oriented call-by-need language,
 so some things are bound look a bit more like SQL or Haskell.
 
 It may seem a small thing, but algebra-style parentheses are much more clear to me than Lisp or Haskell style.
 I think that's also true for most of the world's programmers.
 Things are better when the notation does not interfere with understanding.
 
-## Install/Run
-
-1. `pip install --upgrade booze-tools`
-2. Clone or download the repository.
-3. `py -m sophie examples/turtle.sg`
-
-Yes, it's implemented atop Python. For now. That's a key enabler, actually.
-Python pays the bills right now. C'est la vie.
-
 ## How do I Learn Sophie?
 
 1. [Read the docs](https://sophie.readthedocs.io)
 2. Poke around the [examples](https://github.com/kjosib/sophie/tree/main/examples) and [grammar](https://github.com/kjosib/sophie/blob/main/sophie/Sophie.md)
 3. Contribute to the docs in the usual way.
 
 It sure might be nice to have a *Learn computer science with Sophie*
@@ -50,15 +41,22 @@
 * Sophie has Turtle-graphics! (See [here](https://github.com/kjosib/sophie/blob/main/examples/turtle.sg) for examples.)
 * Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/guess_the_number.sg) as an example.
 * The new type-checker gives excellent feedback and cannot be fooled. Through abstract interpretation it completely rules out *type* errors.
   (Domain errors, such as division by zero, are still possible.)
 * The module system got an upgrade: there is now a notion of a system-package and the beginnings of a standard library.
 * The FFI (into Python): Sophie can call Python; Python can call Sophie; and Python can install I/O drivers into Sophie.
 * Error display is improved in various ways. There is also now an easy way to install helpful messages for parse errors.
-  This works; there just aren't many good messages yet.
+  This works surprisingly well now.
+
+*Caveat:* Type-checking is presently out of commission in HEAD, but the release has it working.
+
+Some things are in progress:
+
+* I'm in progress to add asynchronous message-passing, with an eye towards a safe concurrency model.
+  (That's why type-checking is temporarily turned off)
 
 Certain things are not started yet:
 
 * Variable-Arity Functions.
 * Ad-hoc polymorphic multi-methods.
 * List comprehension (expressions like `[expr FOR name IN expr]`) are removed from the syntax for now.
 * Asynchrony.
```

### Comparing `sophie-lang-0.0.0/setup.py` & `sophie-lang-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
 Packaging script for PyPI.
 """
 import os, setuptools
 from pathlib import Path
 
-_grammar_source = Path(__file__).parent / "sophie" / "Sophie.md"
-if _grammar_source.exists():
+try:
 	from boozetools.macroparse.runtime import make_tables
-	make_tables(_grammar_source)
+except ImportError:
+	pass
+else:
+	make_tables(Path(__file__).parent / "sophie" / "Sophie.md")
 
 setuptools.setup(
 	name='sophie-lang',
 	author='Ian Kjos',
 	author_email='kjosib@gmail.com',
-	version='0.0.0',
+	version='0.0.3',
 	packages=['sophie', "sophie.adapters", ],
 	package_data={
 		'sophie': ["Sophie.automaton"]+["sys/"+f for f in os.listdir("sophie/sys")],
 	},
+	entry_points={
+		'console_scripts': ["sophie = sophie.cmdline:main"],
+	},
 	license='MIT',
 	description='A call-by-need strong-inferred-type language named for French mathematician Sophie Germain',
 	long_description=open('README.md').read(),
 	long_description_content_type="text/markdown",
 	url="https://github.com/kjosib/sophie",
 	classifiers=[
 		"Programming Language :: Python :: 3.9",
```

### Comparing `sophie-lang-0.0.0/sophie/Sophie.automaton` & `sophie-lang-0.0.3/sophie/Sophie.automaton`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9838796741951608%*

 * *Differences: {"'parser'": "{'action': {'edits': {'check': {insert: [(1, 181), (2, 231), (3, 230), (4, 231), (9, "*

 * *             '231), (10, 230), (11, 191), (12, 191), (14, 181), (15, 181), (16, 79), (17, 181), '*

 * *             '(18, 181), (19, 181), (20, 81), (21, 191), (24, 233), (25, 0), (26, 57), (27, 233), '*

 * *             '(29, 66), (31, 110), (32, 52), (33, 233), (34, 191), (35, 233), (39, 110), (40, '*

 * *             '150), (41, 57), (42, 191), (43, 81), (45, 150), (46, 66), (49, 183), (50, 233), (51, '*

 * *             '23 […]*

```diff
@@ -1,788 +1,834 @@
 {
     "description": "MacroParse Automaton",
     "parser": {
         "action": {
             "edits": {
                 "check": [
                     57,
-                    172,
-                    221,
-                    77,
-                    221,
+                    181,
+                    231,
+                    230,
+                    231,
                     57,
                     12,
                     2,
-                    65,
-                    221,
                     54,
-                    63,
-                    52,
-                    172,
-                    172,
-                    172,
-                    0,
-                    172,
-                    172,
-                    172,
+                    231,
+                    230,
+                    191,
+                    191,
                     181,
-                    222,
+                    181,
+                    181,
+                    79,
+                    181,
+                    181,
+                    181,
+                    81,
+                    191,
                     52,
                     57,
-                    222,
+                    233,
+                    0,
+                    57,
+                    233,
                     12,
-                    219,
+                    66,
                     12,
-                    63,
-                    181,
-                    222,
-                    65,
-                    222,
-                    219,
-                    174,
+                    110,
+                    52,
+                    233,
+                    191,
+                    233,
                     57,
                     57,
                     2,
-                    176,
-                    88,
-                    205,
-                    181,
-                    88,
+                    110,
+                    150,
+                    57,
+                    191,
+                    81,
                     54,
+                    150,
+                    66,
                     57,
                     57,
-                    105,
-                    222,
+                    183,
+                    233,
+                    230,
                     57,
-                    181,
+                    230,
                     57,
                     57,
-                    77,
-                    105,
-                    129,
-                    137,
-                    222,
-                    129,
-                    137,
-                    143,
-                    173,
-                    199,
-                    174,
-                    285,
-                    143,
-                    186,
-                    176,
-                    293,
+                    91,
+                    184,
+                    135,
+                    91,
+                    233,
+                    135,
+                    144,
                     186,
-                    293,
+                    210,
+                    144,
+                    216,
+                    183,
+                    196,
+                    79,
+                    298,
+                    196,
+                    307,
                     1,
-                    219,
+                    307,
+                    313,
                     3,
-                    219,
-                    199,
+                    210,
                     4,
-                    173,
                     5,
                     6,
                     7,
                     8,
+                    186,
                     9,
+                    313,
+                    184,
                     10,
                     11,
                     13,
                     14,
                     16,
                     17,
-                    205,
                     18,
                     20,
                     21,
                     22,
                     23,
                     24,
                     26,
-                    285,
                     27,
                     28,
                     31,
                     32,
                     33,
                     35,
+                    298,
                     36,
                     37,
                     40,
                     41,
                     43,
                     44,
                     45,
                     47,
                     48,
                     53,
                     56,
+                    216,
                     59,
                     60,
                     61,
-                    66,
-                    67,
+                    62,
+                    63,
+                    64,
                     68,
                     69,
                     70,
-                    73,
-                    74,
+                    71,
+                    72,
                     75,
                     76,
+                    77,
                     78,
-                    79,
                     80,
-                    81,
                     82,
+                    83,
                     84,
                     85,
                     87,
-                    91,
-                    107,
-                    109,
-                    111,
-                    113,
-                    116,
+                    88,
+                    89,
+                    94,
+                    112,
+                    114,
                     117,
                     118,
                     120,
-                    121,
+                    123,
                     124,
-                    126,
+                    125,
                     127,
-                    128,
+                    130,
                     132,
+                    133,
                     134,
-                    136,
-                    139,
+                    138,
                     140,
                     141,
-                    142,
-                    145,
+                    143,
+                    146,
                     147,
                     148,
-                    166,
-                    170,
+                    149,
+                    152,
+                    154,
+                    155,
                     175,
-                    177,
+                    176,
                     179,
-                    180,
-                    183,
+                    182,
                     185,
-                    188,
-                    194,
+                    187,
+                    189,
+                    190,
+                    193,
                     195,
-                    197,
                     198,
-                    200,
-                    202,
-                    203,
+                    199,
+                    205,
+                    206,
                     208,
                     209,
                     211,
-                    212,
+                    213,
                     214,
-                    215,
-                    216,
+                    219,
                     220,
+                    222,
                     223,
-                    224,
                     225,
                     226,
                     227,
-                    228,
-                    229,
-                    230,
-                    231,
                     232,
-                    233,
                     234,
                     235,
+                    236,
                     237,
+                    238,
                     239,
                     240,
+                    241,
                     242,
                     243,
                     244,
+                    245,
                     246,
-                    247,
+                    249,
+                    252,
                     253,
                     255,
-                    257,
+                    256,
+                    258,
                     259,
-                    260,
-                    262,
-                    263,
-                    267,
-                    279,
-                    281,
-                    290,
-                    291,
+                    265,
+                    268,
+                    270,
+                    272,
+                    273,
+                    275,
+                    276,
+                    280,
                     292,
+                    293,
                     294,
-                    295,
-                    296,
-                    297,
-                    298,
-                    299,
-                    301,
-                    302,
-                    303,
+                    304,
+                    305,
                     306,
+                    308,
+                    309,
                     310,
                     311,
-                    312
+                    312,
+                    314,
+                    315,
+                    316,
+                    317,
+                    320,
+                    321,
+                    325,
+                    326,
+                    328,
+                    330
                 ],
                 "offset": [
-                    -16,
-                    70,
+                    -8,
+                    73,
                     7,
-                    37,
+                    40,
+                    66,
+                    69,
+                    33,
+                    69,
+                    26,
+                    84,
                     63,
-                    67,
-                    34,
-                    67,
-                    28,
-                    81,
-                    58,
-                    71,
-                    -27,
-                    71,
-                    78,
+                    76,
+                    -28,
+                    76,
+                    83,
                     0,
-                    59,
-                    75,
+                    64,
+                    80,
                     37,
-                    229,
-                    77,
+                    243,
+                    81,
                     37,
                     38,
                     39,
-                    84,
-                    229,
-                    43,
-                    72,
-                    86,
-                    229,
-                    229,
-                    86,
-                    64,
                     88,
-                    229,
-                    79,
-                    100,
+                    243,
+                    43,
+                    75,
+                    89,
+                    243,
+                    243,
+                    89,
+                    66,
+                    91,
+                    243,
+                    82,
+                    104,
                     50,
-                    229,
-                    229,
-                    93,
-                    54,
-                    229,
-                    94,
-                    96,
-                    96,
-                    229,
-                    74,
-                    70,
-                    229,
-                    229,
-                    229,
-                    9,
+                    243,
+                    243,
+                    97,
+                    56,
+                    243,
+                    98,
+                    100,
+                    100,
+                    243,
+                    72,
+                    78,
+                    243,
+                    243,
+                    243,
+                    19,
                     60,
+                    -5,
+                    243,
+                    113,
                     -3,
-                    229,
-                    109,
-                    -3,
-                    229,
-                    101,
-                    112,
-                    103,
-                    229,
-                    8,
-                    229,
-                    5,
-                    104,
-                    105,
+                    243,
                     106,
                     107,
                     108,
-                    229,
-                    229,
-                    109,
+                    119,
+                    67,
                     111,
-                    76,
-                    116,
-                    0,
-                    105,
-                    78,
+                    243,
+                    26,
+                    243,
+                    112,
+                    113,
+                    114,
                     115,
                     116,
-                    78,
-                    229,
-                    118,
-                    80,
-                    229,
-                    129,
-                    35,
-                    229,
-                    229,
-                    121,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    1,
-                    229,
-                    122,
-                    229,
-                    120,
-                    229,
-                    85,
-                    229,
-                    125,
-                    229,
-                    229,
-                    87,
-                    92,
-                    132,
-                    229,
+                    243,
+                    243,
+                    117,
+                    119,
+                    81,
+                    124,
+                    13,
+                    113,
+                    17,
+                    83,
+                    123,
+                    124,
+                    82,
+                    243,
+                    126,
+                    84,
+                    137,
+                    243,
+                    52,
+                    243,
+                    243,
                     129,
-                    91,
-                    229,
-                    229,
-                    92,
-                    229,
-                    141,
-                    142,
-                    140,
-                    50,
-                    229,
-                    229,
-                    127,
-                    229,
-                    97,
-                    229,
-                    146,
-                    51,
-                    229,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    -17,
+                    243,
+                    130,
+                    243,
                     128,
-                    122,
-                    140,
-                    142,
-                    52,
-                    229,
+                    243,
+                    243,
+                    89,
+                    109,
+                    243,
                     134,
-                    229,
-                    152,
-                    144,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    106,
-                    229,
-                    229,
-                    229,
-                    155,
-                    229,
-                    0,
-                    31,
-                    22,
-                    147,
-                    26,
-                    138,
-                    229,
-                    113,
-                    156,
-                    7,
-                    229,
+                    243,
+                    243,
+                    92,
+                    98,
+                    141,
+                    243,
+                    95,
+                    243,
+                    243,
+                    96,
+                    243,
+                    149,
+                    150,
                     148,
-                    229,
-                    161,
-                    61,
-                    229,
-                    154,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    163,
-                    161,
-                    229,
-                    138,
-                    157,
-                    48,
-                    122,
-                    229,
-                    163,
-                    160,
-                    229,
-                    36,
-                    229,
-                    229,
-                    161,
-                    171,
-                    229,
-                    163,
-                    164,
-                    229,
+                    54,
+                    243,
+                    243,
+                    135,
+                    243,
+                    101,
+                    145,
+                    243,
+                    155,
+                    58,
+                    243,
+                    137,
                     130,
-                    167,
-                    126,
-                    229,
-                    229,
-                    23,
-                    168,
-                    -4,
+                    149,
+                    151,
+                    33,
+                    243,
+                    143,
+                    243,
+                    161,
+                    153,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    111,
+                    112,
+                    243,
+                    243,
+                    165,
+                    243,
+                    0,
+                    139,
                     19,
+                    45,
+                    158,
+                    42,
+                    149,
+                    243,
+                    121,
+                    167,
+                    -1,
+                    243,
+                    159,
+                    243,
+                    172,
+                    64,
+                    243,
+                    165,
+                    141,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    175,
+                    173,
+                    243,
+                    149,
                     169,
-                    170,
-                    171,
+                    51,
+                    131,
+                    243,
+                    175,
                     172,
+                    243,
+                    62,
+                    243,
+                    243,
                     173,
-                    174,
+                    183,
+                    243,
                     175,
                     176,
-                    177,
-                    178,
+                    243,
+                    139,
                     179,
+                    134,
+                    243,
+                    243,
+                    0,
+                    -4,
                     180,
-                    190,
-                    229,
-                    166,
-                    229,
-                    165,
-                    184,
-                    229,
-                    158,
-                    159,
-                    148,
-                    229,
-                    149,
-                    159,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    199,
-                    229,
-                    155,
-                    229,
-                    196,
-                    229,
-                    193,
-                    194,
-                    229,
-                    195,
-                    196,
-                    229,
-                    229,
-                    229,
-                    198,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    229,
-                    198,
-                    229,
-                    172,
-                    229,
-                    229,
-                    229,
-                    50,
-                    229,
-                    229,
-                    229,
-                    229,
-                    200,
-                    201,
+                    22,
+                    181,
+                    182,
+                    183,
                     184,
-                    38,
+                    185,
+                    186,
+                    187,
+                    188,
+                    189,
+                    190,
+                    191,
+                    192,
+                    176,
+                    243,
+                    243,
                     203,
-                    208,
-                    209,
+                    243,
+                    243,
+                    195,
+                    177,
+                    243,
+                    169,
+                    155,
+                    243,
+                    156,
+                    168,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    210,
+                    243,
+                    243,
+                    163,
+                    243,
+                    207,
+                    243,
+                    204,
+                    205,
+                    243,
                     206,
                     207,
-                    208,
-                    229,
+                    243,
+                    243,
+                    243,
                     209,
-                    192,
-                    193,
-                    229,
-                    229,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    209,
+                    167,
+                    183,
+                    243,
+                    243,
+                    243,
+                    57,
+                    243,
+                    243,
+                    243,
+                    243,
+                    243,
+                    212,
+                    213,
                     195,
-                    229,
-                    229,
-                    229,
-                    174,
-                    214,
-                    215
+                    42,
+                    215,
+                    220,
+                    217,
+                    218,
+                    219,
+                    29,
+                    220,
+                    202,
+                    222,
+                    204,
+                    243,
+                    243,
+                    206,
+                    225,
+                    243,
+                    243,
+                    243,
+                    226,
+                    184,
+                    243,
+                    228,
+                    243,
+                    229
                 ],
                 "value": [
-                    98,
-                    158,
-                    160,
-                    133,
-                    152,
-                    99,
+                    101,
+                    171,
+                    167,
+                    178,
+                    159,
+                    102,
                     22,
                     -1,
-                    77,
-                    -69,
-                    -95,
-                    119,
-                    82,
+                    -102,
                     -74,
-                    151,
-                    161,
-                    4,
-                    156,
-                    155,
-                    164,
+                    176,
+                    175,
                     0,
-                    154,
-                    -162,
-                    105,
-                    149,
-                    24,
-                    165,
-                    -169,
-                    116,
-                    159,
-                    150,
-                    74,
-                    -65,
+                    -77,
                     166,
-                    244,
+                    162,
+                    139,
+                    158,
+                    170,
+                    157,
+                    79,
+                    163,
+                    85,
+                    110,
+                    160,
+                    4,
+                    108,
+                    168,
+                    24,
+                    126,
+                    -177,
+                    188,
+                    -170,
+                    164,
+                    174,
+                    -68,
+                    106,
                     103,
-                    100,
                     5,
-                    -85,
+                    186,
+                    226,
+                    107,
+                    169,
+                    76,
+                    88,
                     -108,
-                    -148,
-                    167,
-                    147,
-                    85,
-                    102,
-                    106,
-                    178,
-                    163,
-                    92,
-                    162,
-                    93,
-                    94,
-                    132,
-                    176,
-                    -147,
-                    -165,
-                    157,
-                    205,
-                    209,
-                    215,
-                    241,
-                    -37,
-                    -116,
-                    -135,
-                    -101,
-                    -140,
-                    -85,
-                    241,
-                    253,
-                    -112,
+                    123,
+                    105,
+                    111,
+                    254,
+                    161,
+                    111,
+                    95,
+                    165,
+                    96,
+                    97,
+                    -115,
+                    256,
+                    -155,
+                    154,
+                    156,
+                    216,
+                    -173,
+                    140,
+                    -39,
+                    220,
+                    -156,
+                    188,
+                    -144,
+                    138,
+                    -150,
+                    265,
+                    254,
                     1,
-                    106,
+                    -119,
+                    63,
                     7,
-                    153,
                     0,
                     8,
-                    178,
                     9,
                     11,
                     12,
                     15,
+                    -88,
                     -2,
+                    62,
+                    -90,
                     17,
                     18,
                     25,
                     26,
                     28,
                     29,
-                    267,
                     32,
                     34,
                     35,
                     36,
-                    -170,
+                    -178,
                     37,
                     38,
-                    300,
                     40,
                     41,
                     46,
-                    48,
+                    47,
                     51,
                     53,
+                    313,
                     56,
-                    -17,
+                    -19,
                     57,
-                    60,
-                    62,
-                    63,
-                    64,
+                    61,
                     65,
+                    66,
                     67,
-                    83,
+                    69,
+                    81,
                     86,
-                    108,
-                    111,
-                    112,
-                    -24,
-                    -23,
-                    -27,
-                    -28,
-                    -29,
-                    -32,
-                    121,
-                    124,
-                    125,
-                    134,
-                    135,
+                    90,
+                    280,
+                    113,
                     -16,
-                    -163,
-                    139,
-                    -90,
-                    145,
+                    -17,
+                    117,
+                    118,
+                    119,
+                    -26,
+                    -25,
+                    -29,
+                    -30,
+                    -31,
+                    -34,
+                    127,
+                    130,
+                    131,
+                    140,
+                    142,
+                    -18,
+                    -171,
                     146,
-                    169,
-                    182,
-                    -41,
-                    188,
-                    -47,
-                    189,
+                    -97,
+                    152,
+                    153,
+                    172,
                     192,
-                    193,
-                    -25,
-                    199,
-                    78,
-                    202,
+                    -45,
+                    198,
+                    -141,
+                    -40,
+                    200,
                     203,
                     204,
-                    134,
-                    207,
-                    208,
-                    53,
-                    211,
+                    210,
+                    80,
                     213,
                     214,
-                    216,
-                    -109,
+                    215,
+                    140,
                     218,
-                    236,
-                    238,
-                    245,
-                    246,
+                    -27,
+                    219,
+                    53,
+                    223,
+                    224,
+                    225,
+                    227,
+                    -116,
+                    229,
+                    247,
                     248,
-                    249,
                     250,
-                    252,
-                    184,
+                    251,
                     257,
                     258,
-                    259,
+                    260,
                     261,
+                    262,
                     264,
-                    -152,
-                    -146,
-                    -164,
-                    -166,
-                    -94,
+                    194,
+                    267,
                     270,
-                    50,
-                    -102,
+                    271,
+                    272,
                     274,
-                    -60,
-                    -58,
-                    -61,
-                    -70,
-                    -66,
-                    -63,
-                    -67,
-                    -72,
-                    -64,
-                    -68,
-                    -73,
-                    -62,
-                    -71,
-                    275,
-                    276,
                     277,
-                    278,
-                    280,
-                    -117,
-                    78,
-                    282,
+                    -160,
+                    -154,
+                    -172,
+                    -174,
                     283,
-                    -141,
+                    -101,
+                    50,
+                    -109,
                     287,
-                    -126,
-                    -33,
+                    -69,
+                    -64,
+                    -65,
+                    -71,
+                    -75,
+                    -63,
+                    -61,
+                    -72,
+                    -67,
+                    -62,
+                    -76,
+                    -73,
+                    -70,
+                    288,
                     289,
+                    290,
+                    291,
+                    293,
+                    80,
+                    295,
+                    296,
+                    -145,
+                    301,
+                    -132,
                     -35,
-                    -36,
-                    206,
-                    292,
-                    -87,
-                    -96,
-                    -56,
-                    -83,
-                    304,
-                    305,
-                    -89,
-                    -82,
+                    303,
+                    -37,
                     -38,
-                    -136,
-                    307,
-                    308,
-                    -113,
-                    310,
-                    312,
-                    -88,
-                    -39
+                    217,
+                    306,
+                    309,
+                    -91,
+                    -103,
+                    -59,
+                    -86,
+                    318,
+                    319,
+                    -85,
+                    -41,
+                    -151,
+                    -96,
+                    322,
+                    323,
+                    -120,
+                    326,
+                    327,
+                    329,
+                    330,
+                    -92,
+                    -42
                 ]
             },
             "fallback": [
                 -1,
                 -1,
                 -1,
                 -1,
@@ -810,132 +856,138 @@
                 -1,
                 -1,
                 -1,
                 -1,
                 8,
                 18,
                 -1,
-                214,
-                -1,
+                225,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
+                313,
                 8,
                 -1,
                 -1,
                 -1,
                 -1,
+                81,
                 -1,
-                65,
                 -1,
                 8,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
-                244,
-                65,
+                256,
+                81,
                 41,
                 -1,
                 -1,
                 -1,
                 -1,
-                124,
                 -1,
-                124,
                 -1,
                 -1,
+                130,
+                -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
+                130,
+                -1,
+                -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 57,
-                291,
+                305,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 57,
                 57,
                 57,
                 -1,
                 -1,
                 -1,
                 -1,
                 57,
+                -1,
+                57,
                 57,
                 -1,
                 -1,
-                188,
+                198,
                 -1,
                 -1,
                 -1,
+                62,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
-                63,
+                -1,
+                66,
                 -1,
                 -1,
                 -1,
+                79,
+                130,
                 -1,
-                77,
-                124,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
+                280,
+                130,
                 -1,
-                267,
-                124,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
-                85,
+                88,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 56,
-                291,
-                57,
+                305,
                 57,
                 57,
                 57,
                 57,
                 57,
                 57,
                 57,
@@ -945,314 +997,339 @@
                 57,
                 57,
                 57,
                 57,
                 57,
                 57,
                 -1,
+                -1,
                 57,
                 -1,
                 -1,
-                181,
                 -1,
-                234,
+                57,
+                191,
                 -1,
+                245,
+                57,
                 -1,
                 -1,
-                132,
-                181,
+                -1,
+                -1,
+                191,
                 57,
                 -1,
                 -1,
-                232,
+                243,
                 -1,
                 -1,
-                63,
+                66,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
-                63,
-                63,
                 -1,
+                66,
+                66,
                 -1,
                 -1,
-                121,
                 -1,
-                65,
+                127,
                 -1,
+                81,
                 -1,
                 -1,
                 -1,
-                124,
                 -1,
-                124,
+                130,
                 -1,
+                130,
                 -1,
-                82,
                 -1,
+                85,
                 -1,
                 -1,
                 -1,
                 -1,
-                85,
+                -1,
+                88,
                 -1,
                 -1,
                 -1,
                 -1,
-                219,
+                241,
+                231,
+                242,
                 230,
+                234,
+                232,
+                181,
+                235,
+                238,
+                236,
                 233,
-                220,
-                223,
-                221,
-                225,
-                224,
-                226,
-                172,
-                222,
-                228,
-                229,
-                227,
-                231,
+                239,
+                237,
+                240,
+                244,
+                191,
                 -1,
                 -1,
-                181,
                 -1,
                 -1,
                 -1,
-                57,
                 -1,
                 -1,
+                57,
                 -1,
                 -1,
                 -1,
-                181,
+                -1,
+                191,
                 -1,
                 57,
                 57,
                 -1,
                 -1,
-                111,
-                -1,
+                117,
                 -1,
+                57,
                 -1,
                 -1,
-                63,
                 -1,
+                66,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
                 -1,
-                124,
                 -1,
+                130,
                 -1,
                 -1,
                 -1,
                 57,
                 -1,
                 -1,
-                291,
-                244,
+                -1,
+                305,
+                -1,
                 -1,
                 -1,
                 57,
-                181,
-                297,
+                191,
+                310,
                 -1,
+                298,
                 -1,
                 -1,
                 -1,
                 -1,
-                181,
+                191,
                 -1,
-                244,
+                293,
                 -1,
                 -1,
+                305,
+                -1,
                 -1,
-                291,
                 -1,
                 -1,
-                41,
                 -1,
                 -1,
                 -1,
                 -1,
                 57,
-                41,
+                313,
+                -1,
+                -1,
+                -1,
+                298,
+                -1,
                 -1,
                 -1,
-                285,
                 -1,
                 -1,
                 -1
             ],
             "reduce": {
                 "check": [
                     15,
                     15,
                     15,
                     15,
                     15,
-                    15,
-                    4,
+                    -1,
                     15,
                     15,
-                    18,
-                    18,
-                    18,
-                    18,
-                    18,
                     15,
+                    16,
+                    16,
+                    16,
                     13,
-                    18,
+                    15,
                     13,
-                    4,
+                    16,
                     -1,
+                    21,
+                    21,
                     15,
                     15,
                     4,
-                    18,
+                    21,
+                    21,
                     15,
                     15,
                     15,
+                    18,
+                    18,
+                    18,
+                    18,
+                    18,
+                    4,
+                    18,
+                    18,
+                    11,
+                    4,
+                    7,
+                    6,
+                    6,
+                    18,
+                    21,
+                    35,
+                    7,
                     5,
-                    3,
-                    -1,
+                    11,
+                    11,
                     18,
-                    3,
-                    3,
+                    11,
+                    35,
+                    11,
                     18,
                     18,
                     18,
-                    25,
-                    25,
                     5,
                     5,
-                    25,
+                    35,
                     5,
-                    9,
+                    6,
                     5,
-                    24,
+                    25,
                     5,
-                    24,
-                    6,
-                    6,
-                    24,
+                    25,
+                    9,
+                    11,
+                    25,
+                    19,
                     5,
-                    3,
+                    34,
                     0,
-                    30,
-                    30,
+                    34,
+                    -1,
+                    25,
                     5,
                     5,
-                    24,
-                    9,
-                    30,
-                    24,
                     25,
-                    -1,
+                    12,
+                    19,
+                    9,
                     0,
                     0,
-                    11,
+                    19,
                     0,
-                    6,
+                    34,
                     0,
-                    -1,
-                    24,
+                    10,
+                    25,
                     0,
-                    24,
-                    24,
+                    19,
+                    25,
+                    25,
                     2,
                     0,
-                    11,
-                    11,
-                    7,
-                    11,
+                    12,
+                    19,
+                    19,
+                    10,
+                    20,
+                    10,
+                    20,
                     10,
-                    11,
-                    14,
-                    14,
-                    7,
                     2,
                     2,
-                    14,
+                    12,
                     2,
                     -1,
                     2,
-                    12,
-                    10,
-                    11,
-                    10,
-                    19,
-                    10,
-                    20,
-                    20,
-                    16,
-                    16,
-                    16,
-                    20,
+                    26,
+                    26,
                     20,
+                    8,
+                    26,
+                    3,
                     26,
-                    16,
-                    14,
-                    19,
                     10,
-                    12,
-                    8,
-                    19,
-                    21,
-                    21,
+                    3,
+                    3,
+                    14,
+                    14,
                     22,
                     22,
-                    33,
-                    12,
-                    33,
-                    17,
-                    17,
-                    20,
+                    27,
+                    14,
                     23,
-                    19,
-                    28,
                     23,
-                    27,
+                    31,
+                    31,
                     8,
+                    17,
+                    17,
+                    24,
+                    31,
                     26,
-                    33,
+                    24,
+                    28,
+                    3,
                     29,
-                    31,
+                    30,
                     32,
+                    33,
                     -1,
+                    14,
                     -1,
-                    -1,
-                    21,
                     22,
+                    -1,
                     27,
-                    29,
+                    23,
+                    30,
+                    28,
                     -1,
                     -1,
-                    31,
+                    32,
+                    33,
+                    -1,
                     -1,
                     -1,
                     -1,
-                    32,
                     -1,
                     -1,
                     -1,
-                    28
+                    -1,
+                    -1,
+                    -1,
+                    29
                 ],
                 "col_class": [
                     0,
                     1,
                     1,
                     2,
                     3,
@@ -1267,49 +1344,53 @@
                     8,
                     1,
                     1,
                     9,
                     1,
                     1,
                     1,
-                    10,
-                    10,
+                    6,
+                    6,
                     1,
                     1,
+                    10,
                     11,
                     12,
                     13,
-                    14,
                     1,
+                    12,
+                    14,
                     15,
                     16,
+                    6,
                     17,
-                    10,
-                    18,
                     1,
+                    18,
                     19,
+                    1,
+                    12,
+                    12,
                     20,
+                    6,
                     1,
-                    13,
-                    13,
+                    12,
                     21,
-                    10,
-                    1,
                     22,
                     23,
                     24,
                     25,
-                    13,
+                    12,
                     26,
                     27,
                     1,
-                    13,
                     28,
-                    13,
-                    29
+                    12,
+                    29,
+                    12,
+                    30
                 ],
                 "d_reduce": [
                     -5,
                     0,
                     0,
                     -7,
                     0,
@@ -1318,147 +1399,156 @@
                     0,
                     0,
                     0,
                     -11,
                     0,
                     0,
                     0,
-                    -181,
-                    -183,
+                    -189,
+                    -191,
                     -13,
                     0,
                     0,
                     -6,
                     0,
                     0,
                     0,
                     0,
                     0,
                     -4,
-                    -182,
+                    -190,
                     -15,
                     0,
                     0,
                     -8,
                     0,
                     0,
                     0,
-                    -179,
-                    -20,
-                    -93,
+                    -187,
+                    -22,
+                    -100,
                     0,
-                    -184,
+                    -192,
                     -3,
                     0,
                     0,
                     -10,
                     0,
                     0,
                     0,
-                    -177,
+                    -185,
                     0,
                     0,
-                    -26,
+                    -28,
                     0,
-                    -180,
+                    -188,
                     0,
                     0,
                     0,
-                    -91,
+                    -98,
                     0,
                     0,
                     -12,
                     0,
-                    -137,
                     0,
-                    -175,
                     0,
-                    -178,
+                    -141,
                     0,
                     0,
+                    -183,
                     0,
+                    -186,
                     0,
                     0,
                     0,
-                    -30,
-                    -31,
                     0,
                     0,
-                    -158,
+                    -32,
+                    -33,
                     0,
                     0,
-                    -21,
+                    -166,
                     0,
                     0,
+                    -23,
                     0,
                     0,
-                    -19,
                     0,
                     0,
-                    -92,
                     0,
+                    -21,
                     0,
-                    -110,
+                    0,
+                    0,
+                    -99,
+                    0,
+                    -117,
                     -14,
                     0,
-                    -48,
-                    -49,
-                    -50,
                     -51,
                     -52,
                     -53,
+                    -54,
+                    -55,
+                    -56,
                     0,
                     0,
                     0,
-                    -75,
                     -78,
-                    -79,
-                    -80,
+                    -81,
+                    -82,
+                    -93,
                     0,
+                    -83,
                     0,
                     0,
-                    -173,
                     0,
+                    -181,
+                    0,
+                    -43,
+                    -142,
+                    0,
+                    0,
+                    -184,
+                    0,
+                    -47,
+                    -48,
+                    -50,
                     -138,
                     0,
-                    -176,
                     0,
-                    -43,
-                    -44,
-                    -46,
-                    -132,
                     0,
+                    -165,
+                    -167,
                     0,
                     0,
                     0,
-                    -157,
-                    -159,
                     0,
+                    -161,
                     0,
+                    -163,
+                    -157,
+                    -23,
                     0,
                     0,
-                    -153,
                     0,
-                    -155,
-                    -149,
-                    -21,
+                    -169,
                     0,
                     0,
-                    -161,
+                    -175,
+                    -22,
                     0,
                     0,
-                    -167,
-                    -20,
                     0,
                     0,
+                    -110,
+                    -104,
+                    -114,
                     0,
                     0,
-                    -103,
-                    -97,
-                    -107,
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
@@ -1467,200 +1557,211 @@
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
+                    -179,
+                    -79,
                     0,
                     0,
                     0,
+                    -80,
                     0,
                     0,
+                    -60,
                     -77,
-                    -171,
                     0,
-                    -57,
-                    -74,
                     0,
                     0,
                     0,
-                    -21,
+                    -23,
                     0,
                     0,
                     0,
-                    -121,
-                    -123,
-                    -174,
+                    -126,
+                    -128,
+                    -182,
                     0,
                     0,
                     0,
                     0,
-                    -142,
-                    -41,
+                    -146,
                     -45,
-                    -131,
-                    -133,
                     0,
+                    -49,
+                    -137,
+                    -139,
                     0,
                     0,
-                    -127,
-                    -129,
                     0,
+                    -133,
+                    -135,
                     0,
                     0,
                     0,
-                    -151,
                     0,
+                    -159,
                     0,
-                    -154,
                     0,
+                    -162,
                     0,
-                    -22,
                     0,
+                    -24,
                     0,
-                    -18,
                     0,
+                    -20,
                     0,
-                    -105,
-                    -99,
                     0,
+                    -112,
+                    -106,
                     0,
-                    -111,
-                    -172,
-                    -59,
-                    -60,
+                    0,
+                    -118,
+                    -180,
+                    -66,
+                    -74,
                     -69,
+                    -68,
+                    -64,
                     -65,
-                    -58,
-                    -61,
-                    -70,
-                    -66,
+                    -71,
+                    -75,
                     -63,
-                    -67,
+                    -61,
                     -72,
-                    -64,
-                    -68,
-                    -73,
+                    -67,
                     -62,
-                    -71,
-                    0,
-                    -55,
+                    -76,
+                    -73,
+                    -70,
                     0,
-                    -54,
+                    -94,
+                    -58,
                     0,
+                    -57,
+                    -95,
                     0,
                     0,
                     0,
                     0,
                     0,
-                    -118,
+                    -123,
                     0,
                     0,
-                    -120,
-                    -122,
+                    -125,
+                    -127,
                     0,
-                    -42,
-                    -139,
+                    -46,
+                    -143,
                     0,
-                    -40,
+                    -44,
                     0,
-                    -125,
                     0,
-                    -128,
+                    -131,
                     0,
+                    -134,
                     0,
-                    -144,
                     0,
+                    -152,
                     0,
-                    -160,
-                    -156,
-                    -150,
                     0,
-                    -34,
                     -168,
-                    -106,
+                    -164,
+                    -158,
                     0,
-                    -100,
-                    -104,
-                    -98,
-                    -76,
+                    -36,
+                    -176,
+                    -113,
                     0,
-                    -81,
-                    -119,
+                    -107,
+                    -111,
+                    -105,
                     0,
+                    -130,
+                    -124,
+                    -84,
                     0,
                     0,
-                    -86,
                     0,
-                    -124,
+                    -89,
                     0,
-                    -143,
-                    -134,
-                    -130,
-                    -145,
+                    -129,
                     0,
-                    -56,
+                    -147,
                     0,
+                    -140,
+                    -136,
+                    -153,
                     0,
+                    -59,
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
                     0,
-                    -114,
                     0,
                     0,
-                    -115,
-                    -84,
+                    -121,
+                    0,
+                    0,
+                    0,
+                    -87,
+                    -122,
                     0,
                     0,
                     0,
+                    -148,
+                    0,
+                    -149,
                     0
                 ],
                 "offset": [
-                    52,
+                    69,
                     0,
-                    74,
-                    24,
-                    6,
-                    27,
-                    40,
-                    76,
+                    91,
+                    108,
+                    21,
+                    44,
+                    31,
+                    35,
                     102,
-                    42,
-                    80,
-                    65,
-                    89,
-                    8,
-                    79,
+                    63,
+                    85,
+                    35,
+                    74,
+                    5,
+                    114,
                     -1,
-                    97,
+                    7,
+                    125,
+                    26,
+                    66,
+                    90,
+                    14,
                     116,
-                    8,
-                    95,
-                    94,
-                    109,
-                    111,
+                    120,
+                    126,
+                    60,
+                    106,
                     118,
-                    44,
-                    35,
-                    101,
-                    110,
+                    119,
+                    134,
+                    123,
                     122,
-                    115,
-                    50,
-                    114,
-                    125,
-                    101
+                    122,
+                    132,
+                    54,
+                    27
                 ],
                 "row_class": [
                     0,
                     1,
                     1,
                     0,
                     1,
@@ -1715,42 +1816,45 @@
                     1,
                     1,
                     8,
                     1,
                     1,
                     4,
                     1,
+                    1,
+                    1,
                     13,
                     1,
+                    1,
                     10,
                     1,
                     11,
                     1,
                     1,
                     1,
                     1,
                     1,
-                    1,
                     14,
                     14,
                     1,
                     1,
                     14,
                     1,
                     1,
                     15,
                     1,
                     1,
                     1,
                     1,
+                    1,
                     16,
                     1,
                     1,
-                    8,
                     1,
+                    8,
                     1,
                     17,
                     9,
                     1,
                     18,
                     18,
                     18,
@@ -1761,54 +1865,58 @@
                     1,
                     1,
                     18,
                     18,
                     18,
                     18,
                     1,
+                    18,
                     1,
                     1,
-                    19,
                     1,
-                    13,
-                    1,
-                    10,
+                    19,
                     1,
                     20,
                     20,
-                    20,
-                    20,
                     1,
                     1,
+                    10,
+                    1,
+                    21,
+                    21,
+                    21,
+                    21,
+                    1,
                     1,
                     1,
                     14,
                     14,
                     1,
                     1,
                     1,
                     1,
-                    21,
+                    22,
                     1,
-                    21,
-                    17,
                     22,
+                    17,
+                    23,
+                    1,
                     1,
                     1,
                     12,
                     1,
                     1,
                     17,
                     17,
                     1,
                     1,
                     1,
                     1,
-                    23,
-                    23,
+                    24,
+                    24,
                     8,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
@@ -1820,68 +1928,72 @@
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
+                    25,
+                    18,
                     1,
                     1,
                     1,
                     18,
-                    24,
+                    1,
                     1,
                     18,
                     18,
                     1,
                     1,
                     1,
-                    25,
                     1,
+                    26,
                     1,
                     1,
-                    21,
-                    21,
+                    1,
+                    22,
+                    22,
                     19,
                     1,
                     1,
                     1,
                     1,
                     17,
                     17,
-                    20,
-                    20,
-                    20,
-                    1,
-                    1,
                     1,
                     21,
                     21,
+                    21,
+                    1,
+                    1,
+                    1,
+                    22,
+                    22,
                     1,
                     1,
                     1,
                     1,
                     14,
                     1,
                     1,
-                    26,
+                    27,
                     1,
                     1,
                     15,
                     1,
                     1,
                     17,
                     1,
                     1,
-                    27,
                     28,
+                    29,
                     1,
                     1,
                     17,
-                    24,
+                    25,
                     18,
                     18,
                     18,
                     18,
                     18,
                     18,
                     18,
@@ -1892,1075 +2004,1132 @@
                     18,
                     18,
                     18,
                     18,
                     18,
                     1,
                     18,
-                    1,
                     18,
                     1,
+                    18,
+                    18,
                     1,
                     1,
                     1,
                     1,
                     1,
-                    29,
+                    30,
                     1,
                     1,
                     18,
-                    26,
+                    27,
                     1,
-                    30,
-                    13,
+                    31,
+                    20,
                     1,
                     17,
                     1,
-                    20,
                     1,
-                    26,
+                    21,
                     1,
+                    27,
                     1,
-                    31,
+                    1,
+                    32,
                     1,
                     1,
                     14,
-                    21,
+                    22,
                     17,
                     1,
                     17,
                     17,
-                    27,
-                    1,
                     28,
-                    23,
-                    23,
-                    18,
                     1,
-                    18,
                     29,
+                    24,
+                    24,
                     1,
+                    18,
+                    30,
+                    18,
                     1,
                     1,
-                    32,
                     1,
-                    21,
+                    33,
+                    1,
+                    22,
                     1,
                     17,
-                    20,
+                    1,
                     21,
-                    31,
+                    22,
+                    32,
                     1,
                     18,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
                     1,
-                    33,
+                    34,
+                    1,
                     1,
                     1,
-                    33,
                     18,
+                    34,
+                    1,
                     1,
                     1,
+                    35,
                     1,
+                    35,
                     1
                 ]
             }
         },
         "breadcrumbs": [
             null,
-            135,
-            100,
-            84,
-            32,
-            30,
-            95,
-            35,
+            141,
+            106,
+            88,
+            33,
+            31,
+            101,
+            36,
             12,
             10,
-            142,
-            44,
+            148,
+            47,
             12,
-            69,
-            78,
-            52,
-            61,
+            73,
+            82,
+            56,
+            65,
             24,
             12,
-            126,
-            94,
-            102,
-            33,
-            110,
-            52,
+            131,
+            100,
+            108,
+            34,
+            115,
+            56,
             13,
             7,
-            82,
+            86,
             27,
             12,
-            128,
-            139,
-            52,
-            94,
+            134,
+            146,
+            56,
+            100,
             13,
-            54,
-            54,
+            58,
+            58,
             10,
-            52,
-            98,
+            56,
+            104,
             25,
             12,
-            122,
-            62,
-            69,
-            139,
+            127,
+            66,
+            73,
+            146,
             13,
-            141,
-            36,
-            133,
-            48,
+            37,
+            147,
+            139,
+            51,
             13,
-            55,
+            59,
             23,
-            88,
-            119,
+            92,
+            124,
             3,
             12,
-            125,
-            91,
-            52,
-            62,
+            133,
+            144,
+            96,
+            54,
+            56,
+            46,
+            66,
             13,
             12,
             13,
-            36,
-            138,
-            41,
-            130,
-            113,
-            143,
-            93,
-            60,
-            116,
+            145,
+            42,
+            136,
+            117,
+            149,
+            98,
+            64,
+            121,
             26,
-            114,
-            120,
+            118,
+            125,
             3,
-            52,
-            69,
-            103,
-            117,
+            56,
+            37,
+            73,
+            109,
+            122,
             3,
-            52,
-            86,
-            46,
+            56,
+            90,
+            49,
+            75,
             4,
-            71,
-            80,
-            114,
-            123,
-            85,
-            51,
-            53,
-            54,
-            97,
-            63,
-            99,
+            84,
+            118,
+            128,
+            89,
+            55,
+            57,
+            58,
+            103,
+            67,
+            105,
             3,
             8,
+            40,
+            118,
+            50,
             39,
-            114,
-            47,
-            38,
-            132,
+            44,
+            29,
+            138,
             26,
-            48,
-            91,
+            51,
+            144,
             13,
-            104,
-            118,
+            95,
+            110,
+            123,
             3,
+            56,
             13,
-            58,
-            92,
-            59,
+            62,
+            97,
+            63,
             20,
-            114,
-            115,
+            118,
+            119,
             3,
-            138,
             12,
-            106,
-            134,
-            48,
+            112,
+            140,
+            51,
             9,
-            72,
-            67,
-            81,
             76,
-            130,
-            90,
-            52,
+            71,
+            85,
+            80,
+            136,
+            94,
+            56,
             3,
             21,
-            49,
-            68,
-            77,
-            96,
-            52,
-            124,
-            87,
-            66,
-            75,
-            89,
+            145,
             52,
+            72,
+            81,
+            102,
+            56,
+            129,
+            91,
+            70,
+            79,
+            93,
+            56,
             4,
             7,
-            85,
-            5,
-            11,
-            14,
+            89,
+            38,
+            19,
+            17,
             8,
-            50,
             2,
-            18,
-            17,
-            37,
-            1,
+            28,
+            15,
             22,
+            11,
+            53,
+            14,
             6,
-            15,
-            42,
-            28,
-            19,
-            3,
-            10,
-            34,
-            97,
+            5,
+            43,
+            18,
+            1,
             13,
-            85,
-            85,
-            85,
-            129,
-            136,
-            144,
-            52,
-            85,
-            45,
-            65,
-            74,
-            85,
+            120,
+            35,
+            12,
+            10,
+            103,
+            3,
+            89,
+            89,
+            89,
+            128,
+            135,
+            142,
+            150,
+            56,
+            89,
+            48,
+            69,
+            78,
+            89,
             13,
-            57,
+            61,
             12,
-            70,
-            79,
+            74,
+            83,
+            116,
+            56,
+            95,
+            56,
             111,
-            52,
-            52,
-            105,
-            131,
-            48,
-            9,
-            64,
-            73,
-            58,
-            127,
             137,
-            52,
-            72,
-            130,
+            51,
+            9,
+            68,
+            77,
+            62,
+            132,
+            143,
+            56,
+            76,
+            136,
             4,
             4,
             7,
             7,
             12,
-            52,
+            56,
             4,
             7,
-            55,
-            30,
-            87,
+            59,
+            91,
+            31,
             13,
             12,
             7,
             21,
-            114,
+            118,
             13,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            85,
-            65,
-            52,
-            85,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            89,
+            56,
+            56,
+            69,
             4,
-            83,
-            144,
-            29,
-            107,
-            140,
+            31,
+            150,
+            87,
+            30,
+            99,
             12,
             13,
             23,
-            85,
-            49,
+            89,
+            52,
             7,
             16,
-            58,
+            62,
             4,
             7,
-            57,
-            64,
-            58,
+            61,
+            37,
+            68,
+            62,
             4,
             7,
-            31,
-            137,
+            32,
+            143,
             13,
-            113,
-            130,
-            49,
-            130,
-            90,
+            117,
+            136,
             52,
-            130,
-            96,
+            136,
+            94,
+            56,
+            136,
+            102,
             13,
-            108,
-            141,
-            89,
-            54,
+            113,
+            147,
+            93,
+            58,
+            30,
             4,
-            29,
-            31,
             13,
-            85,
-            40,
-            114,
+            32,
+            89,
+            41,
+            118,
+            56,
+            45,
+            89,
+            89,
+            116,
+            89,
             52,
-            43,
-            85,
-            85,
-            111,
-            49,
-            58,
+            62,
             13,
-            130,
-            85,
+            136,
+            89,
             13,
-            121,
+            126,
+            60,
             56,
-            112,
+            89,
             114,
-            85,
-            109,
-            145,
-            46,
-            56,
-            101,
-            83,
+            151,
+            49,
+            114,
+            107,
+            60,
+            87,
             13,
             9,
-            125,
+            130,
+            96,
+            32,
             13,
+            89,
+            96,
             31,
-            85,
-            30,
-            109,
-            52
+            13,
+            114,
+            13,
+            56
         ],
         "goto": {
             "col_index": [
-                20,
-                105,
-                20,
-                105,
-                51,
-                37,
-                20,
+                21,
                 101,
+                21,
+                114,
+                51,
+                38,
+                21,
+                107,
                 45,
-                103,
-                105,
+                112,
+                114,
                 63,
                 55,
                 59,
-                98,
+                99,
+                70,
+                43,
+                114,
+                75,
                 69,
-                42,
-                105,
-                74,
-                68,
                 64,
                 57,
                 60,
-                24,
-                70,
-                43,
+                25,
+                71,
+                44,
                 56,
-                20,
-                103,
-                23,
-                103,
-                20,
-                97,
-                32,
+                21,
+                108,
+                24,
+                112,
+                21,
+                98,
+                33,
                 65,
                 58,
-                34,
+                98,
+                100,
                 50,
-                36,
-                97,
-                20,
+                37,
+                21,
+                98,
+                21,
                 61,
-                104,
-                20,
+                113,
+                21,
                 46,
-                22,
-                83,
-                26,
-                40,
+                23,
+                81,
+                27,
+                41,
                 48,
-                72,
+                73,
                 53,
-                77,
-                79,
-                107,
-                27,
-                71,
-                81,
-                105,
-                102,
+                78,
+                112,
+                28,
+                72,
+                114,
+                111,
                 52,
-                38,
-                41,
-                49,
-                33,
+                66,
                 39,
-                80,
-                30,
-                44,
+                42,
+                49,
+                34,
+                40,
+                79,
+                31,
+                114,
                 62,
-                97,
-                25,
-                75,
-                28,
-                66,
-                106,
-                73,
+                82,
+                26,
+                76,
+                35,
+                29,
+                67,
+                115,
+                74,
                 47,
-                31,
+                32,
                 54,
+                22,
+                68,
+                77,
+                107,
+                116,
+                30,
+                98,
                 21,
-                67,
-                76,
-                108,
-                29,
-                78,
-                97,
-                20,
-                35,
-                109,
-                82
+                36,
+                110,
+                80
             ],
-            "mark": 102,
+            "mark": 111,
             "quotient": [
                 -1,
                 6,
                 10,
                 16,
                 27,
                 39,
                 45,
                 52,
-                84,
-                107,
-                183,
-                210,
-                217,
-                254,
-                260,
+                87,
+                193,
+                221,
+                228,
+                255,
                 266,
-                269,
                 273,
-                281,
+                279,
+                282,
                 286,
+                294,
+                299,
+                325,
                 -1,
                 1,
                 2,
                 3,
                 14,
                 19,
                 21,
                 23,
                 30,
                 31,
                 42,
                 49,
                 54,
                 55,
-                59,
-                70,
-                71,
+                58,
                 72,
                 73,
-                76,
-                80,
-                81,
-                87,
-                88,
-                90,
-                96,
-                97,
-                104,
+                74,
+                75,
+                78,
+                83,
+                84,
+                89,
+                91,
+                99,
+                100,
                 109,
-                110,
-                114,
                 115,
-                118,
+                116,
+                121,
                 122,
-                123,
-                127,
+                125,
                 128,
                 129,
-                131,
-                136,
+                133,
+                134,
+                135,
                 137,
-                138,
-                140,
-                142,
                 143,
                 144,
+                145,
+                147,
+                149,
+                150,
+                151,
                 173,
-                174,
-                180,
-                185,
-                186,
-                187,
+                183,
+                184,
                 190,
-                191,
                 195,
+                196,
                 197,
-                198,
-                242,
-                243,
-                271,
-                293,
-                295,
-                299,
-                302,
+                201,
+                202,
+                206,
+                208,
+                209,
+                284,
+                307,
+                312,
+                315,
+                320,
                 -1,
                 13,
                 20,
                 33,
-                47,
-                58,
-                79,
-                89,
-                141,
-                168,
-                212,
-                272,
-                306,
+                48,
+                82,
+                92,
+                114,
+                148,
+                177,
+                199,
+                222,
+                285,
+                308,
+                321,
                 -1,
                 44,
+                60,
+                316,
                 43,
-                61,
+                59,
+                64,
+                112,
+                317,
                 -1,
-                75,
-                239,
-                168,
-                69,
-                68,
-                298,
-                66,
-                240,
-                117,
-                0,
-                168,
-                113,
-                75,
+                253,
+                252,
+                185,
+                77,
                 311,
-                117,
-                69,
+                177,
+                71,
+                70,
                 68,
-                251,
-                120,
-                101,
+                77,
+                328,
                 177,
-                95,
-                101,
-                181,
-                95,
-                179,
-                175,
-                101,
-                181,
-                95,
-                235,
-                101,
-                91,
-                95,
-                75,
+                132,
+                136,
+                104,
+                94,
+                98,
+                93,
+                124,
+                314,
+                177,
+                120,
+                77,
                 0,
                 0,
-                126,
-                130,
-                101,
-                148,
-                95,
-                101,
-                170,
-                95,
-                101,
-                171,
-                95,
-                101,
-                172,
-                95,
-                117,
-                194,
-                75,
-                196,
+                71,
+                70,
+                141,
+                104,
+                94,
+                98,
+                182,
+                104,
+                191,
+                98,
+                189,
+                104,
+                191,
+                98,
+                249,
+                104,
+                155,
+                98,
+                104,
+                179,
+                98,
+                104,
+                180,
+                98,
+                104,
+                181,
+                98,
+                104,
+                187,
+                98,
+                124,
+                205,
+                77,
+                207,
                 0,
-                200,
-                130,
-                101,
-                219,
-                95,
-                101,
-                220,
-                95,
-                101,
-                221,
-                95,
-                101,
-                222,
-                95,
-                101,
-                223,
-                95,
-                101,
-                224,
-                95,
-                101,
-                225,
-                95,
-                101,
-                226,
-                95,
-                101,
-                227,
-                95,
-                101,
-                228,
-                95,
-                101,
-                229,
-                95,
-                101,
+                211,
+                136,
+                104,
                 230,
-                95,
-                101,
+                98,
+                104,
                 231,
-                95,
-                101,
+                98,
+                104,
                 232,
-                95,
-                101,
+                98,
+                104,
                 233,
-                95,
-                101,
+                98,
+                104,
                 234,
-                95,
-                101,
+                98,
+                104,
+                235,
+                98,
+                104,
+                236,
+                98,
+                104,
                 237,
-                95,
-                101,
-                247,
-                95,
-                117,
-                255,
-                75,
-                196,
+                98,
+                104,
+                238,
+                98,
+                104,
+                239,
+                98,
+                104,
+                240,
+                98,
+                104,
+                241,
+                98,
+                104,
+                242,
+                98,
+                104,
+                243,
+                98,
+                104,
+                244,
+                98,
+                104,
+                245,
+                98,
+                104,
+                246,
+                98,
+                104,
+                259,
+                98,
+                124,
+                268,
+                77,
+                207,
                 0,
-                262,
-                263,
-                101,
-                279,
-                95,
-                101,
-                284,
-                95,
-                101,
-                285,
-                95,
-                101,
-                291,
-                95,
-                101,
+                275,
+                276,
+                104,
+                292,
+                98,
+                104,
                 297,
-                95,
-                296,
-                303,
+                98,
+                104,
+                298,
+                98,
+                104,
+                300,
+                98,
+                104,
+                305,
+                98,
+                104,
+                310,
+                98,
+                104,
+                324,
+                98,
+                77,
                 0,
-                301,
-                101,
-                309,
-                95,
-                75,
+                124,
+                124,
+                212,
+                263,
+                269,
+                77,
+                77,
                 0,
-                117,
-                75,
-                201,
-                256,
-                75,
-                265,
-                117,
-                75,
-                268,
-                288,
-                296,
-                290,
+                124,
+                278,
+                281,
+                302,
+                77,
                 0,
-                294
+                0,
+                0,
+                304
             ],
             "row_index": [
-                84,
+                83,
                 0,
                 0,
                 1,
                 0,
                 0,
                 2,
                 0,
-                85,
+                84,
                 0,
                 3,
                 0,
-                86,
+                85,
                 0,
                 0,
                 0,
                 4,
                 0,
-                84,
-                87,
+                83,
+                86,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 5,
                 0,
-                99,
+                102,
                 6,
                 0,
-                88,
+                87,
                 0,
                 0,
                 7,
-                84,
+                83,
                 0,
                 0,
                 0,
                 0,
-                89,
-                100,
+                103,
+                104,
                 0,
                 0,
                 0,
                 0,
+                111,
                 0,
-                102,
                 0,
-                90,
+                88,
                 0,
-                84,
+                83,
                 0,
                 8,
                 0,
-                91,
-                133,
-                9,
+                89,
+                122,
+                105,
                 0,
-                84,
                 0,
                 0,
-                110,
+                90,
                 0,
-                114,
                 0,
                 0,
+                126,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
-                84,
                 0,
-                136,
                 0,
                 0,
+                83,
                 0,
+                117,
                 0,
-                84,
+                130,
                 0,
                 0,
-                92,
                 0,
+                83,
                 0,
                 0,
+                91,
                 0,
-                141,
-                93,
                 0,
                 0,
                 0,
+                148,
+                92,
+                0,
                 0,
                 0,
                 0,
-                144,
-                147,
-                150,
                 0,
                 0,
+                151,
+                154,
+                157,
                 0,
                 0,
-                121,
-                124,
                 0,
                 0,
-                10,
+                136,
                 0,
-                84,
+                160,
+                140,
                 0,
                 0,
+                9,
                 0,
                 0,
+                83,
+                93,
                 0,
-                84,
                 0,
-                153,
                 0,
-                84,
                 0,
                 0,
-                155,
-                243,
+                83,
                 0,
+                163,
+                83,
                 0,
                 0,
+                165,
+                252,
                 0,
                 0,
                 0,
                 0,
-                136,
                 0,
                 0,
                 0,
+                117,
                 0,
                 0,
-                11,
+                0,
+                0,
+                0,
+                0,
+                10,
                 94,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
-                12,
-                93,
-                160,
-                163,
-                166,
-                169,
-                172,
-                175,
-                178,
-                181,
-                184,
-                187,
-                190,
-                193,
-                196,
-                199,
-                202,
-                205,
-                129,
+                11,
+                92,
+                170,
+                173,
+                176,
+                179,
+                182,
+                185,
+                188,
+                191,
+                194,
+                197,
+                200,
+                203,
+                206,
+                209,
+                212,
+                215,
                 0,
-                208,
                 0,
+                218,
                 0,
-                93,
-                93,
-                93,
-                102,
-                84,
                 0,
                 0,
-                93,
-                211,
+                144,
+                92,
+                92,
+                92,
+                148,
+                109,
+                12,
                 0,
                 0,
-                93,
+                92,
+                221,
                 0,
                 0,
-                116,
+                92,
+                0,
+                0,
+                254,
                 0,
                 0,
                 0,
                 13,
                 0,
                 0,
                 0,
-                214,
-                245,
+                0,
+                224,
+                255,
                 0,
                 0,
                 0,
                 14,
                 0,
-                216,
+                226,
                 0,
                 0,
                 0,
                 0,
-                246,
+                259,
                 15,
-                249,
+                260,
                 0,
                 0,
                 16,
                 0,
                 0,
                 0,
                 0,
                 95,
                 17,
                 0,
                 0,
                 0,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
-                93,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
+                92,
                 0,
                 0,
-                93,
                 0,
                 0,
                 0,
-                221,
                 0,
                 0,
+                231,
+                0,
                 18,
                 0,
                 0,
-                93,
+                92,
                 0,
-                224,
-                227,
+                234,
+                237,
                 0,
                 0,
                 19,
                 0,
+                240,
                 0,
                 0,
                 0,
-                251,
+                262,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
                 0,
-                252,
+                266,
                 0,
                 0,
                 0,
+                243,
                 0,
-                230,
                 0,
                 0,
-                93,
-                255,
+                92,
+                96,
                 0,
                 0,
-                233,
-                93,
-                102,
+                246,
+                92,
+                111,
                 0,
+                126,
                 0,
                 0,
                 0,
                 0,
-                93,
+                92,
                 0,
-                236,
+                106,
                 0,
                 0,
+                92,
                 0,
-                93,
                 0,
+                97,
                 0,
-                96,
                 0,
                 0,
                 0,
                 0,
-                240,
-                9,
+                249,
+                20,
+                0,
+                0,
+                0,
+                117,
+                0,
                 0,
                 0,
-                110,
                 0,
                 0,
                 0
             ]
         },
         "initial": {
             "start": 0
@@ -2974,88 +3143,90 @@
             "arrow_of(simple_type)",
             "assume_section",
             "assumption",
             "case_expr",
             "comma_list(arg_type)",
             "comma_list(expr)",
             "comma_list(ffi_symbol)",
-            "comma_list(field)",
+            "comma_list(field_dfn)",
             "comma_list(import_symbol)",
             "comma_list(name)",
             "comma_list(parameter)",
             "comma_list(reference)",
             "comma_list(simple_type)",
             "comma_separated_list(arg_type)",
             "comma_separated_list(expr)",
             "comma_separated_list(ffi_symbol)",
-            "comma_separated_list(field)",
+            "comma_separated_list(field_dfn)",
             "comma_separated_list(import_symbol)",
             "comma_separated_list(name)",
             "comma_separated_list(parameter)",
             "comma_separated_list(reference)",
             "comma_separated_list(simple_type)",
             "define_section",
             "else_clause",
             "export_section",
             "expr",
             "ffi_body",
             "ffi_group",
             "ffi_linkage",
             "ffi_symbol",
-            "field",
+            "field_dfn",
+            "formals",
             "function",
             "generic(arg_type)",
             "generic(simple_type)",
+            "hint",
             "import_directive",
             "import_section",
             "import_symbol",
             "list_expr",
             "main_section",
             "match_expr",
             "module_definition",
             "optional(else_clause)",
             "optional(package)",
             "optional(round_list(import_symbol))",
             "optional(round_list(parameter))",
             "optional(square_list(arg_type))",
             "optional(square_list(simple_type))",
-            "optional(type_hint)",
             "optional(type_parameters)",
             "optional(where_clause)",
             "package",
             "parameter",
-            "pattern",
             "record_spec",
             "reference",
             "round_list(arg_type)",
-            "round_list(field)",
+            "round_list(expr)",
+            "round_list(field_dfn)",
             "round_list(import_symbol)",
             "round_list(parameter)",
             "round_list(reference)",
             "round_list(simple_type)",
             "semicolon_list(alternative)",
             "semicolon_list(assumption)",
             "semicolon_list(expr)",
             "semicolon_list(ffi_group)",
             "semicolon_list(function)",
             "semicolon_list(import_directive)",
             "semicolon_list(subtype)",
+            "semicolon_list(top_level)",
             "semicolon_list(type_declaration)",
             "semicolon_list(when_clause)",
             "simple_type",
             "square_list(arg_type)",
             "square_list(expr)",
             "square_list(name)",
             "square_list(simple_type)",
             "start",
             "subject",
             "subtype",
+            "top_level",
             "type_body",
             "type_declaration",
-            "type_hint",
             "type_parameters",
             "typedef_section",
             "variant_spec",
             "when_clause",
             "where_clause"
         ],
         "rule": {
@@ -3071,19 +3242,19 @@
                 "concrete_type",
                 "generic_type",
                 "type_parameters",
                 "RecordSpec",
                 "VariantSpec",
                 "FormalParameter",
                 "SubTypeSpec",
-                "UserDefinedFunction",
+                "Assumption",
+                "UserFunction",
                 "WhereClause",
                 "ExplicitTypeVariable",
                 "ImplicitTypeVariable",
-                "Assumption",
                 "FieldReference",
                 "Cond",
                 "Negative",
                 "PowerOf",
                 "Mul",
                 "FloatDiv",
                 "FloatMod",
@@ -3108,14 +3279,18 @@
                 "ExplicitList",
                 "CaseWhen",
                 null,
                 "MatchExpr",
                 "simple_subject",
                 "Subject",
                 "Alternative",
+                "Skip",
+                "BoundMethod",
+                "DoBlock",
+                "UserDefinedMethod",
                 "ImportForeign",
                 "FFI_Group",
                 "FFI_Symbol",
                 "FFI_Alias",
                 "first",
                 "more",
                 "ArrowSpec",
@@ -3133,57 +3308,54 @@
                 30,
                 31,
                 31,
                 32,
                 32,
                 33,
                 33,
-                39,
-                40,
+                35,
+                35,
                 41,
                 42,
-                42,
+                43,
                 44,
-                45,
-                51,
-                52,
+                44,
+                46,
+                47,
                 53,
+                54,
                 55,
                 57,
-                57,
-                57,
-                58,
-                58,
+                59,
+                59,
+                59,
                 60,
-                61,
+                60,
+                62,
                 63,
                 65,
-                66,
                 67,
-                78,
-                79,
-                87,
-                88,
-                88,
-                90,
-                90,
-                91,
-                92,
-                106,
-                121,
-                121,
-                121,
-                121,
-                121,
-                121,
-                122,
-                123,
-                124,
-                125,
-                126,
+                68,
+                69,
+                86,
+                99,
+                100,
+                108,
+                109,
+                110,
+                110,
+                112,
+                112,
+                113,
+                114,
+                127,
+                127,
+                127,
+                127,
+                127,
                 127,
                 128,
                 129,
                 130,
                 131,
                 132,
                 133,
@@ -3192,140 +3364,151 @@
                 136,
                 137,
                 138,
                 139,
                 140,
                 141,
                 142,
+                143,
                 144,
                 145,
                 146,
+                147,
                 148,
-                149,
+                150,
                 151,
-                153,
+                152,
                 154,
                 155,
+                157,
                 159,
                 160,
                 161,
-                162,
-                163,
-                164,
-                175,
-                177,
-                177,
-                177,
-                178,
-                178,
-                179,
-                180,
-                181,
-                194,
-                194,
-                192,
-                192,
-                191,
-                191,
-                193,
-                193,
-                197,
-                192,
-                192,
-                191,
-                191,
-                194,
-                194,
-                193,
-                193,
-                194,
-                194,
-                193,
-                193,
-                196,
-                192,
-                192,
-                191,
-                191,
-                73,
-                197,
-                192,
-                192,
-                191,
-                191,
-                72,
-                194,
-                194,
-                196,
-                194,
-                194,
-                194,
-                194,
-                197,
-                192,
-                192,
-                191,
-                191,
-                193,
-                193,
-                197,
-                192,
-                192,
-                191,
-                191,
-                73,
-                197,
-                192,
-                192,
-                191,
-                191,
-                72,
-                194,
-                194,
-                196,
-                196,
-                194,
-                194,
-                197,
-                192,
-                192,
-                191,
+                165,
+                166,
+                167,
+                168,
+                168,
+                169,
+                189,
+                190,
                 191,
-                194,
-                194,
-                193,
-                193,
-                193,
-                193,
                 193,
-                193,
-                193,
-                193,
-                193,
-                193,
-                192,
-                192,
-                191,
-                191
+                207,
+                209,
+                209,
+                209,
+                210,
+                210,
+                211,
+                212,
+                213,
+                226,
+                226,
+                224,
+                224,
+                223,
+                223,
+                225,
+                225,
+                229,
+                224,
+                224,
+                223,
+                223,
+                226,
+                226,
+                225,
+                225,
+                225,
+                225,
+                228,
+                224,
+                224,
+                223,
+                223,
+                229,
+                75,
+                229,
+                224,
+                224,
+                223,
+                223,
+                74,
+                226,
+                226,
+                228,
+                226,
+                226,
+                229,
+                224,
+                224,
+                223,
+                223,
+                225,
+                225,
+                226,
+                226,
+                225,
+                225,
+                229,
+                224,
+                224,
+                223,
+                223,
+                75,
+                229,
+                224,
+                224,
+                223,
+                223,
+                74,
+                226,
+                226,
+                228,
+                228,
+                226,
+                226,
+                229,
+                224,
+                224,
+                223,
+                223,
+                226,
+                226,
+                225,
+                225,
+                225,
+                225,
+                225,
+                225,
+                225,
+                225,
+                225,
+                225,
+                224,
+                224,
+                223,
+                223
             ],
             "rules": [
                 [
-                    80,
+                    82,
                     1,
                     -1,
                     []
                 ],
                 [
-                    80,
+                    82,
                     3,
                     -3,
                     []
                 ],
                 [
-                    45,
+                    47,
                     6,
                     0,
                     [
                         -6,
                         -5,
                         -4,
                         -3,
@@ -3342,33 +3525,33 @@
                 [
                     29,
                     0,
                     1,
                     []
                 ],
                 [
-                    40,
+                    42,
                     3,
                     -1,
                     []
                 ],
                 [
-                    40,
+                    42,
                     0,
                     1,
                     []
                 ],
                 [
-                    87,
+                    89,
                     3,
                     -1,
                     []
                 ],
                 [
-                    87,
+                    89,
                     0,
                     1,
                     []
                 ],
                 [
                     6,
                     3,
@@ -3390,44 +3573,56 @@
                 [
                     27,
                     0,
                     1,
                     []
                 ],
                 [
-                    43,
+                    45,
                     3,
                     -1,
                     []
                 ],
                 [
-                    43,
+                    45,
                     0,
                     1,
                     []
                 ],
                 [
-                    39,
+                    85,
+                    1,
+                    -1,
+                    []
+                ],
+                [
+                    85,
+                    1,
+                    -1,
+                    []
+                ],
+                [
+                    41,
                     4,
                     2,
                     [
                         -4,
                         -3,
                         -2,
                         -1
                     ]
                 ],
                 [
-                    55,
+                    56,
                     2,
                     -2,
                     []
                 ],
                 [
-                    41,
+                    43,
                     2,
                     3,
                     [
                         -2,
                         -1
                     ]
                 ],
@@ -3457,88 +3652,88 @@
                     6,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    84,
+                    87,
                     3,
                     7,
                     [
                         -3
                     ]
                 ],
                 [
-                    84,
+                    87,
                     3,
                     8,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    84,
+                    87,
                     4,
                     9,
                     [
                         -4,
                         -3,
                         -1
                     ]
                 ],
                 [
-                    86,
+                    88,
                     1,
                     10,
                     [
                         -1
                     ]
                 ],
                 [
-                    83,
+                    86,
                     1,
                     -1,
                     []
                 ],
                 [
-                    83,
+                    86,
                     1,
                     -1,
                     []
                 ],
                 [
-                    83,
+                    86,
                     1,
                     -1,
                     []
                 ],
                 [
-                    75,
+                    77,
                     1,
                     -1,
                     []
                 ],
                 [
-                    75,
+                    77,
                     1,
                     -1,
                     []
                 ],
                 [
                     58,
                     1,
                     11,
                     [
                         -1
                     ]
                 ],
                 [
-                    88,
+                    90,
                     4,
                     12,
                     [
                         -2
                     ]
                 ],
                 [
@@ -3547,62 +3742,77 @@
                     13,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    82,
+                    84,
                     2,
                     14,
                     [
                         -2,
                         -1
                     ]
                 ],
                 [
-                    82,
+                    84,
                     2,
                     14,
                     [
                         -2,
                         -1
                     ]
                 ],
                 [
-                    82,
+                    84,
                     1,
                     14,
                     [
                         -1
                     ]
                 ],
                 [
-                    36,
-                    6,
+                    7,
+                    3,
                     15,
                     [
+                        -3,
+                        -1
+                    ]
+                ],
+                [
+                    37,
+                    6,
+                    16,
+                    [
                         -6,
                         -5,
                         -4,
                         -2,
                         -1
                     ]
                 ],
                 [
-                    90,
+                    92,
                     4,
-                    16,
+                    17,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    56,
+                    36,
+                    1,
+                    -1,
+                    []
+                ],
+                [
+                    57,
                     2,
                     13,
                     [
                         -2,
                         -1
                     ]
                 ],
@@ -3629,34 +3839,25 @@
                     1,
                     -1,
                     []
                 ],
                 [
                     3,
                     2,
-                    17,
+                    18,
                     [
                         -2,
                         -1
                     ]
                 ],
                 [
                     3,
                     1,
-                    18,
-                    [
-                        -1
-                    ]
-                ],
-                [
-                    7,
-                    3,
                     19,
                     [
-                        -3,
                         -1
                     ]
                 ],
                 [
                     30,
                     1,
                     -1,
@@ -3902,19 +4103,19 @@
                     40,
                     [
                         -1
                     ]
                 ],
                 [
                     30,
-                    4,
+                    2,
                     41,
                     [
-                        -4,
-                        -2
+                        -2,
+                        -1
                     ]
                 ],
                 [
                     30,
                     2,
                     42,
                     [
@@ -3935,15 +4136,15 @@
                     1,
                     44,
                     [
                         -1
                     ]
                 ],
                 [
-                    42,
+                    44,
                     1,
                     45,
                     [
                         -1
                     ]
                 ],
                 [
@@ -3952,15 +4153,15 @@
                     46,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
-                    89,
+                    91,
                     4,
                     47,
                     [
                         -4,
                         -3,
                         -1
                     ]
@@ -3968,43 +4169,49 @@
                 [
                     28,
                     3,
                     -2,
                     []
                 ],
                 [
-                    44,
+                    46,
                     7,
                     48,
                     [
                         -6,
                         -5,
                         -3,
                         -2
                     ]
                 ],
                 [
-                    81,
+                    83,
                     1,
                     49,
                     [
                         -1
                     ]
                 ],
                 [
-                    81,
+                    83,
                     3,
                     50,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    85,
+                    40,
+                    0,
+                    4,
+                    []
+                ],
+                [
+                    40,
                     2,
                     -1,
                     []
                 ],
                 [
                     1,
                     4,
@@ -4013,23 +4220,51 @@
                         -4,
                         -3,
                         -2,
                         -1
                     ]
                 ],
                 [
-                    57,
+                    30,
                     1,
-                    -1,
+                    52,
                     []
                 ],
                 [
-                    39,
+                    30,
+                    3,
+                    53,
+                    [
+                        -3,
+                        -1
+                    ]
+                ],
+                [
+                    30,
+                    3,
+                    54,
+                    [
+                        -2
+                    ]
+                ],
+                [
+                    37,
+                    6,
+                    55,
+                    [
+                        -5,
+                        -4,
+                        -2,
+                        -1
+                    ]
+                ],
+                [
+                    41,
                     4,
-                    52,
+                    56,
                     [
                         -3,
                         -2,
                         -1
                     ]
                 ],
                 [
@@ -4061,46 +4296,46 @@
                     0,
                     1,
                     []
                 ],
                 [
                     32,
                     4,
-                    53,
+                    57,
                     [
                         -4,
                         -2,
                         -1
                     ]
                 ],
                 [
                     34,
                     1,
-                    54,
+                    58,
                     [
                         -1
                     ]
                 ],
                 [
                     34,
                     3,
-                    55,
+                    59,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    53,
+                    54,
                     0,
                     4,
                     []
                 ],
                 [
-                    53,
+                    54,
                     1,
                     -1,
                     []
                 ],
                 [
                     11,
                     1,
@@ -4112,47 +4347,47 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     20,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     20,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    69,
+                    70,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    69,
+                    70,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
-                    64,
+                    65,
                     3,
                     -2,
                     []
                 ],
                 [
                     16,
                     1,
@@ -4164,88 +4399,76 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     25,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     25,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    46,
+                    48,
                     0,
                     4,
                     []
                 ],
                 [
-                    46,
+                    48,
                     1,
                     -1,
                     []
                 ],
                 [
-                    66,
+                    67,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    66,
+                    67,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
-                    52,
-                    0,
-                    4,
-                    []
-                ],
-                [
-                    52,
-                    1,
-                    -1,
-                    []
-                ],
-                [
-                    74,
+                    76,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    74,
+                    76,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
-                    77,
+                    79,
                     3,
                     -2,
                     []
                 ],
                 [
                     10,
                     1,
@@ -4257,32 +4480,38 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     19,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     19,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
+                    61,
+                    3,
+                    -2,
+                    []
+                ],
+                [
                     4,
                     3,
-                    58,
+                    62,
                     [
                         -3,
                         -2,
                         -1
                     ]
                 ],
                 [
@@ -4302,81 +4531,69 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     18,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     18,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    37,
+                    38,
                     2,
-                    59,
+                    63,
                     [
                         -2,
                         -1
                     ]
                 ],
                 [
-                    50,
+                    52,
                     0,
                     4,
                     []
                 ],
                 [
-                    50,
+                    52,
                     1,
                     -1,
                     []
                 ],
                 [
-                    76,
+                    78,
                     3,
                     -2,
                     []
                 ],
                 [
-                    54,
-                    0,
-                    4,
-                    []
-                ],
-                [
-                    54,
-                    1,
-                    -1,
-                    []
-                ],
-                [
-                    49,
+                    51,
                     0,
                     4,
                     []
                 ],
                 [
-                    49,
+                    51,
                     1,
                     -1,
                     []
                 ],
                 [
-                    63,
+                    64,
                     3,
                     -2,
                     []
                 ],
                 [
                     15,
                     1,
@@ -4388,47 +4605,76 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     24,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     24,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    72,
+                    71,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    72,
+                    71,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
+                    55,
+                    0,
+                    4,
+                    []
+                ],
+                [
+                    55,
+                    1,
+                    -1,
+                    []
+                ],
+                [
+                    73,
+                    2,
+                    60,
+                    [
+                        -2
+                    ]
+                ],
+                [
+                    73,
+                    3,
                     61,
+                    [
+                        -3,
+                        -2
+                    ]
+                ],
+                [
+                    62,
                     3,
                     -2,
                     []
                 ],
                 [
                     12,
                     1,
@@ -4440,40 +4686,40 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     21,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     21,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
                     5,
                     3,
-                    58,
+                    62,
                     [
                         -3,
                         -2,
                         -1
                     ]
                 ],
                 [
-                    65,
+                    66,
                     3,
                     -2,
                     []
                 ],
                 [
                     17,
                     1,
@@ -4485,75 +4731,75 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     26,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     26,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    38,
+                    39,
                     2,
-                    59,
+                    63,
                     [
                         -2,
                         -1
                     ]
                 ],
                 [
-                    51,
+                    53,
                     0,
                     4,
                     []
                 ],
                 [
-                    51,
+                    53,
                     1,
                     -1,
                     []
                 ],
                 [
-                    79,
+                    81,
                     3,
                     -2,
                     []
                 ],
                 [
-                    78,
+                    80,
                     3,
                     -2,
                     []
                 ],
                 [
-                    48,
+                    50,
                     0,
                     4,
                     []
                 ],
                 [
-                    48,
+                    50,
                     1,
                     -1,
                     []
                 ],
                 [
-                    62,
+                    63,
                     3,
                     -2,
                     []
                 ],
                 [
                     13,
                     1,
@@ -4565,120 +4811,120 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     22,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     22,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ],
                 [
-                    47,
+                    49,
                     0,
                     4,
                     []
                 ],
                 [
-                    47,
+                    49,
                     1,
                     -1,
                     []
                 ],
                 [
-                    68,
+                    69,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    68,
+                    69,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
-                    70,
+                    74,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    70,
+                    74,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
-                    67,
+                    68,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    67,
+                    68,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
-                    73,
+                    75,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    73,
+                    75,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
-                    71,
+                    72,
                     2,
-                    56,
+                    60,
                     [
                         -2
                     ]
                 ],
                 [
-                    71,
+                    72,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -2
                     ]
                 ],
                 [
                     14,
@@ -4691,23 +4937,23 @@
                     2,
                     -2,
                     []
                 ],
                 [
                     23,
                     1,
-                    56,
+                    60,
                     [
                         -1
                     ]
                 ],
                 [
                     23,
                     3,
-                    57,
+                    61,
                     [
                         -3,
                         -1
                     ]
                 ]
             ]
         },
@@ -4737,51 +4983,55 @@
             "AND",
             "AS",
             "ASSUME",
             "BEGIN",
             "CASE",
             "DEFINE",
             "DIV",
+            "DO",
             "ELSE",
             "END",
             "ESAC",
             "EXPORT",
             "FOREIGN",
             "IF",
             "IMPORT",
             "IS",
             "MOD",
             "NO",
             "NOT",
             "OF",
             "OPAQUE",
             "OR",
+            "SKIP",
             "THEN",
+            "TO",
             "TYPE",
             "WHEN",
             "WHERE",
             "YES",
             "[",
             "]",
             "^",
+            "actor",
             "integer",
             "name",
             "real",
             "short_string"
         ]
     },
     "scanner": {
         "action": {
             "line_number": [
-                240,
-                241,
-                242,
-                244,
-                245,
-                246
+                276,
+                277,
+                278,
+                280,
+                281,
+                282
             ],
             "message": [
                 [
                     "integer"
                 ],
                 [
                     "real"
```

### Comparing `sophie-lang-0.0.0/sophie/adapters/turtle_adapter.py` & `sophie-lang-0.0.3/sophie/adapters/turtle_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-NIL : dict
+from ..runtime import force, iterate_list
 
-def sophie_init(force, nil):
-	global NIL
-	NIL = force(nil)
+def sophie_init():
 	return {'drawing':do_turtle_graphics}
 
-def do_turtle_graphics(force, env, drawing):
+def do_turtle_graphics(env, drawing):
 	import turtle, tkinter
 	root = tkinter.Tk()
 	root.focus_force()
 	root.title("Sophie: Turtle Graphics")
 	screen = tkinter.Canvas(root, width=1000, height=1000)
 	screen.pack()
 	t = turtle.RawTurtle(screen)
 	t.hideturtle()
 	t.speed(0)
 	t.screen.tracer(2^31)
 	t.screen.delay(0)
 	t.setheading(90)
 	stepCount = 0
-	steps = force(drawing["steps"])
-	while steps is not NIL:
+	for step in iterate_list(drawing["steps"]):
 		stepCount += 1
-		s = force(steps['head'])
-		steps = force(steps['tail'])
-		args = dict(s)  # Make a copy because of (deliberate) aliasing.
+		args = dict(step)  # Make a copy because of (deliberate) aliasing.
 		tag = args.pop("")
 		fn = getattr(t, tag)
 		fn(*map(force, args.values()))  # Insertion-order is assured.
 	t.screen.update()
 	text = str(stepCount)+" turtle steps. Click the drawing or press any key to dismiss it."
 	print(text)
 	label = tkinter.Label(root, text=text)
```

### Comparing `sophie-lang-0.0.0/sophie/calculus.py` & `sophie-lang-0.0.3/sophie/calculus.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,32 +29,35 @@
 I can reuse the one from booze-tools.
 
 """
 from typing import Iterable
 from boozetools.support.foundation import EquivalenceClassifier
 from . import syntax
 from .ontology import Symbol
-from .stacking import StackFrame
+from .stacking import Frame
 
-TYPE_ENV = StackFrame["SophieType"]
+TYPE_ENV = Frame["SophieType"]
 
 _type_numbering_subsystem = EquivalenceClassifier()
 
 class SophieType:
 	"""Value objects so they can play well with the classifier"""
 	def visit(self, visitor:"TypeVisitor"): raise NotImplementedError(type(self))
 
 	def __init__(self, *key):
 		self._key = key
 		self._hash = hash(key)
 		self.number = _type_numbering_subsystem.classify(self)
 	def __hash__(self): return self._hash
 	def __eq__(self, other: "SophieType"): return type(self) is type(other) and self._key == other._key
 	def exemplar(self) -> "SophieType": return _type_numbering_subsystem.exemplars[self.number]
-	def __str__(self) -> str: return self.visit(Render())
+	def __repr__(self) -> str:
+		it = self.visit(Render())
+		assert isinstance(it, str), (it, type(self))
+		return it
 
 class TypeVariable(SophieType):
 	"""Did I say value-object? Not for type variables! These have identity."""
 	def __init__(self):
 		super().__init__(len(_type_numbering_subsystem.catalog))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_variable(self)
 
@@ -82,15 +85,14 @@
 	def __init__(self, variant: syntax.Variant, type_args: Iterable[SophieType]):
 		assert isinstance(variant, syntax.Variant)
 		self.variant = variant
 		self.type_args = tuple(a.exemplar() for a in type_args)
 		assert len(self.type_args) == len(variant.type_params)
 		super().__init__(self.variant, *(a.number for a in self.type_args))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_sum(self)
-	def __repr__(self): return "[SumType:%s]"%self.variant.nom.text
 
 class SubType(SophieType):
 	st : syntax.SubTypeSpec
 
 class EnumType(SubType):
 	def __init__(self, st: syntax.SubTypeSpec):
 		assert st.body is None
@@ -106,41 +108,49 @@
 		self.st = st
 		self.type_args = tuple(a.exemplar() for a in type_args)
 		assert len(self.type_args) == len(st.variant.type_params)
 		super().__init__(st, *(a.number for a in self.type_args))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_tag_record(self)
 	def family(self) -> Symbol: return self.st.variant
 
-
 class ProductType(SophieType):
 	def __init__(self, fields: Iterable[SophieType]):
 		self.fields = tuple(p.exemplar() for p in fields)
 		super().__init__(*(p.number for p in self.fields))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_product(self)
 	
 class ArrowType(SophieType):
 	def __init__(self, arg: ProductType, res: SophieType):
 		self.arg, self.res = arg.exemplar(), res.exemplar()
 		super().__init__(self.arg, self.res)
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_arrow(self)
 
 class UDFType(SophieType):
-	fn: syntax.UserDefinedFunction
-	static_env: StackFrame[SophieType]
+	fn: syntax.UserFunction
+	static_env: TYPE_ENV
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_udf(self)
-	def __init__(self, fn:syntax.UserDefinedFunction, static_env:StackFrame[SophieType]):
+	def __init__(self, fn:syntax.UserFunction, static_env:TYPE_ENV):
 		self.fn = fn
 		self.static_env = static_env
 		# NB: The uniqueness notion here is excessive, but there's a plan to deal with that.
 		#     Whatever instantiates a nested function must enter it in the static scope without duplication.
 		#     Performance hacking may make for an even better cache than that.
 		# TODO: It would be sufficient to key on the types captured in the lexical closure.
 		#       Only DeductionEngine.visit_Lookup creates these, so it could provide the capture.
 		super().__init__(object())
-	def __repr__(self): return "[UDFType:%s]"%self.fn.nom.text
+
+class MethodType(SophieType):
+	pass
+
+class MessageType(SophieType):
+	def visit(self, visitor: "TypeVisitor"):
+		return visitor.on_message(self)
+
+class ActorType(SophieType):
+	pass
 
 class _Bottom(SophieType):
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_bottom()
 
 BOTTOM = _Bottom(None)
 
 class _Error(SophieType):
@@ -156,14 +166,15 @@
 	def on_opaque(self, o: OpaqueType): raise NotImplementedError(type(self))
 	def on_record(self, r:RecordType): raise NotImplementedError(type(self))
 	def on_sum(self, s:SumType): raise NotImplementedError(type(self))
 	def on_tag_enum(self, e: EnumType): raise NotImplementedError(type(self))
 	def on_tag_record(self, t: TaggedRecord): raise NotImplementedError(type(self))
 	def on_arrow(self, a:ArrowType): raise NotImplementedError(type(self))
 	def on_product(self, p:ProductType): raise NotImplementedError(type(self))
+	def on_message(self, m:MessageType): raise NotImplementedError(type(self))
 	def on_udf(self, f:UDFType): raise NotImplementedError(type(self))
 	def on_bottom(self): raise NotImplementedError(type(self))
 	def on_error_type(self): raise NotImplementedError(type(self))
 
 
 class Render(TypeVisitor):
 	""" Return a string representation of the term. """
@@ -172,27 +183,32 @@
 	def on_variable(self, v: TypeVariable):
 		if v not in self._var_names:
 			self._var_names[v] = "?%s" % _name_variable(len(self._var_names) + 1)
 		return self._var_names[v]
 	def on_opaque(self, o: OpaqueType):
 		return o.symbol.nom.text
 	def _generic(self, params:tuple[SophieType]):
-		return "[%s]"%(",".join(t.visit(self) for t in params))
+		if params:
+			return "[%s]"%(",".join(t.visit(self) for t in params))
+		else:
+			return ""
 	def on_record(self, r: RecordType):
 		return r.symbol.nom.text+self._generic(r.type_args)
 	def on_sum(self, s: SumType):
 		return s.variant.nom.text+self._generic(s.type_args)
 	def on_tag_enum(self, e: EnumType):
 		return e.st.nom.text
 	def on_tag_record(self, t: TaggedRecord):
 		return t.st.nom.text+self._generic(t.type_args)
 	def on_arrow(self, a: ArrowType):
 		return a.arg.visit(self)+"->"+a.res.visit(self)
 	def on_product(self, p: ProductType):
 		return "(%s)"%(",".join(t.visit(self) for t in p.fields))
+	def on_message(self, m:MessageType):
+		return "<message>"
 	def on_udf(self, f: UDFType):
 		return "<%s/%d>"%(f.fn.nom.text, len(f.fn.params))
 	def on_bottom(self):
 		return "?"
 	def on_error_type(self):
 		return "-/-"
```

### Comparing `sophie-lang-0.0.0/sophie/front_end.py` & `sophie-lang-0.0.3/sophie/front_end.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 """
 import sys
 from pathlib import Path
-from typing import Union
+from typing import Union, Optional
 
 from boozetools.macroparse.runtime import TypicalApplication, make_tables
 from boozetools.scanning.engine import IterableScanner
 from boozetools.parsing.interface import ParseError
 from boozetools.support.failureprone import Issue
 from boozetools.support.pretty import DOT
 from . import syntax
@@ -50,40 +50,26 @@
 	def unexpected_token(self, kind, semantic, pds):
 		raise SophieParseError(self.stack_symbols(pds), kind, self.yy.slice())
 	
 	pass
 
 sophie_parser = SophieParser(_tables)
 
-def parse_file(path:Path, report:Report):
-	"""Read file given by name; pass contents to next phase."""
-	try:
-		with open(path, "r") as fh:
-			text = fh.read()
-	except FileNotFoundError:
-		report.file_error(path, "I see no file called " + str(path))
-	except OSError:
-		report.file_error(path, "Something went pear-shaped while trying to read " + str(path))
-	else:
-		return parse_text(text, path, report)
-
 def parse_text(text:str, path:Path, report:Report) -> Union[syntax.Module, Issue]:
 	""" Submit text to parser; submit the resulting tree to subsequent pass """
 	assert isinstance(path, Path)
 	try:
 		module = sophie_parser.parse(text, filename=str(path))
-		module.path = path
 		return module
 	except syntax.MismatchedBookendsError as ex:
 		report.error("Checking Bookends", ex.args, "These names don't line up. Has part of a function been lost?")
 	except ParseError as ex:
-		stack_symbols, lookahead, where = ex.args
+		stack_symbols, lookahead, span = ex.args
 		hint = _best_hint(stack_symbols, lookahead)
-		description = "This %r confused Sophie.\n%s"%(lookahead, hint)
-		report.error("Parsing", [where], description)
+		report.generic_parse_error(path, lookahead, span, hint)
 
 ##########################
 #
 #  I've been meaning to improve parse error messages.
 #  Code from here down represents progress in that direction.
 #
 
@@ -137,10 +123,12 @@
 _hint("TYPE : ??? name square_list(name) IS ● OPAQUE", "Opaque types cannot be made generic.")
 _hint("( ??? expr ● ;", "I suspect a missing ')' closing parentheses.")
 _hint("CASE WHEN ??? ● :", "CASE WHEN needs THEN")
 _hint("CASE semicolon_list(when_clause) ELSE expr ; ● ???", "CASE expression is missing ESAC")
 _hint("annotation = expr ● name", "Probably missing a semicolon after the previous definition.")
 _hint("BEGIN : semicolon_list(expr) expr ● <END>", "You need a semicolon after that last expression.")
 _hint("expr ● \"", "Seems to be missing some sort of operator before the string that starts here.")
+_hint("TYPE : ??? name ● =", "A type-name IS something, but a function = something.")
+_hint("TYPE : ??? name type_parameters ● =", "A type-name IS something, but a function = something.")
 
 assert _best_hint("export_section import_section TYPE : name square_list(name) IS".split(), 'OPAQUE')
```

### Comparing `sophie-lang-0.0.0/sophie/ontology.py` & `sophie-lang-0.0.3/sophie/ontology.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Sequence
 from boozetools.support.symtab import NameSpace
 
 class Nom:
 	""" Representing the occurrence of a name anywhere. """
 	_slice: slice  # Empty-slice means pre-defined term.
 	def __init__(self, text, a_slice): self.text, self._slice = text, a_slice or slice(0,0)
 	def head(self) -> slice: return self._slice
@@ -25,22 +25,17 @@
 		return "{%s:%s|%s}" % (self.nom.text, type(self).__name__, getattr(self,"static_depth", "?"))
 	def __str__(self): return self.nom.text
 	def head(self) -> slice: return self.nom.head()
 	def has_value_domain(self) -> bool: raise NotImplementedError(type(self))
 
 NS = NameSpace[Symbol]
 
-class Function(Symbol):
+class Term(Symbol):
 	def has_value_domain(self): return True
 
-class NativeFunction(Function):
-	""" Built-in and foreign (Python) function symbols. """
-	static_depth = 0
-	val:Any  # Fill in during WordDefiner pass
-
 class Expr:
 	def head(self) -> slice:
 		""" Indicate which bit of code this node represents. """
 		raise NotImplementedError(type(self))
 
 class Reference(Expr):
 	nom:Nom
```

### Comparing `sophie-lang-0.0.0/sophie/primitive.py` & `sophie-lang-0.0.3/sophie/primitive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,43 @@
+"""
+Build the primitive namespace.
+Also, some bits used for operator syntax
+and the primitive literal types
+"""
+
 from functools import lru_cache
 from .ontology import NS, Nom
-from .syntax import Opaque, Variant
+from .syntax import Opaque, Variant, FFI_Symbol
 from . import calculus
 
 root_namespace = NS(place=None)
 ops = {}
 
-LIST : Variant  # Generated in the preamble.
-
 def _built_in_type(name:str) -> calculus.OpaqueType:
-	nom = Nom(name, None)
-	symbol = Opaque(nom)
+	symbol = Opaque(Nom(name, None))
 	term = calculus.OpaqueType(symbol)
 	root_namespace[name] = symbol
 	return term
 literal_number = _built_in_type("number")
 literal_string = _built_in_type("string")
 literal_flag = _built_in_type("flag")
 
+# Hack the console object into the root namespace
+root_namespace['console'] = FFI_Symbol(Nom('console', None))
+
+
 @lru_cache()
 def _arrow_of_math(arity:int) -> calculus.ArrowType:
 	return _arrow_of(literal_number, arity)
 
 def _arrow_of(typ: calculus.SophieType, arity:int) -> calculus.ArrowType:
 	assert arity > 0
 	return calculus.ArrowType(calculus.ProductType((typ,) * arity), typ)
 
 def _init():
-	"""
-	Build and return the primitive namespace.
-	Oh, and also some bits used for operator syntax.
-	
-	It's special because it's pre-typed.
-	"""
 	import operator
 	binary = _arrow_of_math(2)
 	ops["PowerOf"] = operator.pow, binary
 	ops["Mul"] = operator.mul, binary
 	ops["FloatDiv"] = operator.truediv, binary
 	ops["FloatMod"] = operator.mod, binary
 	ops["IntDiv"] = operator.ifloordiv, binary
```

### Comparing `sophie-lang-0.0.0/sophie/resolution.py` & `sophie-lang-0.0.3/sophie/resolution.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,113 @@
 """
 All the definition resolution stuff goes here.
 By the time this pass is finished, every name points to its symbol table entry,
 from which we can find the kind, type, and definition.
 """
 from importlib import import_module
+from pathlib import Path
+from traceback import TracebackException
 from typing import Union
+from inspect import signature
 from boozetools.support.foundation import Visitor, strongly_connected_components_hashable
 from boozetools.support.symtab import NoSuchSymbol, SymbolAlreadyExists
-from . import syntax, diagnostics
+from . import syntax, primitive
+from .diagnostics import Report
 from .ontology import NS, Symbol
+from .modularity import Program, SophieParseError, SophieImportError
 
-class _TopDown(Visitor):
+class Yuck(Exception):
+	"""
+	The first argument will be the name of the pass fraught with error.
+	The end-user might not care about this, but it's handy for testing.
+	"""
+	pass
+
+class RoadMap:
+	preamble : syntax.Module
+	list_symbol : syntax.Variant
+	module_scopes : dict[syntax.Module, NS]
+	import_alias : dict[syntax.Module, NS]
+	each_module : list[syntax.Module]
+	each_udf : list[syntax.UserFunction]
+	each_match : list[syntax.MatchExpr]
+	import_map : dict[syntax.ImportModule, syntax.Module]
+
+	def __init__(self, main_path:Path, report:Report):
+		self.module_scopes = {}
+		self.import_alias = {}
+		self.each_module = []
+		self.each_udf = []
+		self.each_match = []
+
+		self.note_udf = self.each_udf.append
+		self.note_match = self.each_match.append
+
+		def register(parent, module):
+			assert isinstance(module, syntax.Module)
+			module_scope = parent.new_child(module.source_path)
+			self.module_scopes[module] = module_scope
+			self.import_alias[module] = NS(place=module.source_path)
+
+			report.set_path(module.source_path)
+			_WordDefiner(self, module, report)
+			if report.sick(): raise Yuck("define")
+
+			resolver = _WordResolver(self, module, report)
+			if report.sick(): raise Yuck("resolve")
+
+			_AliasChecker(self, module, report)
+			if report.sick(): raise Yuck("alias")
+
+			check_constructors(resolver.dubious_constructors, report)
+			if report.sick(): raise Yuck("constructors")
+			
+			for mx in self.each_match:
+				_check_one_match_expression(mx, module_scope, report)
+			if report.sick(): raise Yuck("match_check")
+
+			self.build_match_dispatch_tables()
+			
+			self.each_match.clear()
+			return module
+
+		try: program = Program(main_path, report)
+		except SophieParseError: raise Yuck("parse")
+		except SophieImportError: raise Yuck("import")
+		report.assert_no_issues()
+		self.import_map = program.import_map
+
+		self.preamble = register(primitive.root_namespace, program.preamble)
+		preamble_scope = self.module_scopes[self.preamble]
+		self.list_symbol = preamble_scope['list']
+		for path in program.module_sequence:
+			self.each_module.append(register(preamble_scope, path))
+
+	def build_match_dispatch_tables(self):
+		""" Both the type checker and the simple evaluator uses these. """
+		for mx in self.each_match:
+			mx.dispatch = {
+				alt.nom.key() : alt.sub_expr
+				for alt in mx.alternatives
+			}
+
+
+class TopDown(Visitor):
 	"""
 	Convenience base-class to handle the dreary bits of a
 	perfectly ordinary top-down walk through a syntax tree.
 	"""
+
 	def visit_ArrowSpec(self, it: syntax.ArrowSpec, env):
 		for a in it.lhs:
 			self.visit(a, env)
 		self.visit(it.rhs, env)
-	
+
 	def visit_Literal(self, l:syntax.Literal, env): pass
+
 	def visit_ImplicitType(self, it:syntax.ImplicitTypeVariable, env): pass
 
 	def visit_ShortCutExp(self, it: syntax.ShortCutExp, env):
 		self.visit(it.lhs, env)
 		self.visit(it.rhs, env)
 	
 	def visit_BinExp(self, it: syntax.BinExp, env):
@@ -34,211 +117,204 @@
 	def visit_UnaryExp(self, expr: syntax.UnaryExp, env):
 		self.visit(expr.arg, env)
 	
 	def visit_FieldReference(self, expr: syntax.FieldReference, env):
 		# word-agnostic until we know the type of expr.lhs.
 		self.visit(expr.lhs, env)
 	
+	def visit_BoundMethod(self, expr: syntax.BoundMethod, env):
+		# word-agnostic until we know the type of expr.receiver.
+		self.visit(expr.receiver, env)
+	
 	def visit_Call(self, expr: syntax.Call, env):
 		self.visit(expr.fn_exp, env)
 		for a in expr.args:
 			self.visit(a, env)
 	
 	def visit_Cond(self, expr: syntax.Cond, env):
 		self.visit(expr.if_part, env)
 		self.visit(expr.then_part, env)
 		self.visit(expr.else_part, env)
 	
 	def visit_ExplicitList(self, expr: syntax.ExplicitList, env):
 		for e in expr.elts:
 			self.visit(e, env)
+	
+	def visit_DoBlock(self, db: syntax.DoBlock, env):
+		for s in db.steps:
+			self.visit(s, env)
+
+class _ResolutionPass(TopDown):
+	globals: NS
+	import_alias: NS
+
+	def __init__(self, roadmap: RoadMap, module:syntax.Module, report:Report):
+		self.roadmap = roadmap
+		self.report = report
+		self.globals = self.roadmap.module_scopes[module]
+		self.import_alias = self.roadmap.import_alias[module]
+		self.visit_Module(module)
+
+	def visit_Module(self, module:syntax.Module):
+		raise NotImplementedError(type(self))
 
-class WordDefiner(_TopDown):
+class _WordDefiner(_ResolutionPass):
 	"""
 	At the end of this phase:
 		Names used in declarations have an attached symbol table entry.
 		The entry is installed in all appropriate namespaces.
-		
+
 	Attaches NameSpace objects in key places and install definitions.
 	Takes note of names with more than one definition in the same scope.
 	"""
-	globals : NS
-	
-	def __init__(self, module:syntax.Module, outer:NS, report):
-		self._on_error = report.on_error("Defining words")
-		self.redef, self.missing_foreign, self.broken_foreign = [], [], []
-		self.globals = module.globals = outer.new_child(module)
-		self.all_match_expressions = module.all_match_expressions = []
-		self.all_functions = module.all_functions = []
-		
-		for d in module.imports: self.visit_ImportModule(d, module)
+	def visit_Module(self, module:syntax.Module):
+		self._source_path = module.source_path
+		for d in module.imports: self.visit_ImportModule(d)
 		for td in module.types: self.visit(td)
 		for d in module.foreign: self.visit_ImportForeign(d)
-		
-		if self.missing_foreign:
-			self._on_error(self.missing_foreign, "Some foreign code could not be found.")
-		if self.broken_foreign:
-			self._on_error(self.broken_foreign, "Attempting to import this module threw an exception.")
-			
 		for fn in module.outer_functions:  # Can't iterate all-functions yet; must build it first.
-			self.visit(fn, module.globals)
+			self.visit(fn, self.globals)
 		for expr in module.main:  # Might need to define some case-match symbols here.
-			self.visit(expr, module.globals)
-		if self.redef:
-			self._on_error(self.redef, "I see the same name defined earlier in the same scope:")
+			self.visit(expr, self.globals)
+		pass
 
 	def _install(self, namespace: NS, dfn:Symbol):
-		try: namespace[dfn.nom.text] = dfn
-		except SymbolAlreadyExists: self.redef.append(dfn.nom)
-	
+		try: namespace[dfn.nom.key()] = dfn
+		except SymbolAlreadyExists:
+			earlier = namespace[dfn.nom.key()]
+			self.report.redefined_name(earlier, dfn.nom)
+
 	def _declare_type(self, td:syntax.TypeDeclaration):
 		self._install(self.globals, td)
 		self._define_type_params(td)
-	
+
 	def _define_type_params(self, item:Union[syntax.TypeDeclaration, syntax.FFI_Group]):
 		ps = item.param_space = self.globals.new_child(place=item)
 		for p in item.type_params:
+			assert isinstance(p, syntax.TypeParameter), type(p)
 			self._install(ps, p)
 
 	def visit_Opaque(self, o:syntax.Opaque):
 		self._install(self.globals, o)
 		if o.type_params:
-			self._on_error(o.type_params, "Opaque types are not to be made generic.")
-	
+			self.report.opaque_generic(o.type_params)
+
 	def visit_Variant(self, v:syntax.Variant):
 		self._declare_type(v)
 		ss = v.sub_space = NS(place=v)
 		for st in v.subtypes:
 			self._install(self.globals, st)
 			self._install(ss, st)
 			if st.body is not None:
 				self.visit(st.body)
-				
+
 	def visit_Record(self, r:syntax.Record):
 		self._declare_type(r)
 		self.visit(r.spec)
 
 	def visit_TypeAlias(self, ta:syntax.TypeAlias):
 		self._declare_type(ta)
-		
+
 	def visit_RecordSpec(self, rs:syntax.RecordSpec):
 		# Ought to have a local name-space with names having types.
 		rs.field_space = NS(place=rs)
 		for f in rs.fields:
 			self._install(rs.field_space, f)
 		return
 
 	def visit_TypeCall(self, it:syntax.TypeCall, env:NS):
 		for a in it.arguments:
 			self.visit(a, env)
 
-	def visit_UserDefinedFunction(self, fn:syntax.UserDefinedFunction, env:NS):
-		self.all_functions.append(fn)
-		self._install(env, fn)
-		inner = fn.namespace = env.new_child(fn)
-		for param in fn.params:
+	def visit_UserFunction(self, udf:syntax.UserFunction, env:NS):
+		udf.source_path = self._source_path
+		self.roadmap.note_udf(udf)
+		self._install(env, udf)
+		inner = udf.namespace = env.new_child(udf)
+		for param in udf.params:
 			self.visit(param, inner)
-		if fn.result_type_expr is not None:
-			self.visit(fn.result_type_expr, inner)
-		for sub_fn in fn.where:
+		if udf.result_type_expr is not None:
+			self.visit(udf.result_type_expr, inner)
+		for sub_fn in udf.where:
 			self.visit(sub_fn, inner)
-		self.visit(fn.expr, inner)
-	
+		self.visit(udf.expr, inner)
+
 	def visit_FormalParameter(self, fp:syntax.FormalParameter, env:NS):
 		self._install(env, fp)
 		if fp.type_expr is not None:
 			self.visit(fp.type_expr, env)
-	
+
 	def visit_ExplicitTypeVariable(self, gt:syntax.ExplicitTypeVariable, env:NS):
-		if gt.nom.text not in env:
+		if gt.nom.key() not in env:
 			self._install(env, syntax.TypeParameter(gt.nom))
-	
+
 	def visit_Lookup(self, l:syntax.Lookup, env:NS): pass
 
 	def visit_MatchExpr(self, mx:syntax.MatchExpr, env:NS):
-		self.all_match_expressions.append(mx)
+		self.roadmap.note_match(mx)
 		self.visit(mx.subject.expr, env)
 		inner = mx.namespace = env.new_child(mx)
 		self._install(inner, mx.subject)
 		for alt in mx.alternatives:
 			self.visit(alt, inner)
 		if mx.otherwise is not None:
 			self.visit(mx.otherwise, inner)
 
 	def visit_Alternative(self, alt: syntax.Alternative, env: NS):
 		for sub_ex in alt.where:
 			self.visit(sub_ex, env)
 		self.visit(alt.sub_expr, env)
-	
-	def visit_ImportModule(self, im:syntax.ImportModule, module:syntax.Module):
+
+	def visit_ImportModule(self, im:syntax.ImportModule):
+		source_module = self.roadmap.import_map[im]
+		source_namespace = self.roadmap.module_scopes[source_module]
 		if im.nom is not None:
-			self._install(module.module_imports, im)
+			self._install(self.import_alias, im)
 		for alias in im.vocab:
 			yonder, hither = alias.yonder, alias.hither or alias.yonder
-			try: module.globals[hither.text] = im.module.globals[yonder.text]
-			except SymbolAlreadyExists:
-				collision = module.globals[hither.text].nom
-				self._on_error([collision, hither], "This symbol is already defined.")
-			except KeyError:
-				self._on_error([im.nom, yonder], "There is no corresponding symbol to import.")
+			try: subject = source_namespace[yonder.key()]
+			except KeyError: self.report.undefined_name(yonder.head())
+			else:
+				try: self.globals[hither.key()] = subject
+				except SymbolAlreadyExists:
+					collision = self.globals[hither.key()]
+					self.report.redefined_name(collision, hither)
+
 		pass
-	
+
 	def visit_ImportForeign(self, d:syntax.ImportForeign):
 		try: py_module = import_module(d.source.value)
-		except ModuleNotFoundError: self.missing_foreign.append(d.source)
-		except ImportError: self.broken_foreign.append(d.source)
+		except ModuleNotFoundError:
+			self.report.missing_foreign_module(d.source)
+		except ImportError as ex:
+			tbx = TracebackException.from_exception(ex)
+			self.report.broken_foreign_module(d.source, tbx)
 		else:
+			if d.linkage is not None:
+				if not hasattr(py_module, "sophie_init"):
+					self.report.missing_foreign_linkage(d.source)
+					return
+				arity = len(signature(py_module.sophie_init).parameters)
+				if arity != len(d.linkage):
+					self.report.wrong_linkage_arity(d, arity)
+					return
 			for group in d.groups:
 				self._define_type_params(group)
 				for sym in group.symbols:
-					self.visit(sym, group.param_space, py_module)
-	
-	def visit_FFI_Alias(self, sym:syntax.FFI_Alias, env:NS, py_module):
-		key = sym.nom.text if sym.alias is None else sym.alias.value
+					self.visit(sym, py_module)
+
+	def visit_FFI_Alias(self, sym:syntax.FFI_Alias, py_module):
+		key = sym.nom.key() if sym.alias is None else sym.alias.value
 		try: sym.val = getattr(py_module, key)
-		except KeyError: self.missing_foreign.append(sym)
+		except AttributeError:
+			guilty = (sym.alias or sym.nom).head()
+			self.report.undefined_name(guilty)
 		else: self._install(self.globals, sym)
 
-
-
-class StaticDepthPass(_TopDown):
-	# Assign static depth to the definitions of all parameters and functions.
-	# This pass cannot fail.
-	def __init__(self, module):
-		for fn in module.outer_functions:
-			self.visit_UserDefinedFunction(fn, 0)
-		for expr in module.main:
-			self.visit(expr, 0)
-			
-	def visit_UserDefinedFunction(self, fn:syntax.UserDefinedFunction, depth:int):
-		fn.static_depth = depth
-		inner = depth + (1 if fn.params else 0)
-		for param in fn.params:
-			param.static_depth = inner
-		self.visit(fn.expr, inner)
-		for sub_fn in fn.where:
-			self.visit_UserDefinedFunction(sub_fn, inner)
-		
-	def visit_MatchExpr(self, mx:syntax.MatchExpr, depth:int):
-		mx.subject.static_depth = depth
-		self.visit(mx.subject.expr, depth)
-		for alt in mx.alternatives:
-			self.visit(alt.sub_expr, depth)
-			for sub_ex in alt.where:
-				self.visit(sub_ex, depth)
-		if mx.otherwise is not None:
-			self.visit(mx.otherwise, depth)
-		
-
-	def visit_Lookup(self, l:syntax.Lookup, depth:int):
-		assert not hasattr(l, "source_depth")
-		l.source_depth = depth
-
-
-class WordResolver(_TopDown):
+class _WordResolver(_ResolutionPass):
 	"""
 	At the end of this action, every name-reference in the source text is visible where it's used.
 	That is, a corresponding definition-object is in scope. It may not make sense,
 	or be the right kind of name, but at least it's not an obvious misspelling.
 	
 	This will not be able to handle field-access (or keyword-args, etc) in the first instance,
 	because those depend on some measure of type resolution. And to keep things simple,
@@ -247,32 +323,26 @@
 	Walk the tree looking for undefined words in each static scope.
 	Report on every such occurrence.
 	If this pass succeeds, every syntax.Name object is connected to its corresponding symbol table entry.
 	This is also a good place to pick up interesting lists of syntax objects, such as all match-cases.
 	"""
 	
 	dubious_constructors: list[syntax.Reference]
-	
-	def __init__(self, module:syntax.Module, report):
-		on_error = report.on_error("Finding Definitions")
+
+	def visit_Module(self, module:syntax.Module):
 		self.dubious_constructors = []
-		self.undef:list[syntax.Nom] = []
-		self.module = module
 		for td in module.types:
 			self.visit(td)
-		for d in module.foreign:
-			self.visit(d)
-		for fn in module.all_functions:
-			fn.source_path = module.path
-			self.visit_UserDefinedFunction(fn)
+		for item in module.foreign:
+			self.visit(item)
+		for item in self.roadmap.each_udf:
+			self.visit(item)
 		for expr in module.main:
-			self.visit(expr, module.globals)
-		if self.undef:
-			on_error(self.undef, "I do not see an available definition for:")
-	
+			self.visit(expr, self.globals)
+
 	def visit_Variant(self, v:syntax.Variant):
 		for st in v.subtypes:
 			if st.body is not None:
 				self.visit(st.body, v.param_space)
 	
 	def visit_Record(self, r:syntax.Record):
 		self.visit(r.spec, r.param_space)
@@ -281,111 +351,118 @@
 		self.visit(ta.body, ta.param_space)
 	
 	def visit_RecordSpec(self, rs:syntax.RecordSpec, env:NS):
 		for f in rs.fields:
 			self.visit(f.type_expr, env)
 	
 	def _lookup(self, nom:syntax.Nom, env:NS):
-		try:
-			return env[nom.text]
+		try: return env[nom.key()]
 		except NoSuchSymbol:
-			self.undef.append(nom)
+			self.report.undefined_name(nom.head())
 			return Bogon(nom)
 
 	def visit_PlainReference(self, ref:syntax.PlainReference, env:NS):
 		# This kind of reference searches the local-scoped name-space
 		ref.dfn = self._lookup(ref.nom, env)
 	
 	def visit_QualifiedReference(self, ref:syntax.QualifiedReference, env:NS):
 		# Search among imports.
-		im = self._lookup(ref.space, self.module.module_imports)
+		im = self._lookup(ref.space, self.import_alias)
 		if isinstance(im, Bogon): ref.dfn = im
 		else:
 			assert isinstance(im, syntax.ImportModule)
-			ref.dfn = self._lookup(ref.nom, im.module.globals)
+			target_module = self.roadmap.import_map[im]
+			target_namespace = self.roadmap.module_scopes[target_module]
+			ref.dfn = self._lookup(ref.nom, target_namespace)
 	
 	def visit_TypeCall(self, tc:syntax.TypeCall, env:NS):
 		self.visit(tc.ref, env)
 		for p in tc.arguments:
 			self.visit(p, env)
 
-	def visit_UserDefinedFunction(self, fn:syntax.UserDefinedFunction):
-		for param in fn.params:
+	def visit_UserFunction(self, sym:syntax.UserFunction):
+		for param in sym.params:
 			if param.type_expr is not None:
-				self.visit(param.type_expr, fn.namespace)
-		if fn.result_type_expr is not None:
-			self.visit(fn.result_type_expr, fn.namespace)
-		self.visit(fn.expr, fn.namespace)
+				self.visit(param.type_expr, sym.namespace)
+		if sym.result_type_expr is not None:
+			self.visit(sym.result_type_expr, sym.namespace)
+		self.visit(sym.expr, sym.namespace)
 
 	def visit_MatchExpr(self, mx:syntax.MatchExpr, env:NS):
 		self.visit(mx.subject.expr, env)
+		if mx.hint is not None:
+			self.visit(mx.hint, env)
 		for alt in mx.alternatives:
-			self.visit(alt.pattern, self.module.globals)
 			self.visit(alt.sub_expr, mx.namespace)
 			for sub_ex in alt.where:
 				self.visit(sub_ex)
 		if mx.otherwise is not None:
 			self.visit(mx.otherwise, mx.namespace)
 			
 	def visit_Lookup(self, lu: syntax.Lookup, env: NS):
 		self.visit(lu.ref, env)
 		dfn = lu.ref.dfn
 		if isinstance(dfn, syntax.TypeAlias) or not dfn.has_value_domain():
 			self.dubious_constructors.append(lu.ref)
-
+	
 	def visit_ImportForeign(self, d:syntax.ImportForeign):
 		for ref in d.linkage or ():
-			self.visit(ref, self.module.globals)
+			self.visit(ref, self.globals)
 		for group in d.groups:
 			self.visit(group.type_expr, group.param_space)
 
 class Bogon(syntax.Symbol):
-	
 	def has_value_domain(self) -> bool:
 		return False
-	
 
-class AliasChecker(Visitor):
+class _AliasChecker(Visitor):
 	"""
 	Check the arity of TypeCall forms.
 	Check for aliases being well-founded, up front before getting caught in a loop later:
 	There should be no cycles in the aliasing dependency graph, and no wrong-kind references.
 	Also re-orders type definitions in order of alias topology.
 	
 	Stop worrying about function cycles; I'll catch that problem in the type checker.
 	"""
 	
-	def __init__(self, module: syntax.Module, report: diagnostics.Report):
-		self.on_error = report.on_error("Circular reasoning")
+	def __init__(self, roadmap: RoadMap, module:syntax.Module, report:Report):
+		self.roadmap = roadmap
+		self.report = report
+		self.globals = self.roadmap.module_scopes[module]
+		self.import_alias = self.roadmap.import_alias[module]
+		self.visit_Module(module)
+
+	def visit_Module(self, module: syntax.Module):
 		self.non_types = []
 		self.graph = {td:[] for td in module.types}
-		for td in module.types:
-			self.visit(td)
-		for d in module.foreign:
-			self.visit(d)
-		for fn in module.all_functions:
-			self.visit(fn)
+		self._tour(module.types)
+		self._tour(module.foreign)
+		self._tour(self.roadmap.each_udf)
 		if self.non_types:
-			self.on_error(self.non_types, "Need a type-name here; found this instead.")
+			self.report.these_are_not_types(self.non_types)
 		alias_order = []
 		ok = True
 		for scc in strongly_connected_components_hashable(self.graph):
 			if len(scc) == 1:
 				node = scc[0]
 				if node in self.graph[node]:
-					self.on_error([node], "This is a circular definition.")
+					self.report.circular_type(scc)
 				elif isinstance(node, syntax.TypeDeclaration):
 					alias_order.append(node)
 			else:
-				self.on_error(scc, "These make a circular definition.")
+				self.report.circular_type(scc)
 				ok = False
 		if ok:
 			assert len(alias_order) == len(module.types)
 			module.types = alias_order
 	pass
+
+	def _tour(self, them):
+		for item in them:
+			self.visit(item)
 	
 	def visit_TypeAlias(self, ta:syntax.TypeAlias):
 		self.graph[ta].append(ta.body)
 		self.visit(ta.body)
 	
 	def visit_TypeCall(self, tc:syntax.TypeCall):
 		assert tc not in self.graph
@@ -398,16 +475,15 @@
 			param_arity = 0
 		else:
 			self.non_types.append(tc)
 			return
 		# a. Do we have the correct arity?
 		arg_arity = len(tc.arguments)
 		if arg_arity != param_arity:
-			pattern = "%d type-arguments were given; %d are needed."
-			self.on_error([tc], pattern % (arg_arity, param_arity))
+			self.report.wrong_type_arity(tc, arg_arity, param_arity)
 		for arg in tc.arguments:
 			self.visit(arg)
 
 	def visit_Variant(self, v: syntax.Variant):
 		# A variant cannot participate in an aliasing cycle because it is a nominal type.
 		for st in v.subtypes:
 			if st.body is not None:
@@ -432,160 +508,59 @@
 		if expr.rhs is not None:
 			self.graph[expr].append(expr.rhs)
 			self.visit(expr.rhs)
 
 	def visit_ExplicitTypeVariable(self, expr:syntax.ExplicitTypeVariable): pass
 	def visit_ImplicitTypeVariable(self, it:syntax.ImplicitTypeVariable): pass
 
-	def visit_UserDefinedFunction(self, fn:syntax.UserDefinedFunction):
-		for p in fn.params:
-			self.visit(p)
-		if fn.result_type_expr:
-			self.visit(fn.result_type_expr)
-	
+	def visit_UserFunction(self, sym:syntax.UserFunction):
+		for p in sym.params: self.visit(p)
+		if sym.result_type_expr: self.visit(sym.result_type_expr)
+
 	def visit_ImportForeign(self, d:syntax.ImportForeign):
 		for group in d.groups:
 			self.visit(group.type_expr)
 
-def check_constructors(dubious_constructors:list[syntax.Reference], report:diagnostics.Report):
+def check_constructors(dubious_constructors:list[syntax.Reference], report:Report):
 	bogons = [ref.head() for ref in dubious_constructors if not ref.dfn.has_value_domain()]
 	if bogons: report.error("Checking Constructors", bogons, "These type-names are not data-constructors.")
 
-def check_all_match_expressions(module: syntax.Module, report):
-	on_match_error = report.on_error("Checking Type-Case Matches")
-	for mx in module.all_match_expressions:
-		_check_one_match_expression(mx, on_match_error)
-
-def _check_one_match_expression(mx:syntax.MatchExpr, on_error):
-	non_subtypes = []
-	duplicates = set()
-	first = {}
-	
-	subtypes : list[syntax.SubTypeSpec] = []
-	
-	for alt in mx.alternatives:
-		dfn = alt.pattern.dfn
-		if isinstance(dfn, syntax.SubTypeSpec):
-			subtypes.append(dfn)
-			if dfn in first:
-				duplicates.add(first[dfn])
-				duplicates.add(alt.pattern)
-			else:
-				first[dfn] = alt.pattern
-		else:
-			non_subtypes.append(alt.pattern)
-	
-	if non_subtypes:
-		on_error(non_subtypes, "This case is not a member of any variant.")
-	if duplicates:
-		on_error(list(duplicates), "Duplicate cases here...")
-	if non_subtypes or duplicates:
-		return
-	
-	primary_variant = subtypes[0].variant
-	mistypes = [alt.pattern for alt in mx.alternatives if alt.pattern.dfn.variant is not primary_variant]
-	
-	if mistypes:
-		on_error([mx.alternatives[0].pattern] + mistypes, "These do not all come from the same variant type.")
-		return
-
-	mx.variant = primary_variant
-	exhaustive = len(first) == len(primary_variant.subtypes)
-	if exhaustive and mx.otherwise:
-		on_error([mx, mx.otherwise], "This case-construction is exhaustive; the else-clause cannot happen.")
-	if not (exhaustive or mx.otherwise):
-		on_error([mx], "This case-construction does not cover all the cases of <%s> and lacks an otherwise-clause." % mx.variant.nom.text)
-	pass
-
-def build_match_dispatch_tables(module: syntax.Module):
-	""" The simple evaluator uses these. """
-	for mx in module.all_match_expressions:
-		mx.dispatch = {}
-		for alt in mx.alternatives:
-			key = alt.pattern.nom.key()
-			mx.dispatch[key] = alt.sub_expr
-
-class DependencyPass(_TopDown):
-	"""
-	Solve the problem of which-all formal parameters does the value (and thus, type)
-	of each user-defined function actually depend on. A simplistic answer would be to just
-	use the parameters of the outermost function in a given nest. But inner functions
-	might not be so generic as all that. Better precision here means smarter memoization,
-	and thus faster type-checking.
-	
-	Incidentally:
-	The same analysis could determine the deepest non-local needed for a function,
-	which could possibly allow some functions to run at a shallower static-depth
-	than however they may appear in the source code. This could make the simple evaluator
-	a bit faster by improving the lifetime of thunks.
-	"""
-	def __init__(self):
-		self.depends : dict[Symbol:syntax.FormalParameter] = {}
-		self._outer = {}
-		self._outflows = {}
-		self._overflowing = set()
-		
-	def _prepare(self, sym:Symbol):
-		self.depends[sym] = set()
-		self._outer[sym] = set()
-		self._outflows[sym] = set()
-	
-	def _insert(self, parameter:syntax.FormalParameter, env:Symbol):
-		self.depends[env].add(parameter)
-		if parameter.static_depth <= env.static_depth:
-			# i.e. The parameter is non-local...
-			outer = self._outer[env]
-			if parameter not in outer:
-				self._outer[env].add(parameter)
-				self._overflowing.add(env)
-
-	def _flow_dependencies(self):
-		# This algorithm might not be theoretically perfect,
-		# but for what it's about, it should be plenty fast.
-		# And it's straightforward to understand.
-		while self._overflowing:
-			source = self._overflowing.pop()
-			spill = self._outer[source]
-			for destination in self._outflows[source]:
-				for parameter in spill:
-					self._insert(parameter, destination)
-	
-	def _clean_up_after(self, module: syntax.Module):
-		self._outer.clear()
-		self._overflowing.clear()
-		self._outflows.clear()
-		for mx in module.all_match_expressions:
-			del self.depends[mx.subject]
-
-	def visit_Module(self, module: syntax.Module):
-		for fn in module.all_functions:
-			self._prepare(fn)
-		for mx in module.all_match_expressions:
-			self._prepare(mx.subject)
-		for fn in module.all_functions:
-			self.visit(fn.expr, fn)
-		self._flow_dependencies()
-		self._clean_up_after(module)
-
-	def visit_Lookup(self, lu: syntax.Lookup, env):
-		self.visit(lu.ref, env)
-		
-	def visit_PlainReference(self, ref:syntax.PlainReference, env):
-		dfn = ref.dfn
-		if dfn.static_depth == 0:
+def _check_one_match_expression(mx: syntax.MatchExpr, module_scope: NS, report: Report):
+	# Figure out what type of variant-record this MatchExpr is dissecting.
+	if mx.hint is None:
+		# Guess the variant based on the first alternative.
+		#
+		# Someday: Expand this to deal with local ambiguity
+		#          by consulting a larger amount of context.
+		first = mx.alternatives[0].nom
+		try: case = module_scope[first.key()]
+		except NoSuchSymbol:
+			report.undefined_name(first.head())
 			return
-		elif isinstance(dfn, syntax.FormalParameter):
-			self._insert(dfn, env)
-		elif isinstance(dfn, (syntax.UserDefinedFunction, syntax.Subject)):
-			assert hasattr(dfn, "static_depth"), dfn
-			if dfn.static_depth:
-				self._outflows[dfn].add(env)
-		else:
-			assert False, (dfn, type(dfn))
-				
-	def visit_MatchExpr(self, mx:syntax.MatchExpr, env:NS):
-		self.visit(mx.subject.expr, mx.subject)
-		for alt in mx.alternatives:
-			self.visit(alt.sub_expr, env)
-		if mx.otherwise is not None:
-			self.visit(mx.otherwise, env)
+		if not isinstance(case, syntax.SubTypeSpec):
+			report.not_a_case(first)
+			return
+		variant = case.variant
+	else:
+		variant = mx.hint.dfn
+		if not isinstance(variant, syntax.Variant):
+			report.not_a_variant(mx.hint)
+			return 
+
+	# Check for duplicate cases and typos.
+	seen, err = {}, False
+	for alt in mx.alternatives:
+		key = alt.nom.key()
+		if key in seen:
+			report.redefined_name(seen[key], alt.nom)
+			err = True
+		else: seen[key] = alt
+		if key not in variant.sub_space:
+			report.not_a_case_of(alt.nom, variant)
+	
+	# Check for exhaustiveness.
+
+	mx.variant = variant
+	exhaustive = len(seen) == len(variant.subtypes)
+	if      exhaustive and mx.otherwise : report.redundant_else(mx)
+	if not (exhaustive or  mx.otherwise): report.not_exhaustive(mx)
```

### Comparing `sophie-lang-0.0.0/sophie/simple_evaluator.py` & `sophie-lang-0.0.3/sophie/runtime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,289 +1,346 @@
-"""
-Call-By-Need with Direct Interpretation
-No longer quite the simplest, most straight-forward possible implementation.
-
-"""
-import sys
+import traceback
 from typing import Any, Union, Sequence, Optional
-from collections import namedtuple, deque
-import abc
-from . import syntax, primitive, ontology
-from .stacking import StackFrame, StackBottom, ActivationRecord
-
-FAKE_SOURCE_PATH = "FAKE_SOURCE_PATH" # until fixed.
-
-STRICT_VALUE = Union[int, float, str, "Procedure", namedtuple, dict]
+from collections import deque
+from . import syntax, primitive
+from .stacking import Frame, Activation
+
+STRICT_VALUE = Union[
+	int, float, str, dict,
+	"Procedure", "BoundMethod", "Message", "Step",
+]
 LAZY_VALUE = Union[STRICT_VALUE, "Thunk"]
-ENV = StackFrame[LAZY_VALUE]
+ENV = Frame[LAZY_VALUE]
+
+###############################################################################
 
 ABSENT = object()
 class Thunk:
 	""" A kind of not-yet-value which can be forced. """
 	def __init__(self, dynamic_env:ENV, expr: syntax.ValExpr):
 		assert isinstance(expr, syntax.ValExpr), type(expr)
 		self._dynamic_env = dynamic_env
 		self._expr = expr
 		self._value = ABSENT
 		
 	def force(self) -> STRICT_VALUE:
 		if self._value is ABSENT:
-			self._value = strict(self._expr, self._dynamic_env)
+			self._value = _strict(self._expr, self._dynamic_env)
+			assert not isinstance(self._value, syntax.ValExpr), type(self._expr)
 			del self._dynamic_env, self._expr
 		return self._value
 	
 	def __str__(self):
 		if self._value is ABSENT:
 			return "<Thunk: %s>"%self._expr
 		else:
 			return str(self._value)
 
-
-class Procedure(abc.ABC):
-	""" A run-time object that can be applied with arguments. """
-	@abc.abstractmethod
-	def apply(self, dynamic_env:ENV, args: list[LAZY_VALUE]) -> Any:
-		pass
-
-def actual_value(it:LAZY_VALUE) -> STRICT_VALUE:
+def force(it:LAZY_VALUE) -> STRICT_VALUE:
 	"""
 	While this will not return a thunk as such,
 	it may return a structure which contains thunks.
 	"""
 	while isinstance(it, Thunk):
 		it = it.force()
 	return it
 
-def strict(expr:syntax.ValExpr, dynamic_env:ENV):
-	return actual_value(evaluate(expr, dynamic_env))
+def _strict(expr:syntax.ValExpr, dynamic_env:ENV):
+	return force(evaluate(expr, dynamic_env))
+
+###############################################################################
 
 def _eval_literal(expr:syntax.Literal, dynamic_env:ENV):
 	return expr.value
 
 def _eval_lookup(expr:syntax.Lookup, dynamic_env:ENV):
-	dfn = expr.ref.dfn
-	return lookup(dfn, dynamic_env.chase(dfn))
-
+	sym = expr.ref.dfn
+	static_env = dynamic_env.chase(sym)
+	try: return static_env.fetch(sym)
+	except KeyError:
+		if isinstance(sym, syntax.UserFunction):
+			if sym.params:
+				value = Closure(static_env, sym)
+			else:
+				inner = Activation.for_function(static_env, sym, ())
+				value = delay(inner, sym.expr)
+		elif isinstance(sym, syntax.TypeAlias):
+			value = _snap_type_alias(sym, static_env)
+		else:
+			assert False, type(sym)
+		return static_env.assign(sym, value)
 
 def _eval_bin_exp(expr:syntax.BinExp, dynamic_env:ENV):
-	return OPS[expr.glyph](strict(expr.lhs, dynamic_env), strict(expr.rhs, dynamic_env))
+	return OPS[expr.glyph](_strict(expr.lhs, dynamic_env), _strict(expr.rhs, dynamic_env))
 
 def _eval_unary_exp(expr:syntax.UnaryExp, dynamic_env:ENV):
-	return OPS[expr.glyph](strict(expr.arg, dynamic_env))
+	return OPS[expr.glyph](_strict(expr.arg, dynamic_env))
 
 def _eval_shortcut_exp(expr:syntax.ShortCutExp, dynamic_env:ENV):
-	lhs = strict(expr.lhs, dynamic_env)
+	lhs = _strict(expr.lhs, dynamic_env)
 	assert isinstance(lhs, bool)
-	return lhs if lhs == OPS[expr.glyph] else strict(expr.rhs, dynamic_env)
+	return lhs if lhs == OPS[expr.glyph] else _strict(expr.rhs, dynamic_env)
 
 def _eval_call(expr:syntax.Call, dynamic_env:ENV):
-	procedure = strict(expr.fn_exp, dynamic_env)
-	return procedure.apply(dynamic_env, [delay(dynamic_env, a) for a in expr.args])
+	procedure = _strict(expr.fn_exp, dynamic_env)
+	thunks = tuple(delay(dynamic_env, a) for a in expr.args)
+	return procedure.apply(thunks)
 
 def _eval_cond(expr:syntax.Cond, dynamic_env:ENV):
-	if_part = strict(expr.if_part, dynamic_env)
+	if_part = _strict(expr.if_part, dynamic_env)
 	sequel = expr.then_part if if_part else expr.else_part
 	return delay(dynamic_env, sequel)
 
 def _eval_field_ref(expr:syntax.FieldReference, dynamic_env:ENV):
-	lhs = strict(expr.lhs, dynamic_env)
+	lhs = _strict(expr.lhs, dynamic_env)
 	key = expr.field_name.text
 	if isinstance(lhs, dict):
 		return lhs[key]
 	else:
 		return getattr(lhs, key)
 
 def _eval_explicit_list(expr:syntax.ExplicitList, dynamic_env:ENV):
-	it = NIL
+	tail = NIL
 	for sx in reversed(expr.elts):
-		it = CONS.apply(dynamic_env, [evaluate(sx, dynamic_env), it])
-	return it
+		head = delay(dynamic_env, sx)
+		tail = CONS.apply((head, tail))
+	return tail
 
 def _eval_match_expr(expr:syntax.MatchExpr, dynamic_env:ENV):
-	dynamic_env.bindings[expr.subject] = subject = strict(expr.subject.expr, dynamic_env)
+	subject = dynamic_env.assign(expr.subject, _strict(expr.subject.expr, dynamic_env))
 	tag = subject[""]
 	try:
 		branch = expr.dispatch[tag]
 	except KeyError:
 		branch = expr.otherwise
 		if branch is None:
 			raise RuntimeError("Confused by tag %r; should not be possible now that type-checking works."%tag)
 	return delay(dynamic_env, branch)
 
-def _snap_type_alias(alias:syntax.TypeAlias, env:ENV):
-	assert isinstance(alias.body, syntax.TypeCall)  # resolution.check_constructors guarantees this.
-	return lookup(alias.body.ref.dfn, env)
-
-def _snap_udf(udf:syntax.UserDefinedFunction, env:ENV):
-	return Closure(env, udf) if udf.params else delay(env, udf.expr)
+def _eval_do_block(expr:syntax.DoBlock, dynamic_env:ENV):
+	return CompoundStep(expr.steps, dynamic_env)
 
-SNAP : dict[type, callable] = {
-	syntax.TypeAlias: _snap_type_alias,
-	syntax.UserDefinedFunction:_snap_udf,
-}
+def _eval_bind_method(expr:syntax.BoundMethod, dynamic_env:ENV):
+	return Method(_strict(expr.receiver, dynamic_env), expr.method_name.text)
 
-def lookup(dfn:ontology.Symbol, env:ENV):
-	try: return env.bindings[dfn]
+def _snap_type_alias(alias:syntax.TypeAlias, global_env:ENV):
+	# It helps to remember this is a run-time thing so type-parameters are irrelevant here.
+	assert isinstance(alias.body, syntax.TypeCall)  # resolution.check_constructors guarantees this.
+	dfn = alias.body.ref.dfn
+	try: return global_env.fetch(dfn)
 	except KeyError:
-		env.bindings[dfn] = it = SNAP[type(dfn)](dfn, env)
-		return it
+		assert isinstance(dfn, syntax.TypeAlias)
+		return global_env.assign(dfn, _snap_type_alias(dfn, global_env))
 
 EVALUABLE = Union[syntax.ValExpr, syntax.Reference]
 
 def evaluate(expr:EVALUABLE, dynamic_env:ENV) -> LAZY_VALUE:
-	assert isinstance(dynamic_env, StackFrame), type(dynamic_env)
+	assert isinstance(dynamic_env, Frame), type(dynamic_env)
 	try: fn = EVALUATE[type(expr)]
 	except KeyError: raise NotImplementedError(type(expr), expr)
-	else: return fn(expr, dynamic_env)
+	try: return fn(expr, dynamic_env)
+	except Exception:
+		traceback.print_exc()
+		# for frame in THE_STACK:
+		# 	frame.trace(tracer)
+		exit(1)
 
-def delay(dynamic_env:ENV, item:syntax.ValExpr) -> LAZY_VALUE:
+def delay(dynamic_env:ENV, expr:syntax.ValExpr) -> LAZY_VALUE:
 	# For two kinds of expression, there is no profit to delay:
-	if isinstance(item, syntax.Literal): return item.value
-	if isinstance(item, syntax.Lookup): return _eval_lookup(item, dynamic_env)
+	if isinstance(expr, syntax.Literal): return expr.value
+	if isinstance(expr, syntax.Lookup): return _eval_lookup(expr, dynamic_env)
 	# In less trivial cases, make a thunk and pass that instead.
-	assert isinstance(item, syntax.ValExpr)
-	return Thunk(dynamic_env, item)
+	return Thunk(dynamic_env, expr)
+
+EVALUATE = {}
+for _k, _v in list(globals().items()):
+	if _k.startswith("_eval_"):
+		_t = _v.__annotations__["expr"]
+		assert isinstance(_t, type), (_k, _t)
+		EVALUATE[_t] = _v
+OPS = {glyph:op for glyph, (op, typ) in primitive.ops.items()}
+
+###############################################################################
+
+class Procedure:
+	""" A run-time object that can be applied with arguments. """
+	def apply(self, args: Sequence[LAZY_VALUE]) -> Any:
+		# It must be a LAZY_VALUE and not a syntax.ValExpr
+		# lest various internal things fail to work,
+		# which things to not tie back to specific syntax objects.
+		# For example, explicit lists.
+		raise NotImplementedError
 
 class Closure(Procedure):
 	""" The run-time manifestation of a sub-function: a callable value tied to its natal environment. """
 
-	def __init__(self, static_link:ENV, udf:syntax.UserDefinedFunction):
+	def __init__(self, static_link:ENV, udf:syntax.UserFunction):
 		self._static_link = static_link
 		self._udf = udf
 	
 	def _name(self): return self._udf.nom.text
 
-	def apply(self, dynamic_env:ENV, args: list[LAZY_VALUE]) -> LAZY_VALUE:
-		inner_env = ActivationRecord(self._udf, dynamic_env, self._static_link, args)
+	def apply(self, args: Sequence[LAZY_VALUE]) -> LAZY_VALUE:
+		inner_env = Activation.for_function(self._static_link, self._udf, args)
 		return evaluate(self._udf.expr, inner_env)
 
 class Primitive(Procedure):
 	""" All parameters to primitive procedures are strict. Also a kind of value, like a closure. """
-	def __init__(self, fn:callable):
+	def __init__(self, fn: callable):
 		self._fn = fn
-		
-	def apply(self, dynamic_env:ENV, args: list[LAZY_VALUE]) -> STRICT_VALUE:
-		return self._fn(*(actual_value(a) for a in args))
+	
+	def apply(self, args: Sequence[LAZY_VALUE]) -> STRICT_VALUE:
+		return self._fn(*map(force, args))
 
 class Constructor(Procedure):
 	def __init__(self, key:str, fields:list[str]):
 		self.key = key
 		self.fields = fields
 	
-	def apply(self, dynamic_env:ENV, args: list[LAZY_VALUE]) -> Any:
+	def apply(self, args: Sequence[LAZY_VALUE]) -> Any:
 		# TODO: It would be well to handle tagged values as Python pairs.
 		#  This way any value could be tagged, and various case-matching
 		#  things could work more nicely (and completely).
 		assert len(args) == len(self.fields)
-		structure = {"":self.key}
+		structure = {"": self.key}
 		for field, arg in zip(self.fields, args):
+			assert not isinstance(arg, syntax.ValExpr)
 			structure[field] = arg
 		return structure
 
-def run_program(static_root, each_module: Sequence[syntax.Module]):
-	drivers = {}
-	env = StackBottom(None)
-	_prepare_root_environment(env, static_root)
-	result = None  # Pacify the IDE
-	for module in each_module:
-		env.current_path = module.path
-		_prepare_global_scope(env, module.globals.local.items())
-		for d in module.foreign:
-			if d.linkage is not None:
-				py_module = sys.modules[d.source.value]
-				linkage = [env.bindings[ref.dfn] for ref in d.linkage]
-				drivers.update(py_module.sophie_init(actual_value, *linkage))
-				
-		for expr in module.main:
+class NativeObjectProxy:
+	""" Wrap Python objects in one of these to use them as actors. """
+	def __init__(self, principal):
+		self._principal = principal
+	def receive(self, method_name, args):
+		method = getattr(self._principal, method_name)
+		method(*args)
+
+###############################################################################
+
+class ParametricTask(Procedure):
+	def __init__(self, closure):
+		self._closure = closure
+	def apply(self, args: Sequence[LAZY_VALUE]) -> Any:
+		return ClosureMessage(self._closure, *(promote(a) for a in args))
+
+class Method(Procedure):
+	def __init__(self, receiver, method_name):
+		self._receiver = receiver
+		self._method_name = method_name
+	def apply(self, args: Sequence[LAZY_VALUE]) -> LAZY_VALUE:
+		return MethodMessage(self._receiver, self._method_name, *(promote(a) for a in args))
+	def run(self):
+		# Mild hack r/n...
+		self.apply(()).run()
+
+def promote(arg):
+	# Convert a closure to a task, but all other things stay the same.
+	it = force(arg)
+	if isinstance(it, Closure): return ParametricTask(it)
+	else: return it
+
+
+###############################################################################
+
+class Step:
+	def run(self):
+		raise NotImplementedError(type(self))
+
+class Nop(Step):
+	def run(self): pass
+
+class CompoundStep(Step):
+	def __init__(self, steps:Sequence[syntax.ValExpr], dynamic_env:ENV):
+		self._steps = steps
+		self._dynamic_env = dynamic_env
+	def run(self):
+		# TODO: Solve the tail-recursion problem.
+		env = self._dynamic_env
+		for expr in self._steps:
 			env.pc = expr
-			result = strict(expr, env)
-			if isinstance(result, dict):
-				tag = result.get("")
-				if tag in drivers:
-					drivers[tag](actual_value, env, result)
-					continue
-				dethunk(result)
-				if tag == 'cons':
-					result = decons(result)
-			if result is not None:
-				print(result)
-	return result
+			step = _strict(expr, self._dynamic_env)
+			step.run()
+
 
-NIL:dict
+###############################################################################
+
+THE_QUEUE = deque()
+
+def drain_queue():
+	while THE_QUEUE:
+		message = THE_QUEUE.popleft()
+		# print("  -> Dequeue", message)
+		message.proceed()
+
+class Message(Step):
+	def run(self):
+		# print("  <- Enqueue", self)
+		assert hasattr(self, "proceed")
+		THE_QUEUE.append(self)
+	def proceed(self):
+		raise NotImplementedError(type(self))
+
+class ClosureMessage(Message):
+	def __init__(self, closure:Procedure, *args):
+		self._closure = closure
+		self._args = args
+	def proceed(self):
+		thunk = self._closure.apply(self._args)
+		step = force(thunk)
+		step.run()
+
+class SimpleTask(Message):
+	def __init__(self, thunk):
+		self._thunk = thunk
+	def proceed(self):
+		step = force(self._thunk)
+		step.run()
+
+class MethodMessage(Message):
+	def __init__(self, receiver, method_name, *args):
+		self._receiver = receiver
+		self._method_name = method_name
+		self._args = args
+	def proceed(self):
+		self._receiver.receive(self._method_name, self._args)
+
+###############################################################################
+
+NIL:Optional[dict] = None # Gets replaced at runtime.
 CONS:Constructor
 
-def _prepare_root_environment(env:StackBottom, static_root):
-	global NIL, CONS
-	_prepare_global_scope(env, primitive.root_namespace.local.items())
-	_prepare_global_scope(env, static_root.local.items())
-	if 'nil' in static_root:
-		NIL = env.bindings[static_root['nil']]
-		CONS = env.bindings[static_root['cons']]
-	else:
-		NIL, CONS = None, None
+def iterate_list(lst:LAZY_VALUE):
+	lst = force(lst)
+	while lst is not NIL:
+		yield force(lst['head'])
+		lst = force(lst['tail'])
+
+###############################################################################
+#
+#  Give the console object run-time teeth
 
-def _prepare_global_scope(env:StackBottom, items):
-	for key, dfn in items:
-		if isinstance(dfn, syntax.Record):
-			env.bindings[dfn] = Constructor(key, dfn.spec.field_names())
-		elif isinstance(dfn, (syntax.SubTypeSpec, syntax.TypeAlias)):
-			if isinstance(dfn.body, (syntax.ArrowSpec, syntax.TypeCall)):
-				pass
-			elif isinstance(dfn.body, syntax.RecordSpec):
-				env.bindings[dfn] = Constructor(key, dfn.body.field_names())
-			elif dfn.body is None:
-				env.bindings[dfn] = {"": key}
-			else:
-				raise ValueError("Tagged scalars (%r) are not implemented."%key)
-		elif isinstance(dfn, ontology.NativeFunction):
-			env.bindings[dfn] = _native_object(dfn)
-		elif type(dfn) in _ignore_these:
-			pass
-		else:
-			raise ValueError("Don't know how to deal with %r %r"%(type(dfn), key))
+import sys
+import random
 
-def _native_object(dfn:ontology.NativeFunction):
-	if callable(dfn.val):
-		return Primitive(dfn.val)
-	else:
-		return dfn.val
+class Console:
+	@staticmethod
+	def echo(text):
+		for fragment in iterate_list(text):
+			sys.stdout.write(fragment)
+		sys.stdout.flush()
+
+	@staticmethod
+	def read(target:Procedure):
+		message = target.apply([input()])
+		message.run()
+
+	@staticmethod
+	def random(target:Procedure):
+		message = target.apply([random.random()])
+		message.run()
 
-_ignore_these = {
-	# type(None),
-	syntax.UserDefinedFunction,  # Gets built on-demand.
-	syntax.ArrowSpec,
-	syntax.TypeCall,
-	syntax.Variant,
-	syntax.Opaque,
-}
+primitive.root_namespace['console'].val = NativeObjectProxy(Console())
 
-def dethunk(result:dict):
-	"""
-	This can be considered as (most of) the first and most trivial I/O driver.
-	Its entire job is to push a program to completion by evaluating every thunk it produces.
-	There should be a better way, but it will probably be the consequence of an I/O subsystem.
-	"""
-	dict_queue = deque()
-	dict_queue.append(result)
-	while dict_queue:
-		work_dict = dict_queue.popleft()
-		for k,v in work_dict.items():
-			if isinstance(v, Thunk): work_dict[k] = v = actual_value(v)
-			if isinstance(v, dict): dict_queue.append(v)
-
-def decons(item:dict) -> list:
-	result = []
-	while isinstance(item, dict) and item.get("") == 'cons':
-		result.append(item['head'])
-		item = item['tail']
-	if item is not NIL:
-		result.append(item)
-	return result
+###############################################################################
 
 
-EVALUATE = {}
-for _k, _v in list(globals().items()):
-	if _k.startswith("_eval_"):
-		_t = _v.__annotations__["expr"]
-		assert isinstance(_t, type), (_k, _t)
-		EVALUATE[_t] = _v
-OPS = {glyph:op for glyph, (op, typ) in primitive.ops.items()}
```

### Comparing `sophie-lang-0.0.0/sophie/syntax.py` & `sophie-lang-0.0.3/sophie/syntax.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 The parser calls these constructors with subordinate semantic-values in a bottom-up tree transduction.
 These constructors may add a touch of organization.
 Class-level type annotations make peace with pycharm wherever later passes add fields.
 """
 from pathlib import Path
 from typing import Optional, Any, Sequence, NamedTuple, Union
 from boozetools.parsing.interface import SemanticError
-from boozetools.support.symtab import NameSpace
 from .ontology import (
-	Nom, Symbol, NativeFunction, NS, Reference,
-	Expr, Function,
+	Nom, Symbol, NS, Reference,
+	Expr, Term,
 )
 
 class MismatchedBookendsError(SemanticError):
 	# The one semantic error we catch early enough to interrupt the parse.
 	# It's early warning that things have gotten out of whack.
 	def __init__(self, head: slice, coda: slice):
 		super().__init__(head, coda)
@@ -27,17 +26,17 @@
 		return self.nom.head()
 	def has_value_domain(self) -> bool:
 		return False
 
 class TypeDeclaration(Symbol):
 	static_depth = 0
 	param_space: NS   # Will address the type parameters. Word-definer fills this.
-	type_params: tuple[TypeParameter]
+	type_params: tuple[TypeParameter, ...]
 	
-	def __init__(self, nom: Nom, type_params:Sequence[TypeParameter]):
+	def __init__(self, nom: Nom, type_params:tuple[TypeParameter, ...]):
 		super().__init__(nom)
 		self.type_params = type_params
 
 def type_parameters(param_names:Sequence[Nom]):
 	return tuple(TypeParameter(n) for n in param_names)
 
 class SimpleType(Expr):
@@ -45,14 +44,15 @@
 
 class ValExpr(Expr):
 	pass
 
 class PlainReference(Reference):
 	def head(self) -> slice:
 		return self.nom.head()
+	def __str__(self): return "<ref:%s>"%self.nom.text
 
 class QualifiedReference(Reference):
 	space: Nom
 	def __init__(self, nom:Nom, space:Nom):
 		super().__init__(nom)
 		self.space = space
 	def head(self) -> slice:
@@ -118,43 +118,43 @@
 class Opaque(TypeDeclaration):
 	def __init__(self, nom: Nom):
 		super().__init__(nom, ())
 	def has_value_domain(self): return False
 
 class TypeAlias(TypeDeclaration):
 	body: SimpleType
-	def __init__(self, nom: Nom, param_names:list[Nom], body:SimpleType):
-		super().__init__(nom, param_names)
+	def __init__(self, nom: Nom, type_params:tuple[TypeParameter, ...], body:SimpleType):
+		super().__init__(nom, type_params)
 		self.body = body
 	def has_value_domain(self) -> bool: return self.body.can_construct()
 
 class Record(TypeDeclaration):
-	def __init__(self, nom: Nom, param_names:list[Nom], spec:RecordSpec):
-		super().__init__(nom, param_names)
+	def __init__(self, nom: Nom, type_params:tuple[TypeParameter, ...], spec:RecordSpec):
+		super().__init__(nom, type_params)
 		self.spec = spec
 	def has_value_domain(self) -> bool: return True
 
 class Variant(TypeDeclaration):
 	sub_space: NS  # WordDefiner pass fills this in.
-	def __init__(self, nom: Nom, param_names:list[Nom], spec:VariantSpec):
-		super().__init__(nom, param_names)
+	def __init__(self, nom: Nom, type_params:tuple[TypeParameter, ...], spec:VariantSpec):
+		super().__init__(nom, type_params)
 		self.subtypes = spec.subtypes
 		for s in spec.subtypes: s.variant = self
 	def has_value_domain(self) -> bool: return False
 
 _spec_to_decl = {
 	RecordSpec : Record,
 	VariantSpec : Variant,
 	TypeCall : TypeAlias,
 	ArrowSpec : TypeAlias,
 }
 
 def concrete_type(nom: Nom, body): return generic_type(nom, (), body)
-def generic_type(nom: Nom, param_names: Sequence[Nom], body):
-	return _spec_to_decl[body.__class__](nom, param_names, body)
+def generic_type(nom: Nom, type_params:tuple[TypeParameter, ...], body):
+	return _spec_to_decl[body.__class__](nom, type_params, body)
 
 class SubTypeSpec(Symbol):
 	body: Optional[Union[RecordSpec, TypeCall, ArrowSpec]]
 	variant: Variant
 	static_depth = 0
 	# To clarify: The SubType here describes a *tagged* value, not the type of the value so tagged.
 	# One can tag any kind of value; even a function. Therefore yes, you can always
@@ -171,24 +171,24 @@
 	names: list[Nom]
 	type_expr: SimpleType
 
 def _bookend(head: Nom, coda: Nom):
 	if head.text != coda.text:
 		raise MismatchedBookendsError(head.head(), coda.head())
 
-class UserDefinedFunction(Function):
+class UserFunction(Term):
 	source_path: Path
 	namespace: NS
-	sub_fns: dict[str:"UserDefinedFunction"]  # for simple evaluator
-	where: Sequence["UserDefinedFunction"]
-	
+	params: Sequence[FormalParameter]
+	where: Sequence["UserFunction"]
 	def has_value_domain(self): return True
+	def head(self) -> slice: return self.nom.head()
 	def __repr__(self):
 		p = ", ".join(map(str, self.params))
-		return "{fn:%s(%s)|%s}"%(self.nom.text, p, getattr(self, "static_depth", "?"))
+		return "{fn:%s(%s)}" % (self.nom.text, p)
 	def __init__(
 			self,
 			nom: Nom,
 			params: Sequence[FormalParameter],
 			expr_type: Optional[ARGUMENT_TYPE],
 			expr: ValExpr,
 			where: Optional["WhereClause"]
@@ -198,19 +198,18 @@
 		self.result_type_expr = expr_type
 		self.expr = expr
 		if where:
 			_bookend(nom, where.end_name)
 			self.where = where.sub_fns
 		else:
 			self.where = ()
-	
-	def head(self) -> slice: return self.nom.head()
+
 
 class WhereClause(NamedTuple):
-	sub_fns: Sequence[UserDefinedFunction]
+	sub_fns: Sequence[UserFunction]
 	end_name: Nom
 
 class Literal(ValExpr):
 	def __init__(self, value: Any, a_slice: slice):
 		self.value, self._slice = value, a_slice
 	
 	def __str__(self):
@@ -219,24 +218,32 @@
 	def head(self) -> slice:
 		return self._slice
 
 def truth(a_slice:slice): return Literal(True, a_slice)
 def falsehood(a_slice:slice): return Literal(False, a_slice)
 
 class Lookup(ValExpr):
+	# Reminder: This AST node exists in opposition to TypeCall so I can write
+	# behavior for references in value context vs. references in type context.
 	ref:Reference
-	source_depth:int
 	def __init__(self, ref: Reference): self.ref = ref
 	def head(self) -> slice: return self.ref.head()
+	def __str__(self): return str(self.ref)
 
 class FieldReference(ValExpr):
 	def __init__(self, lhs: ValExpr, field_name: Nom): self.lhs, self.field_name = lhs, field_name
 	def __str__(self): return "(%s.%s)" % (self.lhs, self.field_name.text)
 	def head(self) -> slice: return self.field_name.head()
 
+class BoundMethod(ValExpr):
+	def __init__(self, receiver: ValExpr, method_name: Nom):
+		self.receiver, self.method_name = receiver, method_name
+	def __str__(self): return "(%s.%s)" % (self.receiver, self.method_name.text)
+	def head(self) -> slice: return self.method_name.head()
+
 class BinExp(ValExpr):
 	def __init__(self, glyph: str, lhs: ValExpr, o:slice, rhs: ValExpr):
 		self.glyph, self.lhs, self.rhs = glyph, lhs, rhs
 		self._head = o
 	def head(self) -> slice: return self._head
 
 def _be(glyph: str): return lambda a, o, b: BinExp(glyph, a, o, b)
@@ -306,27 +313,26 @@
 	def __init__(self, elts: list[ValExpr]):
 		for e in elts:
 			assert isinstance(e, ValExpr), e
 		self.elts = elts
 	def head(self) -> slice:
 		raise AssertionError
 
-class Alternative(ValExpr):
-	pattern: Reference
+class Alternative(Symbol):
 	sub_expr: ValExpr
-	where: Sequence[UserDefinedFunction]
+	where: Sequence[UserFunction]
 	
 	namespace: NS  # WordDefiner fills
-	
-	def __init__(self, pattern:Reference, _head, sub_expr:ValExpr, where:WhereClause):
-		self.pattern = pattern
+
+	def __init__(self, pattern:Nom, _head, sub_expr:ValExpr, where:WhereClause):
+		super().__init__(pattern)
 		self._head = _head
 		self.sub_expr = sub_expr
 		if where:
-			_bookend(pattern.nom, where.end_name)
+			_bookend(pattern, where.end_name)
 			self.where = where.sub_fns
 		else:
 			self.where = ()
 	def head(self) -> slice:
 		return self._head
 	
 class Subject(Symbol):
@@ -344,38 +350,45 @@
 	subject:Subject  # Symbol in scope within alternative expressions; contains the value of interest
 	hint: Optional[Reference]
 	alternatives: list[Alternative]
 	otherwise: Optional[ValExpr]
 	
 	namespace: NS  # WordDefiner fills
 	
-	variant:Variant  # check_match_expression infers this from the patterns
+	variant:Variant  # Filled in match-check pass
 	dispatch: dict[Optional[str]:ValExpr]
 	
-	def __init__(self, subject:Subject, hint:Optional[Reference], alternatives: list[Alternative], otherwise: Optional[ValExpr]):
+	def __init__(self, subject, hint, alternatives, otherwise):
 		self.subject = subject
 		self.hint = hint
 		self.alternatives, self.otherwise = alternatives, otherwise
 	
 	def head(self) -> slice:
 		return self.subject.head()
 
+class DoBlock(ValExpr):
+	def __init__(self, steps:list[ValExpr]):
+		self.steps = steps
+
 class ImportSymbol(NamedTuple):
 	yonder : Nom
 	hither : Optional[Nom]
 
 class ImportModule(Symbol):
-	module : "Module"  # Module loader fills this.
+	module_key: Path  # Module loader fills this.
 	def __init__(self, package:Optional[Nom], relative_path:Literal, nom:Optional[Nom], vocab:Optional[Sequence[ImportSymbol]]):
 		super().__init__(nom)
 		self.package = package
 		self.relative_path = relative_path
 		self.vocab = vocab or ()
 
-class FFI_Alias(NativeFunction):
+class FFI_Alias(Term):
+	""" Built-in and foreign (Python) function symbols. """
+	val:Any  # Fill in during WordDefiner pass
+	
 	def __init__(self, nom:Nom, alias:Optional[Literal]):
 		super().__init__(nom)
 		self.nom = nom
 		self.alias = alias
 
 def FFI_Symbol(nom:Nom):
 	return FFI_Alias(nom, None)
@@ -392,24 +405,20 @@
 		self.source = source
 		self.linkage = linkage
 		self.groups = groups
 
 ImportDirective = Union[ImportModule, ImportForeign]
 
 class Module:
-	path: Path # Front end fills this in.
 	imports: list[ImportModule]
 	foreign: list[ImportForeign]
-	module_imports: NS  # Modules imported with an "as" clause.
-	wildcard_imports: NS  # Names imported with a wildcard. Sits underneath globals.
-	globals: NS  # WordDefiner pass creates this.
-	all_functions: list[UserDefinedFunction]  # WordDefiner pass creates this.
-	all_match_expressions: list[MatchExpr]  # WordResolver pass creates this.
-	
-	def __init__(self, exports:list, imports:list[ImportDirective], types:list[TypeDeclaration], assumption:list[Assumption], functions:list[UserDefinedFunction], main:list):
+	source_path: Path  # Module loader fills this.
+
+	def __init__(self, exports:list, imports:list[ImportDirective], types:list[TypeDeclaration], assumption:list[Assumption], functions:list[UserFunction], main:list):
 		self.exports = exports
 		self.imports = [i for i in imports if isinstance(i, ImportModule)]
 		self.foreign = [i for i in imports if isinstance(i, ImportForeign)]
 		self.types = types
 		self.outer_functions = functions
 		self.main = main
-		self.module_imports = NameSpace(place=self)
+	
+	def head(self): return slice(0,0)
```

### Comparing `sophie-lang-0.0.0/sophie/sys/game.sg` & `sophie-lang-0.0.3/sophie/sys/game.sg`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Types and functions useful for making 2-D interactive games. Oh, and a driver.
 #
 # Eventually.
 #
 # For now, it's just a spike.
 
 import:
-    foreign "sophie.adapters.game_adapter"(nil);
+    foreign "sophie.adapters.game_adapter"();
 
 type:
     screen is (size:rect, background:color);
     color is (red:number, green:number, blue:number);
     rect is (x:number, y:number);
     polar is (magnitude:number, angle:number);  # Angle in radians, presumably.
```

### Comparing `sophie-lang-0.0.0/sophie/sys/preamble.sg` & `sophie-lang-0.0.3/sophie/sys/preamble.sg`

 * *Files 3% similar despite different names*

```diff
@@ -91,29 +91,29 @@
 	esac;
 
 	take(n, xs) = nil if n < 1 else case xs of
 		nil -> nil;
 		cons -> cons(xs.head, take(n-1, xs.tail));
 	esac;
 
-	skip(n, xs) = xs if n < 1 else case xs of
+	drop(n, xs) = xs if n < 1 else case xs of
 		nil -> nil;
-		cons -> skip(n-1, xs.tail);
+		cons -> drop(n-1, xs.tail);
 	esac;
 
 	sum(xs) = reduce(add, 0, xs) where add(a,b) = a+b; end sum;
 	product(xs) = reduce(mul, 1, xs) where mul(a,b) = a*b; end product;
 	hypot(xs) = sqrt(sum(map(square, xs))) where square(x) = x*x; end hypot;
 
 	## Sophie's first namespace conflict:
 	# left(s, n) = mid(s, 0, n);
 	# right(s, n) = mid(s, len(s)-n, len(s));
 
 	join(ss) = reduce(strcat, "", ss);  # Yes, this is O(n^2). Fixing that from within is nontrivial.
 
-	interleave(x, ys) = skip(1, flat(map(prefix, ys))) where prefix(y)=cons(x, cons(y, nil)); end interleave;
+	interleave(x, ys) = drop(1, flat(map(prefix, ys))) where prefix(y)=cons(x, cons(y, nil)); end interleave;
 
 	each_chr(s) = from(0) where
 		from(n) = nil if n >= len(s) else cons(mid(s,n,1), from(n+1));
 	end each_chr;
 
 end.
```

### Comparing `sophie-lang-0.0.0/sophie/sys/turtle.sg` & `sophie-lang-0.0.3/sophie/sys/turtle.sg`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Bits for Turtle Graphics.
 
 # This moved out of the standard preamble to prove it could be done.
 
 import:
-foreign "sophie.adapters.turtle_adapter" (nil) ;
+foreign "sophie.adapters.turtle_adapter"();
 
 type:
 
 	drawing is (steps: list[turtle_step]);
 
 	turtle_step is case:
 		forward(distance:number);
```

### Comparing `sophie-lang-0.0.0/sophie/type_evaluator.py` & `sophie-lang-0.0.3/sophie/type_evaluator.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,27 +9,149 @@
 
 This module represents one straightforward type-level execution mechanism.
 The type side of things can be call-by-value, which is a bit easier I think.
 The tricky bit is (mutually) recursive functions.
 """
 from typing import Iterable, Sequence
 from boozetools.support.foundation import Visitor
-from .ontology import Symbol, Expr
+from .ontology import Symbol
 from . import syntax, primitive, diagnostics
-from .resolution import DependencyPass
-from .stacking import StackBottom, ActivationRecord
+from .resolution import RoadMap, TopDown
+from .stacking import RootFrame, Activation
+from .syntax import ValExpr
 from .calculus import (
 	TYPE_ENV,
 	SophieType, TypeVisitor,
 	OpaqueType, ProductType, ArrowType, TypeVariable,
 	RecordType, SumType, SubType, TaggedRecord, EnumType,
-	UDFType,
+	MethodType, MessageType,
+	UDFType, ActorType,
 	BOTTOM, ERROR,
 )
 
+class DependencyPass(TopDown):
+	"""
+	Solve the problem of which-all formal parameters does the value (and thus, type)
+	of each user-defined function actually depend on. A simplistic answer would be to just
+	use the parameters of the outermost function in a given nest. But inner functions
+	might not be so generic as all that. Better precision here means smarter memoization,
+	and thus faster type-checking.
+	
+	The nature of the algorithm is a transitive-closure / least-fixpoint operation.
+	Preparation is by means of a tree-walk.
+	
+	Incidentally:
+	Related analysis could determine the deepest non-local needed for a function,
+	which could possibly allow some functions to run at a shallower static-depth
+	than however they may appear in the source code. This could make the simple evaluator
+	a bit faster by improving the lifetime of thunks.
+	"""
+
+	def __init__(self):
+		# The interesting result:
+		self.depends: dict[Symbol, set[syntax.FormalParameter]] = {}
+		
+		# All manner of temp data, which should be cleaned afterward:
+		self._outer: dict[Symbol, set[syntax.FormalParameter]] = {}
+		self._parent: dict[Symbol, Symbol] = {}
+		self._outflows: dict[Symbol, set[Symbol]] = {}
+		self._overflowing = set()
+		
+	def visit_Module(self, module: syntax.Module):
+		self._walk_children(module.outer_functions, None)
+		for expr in module.main:
+			self.visit(expr, None)
+		self._flow_dependencies()
+		self._clean_up_after()
+
+	def _prepare(self, sym:Symbol, parent):
+		self._parent[sym] = parent
+		self.depends[sym] = set()
+		self._outer[sym] = set()
+		self._outflows[sym] = set()
+
+	def _walk_children(self, children: Sequence[syntax.UserFunction], parent):
+		for child in children: self._prepare(child, parent)
+		for child in children: self.visit_UserFunction(child, parent)
+
+	def _insert(self, param:syntax.FormalParameter, env:Symbol):
+		depends = self.depends[env]
+		if self._is_in_scope(param, env) and param not in depends:
+			depends.add(param)
+			outer = self._outer[env]
+			if self._is_non_local(param, env) and param not in outer:
+				outer.add(param)
+				self._overflowing.add(env)
+	
+	def _flow_dependencies(self):
+		# This algorithm might not be theoretically perfect,
+		# but for what it's about, it should be plenty fast.
+		# And it's straightforward to understand.
+		while self._overflowing:
+			source = self._overflowing.pop()
+			spill = self._outer[source]
+			for destination in self._outflows[source]:
+				for parameter in spill:
+					self._insert(parameter, destination)
+	
+	def _clean_up_after(self):
+		self._outer.clear()
+		self._parent.clear()
+		self._outflows.clear()
+		self._overflowing.clear()
+
+	def _is_in_scope(self, param:syntax.FormalParameter, env:Symbol):
+		if env is None:
+			return False
+		if isinstance(env, syntax.UserFunction):
+			return param in env.params or self._is_in_scope(param, self._parent[env])
+		if isinstance(env, syntax.Subject):
+			return self._is_in_scope(param, self._parent[env])
+		assert False, type(env)
+
+	@staticmethod
+	def _is_non_local(param:syntax.FormalParameter, env:Symbol):
+		if isinstance(env, syntax.UserFunction):
+			return param not in env.params
+		if isinstance(env, syntax.Subject):
+			return True
+		assert False, type(env)
+
+	def visit_UserFunction(self, udf: syntax.UserFunction, env):
+		# Params refer to themselves in this arrangement.
+		# The "breadcrumb" serves to indicate the nearest enclosing symbol.
+		self._parent[udf] = env
+		self._walk_children(udf.where, udf)
+		self.visit(udf.expr, udf)
+
+	def visit_Lookup(self, lu: syntax.Lookup, env):
+		self.visit(lu.ref, env)
+
+	def _is_relevant(self, sym):
+		return self._parent.get(sym) is not None
+
+	def visit_PlainReference(self, ref: syntax.PlainReference, env:Symbol):
+		dfn = ref.dfn
+		if isinstance(dfn, syntax.FormalParameter):
+			self._insert(dfn, env)
+		elif self._is_relevant(dfn):
+			self._outflows[dfn].add(env)
+			
+	def visit_QualifiedReference(self, ref:syntax.QualifiedReference, env:Symbol):
+		pass
+
+	def visit_MatchExpr(self, mx: syntax.MatchExpr, env:Symbol):
+		self._prepare(mx.subject, env)
+		self._outflows[mx.subject].add(env)
+		self.visit(mx.subject.expr, env)
+		for alt in mx.alternatives:
+			self._walk_children(alt.where, mx.subject)
+			self.visit(alt.sub_expr, mx.subject)
+		if mx.otherwise is not None:
+			self.visit(mx.otherwise, mx.subject)
 
 class ArityError(Exception):
 	pass
 
 _literal_type_map : dict[type, OpaqueType] = {
 	bool: primitive.literal_flag,
 	str: primitive.literal_string,
@@ -172,15 +294,15 @@
 				self.fail()
 		elif isinstance(actual, EnumType):
 			if formal.variant is actual.st.variant:
 				pass
 			else:
 				self.fail()
 		else:
-			raise NotImplementedError(actual)
+			self.fail()
 	
 	def visit_RecordType(self, formal: RecordType, actual: SophieType):
 		if isinstance(actual, RecordType) and formal.symbol is actual.symbol:
 			self.parallel(formal.type_args, actual.type_args)
 		else:
 			self.fail()
 
@@ -189,18 +311,17 @@
 		self._prototype = prototype
 		self.died = False
 	def result(self):
 		return self._prototype
 	def unify_with(self, that):
 		if self._prototype is not ERROR:
 			union = self.do(self._prototype, that)
-			if union is ERROR and that is not ERROR:
-				print("Failed to unify:")
-				print(self._prototype)
-				print(that)
+			# TODO: Put the specific mismatch on report.
+			# 	if union is ERROR and that is not ERROR:
+			#		mumble.failed_to_unify(self._prototype, that)
 			self._prototype = union
 	
 	def parallel(self, these:Sequence[SophieType], those:Sequence[SophieType]):
 		assert len(these) == len(those)
 		return [self.do(a, b) for a,b in zip(these, those)]
 	
 	def do(self, this: SophieType, that: SophieType):
@@ -280,33 +401,55 @@
 			return None  # Not a function.
 	
 	@staticmethod
 	def visit__Error(this: ERROR, that: SophieType):
 		return this
 
 class DeductionEngine(Visitor):
-	def __init__(self, report:diagnostics.Report):
+	def __init__(self, roadmap:RoadMap, report:diagnostics.Report):
+		# self._trace_depth = 0
 		self._report = report  # .on_error("Checking Types")
 		self._types = { ot.symbol: ot for ot in _literal_type_map.values() }
 		self._constructors : dict[syntax.Symbol, SophieType] = {}
-		self._ffi = {}
+		self._ffi : dict[syntax.FFI_Alias, SophieType] = {
+			primitive.root_namespace['console'] : ActorType(),
+		}
 		self._memo = {}
 		self._recursion = {}
 		self._deps_pass = DependencyPass()
-	
+		self._list_symbol = roadmap.list_symbol
+		self._udf = {}
+		self._root = RootFrame()
+		self.visit_Module(roadmap.preamble)
+		for module in roadmap.each_module:
+			self.visit_Module(module)
+	
+	# def visit(self, host, *args, **kwargs):
+	# 	prefix = " "*self._trace_depth
+	# 	self._trace_depth += 1
+	# 	self._report.trace(prefix, ">", type(host).__name__, host)
+	# 	result = super().visit(host, *args, **kwargs)
+	# 	self._report.trace(prefix, "<", type(host).__name__, result)
+	# 	self._trace_depth -= 1
+	# 	return result
+
 	def visit_Module(self, module:syntax.Module):
-		self._deps_pass.visit(module)
+		self._report.info("Type-Check", module.source_path)
+		self._deps_pass.visit_Module(module)
 		for td in module.types: self.visit(td)
 		for fi in module.foreign: self.visit(fi)
-		env = StackBottom(module.path)
+		local = Activation.for_module(self._root, module)
 		for expr in module.main:
-			result = self.visit(expr, env)
+			self._report.trace(" -->", expr)
+			result = self.visit(expr, local)
 			self._report.info(result)
-		pass
-	
+		self._root._bindings.update(local._bindings)
+
+	###############################################################################
+
 	def visit_Record(self, r: syntax.Record):
 		type_args = [TypeVariable() for _ in r.type_params]
 		self._types[r] = RecordType(r, type_args)
 		arg = ManifestBuilder(r.type_params, type_args).visit(r.spec)
 		self._constructors[r] = ArrowType(arg, self._types[r])
 	
 	def visit_Variant(self, v: syntax.Variant):
@@ -325,93 +468,105 @@
 		type_args = [TypeVariable() for _ in a.type_params]
 		self._types[a] = it = ManifestBuilder(a.type_params, type_args).visit(a.body)
 		if isinstance(it, RecordType):
 			formals = self._types[it.symbol].type_args
 			original = self._constructors[it.symbol]
 			gamma = dict(zip(formals, it.type_args))
 			self._constructors[a] = original.visit(Rewriter(gamma))
-	
+
+	###############################################################################
+
 	def visit_ImportForeign(self, d:syntax.ImportForeign):
 		for group in d.groups:
 			type_args = [TypeVariable() for _ in group.type_params]
 			typ = ManifestBuilder(group.type_params, type_args).visit(group.type_expr)
 			for sym in group.symbols:
 				self._ffi[sym] = typ
-	
+
+	###############################################################################
+
 	@staticmethod
 	def visit_Literal(expr: syntax.Literal, env:TYPE_ENV) -> SophieType:
 		return _literal_type_map[type(expr.value)]
 	
 	def apply_UDF(self, fn_type:UDFType, arg_types:Sequence[SophieType], env:TYPE_ENV) -> SophieType:
 		fn = fn_type.fn
 		arity = len(fn.params)
 		if arity != len(arg_types): raise ArityError
-		inner = ActivationRecord(fn, env, fn_type.static_env, arg_types)
+		inner = Activation.for_function(fn_type.static_env, fn, arg_types)
 		return self.exec_UDF(fn, inner)
 		
-	def exec_UDF(self, fn:syntax.UserDefinedFunction, env:TYPE_ENV):
+	def exec_UDF(self, fn:syntax.UserFunction, env:TYPE_ENV):
 		# The part where memoization must happen.
 		memo_symbols = self._deps_pass.depends[fn]
+		assert all(isinstance(s, syntax.FormalParameter) for s in memo_symbols)
 		memo_types = tuple(
-			env.chase(p).bindings[p].number
+			env.chase(p).fetch(p)  # .number
 			for p in memo_symbols
 		)
 		memo_key = fn, memo_types
 		if memo_key in self._memo:
 			return self._memo[memo_key]
 		elif memo_key in self._recursion:
 			self._recursion[memo_key] = True
+			# self._report.trace(">Recursive:", fn, dict(zip((s.nom.text for s in memo_symbols), memo_types)))
 			return BOTTOM
 		else:
 			# TODO: check argument and return against declared contract.
 			#       Could do this with a binder if FormalParam gets associated SophieType.
 			#       Also, pass around judgements not just types.
 			self._recursion[memo_key] = False
 			self._memo[memo_key] = self.visit(fn.expr, env)
 			if self._recursion.pop(memo_key):
 				prior = BOTTOM
 				while prior != self._memo[memo_key]:
 					prior = self._memo[memo_key]
 					self._memo[memo_key] = self.visit(fn.expr, env)
 				if prior is BOTTOM:
-					self._report.ill_founded_function(env.path(), fn)
+					self._report.ill_founded_function(env, fn)
+				# self._report.trace("<Resolved:", fn)
 					
 		return self._memo[memo_key]
 	
-	def _call_site(self, site: syntax.ValExpr, fn_type, args:Sequence[Expr], env:TYPE_ENV) -> SophieType:
+	def _call_site(self, site: syntax.ValExpr, fn_type, args:Sequence[ValExpr], env:TYPE_ENV) -> SophieType:
 		arg_types = [self.visit(a, env) for a in args]
-		if any(t is ERROR for t in arg_types):
+		if ERROR in arg_types:
 			return ERROR
 
 		env.pc = site
 
 		if isinstance(fn_type, ArrowType):
 			assert isinstance(fn_type.arg, ProductType)  # Maybe not forever, but now.
 			arity = len(fn_type.arg.fields)
 			if arity != len(args):
-				self._report.wrong_arity(env.path(), arity, args)
+				self._report.wrong_arity(env, site, arity, args)
 				return ERROR
 			
 			binder = Binder(self, env)
 			for expr, need, got in zip(args, fn_type.arg.fields, arg_types):
 				binder.bind(need, got)
 				if not binder.ok:
 					self._report.bad_type(env, expr, need, got)
 					return ERROR
 
 			# 2. Return the arrow's result-type rewritten using the bindings thus found.
 			return fn_type.res.visit(Rewriter(binder.gamma))
 		
 		elif isinstance(fn_type, UDFType):
 			try:
-				return self.apply_UDF(fn_type, arg_types, env)
+				result = self.apply_UDF(fn_type, arg_types, env)
+				# self._report.trace("     ", fn_type, tuple(arg_types), '-->', result)
+				return result
 			except ArityError:
-				self._report.wrong_arity(env.path(), len(fn_type.fn.params), args)
+				self._report.wrong_arity(env, site, len(fn_type.fn.params), args)
 				return ERROR
 			
+		elif isinstance(fn_type, MethodType):
+			return MessageType()  # TODO
+			
 		else:
 			raise NotImplementedError(type(fn_type))
 	
 	def visit_Call(self, site: syntax.Call, env: TYPE_ENV) -> SophieType:
 		fn_type = self.visit(site.fn_exp, env)
 		if fn_type is ERROR: return ERROR
 		return self._call_site(site, fn_type, site.args, env)
@@ -429,71 +584,87 @@
 		target = lu.ref.dfn
 		if isinstance(target, (syntax.TypeDeclaration, syntax.SubTypeSpec)):
 			return self._constructors[target]  # Must succeed because of resolution.check_constructors
 		if isinstance(target, syntax.FFI_Alias):
 			return self._ffi[target]
 		
 		static_env = env.chase(target)
-		if isinstance(target, syntax.UserDefinedFunction):
+		if isinstance(target, syntax.UserFunction):
 			if target.params:
 				return UDFType(target, static_env).exemplar()
 			else:
-				return self.exec_UDF(target, static_env)
+				inner = Activation.for_function(static_env, target, ())
+				return self.exec_UDF(target, inner)
 		else:
 			assert isinstance(target, (syntax.FormalParameter, syntax.Subject))
-			return static_env.bindings[target]
+			return static_env.fetch(target)
 		
 	def visit_ExplicitList(self, el:syntax.ExplicitList, env:TYPE_ENV) -> SumType:
 		# Since there's guaranteed to be at least one value,
 		# we should be able to glean a concrete type from it.
 		# Having that, we should be able to get a union over them all.
 		union_find = UnionFinder(BOTTOM)
 		for e in el.elts:
 			union_find.unify_with(self.visit(e, env))
 			if union_find.died:
-				self._report.type_mismatch(env.path(), el.elts[0], e)
+				self._report.type_mismatch(env, el.elts[0], e)
 				return ERROR
 		element_type = union_find.result()
-		return SumType(primitive.LIST, (element_type,))
+		return SumType(self._list_symbol, (element_type,))
 
 	def visit_Cond(self, cond:syntax.Cond, env:TYPE_ENV) -> SophieType:
 		if_part_type = self.visit(cond.if_part, env)
 		if if_part_type is ERROR: return ERROR
 		if if_part_type != primitive.literal_flag:
 			self._report.bad_type(env, cond.if_part, primitive.literal_flag, if_part_type)
 			return ERROR
 		union_find = UnionFinder(self.visit(cond.then_part, env))
 		union_find.unify_with(self.visit(cond.else_part, env))
 		if union_find.died:
-			self._report.type_mismatch(env.path(), cond.then_part, cond.else_part)
+			self._report.type_mismatch(env, cond.then_part, cond.else_part)
 			return ERROR
 		return union_find.result()
 	
 	def visit_MatchExpr(self, mx:syntax.MatchExpr, env:TYPE_ENV) -> SophieType:
 		def try_everything(type_args:Sequence[SophieType]):
 			union_find = UnionFinder(BOTTOM)
 			for alt in mx.alternatives:
-				env.bindings[mx.subject] = _hypothesis(alt.pattern.dfn, type_args)
-				union_find.unify_with(self.visit(alt.sub_expr, env))
+				subtype_symbol = mx.namespace[alt.nom.key()]
+				inner = Activation.for_subject(env, mx.subject)
+				inner.assign(mx.subject,  _hypothesis(subtype_symbol, type_args))
+				for subfn in alt.where: inner.declare(subfn)
+				union_find.unify_with(self.visit(alt.sub_expr, inner))
+				if union_find.died:
+					self._report.type_mismatch(env, mx.alternatives[0].sub_expr, alt.sub_expr)
+					return ERROR
+			if mx.otherwise is not None:
+				inner = Activation.for_subject(env, mx.subject)
+				inner.assign(mx.subject, subject_type)
+				union_find.unify_with(self.visit(mx.otherwise, inner))
 				if union_find.died:
-					self._report.type_mismatch(env.path(), mx.alternatives[0].sub_expr, alt.sub_expr)
+					self._report.type_mismatch(env, mx.alternatives[0].sub_expr, mx.otherwise)
 					return ERROR
 			return union_find.result()
 
 		subject_type = self.visit(mx.subject.expr, env)
-		if subject_type is ERROR: return ERROR
-		assert isinstance(mx.variant, syntax.Variant)
-		if isinstance(subject_type, SumType) and subject_type.variant is mx.variant:
+		if subject_type is ERROR:
+			return ERROR
+
+		if isinstance(subject_type, SumType):
 			return try_everything(subject_type.type_args)
+		
 		elif subject_type is BOTTOM:
 			return try_everything([BOTTOM] * len(mx.variant.type_params))
+		
 		elif isinstance(subject_type, SubType) and subject_type.st.variant is mx.variant:
-			branch = mx.dispatch.get(subject_type.st.nom.text, mx.otherwise)
-			env.bindings[mx.subject] = subject_type
+			case_key = subject_type.st.nom.text
+			branch = mx.dispatch.get(case_key, mx.otherwise)
+			env.assign(mx.subject, subject_type)
 			return self.visit(branch, env)
+		
 		else:
 			self._report.bad_type(env, mx.subject.expr, mx.variant, subject_type)
 			return ERROR
 
 	def visit_FieldReference(self, fr:syntax.FieldReference, env:TYPE_ENV) -> SophieType:
 		lhs_type = self.visit(fr.lhs, env)
 		if isinstance(lhs_type, RecordType):
@@ -505,24 +676,33 @@
 		elif lhs_type is BOTTOM:
 			# In principle the evaluator could make an observation / infer a constraint
 			return lhs_type
 		elif lhs_type is ERROR:
 			# Complaint has already been issued.
 			return lhs_type
 		else:
-			self._report.type_has_no_fields(env.path(), fr, lhs_type)
+			self._report.type_has_no_fields(env, fr, lhs_type)
 			return ERROR
 		try:
 			field_spec = spec.field_space[fr.field_name.text]
 		except KeyError:
-			self._report.record_lacks_field(env.path(), fr, lhs_type)
+			self._report.record_lacks_field(env, fr, lhs_type)
 			return ERROR
 		assert isinstance(field_spec, syntax.FormalParameter), field_spec
 		return ManifestBuilder(parameters, lhs_type.type_args).visit(field_spec.type_expr)
 
+	def visit_BoundMethod(self, mr:syntax.BoundMethod, env:TYPE_ENV) -> SophieType:
+		receiver_type = self.visit(mr.receiver, env)
+		if receiver_type is ERROR: return ERROR
+		if not isinstance(receiver_type, ActorType):
+			need = "to receive message '%s' but it is not an actor" % mr.method_name.text
+			self._report.bad_type(env, mr.receiver, need, receiver_type)
+			return ERROR
+		return MethodType()  # TODO
+
 def _hypothesis(st:Symbol, type_args:Sequence[SophieType]) -> SubType:
 	assert isinstance(st, syntax.SubTypeSpec)
 	body = st.body
 	if body is None:
 		return EnumType(st)
 	if isinstance(body, syntax.RecordSpec):
 		return TaggedRecord(st, type_args)
```

### Comparing `sophie-lang-0.0.0/sophie_lang.egg-info/PKG-INFO` & `sophie-lang-0.0.3/sophie_lang.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophie-lang
-Version: 0.0.0
+Version: 0.0.3
 Summary: A call-by-need strong-inferred-type language named for French mathematician Sophie Germain
 Home-page: https://github.com/kjosib/sophie
 Author: Ian Kjos
 Author-email: kjosib@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -42,23 +42,14 @@
 this should not break too many brains. However, Sophie is an expression-oriented call-by-need language,
 so some things are bound look a bit more like SQL or Haskell.
 
 It may seem a small thing, but algebra-style parentheses are much more clear to me than Lisp or Haskell style.
 I think that's also true for most of the world's programmers.
 Things are better when the notation does not interfere with understanding.
 
-## Install/Run
-
-1. `pip install --upgrade booze-tools`
-2. Clone or download the repository.
-3. `py -m sophie examples/turtle.sg`
-
-Yes, it's implemented atop Python. For now. That's a key enabler, actually.
-Python pays the bills right now. C'est la vie.
-
 ## How do I Learn Sophie?
 
 1. [Read the docs](https://sophie.readthedocs.io)
 2. Poke around the [examples](https://github.com/kjosib/sophie/tree/main/examples) and [grammar](https://github.com/kjosib/sophie/blob/main/sophie/Sophie.md)
 3. Contribute to the docs in the usual way.
 
 It sure might be nice to have a *Learn computer science with Sophie*
@@ -73,15 +64,22 @@
 * Sophie has Turtle-graphics! (See [here](https://github.com/kjosib/sophie/blob/main/examples/turtle.sg) for examples.)
 * Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/guess_the_number.sg) as an example.
 * The new type-checker gives excellent feedback and cannot be fooled. Through abstract interpretation it completely rules out *type* errors.
   (Domain errors, such as division by zero, are still possible.)
 * The module system got an upgrade: there is now a notion of a system-package and the beginnings of a standard library.
 * The FFI (into Python): Sophie can call Python; Python can call Sophie; and Python can install I/O drivers into Sophie.
 * Error display is improved in various ways. There is also now an easy way to install helpful messages for parse errors.
-  This works; there just aren't many good messages yet.
+  This works surprisingly well now.
+
+*Caveat:* Type-checking is presently out of commission in HEAD, but the release has it working.
+
+Some things are in progress:
+
+* I'm in progress to add asynchronous message-passing, with an eye towards a safe concurrency model.
+  (That's why type-checking is temporarily turned off)
 
 Certain things are not started yet:
 
 * Variable-Arity Functions.
 * Ad-hoc polymorphic multi-methods.
 * List comprehension (expressions like `[expr FOR name IN expr]`) are removed from the syntax for now.
 * Asynchrony.
```

### Comparing `sophie-lang-0.0.0/sophie_lang.egg-info/SOURCES.txt` & `sophie-lang-0.0.3/sophie_lang.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 LICENSE
 README.md
 setup.py
 sophie/Sophie.automaton
 sophie/__init__.py
 sophie/__main__.py
 sophie/calculus.py
+sophie/cmdline.py
 sophie/diagnostics.py
+sophie/executive.py
 sophie/front_end.py
 sophie/modularity.py
 sophie/ontology.py
 sophie/primitive.py
 sophie/resolution.py
-sophie/simple_evaluator.py
+sophie/runtime.py
 sophie/stacking.py
 sophie/syntax.py
 sophie/type_evaluator.py
 sophie/adapters/__init__.py
 sophie/adapters/game_adapter.py
 sophie/adapters/teletype_adapter.py
 sophie/adapters/turtle_adapter.py
@@ -23,9 +25,10 @@
 sophie/sys/game.sg
 sophie/sys/preamble.sg
 sophie/sys/teletype.sg
 sophie/sys/turtle.sg
 sophie_lang.egg-info/PKG-INFO
 sophie_lang.egg-info/SOURCES.txt
 sophie_lang.egg-info/dependency_links.txt
+sophie_lang.egg-info/entry_points.txt
 sophie_lang.egg-info/requires.txt
 sophie_lang.egg-info/top_level.txt
```

