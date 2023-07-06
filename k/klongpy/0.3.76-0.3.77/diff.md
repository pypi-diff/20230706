# Comparing `tmp/klongpy-0.3.76.tar.gz` & `tmp/klongpy-0.3.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.3.76.tar", last modified: Fri Jun 30 23:36:08 2023, max compression
+gzip compressed data, was "klongpy-0.3.77.tar", last modified: Thu Jul  6 15:05:25 2023, max compression
```

## Comparing `klongpy-0.3.76.tar` & `klongpy-0.3.77.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-30 23:36:08.170746 klongpy-0.3.76/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.76/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-30 23:36:08.170746 klongpy-0.3.76/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    10605 2023-04-13 20:55:52.000000 klongpy-0.3.76/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-30 23:36:08.170746 klongpy-0.3.76/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.76/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.3.76/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.3.76/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    25944 2023-06-30 23:35:49.000000 klongpy-0.3.76/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30733 2023-06-30 23:35:49.000000 klongpy-0.3.76/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20337 2023-06-30 23:35:49.000000 klongpy-0.3.76/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.3.76/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11966 2023-06-29 19:31:08.000000 klongpy-0.3.76/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.76/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.76/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-30 23:36:08.170746 klongpy-0.3.76/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-30 23:36:08.000000 klongpy-0.3.76/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-06-30 23:36:08.000000 klongpy-0.3.76/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-06-30 23:36:08.000000 klongpy-0.3.76/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-06-30 23:36:08.000000 klongpy-0.3.76/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-06-30 23:36:08.000000 klongpy-0.3.76/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-30 23:36:08.170746 klongpy-0.3.76/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6592 2023-06-26 15:14:16.000000 klongpy-0.3.76/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-06-30 23:36:08.170746 klongpy-0.3.76/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-06-30 23:35:49.000000 klongpy-0.3.76/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-30 23:36:08.170746 klongpy-0.3.76/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.3.76/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.76/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    23327 2023-06-29 19:31:08.000000 klongpy-0.3.76/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.3.76/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.3.76/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.3.76/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.76/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.76/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.76/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12559 2023-06-29 19:31:08.000000 klongpy-0.3.76/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.3.76/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.77/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12794 2023-07-06 15:05:25.731818 klongpy-0.3.77/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12259 2023-07-06 15:05:05.000000 klongpy-0.3.77/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.77/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.3.77/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.3.77/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    25901 2023-07-06 15:05:05.000000 klongpy-0.3.77/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30733 2023-06-30 23:35:49.000000 klongpy-0.3.77/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20366 2023-07-06 15:05:05.000000 klongpy-0.3.77/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.3.77/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    15564 2023-07-06 15:05:05.000000 klongpy-0.3.77/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.77/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.77/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12794 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6736 2023-07-06 15:05:05.000000 klongpy-0.3.77/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-06 15:05:25.731818 klongpy-0.3.77/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-07-06 15:05:05.000000 klongpy-0.3.77/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.3.77/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.77/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    23466 2023-07-06 15:05:05.000000 klongpy-0.3.77/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.3.77/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.3.77/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.3.77/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.77/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.77/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.77/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    13888 2023-07-06 15:05:05.000000 klongpy-0.3.77/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.3.77/tests/test_util.py
```

### Comparing `klongpy-0.3.76/LICENSE` & `klongpy-0.3.77/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/PKG-INFO` & `klongpy-0.3.77/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.76
+Version: 0.3.77
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -219,14 +219,74 @@
 ```
 outputs
 ```
 called from KlongPy: 2018-06-21 00:00:00
 called from KlongPy: {'timestamp': datetime.datetime(2018, 6, 21, 0, 0)}
 ```
 
+## Loading Python Modules directly into KlongPy
+
+KlongPy has the powerful ability to load Python modules directly. This can be extremely useful when you want to utilize the functionality offered by various Python libraries, and seamlessly integrate them into your KlongPy programs.
+
+Here is an example of how you can load a Python module into KlongPy:
+
+```bash
+$ rlwrap kgpy
+
+Welcome to KlongPy REPL v0.3.76
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
+
+?> .py("math")
+1
+?> sqrt(64)
+8.0
+```
+
+## Loading Custom Python Modules
+
+Custom modules can be written for KlongPy in the same way as any Python module, the main
+difference is that they don't need to be installed (e.g. via pip).
+
+Simply create a directory with a __init__.py and appropriate files, as in:
+
+
+```Python
+# __init__.py
+from .hello_world import hello
+```
+
+```Python
+# hello_world.py
+
+def hello():
+    return "world!"
+
+def not_exported():
+    raise RuntimeError()
+```
+
+Now, you can import the module with the .py command and run the "hello" function.
+
+```bash
+$ rlwrap kgpy
+
+Welcome to KlongPy REPL v0.3.76
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
+
+?> .py("tests/plugins/greetings")
+1
+?> hello()
+world!
+```
+
+
 # Pandas DataFrame integration
 
 This a work in progress, but it's very interesting to think about what DataFrames look like in Klong since they are basically a dictionary of columns.
 
 For now, the following works where we convert a DataFrame into a dictionary of columns:
 
 ```Python
@@ -373,15 +433,20 @@
 * Additional tests to
     * ensure proper vectorization
     * increase Klong grammar coverage
 * Make REPL (kgpy) compatible with original Klong (kg) REPL
 
 # Differences from Klong
 
-The main difference between Klong and KlongPy is that KlongPy doesn't infinite precision because it's backed by NumPy which is restricted to doubles.
+While KlongPy aims to be 100% compatible with Klong language, the KlongPy system has different goals:
+
+    * Infinite precision: The main difference in this implementation of Klong is the lack of infinite precision.  By using NumPy we are restricted to doubles.
+    * Python integration: Most notably, the ".py" command allows direct import of Python modules into the current Klong context.
+    * IPC - KlongPy will support IPC between KlongPy processes, allowing one KlongPy process to interact with other KlongPy processes over the network.
+
 
 # Running tests
 
 ```bash
 python3 -m unittest
 ```
```

### Comparing `klongpy-0.3.76/README.md` & `klongpy-0.3.77/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -198,14 +198,74 @@
 ```
 outputs
 ```
 called from KlongPy: 2018-06-21 00:00:00
 called from KlongPy: {'timestamp': datetime.datetime(2018, 6, 21, 0, 0)}
 ```
 
+## Loading Python Modules directly into KlongPy
+
+KlongPy has the powerful ability to load Python modules directly. This can be extremely useful when you want to utilize the functionality offered by various Python libraries, and seamlessly integrate them into your KlongPy programs.
+
+Here is an example of how you can load a Python module into KlongPy:
+
+```bash
+$ rlwrap kgpy
+
+Welcome to KlongPy REPL v0.3.76
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
+
+?> .py("math")
+1
+?> sqrt(64)
+8.0
+```
+
+## Loading Custom Python Modules
+
+Custom modules can be written for KlongPy in the same way as any Python module, the main
+difference is that they don't need to be installed (e.g. via pip).
+
+Simply create a directory with a __init__.py and appropriate files, as in:
+
+
+```Python
+# __init__.py
+from .hello_world import hello
+```
+
+```Python
+# hello_world.py
+
+def hello():
+    return "world!"
+
+def not_exported():
+    raise RuntimeError()
+```
+
+Now, you can import the module with the .py command and run the "hello" function.
+
+```bash
+$ rlwrap kgpy
+
+Welcome to KlongPy REPL v0.3.76
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
+
+?> .py("tests/plugins/greetings")
+1
+?> hello()
+world!
+```
+
+
 # Pandas DataFrame integration
 
 This a work in progress, but it's very interesting to think about what DataFrames look like in Klong since they are basically a dictionary of columns.
 
 For now, the following works where we convert a DataFrame into a dictionary of columns:
 
 ```Python
@@ -352,15 +412,20 @@
 * Additional tests to
     * ensure proper vectorization
     * increase Klong grammar coverage
 * Make REPL (kgpy) compatible with original Klong (kg) REPL
 
 # Differences from Klong
 
-The main difference between Klong and KlongPy is that KlongPy doesn't infinite precision because it's backed by NumPy which is restricted to doubles.
+While KlongPy aims to be 100% compatible with Klong language, the KlongPy system has different goals:
+
+    * Infinite precision: The main difference in this implementation of Klong is the lack of infinite precision.  By using NumPy we are restricted to doubles.
+    * Python integration: Most notably, the ".py" command allows direct import of Python modules into the current Klong context.
+    * IPC - KlongPy will support IPC between KlongPy processes, allowing one KlongPy process to interact with other KlongPy processes over the network.
+
 
 # Running tests
 
 ```bash
 python3 -m unittest
 ```
```

### Comparing `klongpy-0.3.76/klongpy/adverbs.py` & `klongpy-0.3.77/klongpy/adverbs.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/klongpy/backend.py` & `klongpy-0.3.77/klongpy/backend.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/klongpy/core.py` & `klongpy-0.3.77/klongpy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,23 +327,22 @@
 def rec_flatten(a):
     if is_list(a) and len(a) > 0:
         return np.concatenate([rec_flatten(x) if is_list(x) else np.array([x]) for x in a]).ravel()
     return a
 
 
 def rec_fn(a,f):
-    return np.asarray([rec_fn(x, f) for x in a], dtype=object) if is_list(a) else f(a)
+    return kg_asarray([rec_fn(x, f) for x in a]) if is_list(a) else f(a)
 
 
 def vec_fn(a, f):
-    """apply vector function to array with nested array support"""
-    # dtype == O for heterogeneous (nested) arrays otherwise apply the function directly for vectorization perf
-    if np.isarray(a) and a.dtype == 'O':
-        return np.asarray([((vec_fn(x, f)) if is_list(x) else f(x)) for x in a] if is_list(a) else f(a), dtype=object)
-    return f(a)
+    """
+    Apply a function `f` to an array `a`, with support for both nested arrays and direct vectorized operation.
+    """
+    return kg_asarray([((vec_fn(x, f)) if is_list(x) else f(x)) for x in a]) if np.isarray(a) and a.dtype == 'O' else f(a)
 
 
 def vec_fn2(a, b, f):
     """
     Apply function `f` recursively to the elements of `a` and `b`, which can be scalar values, vectors, or nested vectors.
 
     This function distinguishes 8 cases based on the types and dimensions of `a` and `b`:
@@ -377,18 +376,20 @@
     This function assumes that `f` can handle the types and dimensions of `a` and `b`, and that `a` and `b` have the same 
     shape if they are arrays. It does not check these conditions, so unexpected results or errors may occur if they are 
     not satisfied.
     """
     if np.isarray(a):
         if a.dtype == 'O':
             if np.isarray(b):
+                assert len(a) == len(b)
                 return kg_asarray([vec_fn2(x, y, f) for x,y in zip(a,b)])
             else:
                 return kg_asarray([vec_fn2(x, b, f) for x in a])
         elif np.isarray(b) and b.dtype == 'O':
+            assert len(a) == len(b)
             return kg_asarray([vec_fn2(x, y, f) for x,y in zip(a,b)])
     elif np.isarray(b) and b.dtype == 'O':
         return kg_asarray([vec_fn2(a, x, f) for x in b])
     return f(a,b)
 
 
 def is_symbolic(c):
```

### Comparing `klongpy-0.3.76/klongpy/dyads.py` & `klongpy-0.3.77/klongpy/dyads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/klongpy/interpreter.py` & `klongpy-0.3.77/klongpy/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,15 +579,16 @@
         assert r == 2
 
         or more succinctly
 
         assert 2 == KlongInterpreter()("1+1")
 
         """
-        return self.exec(x)[-1]
+        r = self.exec(x)
+        return r[-1] if r else None
 
     def exec(self, x):
         """
         Execute a Klong program.
 
         Each subprogram is executed in order and the resulting array contains the resulst of each sub-program.
         """
```

### Comparing `klongpy-0.3.76/klongpy/monads.py` & `klongpy-0.3.77/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/klongpy/sys_fn.py` & `klongpy-0.3.77/klongpy/sys_fn.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 import errno
+import importlib.util
 import os
 import random
 import subprocess
 import sys
 import time
 
 from .core import KGChannel, KGChannelDir, is_empty, kg_read, kg_write, safe_eq
@@ -157,33 +158,44 @@
         (without a prefix from KLONGPATH) by starting "x" with a "/"
         or "." character.
 
         .l will return the last expression evaluated, i.e. it can be
         used to load the value of a single expression from a file.
 
     """
-    if os.path.exists(x):
-        try:
-            # TODO: support path defaults as mentioned above
-            with open(x, "r") as f:
-                # This is a "hack" to keep the load operation in the same context it was called in
-                #   The interpeter pushes a context when it calls a function, so here
-                #   we pop it, run the load in the original context, and push the context back on
-                #   so that the interpreter can pop it's temporary context off as normal.
-                ctx = klong._context.pop()
-                try:
-                    r = klong(f.read())
-                finally:
-                    klong._context.push(ctx)
-                return r
-        except IOError:
-            raise RuntimeError("file could not be opened: {x}")
-    else:
+    # if not (os.path.isfile(x) or os.path.isfile(os.path.join(x,".kg"))):
+    alt_dirs = str((os.environ.get('KLONGPATH') or ".:lib")).split(':')
+    for ad in alt_dirs:
+        adx = os.path.join(ad,x)
+        if os.path.isfile(adx):
+            x = adx
+            break
+        adx = os.path.join(adx,".kg")
+        if os.path.isfile(adx):
+            x = adx
+            break
+
+    if not os.path.isfile(x):
         raise FileNotFoundError("file does not exist: {x}")
 
+    try:
+        with open(x, "r") as f:
+            # This is a "hack" to keep the load operation in the same context it was called in
+            #   The interpeter pushes a context when it calls a function, so here
+            #   we pop it, run the load in the original context, and push the context back on
+            #   so that the interpreter can pop it's temporary context off as normal.
+            ctx = klong._context.pop()
+            try:
+                r = klong(f.read())
+            finally:
+                klong._context.push(ctx)
+            return r
+    except IOError:
+        raise RuntimeError("file could not be opened: {x}")
+
 
 def eval_sys_more_input(klong):
     """
 
         .mi(x)                                              [More-Input]
 
         This function returns 1, if the From Channel is not exhausted
@@ -256,14 +268,101 @@
 
     """
     o = str(x)
     klong['.sys.cout'].raw.write(o+"\n")
     return o
 
 
+def eval_sys_python(klong, x):
+    """
+    
+        .py(x)                                                    [Python]
+
+        Import a python module in to the current context.  All methods exposed in the module
+        are loaded into the current context space and callable from within KlongPy.
+    
+        If the string "x" refers to a directory, KlongPy will append __init__.py 
+        to determine if the directory is a Python module and attempt to load the module.
+          
+        If the string "x" ends with a .py, then KlongPy will attempt to load this file
+        as a Python module.
+
+        Example:
+
+            Consider a python module called Greetings that exports the "hello" method such as:
+
+                def hello():
+                    print("Hello, World!")
+
+            The following will load the "greetings" module from the Python modules in the same 
+            way that 'import hello' would do.  Then we can call 'hello'
+
+                .py("greetings")
+                hello() --> "Hello, World!"
+             
+            Additionally, a full path to a module can be specified.  This can be useful for 
+            when creating custom modules that don't need to be installed into Python modules.
+
+                .py("<path>/<to>/greetings")            
+
+    """
+    if os.path.isdir(x) or x.endswith("__init__.py"):
+        x = os.path.realpath(x)
+        if x.endswith("__init__.py"):
+            x = os.path.dirname(x)
+        if os.path.isfile(os.path.join(x,"__init__.py")):
+            module = None
+            try:
+                pardir = os.path.dirname(x)
+                sys.path.insert(0,pardir)
+                module_name = os.path.basename(os.path.normpath(x))
+                module = importlib.import_module(module_name)
+            except Exception as e:
+                print(e)
+                raise e
+            finally:
+                sys.path.pop(0)
+        else:
+            raise FileNotFoundError("Not a valid Python module (missing __init__.py): {x}")
+    elif os.path.isfile(x):
+        module_name = os.path.dirname(x)
+        location = x
+        spec = importlib.util.spec_from_file_location(module_name, location=location)
+        module = importlib.util.module_from_spec(spec)
+        try:
+            spec.loader.exec_module(module)
+        except Exception as e:
+            print(e)
+            raise RuntimeError("module could not be imported: {x}")
+    else:
+        if (spec := importlib.util.find_spec(x)) is not None:
+            module = importlib.util.module_from_spec(spec)
+            try:
+                spec.loader.exec_module(module)
+            except Exception as e:
+                print(e)
+                raise RuntimeError("module could not be imported: {x}")
+    try:
+        import_items = filter(lambda p: not p[0].startswith("__"), module.__dict__.items())
+        if import_items is not None:
+            ctx = klong._context.pop()
+            try:
+                for p,q in import_items:
+                    try:
+                        klong[p] = q
+                    except Exception as e:
+                        print(e)
+            finally:
+                klong._context.push(ctx)
+            return 1
+    except Exception as e:
+        print(e)
+        raise RuntimeError("failed to load module: {x}")
+
+
 def eval_sys_random_number():
     """
 
         .rn()                                            [Random-Number]
 
         Return a random number x, such that 0 <= x < 1.
```

### Comparing `klongpy-0.3.76/klongpy/sys_var.py` & `klongpy-0.3.77/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/klongpy/utils.py` & `klongpy-0.3.77/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/klongpy.egg-info/PKG-INFO` & `klongpy-0.3.77/klongpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.76
+Version: 0.3.77
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -219,14 +219,74 @@
 ```
 outputs
 ```
 called from KlongPy: 2018-06-21 00:00:00
 called from KlongPy: {'timestamp': datetime.datetime(2018, 6, 21, 0, 0)}
 ```
 
+## Loading Python Modules directly into KlongPy
+
+KlongPy has the powerful ability to load Python modules directly. This can be extremely useful when you want to utilize the functionality offered by various Python libraries, and seamlessly integrate them into your KlongPy programs.
+
+Here is an example of how you can load a Python module into KlongPy:
+
+```bash
+$ rlwrap kgpy
+
+Welcome to KlongPy REPL v0.3.76
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
+
+?> .py("math")
+1
+?> sqrt(64)
+8.0
+```
+
+## Loading Custom Python Modules
+
+Custom modules can be written for KlongPy in the same way as any Python module, the main
+difference is that they don't need to be installed (e.g. via pip).
+
+Simply create a directory with a __init__.py and appropriate files, as in:
+
+
+```Python
+# __init__.py
+from .hello_world import hello
+```
+
+```Python
+# hello_world.py
+
+def hello():
+    return "world!"
+
+def not_exported():
+    raise RuntimeError()
+```
+
+Now, you can import the module with the .py command and run the "hello" function.
+
+```bash
+$ rlwrap kgpy
+
+Welcome to KlongPy REPL v0.3.76
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
+
+?> .py("tests/plugins/greetings")
+1
+?> hello()
+world!
+```
+
+
 # Pandas DataFrame integration
 
 This a work in progress, but it's very interesting to think about what DataFrames look like in Klong since they are basically a dictionary of columns.
 
 For now, the following works where we convert a DataFrame into a dictionary of columns:
 
 ```Python
@@ -373,15 +433,20 @@
 * Additional tests to
     * ensure proper vectorization
     * increase Klong grammar coverage
 * Make REPL (kgpy) compatible with original Klong (kg) REPL
 
 # Differences from Klong
 
-The main difference between Klong and KlongPy is that KlongPy doesn't infinite precision because it's backed by NumPy which is restricted to doubles.
+While KlongPy aims to be 100% compatible with Klong language, the KlongPy system has different goals:
+
+    * Infinite precision: The main difference in this implementation of Klong is the lack of infinite precision.  By using NumPy we are restricted to doubles.
+    * Python integration: Most notably, the ".py" command allows direct import of Python modules into the current Klong context.
+    * IPC - KlongPy will support IPC between KlongPy processes, allowing one KlongPy process to interact with other KlongPy processes over the network.
+
 
 # Running tests
 
 ```bash
 python3 -m unittest
 ```
```

### Comparing `klongpy-0.3.76/klongpy.egg-info/SOURCES.txt` & `klongpy-0.3.77/klongpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/scripts/kgpy` & `klongpy-0.3.77/scripts/kgpy`

 * *Files 6% similar despite different names*

```diff
@@ -129,45 +129,49 @@
 
         For one iteration, it's possible this Klong timeit is more accurate than the native Python timeit due to overhead.
 
         Note: Added in KlongPy.
 
     """
     n = int(cmd[3:cmd.index(" ")]) if cmd[2] == ":" else 1
-    return timeit.timeit(lambda k=klong,p=cmd[cmd.index(" "):]: k(p), number=n)
+    prog = klong.prog(cmd[cmd.index(" "):])
+    r = timeit.timeit(lambda k=klong,p=prog: k.eval(p), number=n)
+    return f"total: {r} per: {r/n}"
 
 
 def create_sys_cmd_functions():
     def _get_name(s):
         s = s.strip()
         x = s.index(']')+1
         return s[x:x+1]
 
     registry = {}
 
     m = sys.modules[__name__]
     for x in filter(lambda n: n.startswith("sys_cmd_"), dir(m)):
         fn = getattr(m,x)
         name = _get_name(fn.__doc__)
-        registry[name] = fn
+        registry[name] = fn 
 
     return registry
 
 
 success = lambda input: f"{Fore.GREEN}{input}"
 failure = lambda input: f"{Fore.RED}{input}"
 
 
-def repl_eval(klong, p):
+def repl_eval(klong, p, verbose=False):
     try:
-        r = success(klong(p))
+        r = klong(p)
+        r = r if r is None else success(r)
     except Exception as e:
         r = failure(f"Error: {e.args}")
-        import traceback
-        traceback.print_exc(e)
+        if verbose:
+            import traceback
+            traceback.print_exc(e)
     return r
 
 
 # https://dev.to/amal/building-the-python-repl-3468
 def repl(klong=None):
 
     print()
```

### Comparing `klongpy-0.3.76/setup.py` & `klongpy-0.3.77/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
     packages=['klongpy'],
-    version='0.3.76',
+    version='0.3.77',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `klongpy-0.3.76/tests/test_accel.py` & `klongpy-0.3.77/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/tests/test_examples.py` & `klongpy-0.3.77/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/tests/test_extra_suite.py` & `klongpy-0.3.77/tests/test_extra_suite.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 # add tests not included in the original kg suite
 class TestExtraCoreSuite(unittest.TestCase):
 
     def assert_eval_cmp(self, a, b, klong=None):
         self.assertTrue(eval_cmp(a, b, klong=klong))
 
+    def test_eval_quote_string(self):
+        klong = KlongInterpreter()
+        r = klong(':"hello"')
+        self.assertTrue(r is None)
+
     def test_array_identity(self):
         klong = KlongInterpreter()
         r = klong('[]')
         self.assertTrue(kg_equal(r, np.array([],dtype=object)))
         r = klong('[1]')
         self.assertTrue(kg_equal(r, np.array([1],dtype=object)))
         r = klong('[[1]]')
```

### Comparing `klongpy-0.3.76/tests/test_fn.py` & `klongpy-0.3.77/tests/test_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/tests/test_interop.py` & `klongpy-0.3.77/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/tests/test_join_over.py` & `klongpy-0.3.77/tests/test_join_over.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/tests/test_prog.py` & `klongpy-0.3.77/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/tests/test_suite.py` & `klongpy-0.3.77/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/tests/test_suite_file.py` & `klongpy-0.3.77/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.76/tests/test_sys_fn.py` & `klongpy-0.3.77/tests/test_sys_fn.py`

 * *Files 12% similar despite different names*

```diff
@@ -206,14 +206,47 @@
                 self.assertEqual(r, f"{expected}\n")
 
     def test_sys_print_result(self):
         klong = KlongInterpreter()
         r = klong(".p(1)")
         self.assertEqual(r,"1")
 
+    def test_sys_python_load_module(self):
+        klong = KlongInterpreter()
+        r = klong(f'.py("math")')
+        self.assertEqual(r,1)
+        r = klong('sqrt(64)')
+        self.assertEqual(r,8)
+
+    def test_sys_python_load_custom_module(self):
+        tests_dir = os.path.dirname(os.path.abspath(__file__))
+        plugins_dir = os.path.join(tests_dir, "plugins")
+        tests = []
+        tests.append(os.path.join("tests", os.path.join("plugins", "greetings")))
+        tests.append(os.path.join(plugins_dir, "greetings"))
+        tests.append(os.path.join(plugins_dir, "greetings/__init__.py"))
+        tests.append(os.path.join(plugins_dir, "greetings/hello_world.py"))
+        tests.append("greetings")
+        try:
+            sys.path.append(plugins_dir)
+            for fpath in tests:
+                klong = KlongInterpreter()
+                r = klong(f'.py("{fpath}")')
+                self.assertEqual(r,1)
+                r = klong('hello()')
+                self.assertEqual(r,"world!")
+                if fpath.endswith("hello_world.py"):
+                    r = klong['not_exported']
+                    self.assertTrue(r is not None)
+                else:
+                    with self.assertRaises(KeyError):
+                        klong['not_exported']
+        finally:
+            sys.path.pop()
+
     def test_eval_sys_random_number(self):
         r = eval_sys_random_number()
         r2 = eval_sys_random_number()
         i = 0
         while r == r2 and i < 3:
             i += 1
             r2 = eval_sys_random_number()
```

### Comparing `klongpy-0.3.76/tests/test_util.py` & `klongpy-0.3.77/tests/test_util.py`

 * *Files identical despite different names*

