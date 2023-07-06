# Comparing `tmp/klongpy-0.3.77.tar.gz` & `tmp/klongpy-0.3.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.3.77.tar", last modified: Thu Jul  6 15:05:25 2023, max compression
+gzip compressed data, was "klongpy-0.3.78.tar", last modified: Thu Jul  6 16:14:57 2023, max compression
```

## Comparing `klongpy-0.3.77.tar` & `klongpy-0.3.78.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.77/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    12794 2023-07-06 15:05:25.731818 klongpy-0.3.77/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    12259 2023-07-06 15:05:05.000000 klongpy-0.3.77/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.77/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.3.77/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.3.77/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    25901 2023-07-06 15:05:05.000000 klongpy-0.3.77/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30733 2023-06-30 23:35:49.000000 klongpy-0.3.77/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20366 2023-07-06 15:05:05.000000 klongpy-0.3.77/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.3.77/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    15564 2023-07-06 15:05:05.000000 klongpy-0.3.77/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.77/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.77/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    12794 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-06 15:05:25.000000 klongpy-0.3.77/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6736 2023-07-06 15:05:05.000000 klongpy-0.3.77/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-06 15:05:25.731818 klongpy-0.3.77/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-07-06 15:05:05.000000 klongpy-0.3.77/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 15:05:25.731818 klongpy-0.3.77/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.3.77/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.77/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    23466 2023-07-06 15:05:05.000000 klongpy-0.3.77/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.3.77/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.3.77/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.3.77/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.77/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.77/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.77/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    13888 2023-07-06 15:05:05.000000 klongpy-0.3.77/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.3.77/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.452793 klongpy-0.3.78/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.78/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12794 2023-07-06 16:14:57.452793 klongpy-0.3.78/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12259 2023-07-06 15:05:05.000000 klongpy-0.3.78/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.448794 klongpy-0.3.78/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.78/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.3.78/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.3.78/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    25913 2023-07-06 16:14:39.000000 klongpy-0.3.78/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30733 2023-06-30 23:35:49.000000 klongpy-0.3.78/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20366 2023-07-06 15:05:05.000000 klongpy-0.3.78/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.3.78/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    16345 2023-07-06 16:14:39.000000 klongpy-0.3.78/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.78/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.78/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.448794 klongpy-0.3.78/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12794 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.448794 klongpy-0.3.78/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6736 2023-07-06 15:05:05.000000 klongpy-0.3.78/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-06 16:14:57.452793 klongpy-0.3.78/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-07-06 16:14:39.000000 klongpy-0.3.78/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.452793 klongpy-0.3.78/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.3.78/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.78/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    23466 2023-07-06 15:05:05.000000 klongpy-0.3.78/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.3.78/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.3.78/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.3.78/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.78/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.78/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.78/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    13952 2023-07-06 16:14:39.000000 klongpy-0.3.78/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.3.78/tests/test_util.py
```

### Comparing `klongpy-0.3.77/LICENSE` & `klongpy-0.3.78/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/PKG-INFO` & `klongpy-0.3.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.77
+Version: 0.3.78
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `klongpy-0.3.77/README.md` & `klongpy-0.3.78/README.md`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/klongpy/adverbs.py` & `klongpy-0.3.78/klongpy/adverbs.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/klongpy/backend.py` & `klongpy-0.3.78/klongpy/backend.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/klongpy/core.py` & `klongpy-0.3.78/klongpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,23 +94,24 @@
 
     lambda x,y: x + y
     lambda klong, x: klong(x)
 
     """
     def __init__(self, fn):
         self.fn = fn
-        self.args = inspect.signature(self.fn, follow_wrapped=True).parameters
-        self.provide_klong = 'klong' in self.args
+        params = inspect.signature(self.fn, follow_wrapped=True).parameters
+        self.args = [x for x in params if x in reserved_fn_args]
+        self.provide_klong = 'klong' in params
 
     def __call__(self, klong, ctx):
-        params = [ctx[reserved_fn_symbol_map[x]] for x in reserved_fn_args if x in self.args]
+        params = [ctx[reserved_fn_symbol_map[x]] for x in reserved_fn_args[:len(self.args)]]
         return self.fn(klong, *params) if self.provide_klong else self.fn(*params)
 
     def get_arity(self):
-        return len(self.args) - 1 if self.provide_klong else len(self.args)
+        return len(self.args)
 
 
 class KGChannelDir(Enum):
     INPUT=1
     OUTPUT=2
```

### Comparing `klongpy-0.3.77/klongpy/dyads.py` & `klongpy-0.3.78/klongpy/dyads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/klongpy/interpreter.py` & `klongpy-0.3.78/klongpy/interpreter.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/klongpy/monads.py` & `klongpy-0.3.78/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/klongpy/sys_fn.py` & `klongpy-0.3.78/klongpy/sys_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import importlib.util
 import os
 import random
 import subprocess
 import sys
 import time
 
-from .core import KGChannel, KGChannelDir, is_empty, kg_read, kg_write, safe_eq
+from .core import KGChannel, KGChannelDir, is_empty, kg_read, kg_write, safe_eq, reserved_fn_args
 
 
 def eval_sys_append_channel(x):
     """
 
         .ac(x)                                          [Append-Channel]
 
@@ -342,16 +342,30 @@
                 print(e)
                 raise RuntimeError("module could not be imported: {x}")
     try:
         import_items = filter(lambda p: not p[0].startswith("__"), module.__dict__.items())
         if import_items is not None:
             ctx = klong._context.pop()
             try:
+                import inspect
+
                 for p,q in import_items:
                     try:
+                        args = inspect.signature(q, follow_wrapped=True).parameters
+                        if len(args) > len(reserved_fn_args):
+                            print("skipping {p} - too many paramters {len(args)}")
+                        if reserved_fn_args[0] not in args:
+                            print("remapping {p} using reserved parameter names")
+                            n_args = len(args)
+                            if n_args == 3:
+                                q = lambda x,y,z,f=q: f(x,y,z)
+                            elif n_args == 2:
+                                q = lambda x,y,f=q: f(x,y)
+                            elif n_args == 1:
+                                q = lambda x,f=q: f(x)
                         klong[p] = q
                     except Exception as e:
                         print(e)
             finally:
                 klong._context.push(ctx)
             return 1
     except Exception as e:
```

### Comparing `klongpy-0.3.77/klongpy/sys_var.py` & `klongpy-0.3.78/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/klongpy/utils.py` & `klongpy-0.3.78/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/klongpy.egg-info/PKG-INFO` & `klongpy-0.3.78/klongpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.77
+Version: 0.3.78
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `klongpy-0.3.77/klongpy.egg-info/SOURCES.txt` & `klongpy-0.3.78/klongpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/scripts/kgpy` & `klongpy-0.3.78/scripts/kgpy`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/setup.py` & `klongpy-0.3.78/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
     packages=['klongpy'],
-    version='0.3.77',
+    version='0.3.78',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `klongpy-0.3.77/tests/test_accel.py` & `klongpy-0.3.78/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_examples.py` & `klongpy-0.3.78/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_extra_suite.py` & `klongpy-0.3.78/tests/test_extra_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_fn.py` & `klongpy-0.3.78/tests/test_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_interop.py` & `klongpy-0.3.78/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_join_over.py` & `klongpy-0.3.78/tests/test_join_over.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_prog.py` & `klongpy-0.3.78/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_suite.py` & `klongpy-0.3.78/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_suite_file.py` & `klongpy-0.3.78/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.77/tests/test_sys_fn.py` & `klongpy-0.3.78/tests/test_sys_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,16 @@
 
     def test_sys_python_load_module(self):
         klong = KlongInterpreter()
         r = klong(f'.py("math")')
         self.assertEqual(r,1)
         r = klong('sqrt(64)')
         self.assertEqual(r,8)
+        r = klong('fsum(1+!10)')
+        self.assertEqual(r,55)
 
     def test_sys_python_load_custom_module(self):
         tests_dir = os.path.dirname(os.path.abspath(__file__))
         plugins_dir = os.path.join(tests_dir, "plugins")
         tests = []
         tests.append(os.path.join("tests", os.path.join("plugins", "greetings")))
         tests.append(os.path.join(plugins_dir, "greetings"))
```

### Comparing `klongpy-0.3.77/tests/test_util.py` & `klongpy-0.3.78/tests/test_util.py`

 * *Files identical despite different names*

