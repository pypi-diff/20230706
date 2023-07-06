# Comparing `tmp/hyrule-0.3.0.tar.gz` & `tmp/hyrule-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyrule-0.3.0.tar", last modified: Wed Feb  8 19:09:18 2023, max compression
+gzip compressed data, was "hyrule-0.4.0.tar", last modified: Thu Jul  6 19:53:42 2023, max compression
```

## Comparing `hyrule-0.3.0.tar` & `hyrule-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,26 @@
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-02-08 19:09:18.163011 hyrule-0.3.0/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4411 2023-02-08 18:55:49.000000 hyrule-0.3.0/AUTHORS
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1053 2023-02-08 18:55:49.000000 hyrule-0.3.0/LICENSE
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1583 2023-02-08 19:09:18.163011 hyrule-0.3.0/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      723 2022-05-15 21:26:03.000000 hyrule-0.3.0/README.rst
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-02-08 19:09:18.159011 hyrule-0.3.0/hyrule/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      399 2023-02-08 19:08:18.000000 hyrule-0.3.0/hyrule/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7155 2023-02-08 18:55:49.000000 hyrule-0.3.0/hyrule/anaphoric.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4506 2023-02-08 18:55:49.000000 hyrule-0.3.0/hyrule/argmove.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    11188 2022-05-15 21:26:03.000000 hyrule-0.3.0/hyrule/collections.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    14180 2022-05-15 21:26:03.000000 hyrule-0.3.0/hyrule/control.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    14883 2022-05-15 21:26:03.000000 hyrule-0.3.0/hyrule/destructure.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      351 2022-05-15 21:26:03.000000 hyrule-0.3.0/hyrule/hy_init.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    13084 2023-02-08 18:55:49.000000 hyrule-0.3.0/hyrule/hypprint.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2941 2022-05-15 21:26:03.000000 hyrule-0.3.0/hyrule/iterables.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4874 2022-05-15 21:26:03.000000 hyrule-0.3.0/hyrule/macrotools.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7861 2023-02-08 18:55:49.000000 hyrule-0.3.0/hyrule/misc.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3998 2022-05-15 21:26:03.000000 hyrule-0.3.0/hyrule/sequences.hy
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-02-08 19:09:18.159011 hyrule-0.3.0/hyrule.egg-info/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1583 2023-02-08 19:09:17.000000 hyrule-0.3.0/hyrule.egg-info/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      780 2023-02-08 19:09:18.000000 hyrule-0.3.0/hyrule.egg-info/SOURCES.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2023-02-08 19:09:17.000000 hyrule-0.3.0/hyrule.egg-info/dependency_links.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       17 2023-02-08 19:09:18.000000 hyrule-0.3.0/hyrule.egg-info/requires.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       13 2023-02-08 19:09:18.000000 hyrule-0.3.0/hyrule.egg-info/top_level.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2023-02-08 19:09:18.163011 hyrule-0.3.0/setup.cfg
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1828 2023-02-08 19:07:51.000000 hyrule-0.3.0/setup.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-02-08 19:09:18.163011 hyrule-0.3.0/tests/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2023-02-08 18:55:49.000000 hyrule-0.3.0/tests/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     6292 2023-02-08 18:55:49.000000 hyrule-0.3.0/tests/test_anaphoric.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      288 2022-05-15 21:26:03.000000 hyrule-0.3.0/tests/test_anaphoric_single.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1978 2023-02-08 18:55:49.000000 hyrule-0.3.0/tests/test_argmove.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      656 2022-06-20 20:00:40.000000 hyrule-0.3.0/tests/test_collections.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7632 2022-05-15 21:26:03.000000 hyrule-0.3.0/tests/test_control.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1783 2022-06-20 20:00:40.000000 hyrule-0.3.0/tests/test_defmain.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    10437 2022-05-31 20:21:49.000000 hyrule-0.3.0/tests/test_destructure.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2367 2022-05-15 21:26:03.000000 hyrule-0.3.0/tests/test_iterables.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1066 2022-05-15 21:26:03.000000 hyrule-0.3.0/tests/test_loop.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3907 2022-05-31 20:21:49.000000 hyrule-0.3.0/tests/test_macrotools.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2399 2023-02-08 18:55:49.000000 hyrule-0.3.0/tests/test_misc.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5147 2022-05-15 21:26:03.000000 hyrule-0.3.0/tests/test_pprint.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2715 2022-05-15 21:26:03.000000 hyrule-0.3.0/tests/test_sequences.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1421 2022-06-20 20:00:40.000000 hyrule-0.3.0/tests/test_slicing.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1581 2022-05-15 21:26:03.000000 hyrule-0.3.0/tests/test_walk.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-06 19:53:42.857113 hyrule-0.4.0/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4453 2023-07-02 12:55:15.000000 hyrule-0.4.0/AUTHORS
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1053 2023-07-02 12:55:15.000000 hyrule-0.4.0/LICENSE
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1248 2023-07-06 19:53:42.857113 hyrule-0.4.0/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      723 2023-07-02 12:55:15.000000 hyrule-0.4.0/README.rst
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-06 19:53:42.857113 hyrule-0.4.0/hyrule/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      399 2023-07-06 19:52:34.000000 hyrule-0.4.0/hyrule/__init__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     7155 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/anaphoric.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4506 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/argmove.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    11188 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/collections.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    14392 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/control.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    14883 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/destructure.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      362 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/hy_init.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    12832 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/hypprint.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2941 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/iterables.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     5676 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/macrotools.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     7861 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/misc.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4189 2023-07-02 12:55:15.000000 hyrule-0.4.0/hyrule/sequences.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-07-06 19:53:42.857113 hyrule-0.4.0/hyrule.egg-info/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1248 2023-07-06 19:53:42.000000 hyrule-0.4.0/hyrule.egg-info/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      416 2023-07-06 19:53:42.000000 hyrule-0.4.0/hyrule.egg-info/SOURCES.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2023-07-06 19:53:42.000000 hyrule-0.4.0/hyrule.egg-info/dependency_links.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       17 2023-07-06 19:53:42.000000 hyrule-0.4.0/hyrule.egg-info/requires.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        7 2023-07-06 19:53:42.000000 hyrule-0.4.0/hyrule.egg-info/top_level.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2023-07-06 19:53:42.857113 hyrule-0.4.0/setup.cfg
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1522 2023-07-06 19:53:07.000000 hyrule-0.4.0/setup.py
```

### Comparing `hyrule-0.3.0/AUTHORS` & `hyrule-0.4.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -104,7 +104,8 @@
 * Allie Jo Casey <allie.jo.casey@gmail.com>
 * Joshua Munn <public@elysee-munn.family>
 * Peter Andreev <appa@gmx.co.uk>
 * Sunjay Cauligi <scauligi@eng.ucsd.edu>
 * David Tscheppen <david.tscheppen@gmail.com>
 * Gabriel F. C. Pereira <empresagabriel@gmail.com>
 * Daniel Nagy <danielnagy@posteo.de>
+* John Blundell <jlobblet@jlobblet.co.uk>
```

### Comparing `hyrule-0.3.0/LICENSE` & `hyrule-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyrule-0.3.0/PKG-INFO` & `hyrule-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 Metadata-Version: 2.1
 Name: hyrule
-Version: 0.3.0
+Version: 0.4.0
 Summary: A utility library for the Hy programming language
 Author: Paul Tagliamonte
 Author-email: tag@pault.ag
 License: Expat
 Project-URL: Documentation, https://hyrule.readthedocs.io
 Project-URL: Source, https://github.com/hylang/hyrule
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: DFSG approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Lisp
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 License-File: AUTHORS
 
 Hyrule is a utility library for the `Hy <http://hylang.org>`_ programming language. It can be thought of as the Hy equivalent, or addition, to Python's standard library. While intended primarily for Hy programs, its functions and classes can be used in Python as with any other Python library; just ``import hyrule``. Hyrule's macros, on the other hand, are only really usable in Hy.
 
 All of Hyrule's contents can be imported or required directly from the top-level module ``hyrule``.
 
 `Hyrule's documentation can be read online on Read the Docs. <https://hyrule.readthedocs.io>`_
 
 You can run Hyrule's test suite with the command ``pytest`` and build its documentation with ``( cd docs; sphinx-build . _build -b html )``.
-
-
```

### Comparing `hyrule-0.3.0/README.rst` & `hyrule-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `hyrule-0.3.0/hyrule/anaphoric.hy` & `hyrule-0.4.0/hyrule/anaphoric.hy`

 * *Files identical despite different names*

### Comparing `hyrule-0.3.0/hyrule/argmove.hy` & `hyrule-0.4.0/hyrule/argmove.hy`

 * *Files identical despite different names*

### Comparing `hyrule-0.3.0/hyrule/collections.hy` & `hyrule-0.4.0/hyrule/collections.hy`

 * *Files identical despite different names*

### Comparing `hyrule-0.3.0/hyrule/control.hy` & `hyrule-0.4.0/hyrule/control.hy`

 * *Files 3% similar despite different names*

```diff
@@ -94,16 +94,16 @@
         …)
 
   For example, you could translate direction names to vectors like this::
 
       (case direction
         "north" [ 0  1]
         "south" [ 0 -1]
-        "east"  [-1  0]
-        "west"  [ 1  0])
+        "east"  [ 1  0]
+        "west"  [-1  0])
 
   Thus, ``(case KEY …)`` is equivalent to ``(branch (= it KEY) …)``, except
   ``KEY`` is evaluated exactly once, regardless of the number of cases.
 
   Like :hy:func:`branch`, ``case`` treats the symbol ``else`` as a default
   case, and it has an error-raising version, :hy:func:`ecase`.
 
@@ -146,15 +146,15 @@
 
   ::
      => (cfor tuple x (range 10) :if (% x 2) x)
      #(1 3 5 7 9)
 
   The equivalent in python would be:
 
-     >>> tuple(x for x in range(10) if is_odd(x))
+     >>> tuple(x for x in range(10) if x % 2)
 
   Some other common functions that take iterables::
 
      => (cfor all x [1 3 8 5] (< x 10))
      True
 
      => (with [f (open "AUTHORS")]
@@ -165,33 +165,39 @@
      ...        (len name)))
      20 ;; The number of characters in the longest author's name that starts with 'A'
   ]]
   `(~f (gfor ~@generator)))
 
 
 (defn _do-n [count-form body]
-  `(for [~(hy.gensym) (range ~count-form)]
-    ~@body))
+  (setv count (hy.gensym))
+  `(do
+    (setv ~count ~count-form)
+    (for [~(hy.gensym)
+        (if (= ~count Inf)
+          (hy.M.itertools.repeat None)
+          (range ~count))]
+      ~@body)))
 
 
 (defmacro do-n [count-form #* body]
-  "Execute `body` a number of times equal to `count-form` and return
+  #[[Execute `body` a number of times equal to `count-form` and return
   ``None``. (To collect return values, use :hy:macro:`list-n`
-  instead.) Negative values of the count are treated as 0.
-
-  This macro is implemented as a :hy:func:`for` loop, so you can use
-  :hy:func:`break` and :hy:func:`continue` in the body.
+  instead.)
 
-  ::
+  The macro is implemented as a :hy:func:`for` loop over a
+  :func:`range` call, with the attendent consequences for negative
+  counts, :hy:func:`break`, etc. As an exception, if the count is
+  `Inf`, the loop is run over an infinite iterator instead. ::
 
-     => (do-n 3 (print \"hi\"))
+     => (do-n 3 (print "hi"))
      hi
      hi
-     hi
-  "
+     hi]]
+
   (_do-n count-form body))
 
 
 (defmacro defmain [args #* body]
   #[[Define a function to be called when :attr:`__name__` equals ``"__main__"``
   (see :mod:`__main__`). ``args`` is the function's lambda list, which will be
   matched against :data:`sys.argv`. Recall that the first element of
```

### Comparing `hyrule-0.3.0/hyrule/destructure.hy` & `hyrule-0.4.0/hyrule/destructure.hy`

 * *Files identical despite different names*

### Comparing `hyrule-0.3.0/hyrule/hypprint.hy` & `hyrule-0.4.0/hyrule/hypprint.hy`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,18 @@
         re
         collections
         pprint [PrettyPrinter :as PyPrettyPrinter
                 _recursion
                 _safe-tuple
                 _safe-key]
         hy.core.hy-repr
-        hy._compat [PY3_8 PY3_10]
+        hy._compat [PY3_10]
         hyrule.misc [inc dec constantly])
 
-(setv __all__ ["pprint" "pformat" "saferepr" "PrettyPrinter" "is_readable" "is_recursive" "pp"])
+(export [pprint pformat saferepr PrettyPrinter readable? recursive? pp])
 
 (if PY3_10
   (defn _safe-py-repr [object context maxlevels level sort-dicts]
     (._safe-repr (PyPrettyPrinter :sort-dicts sort-dicts)
       object context maxlevels level))
   (import pprint [_safe-repr :as _safe-py-repr]))
 
@@ -158,17 +158,15 @@
     (return #((% format (.join " " components))
                readable?
                recursive?)))
 
   (when (in typ hy.core.hy-repr._registry)
     (return #((hy.repr object) True False)))
 
-  (if PY3_8
-      (_safe-py-repr object context maxlevels level sort-dicts)
-      (_safe-py-repr object context maxlevels level)))
+  (_safe-py-repr object context maxlevels level sort-dicts))
 
 
 (setv CHUNK-SIZE 4)
 
 (defn _wrap-bytes-repr [object width allowance]
   (setv current b""
         _last (* (// (len object) CHUNK-SIZE) CHUNK-SIZE))
@@ -194,24 +192,22 @@
      depth: The maximum depth to print out nested structures.
      stream: The desired output stream.  If omitted (or false), the standard
        output stream available at construction will be used.
      compact: If true, several items will be combined in one line.
      sort-dicts: If True, dict keys are sorted. (only available for python >= 3.8)"
   (defn __init__ [self [indent 1] [width 80] [depth None] [stream None]
                   * [compact False] [sort-dicts True]]
-    (when (and (not PY3_8) (not sort-dicts))
-        (raise (ValueError "sort-dicts is not available for python versions < 3.8")))
     (setv self._sort-dicts True)
     (.__init__ (super)
                :indent indent
                :width width
                :depth depth
                :stream stream
                :compact compact
-               #** (if PY3_8 {"sort_dicts" sort-dicts} {})))
+               :sort-dicts sort-dicts))
 
   (defn format [self object context maxlevels level]
     "Format object for a specific context, returning a string
     and flags indicating whether the representation is 'readable'
     and whether the object represents a recursive construct.
     "
     (_safe-repr object context maxlevels level self._sort-dicts))
```

### Comparing `hyrule-0.3.0/hyrule/iterables.hy` & `hyrule-0.4.0/hyrule/iterables.hy`

 * *Files identical despite different names*

### Comparing `hyrule-0.3.0/hyrule/macrotools.hy` & `hyrule-0.4.0/hyrule/macrotools.hy`

 * *Files 18% similar despite different names*

```diff
@@ -154,7 +154,38 @@
   "
   (setv syms [])
   (for [arg args]
     (.extend syms [arg `(hy.gensym '~arg)]))
   `(do
     (setv ~@syms)
     ~@body))
+
+
+(defreader /
+  #[[Sugar for :hy:class:`hy.M`, to access modules without needing to explicitly import them first.
+  Unlike ``hy.M``, ``#/`` cannot be used if the module name is only known at runtime.
+
+  Examples:
+
+    Access modules and their elements directly by name:
+
+    ::
+
+      => (type #/ re)
+      <class 'module'>
+      => #/ os.curdir
+      "."
+      => (#/ re.search r"[a-z]+" "HAYneedleSTACK")
+      <re.Match object; :span #(3 9) :match "needle">
+
+    Like ``hy.M``, separate submodule names with ``/``:
+
+    ::
+
+      => (#/ os/path.basename "path/to/file")
+      "file"]]
+  (.slurp-space hy.&reader)
+  (setv [mod #* ident] (.split (.read-ident hy.&reader) ".")
+        imp `(hy.M ~(hy.mangle (.replace mod "/" "."))))
+  (if ident
+    `(. ~imp ~@(map hy.models.Symbol ident))
+    imp))
```

### Comparing `hyrule-0.3.0/hyrule/misc.hy` & `hyrule-0.4.0/hyrule/misc.hy`

 * *Files identical despite different names*

### Comparing `hyrule-0.3.0/hyrule/sequences.hy` & `hyrule-0.4.0/hyrule/sequences.hy`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 This results in the sequence ``[0 1 1 2 3 5 8 13 21 34 ...]``.
 "
 
 (import
   itertools [islice]
   hyrule.misc [inc])
 
+(require hyrule.macrotools [defmacro/g!])
+
 (defclass Sequence []
   "Container for construction of lazy sequences."
 
   (defn __init__ [self func]
     "initialize a new sequence with a function to compute values"
     (setv (. self func) func)
     (setv (. self cache) [])
@@ -90,29 +92,33 @@
                 "[{0}]")
               (.join ", " (map str items))))
 
    (defn __repr__ [self]
      "string representation of this sequence"
      (.__str__ self)))
 
-(defmacro seq [param #* seq-code]
+(defmacro/g! seq [param #* seq-code]
   "Creates a sequence defined in terms of ``n``.
 
   Examples:
     => (seq [n] (* n n))
   "
-  `(Sequence (fn ~param (do ~@seq-code))))
+  `(do
+     (import hyrule.sequences [Sequence :as ~g!Sequence])
+     (~g!Sequence (fn ~param (do ~@seq-code)))))
 
-(defmacro defseq [seq-name param #* seq-code]
+(defmacro/g! defseq [seq-name param #* seq-code]
   "Creates a sequence defined in terms of ``n`` and assigns it to a given name.
 
   Examples:
     => (defseq numbers [n] n)
   "
-  `(setv ~seq-name (Sequence (fn ~param (do ~@seq-code)))))
+  `(do
+     (import hyrule.sequences [Sequence :as ~g!Sequence])
+     (setv ~seq-name (~g!Sequence (fn ~param (do ~@seq-code))))))
 
 (defn end-sequence []
   "Signals the end of a sequence when an iterator reaches the given point of the sequence.
 
   Internally, this is done by raising
   ``IndexError``, catching that in the iterator, and raising
   ``StopIteration``
```

### Comparing `hyrule-0.3.0/hyrule.egg-info/PKG-INFO` & `hyrule-0.4.0/hyrule.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 Metadata-Version: 2.1
 Name: hyrule
-Version: 0.3.0
+Version: 0.4.0
 Summary: A utility library for the Hy programming language
 Author: Paul Tagliamonte
 Author-email: tag@pault.ag
 License: Expat
 Project-URL: Documentation, https://hyrule.readthedocs.io
 Project-URL: Source, https://github.com/hylang/hyrule
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: DFSG approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Lisp
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 License-File: AUTHORS
 
 Hyrule is a utility library for the `Hy <http://hylang.org>`_ programming language. It can be thought of as the Hy equivalent, or addition, to Python's standard library. While intended primarily for Hy programs, its functions and classes can be used in Python as with any other Python library; just ``import hyrule``. Hyrule's macros, on the other hand, are only really usable in Hy.
 
 All of Hyrule's contents can be imported or required directly from the top-level module ``hyrule``.
 
 `Hyrule's documentation can be read online on Read the Docs. <https://hyrule.readthedocs.io>`_
 
 You can run Hyrule's test suite with the command ``pytest`` and build its documentation with ``( cd docs; sphinx-build . _build -b html )``.
-
-
```

### Comparing `hyrule-0.3.0/setup.py` & `hyrule-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,40 +21,33 @@
                     invalidation_mode=py_compile.PycInvalidationMode.CHECKED_HASH,
                 )
 
 
 # both setup_requires and install_requires
 # since we need to compile .hy files during setup
 requires = [
-    'hy >= 0.26.0, < 0.27'
+    'hy >= 0.27.0, < 0.28'
 ]
 
 
 setuptools.setup(
     name = 'hyrule',
-    version = '0.3.0',
+    version = '0.4.0',
     setup_requires=['wheel'] + requires,
     install_requires=requires,
-    packages = setuptools.find_packages(),
+    packages = setuptools.find_packages(exclude = ["tests*"]),
     package_data={'': ['*.hy']},
     author = "Paul Tagliamonte",
     author_email = "tag@pault.ag",
     description = 'A utility library for the Hy programming language',
     long_description = long_description,
     license = 'Expat',
     project_urls = dict(
         Documentation = 'https://hyrule.readthedocs.io',
         Source = 'https://github.com/hylang/hyrule'),
     platforms = ['any'],
     classifiers = [
         "Development Status :: 4 - Beta",
         "License :: DFSG approved",
         "License :: OSI Approved :: MIT License",  # Really "Expat". Ugh.
-        "Operating System :: OS Independent",
-        "Programming Language :: Lisp",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10"],
+        "Operating System :: OS Independent"],
     cmdclass={'install': install})
```

