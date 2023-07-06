# Comparing `tmp/httptools-0.5.0.tar.gz` & `tmp/httptools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httptools-0.5.0.tar", last modified: Tue Sep 13 05:00:03 2022, max compression
+gzip compressed data, was "httptools-0.6.0.tar", last modified: Thu Jul  6 21:29:56 2023, max compression
```

## Comparing `httptools-0.5.0.tar` & `httptools-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.426337 httptools-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-09-13 04:59:51.000000 httptools-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-13 04:59:51.000000 httptools-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-09-13 05:00:03.426337 httptools-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-09-13 04:59:51.000000 httptools-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.422337 httptools-0.5.0/httptools/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-13 04:59:51.000000 httptools-0.5.0/httptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-13 04:59:51.000000 httptools-0.5.0/httptools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.422337 httptools-0.5.0/httptools/parser/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-13 04:59:51.000000 httptools-0.5.0/httptools/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-09-13 04:59:51.000000 httptools-0.5.0/httptools/parser/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)   404509 2022-09-13 05:00:03.000000 httptools-0.5.0/httptools/parser/parser.c
--rw-r--r--   0 runner    (1001) docker     (121)   240897 2022-09-13 05:00:03.000000 httptools-0.5.0/httptools/parser/url_parser.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.422337 httptools-0.5.0/httptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-09-13 05:00:01.000000 httptools-0.5.0/httptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-09-13 05:00:03.000000 httptools-0.5.0/httptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 05:00:01.000000 httptools-0.5.0/httptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 05:00:01.000000 httptools-0.5.0/httptools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-13 05:00:01.000000 httptools-0.5.0/httptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-13 05:00:01.000000 httptools-0.5.0/httptools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-13 05:00:03.426337 httptools-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7252 2022-09-13 04:59:51.000000 httptools-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.418337 httptools-0.5.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.422337 httptools-0.5.0/vendor/http-parser/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-09-13 04:59:54.000000 httptools-0.5.0/vendor/http-parser/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (121)     9343 2022-09-13 04:59:54.000000 httptools-0.5.0/vendor/http-parser/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3786 2022-09-13 04:59:54.000000 httptools-0.5.0/vendor/http-parser/bench.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.422337 httptools-0.5.0/vendor/http-parser/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)     4188 2022-09-13 04:59:54.000000 httptools-0.5.0/vendor/http-parser/contrib/parsertrace.c
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-09-13 04:59:54.000000 httptools-0.5.0/vendor/http-parser/contrib/url_parser.c
--rw-r--r--   0 runner    (1001) docker     (121)    75384 2022-09-13 04:59:54.000000 httptools-0.5.0/vendor/http-parser/http_parser.c
--rw-r--r--   0 runner    (1001) docker     (121)    19257 2022-09-13 04:59:54.000000 httptools-0.5.0/vendor/http-parser/http_parser.h
--rw-r--r--   0 runner    (1001) docker     (121)   123291 2022-09-13 04:59:54.000000 httptools-0.5.0/vendor/http-parser/test.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.426337 httptools-0.5.0/vendor/llhttp/
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-09-13 04:59:56.000000 httptools-0.5.0/vendor/llhttp/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2022-09-13 04:59:56.000000 httptools-0.5.0/vendor/llhttp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.426337 httptools-0.5.0/vendor/llhttp/include/
--rw-r--r--   0 runner    (1001) docker     (121)    16416 2022-09-13 04:59:56.000000 httptools-0.5.0/vendor/llhttp/include/llhttp.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 05:00:03.426337 httptools-0.5.0/vendor/llhttp/src/
--rw-r--r--   0 runner    (1001) docker     (121)     9664 2022-09-13 04:59:56.000000 httptools-0.5.0/vendor/llhttp/src/api.c
--rw-r--r--   0 runner    (1001) docker     (121)     4542 2022-09-13 04:59:56.000000 httptools-0.5.0/vendor/llhttp/src/http.c
--rw-r--r--   0 runner    (1001) docker     (121)   467598 2022-09-13 04:59:56.000000 httptools-0.5.0/vendor/llhttp/src/llhttp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.134668 httptools-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-06 21:29:45.000000 httptools-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 21:29:45.000000 httptools-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-06 21:29:56.134668 httptools-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-06 21:29:45.000000 httptools-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.130668 httptools-0.6.0/httptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-06 21:29:45.000000 httptools-0.6.0/httptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-06 21:29:45.000000 httptools-0.6.0/httptools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.130668 httptools-0.6.0/httptools/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 21:29:45.000000 httptools-0.6.0/httptools/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-06 21:29:45.000000 httptools-0.6.0/httptools/parser/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   406227 2023-07-06 21:29:55.000000 httptools-0.6.0/httptools/parser/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)   242528 2023-07-06 21:29:56.000000 httptools-0.6.0/httptools/parser/url_parser.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.130668 httptools-0.6.0/httptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-06 21:29:53.000000 httptools-0.6.0/httptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 21:29:56.000000 httptools-0.6.0/httptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:29:53.000000 httptools-0.6.0/httptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:29:53.000000 httptools-0.6.0/httptools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 21:29:53.000000 httptools-0.6.0/httptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 21:29:53.000000 httptools-0.6.0/httptools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:29:56.134668 httptools-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-07-06 21:29:45.000000 httptools-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.130668 httptools-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-07-06 21:29:45.000000 httptools-0.6.0/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.126668 httptools-0.6.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.130668 httptools-0.6.0/vendor/http-parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 21:29:46.000000 httptools-0.6.0/vendor/http-parser/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-07-06 21:29:46.000000 httptools-0.6.0/vendor/http-parser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-06 21:29:46.000000 httptools-0.6.0/vendor/http-parser/bench.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.134668 httptools-0.6.0/vendor/http-parser/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-06 21:29:46.000000 httptools-0.6.0/vendor/http-parser/contrib/parsertrace.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-06 21:29:46.000000 httptools-0.6.0/vendor/http-parser/contrib/url_parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)    75384 2023-07-06 21:29:46.000000 httptools-0.6.0/vendor/http-parser/http_parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-07-06 21:29:46.000000 httptools-0.6.0/vendor/http-parser/http_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)   123291 2023-07-06 21:29:46.000000 httptools-0.6.0/vendor/http-parser/test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.134668 httptools-0.6.0/vendor/llhttp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-06 21:29:48.000000 httptools-0.6.0/vendor/llhttp/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 21:29:48.000000 httptools-0.6.0/vendor/llhttp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.134668 httptools-0.6.0/vendor/llhttp/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    26812 2023-07-06 21:29:48.000000 httptools-0.6.0/vendor/llhttp/include/llhttp.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:29:56.134668 httptools-0.6.0/vendor/llhttp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-06 21:29:48.000000 httptools-0.6.0/vendor/llhttp/src/api.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-06 21:29:48.000000 httptools-0.6.0/vendor/llhttp/src/http.c
+-rw-r--r--   0 runner    (1001) docker     (123)   568827 2023-07-06 21:29:48.000000 httptools-0.6.0/vendor/llhttp/src/llhttp.c
```

### Comparing `httptools-0.5.0/LICENSE` & `httptools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/PKG-INFO` & `httptools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httptools
-Version: 0.5.0
+Version: 0.6.0
 Summary: A collection of framework independent HTTP protocol utils.
 Home-page: https://github.com/MagicStack/httptools
 Author: Yury Selivanov
 Author-email: yury@magic.io
 License: MIT
 Platform: macOS
 Platform: POSIX
```

### Comparing `httptools-0.5.0/README.md` & `httptools-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/httptools/_version.py` & `httptools-0.6.0/httptools/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 # The commit message MUST contain a properly formatted release
 # log, and the commit must be signed.
 #
 # The release automation will: build and test the packages for the
 # supported platforms, publish the packages on PyPI, merge the PR
 # to the target branch, create a Git tag pointing to the commit.
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
```

### Comparing `httptools-0.5.0/httptools/parser/errors.py` & `httptools-0.6.0/httptools/parser/errors.py`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/httptools/parser/parser.c` & `httptools-0.6.0/httptools/parser/parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O2"
@@ -21,16 +21,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,24 +90,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -215,15 +219,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -254,15 +258,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -377,17 +381,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -457,14 +458,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -564,35 +570,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -969,17 +975,17 @@
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "httptools/parser/parser.pyx",
   "stringsource",
-  ".eggs/Cython-0.29.32-py3.10-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
-  ".eggs/Cython-0.29.32-py3.10-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd",
-  ".eggs/Cython-0.29.32-py3.10-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd",
+  ".eggs/Cython-0.29.36-py3.11.egg/Cython/Includes/cpython/type.pxd",
+  ".eggs/Cython-0.29.36-py3.11.egg/Cython/Includes/cpython/bool.pxd",
+  ".eggs/Cython-0.29.36-py3.11.egg/Cython/Includes/cpython/complex.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9httptools_6parser_6parser_HttpParser;
 struct __pyx_obj_9httptools_6parser_6parser_HttpRequestParser;
 struct __pyx_obj_9httptools_6parser_6parser_HttpResponseParser;
 
@@ -1298,26 +1304,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1426,22 +1432,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -6961,15 +6975,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_9httptools_6parser_6parser_HttpParser(PyObject *o) {
   struct __pyx_obj_9httptools_6parser_6parser_HttpParser *p = (struct __pyx_obj_9httptools_6parser_6parser_HttpParser *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -7142,15 +7156,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_9httptools_6parser_6parser_HttpRequestParser __pyx_vtable_9httptools_6parser_6parser_HttpRequestParser;
 
 static PyObject *__pyx_tp_new_9httptools_6parser_6parser_HttpRequestParser(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_9httptools_6parser_6parser_HttpRequestParser *p;
@@ -7231,15 +7245,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_9httptools_6parser_6parser_HttpResponseParser __pyx_vtable_9httptools_6parser_6parser_HttpResponseParser;
 
 static PyObject *__pyx_tp_new_9httptools_6parser_6parser_HttpResponseParser(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_9httptools_6parser_6parser_HttpResponseParser *p;
@@ -7320,15 +7334,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -7503,15 +7517,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -7611,32 +7625,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -7821,15 +7832,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_httptools__parser__parser) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8334,15 +8345,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -8615,28 +8626,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -9154,61 +9165,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -9295,15 +9324,15 @@
         #endif
     }
     return value;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -9794,15 +9823,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9990,15 +10019,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `httptools-0.5.0/httptools/parser/url_parser.c` & `httptools-0.6.0/httptools/parser/url_parser.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O2"
@@ -21,16 +21,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,24 +90,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -215,15 +219,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -254,15 +258,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -377,17 +381,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -457,14 +458,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -564,35 +570,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -969,17 +975,17 @@
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "stringsource",
   "httptools/parser/url_parser.pyx",
-  ".eggs/Cython-0.29.32-py3.10-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
-  ".eggs/Cython-0.29.32-py3.10-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd",
-  ".eggs/Cython-0.29.32-py3.10-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd",
+  ".eggs/Cython-0.29.36-py3.11.egg/Cython/Includes/cpython/type.pxd",
+  ".eggs/Cython-0.29.36-py3.11.egg/Cython/Includes/cpython/bool.pxd",
+  ".eggs/Cython-0.29.36-py3.11.egg/Cython/Includes/cpython/complex.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9httptools_6parser_10url_parser_URL;
 
 /* "httptools/parser/url_parser.pyx":16
  * 
@@ -1200,26 +1206,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1294,22 +1300,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -3113,15 +3127,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_9httptools_6parser_10url_parser_URL(PyObject *o) {
   struct __pyx_obj_9httptools_6parser_10url_parser_URL *p = (struct __pyx_obj_9httptools_6parser_10url_parser_URL *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->schema);
   Py_CLEAR(p->host);
   Py_CLEAR(p->port);
@@ -3262,15 +3276,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -3414,15 +3428,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -3486,32 +3500,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -3696,15 +3707,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_httptools__parser__url_parser) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -4339,28 +4350,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -4878,61 +4889,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -5019,15 +5048,15 @@
         #endif
     }
     return value;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -5404,15 +5433,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5600,15 +5629,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `httptools-0.5.0/httptools.egg-info/PKG-INFO` & `httptools-0.6.0/httptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httptools
-Version: 0.5.0
+Version: 0.6.0
 Summary: A collection of framework independent HTTP protocol utils.
 Home-page: https://github.com/MagicStack/httptools
 Author: Yury Selivanov
 Author-email: yury@magic.io
 License: MIT
 Platform: macOS
 Platform: POSIX
```

### Comparing `httptools-0.5.0/httptools.egg-info/SOURCES.txt` & `httptools-0.6.0/httptools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 httptools.egg-info/not-zip-safe
 httptools.egg-info/requires.txt
 httptools.egg-info/top_level.txt
 httptools/parser/__init__.py
 httptools/parser/errors.py
 httptools/parser/parser.c
 httptools/parser/url_parser.c
+tests/test_parser.py
 vendor/http-parser/LICENSE-MIT
 vendor/http-parser/README.md
 vendor/http-parser/bench.c
 vendor/http-parser/http_parser.c
 vendor/http-parser/http_parser.h
 vendor/http-parser/test.c
 vendor/http-parser/contrib/parsertrace.c
```

### Comparing `httptools-0.5.0/setup.py` & `httptools-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/http-parser/LICENSE-MIT` & `httptools-0.6.0/vendor/http-parser/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/http-parser/README.md` & `httptools-0.6.0/vendor/http-parser/README.md`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/http-parser/bench.c` & `httptools-0.6.0/vendor/http-parser/bench.c`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/http-parser/contrib/parsertrace.c` & `httptools-0.6.0/vendor/http-parser/contrib/parsertrace.c`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/http-parser/contrib/url_parser.c` & `httptools-0.6.0/vendor/http-parser/contrib/url_parser.c`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/http-parser/http_parser.c` & `httptools-0.6.0/vendor/http-parser/http_parser.c`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/http-parser/http_parser.h` & `httptools-0.6.0/vendor/http-parser/http_parser.h`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/http-parser/test.c` & `httptools-0.6.0/vendor/http-parser/test.c`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/llhttp/LICENSE-MIT` & `httptools-0.6.0/vendor/llhttp/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/llhttp/src/api.c` & `httptools-0.6.0/vendor/llhttp/src/api.c`

 * *Files 11% similar despite different names*

```diff
@@ -56,34 +56,49 @@
                                   llhttp_should_keep_alive(p));
 }
 
 const llhttp_settings_t wasm_settings = {
   wasm_on_message_begin,
   wasm_on_url,
   wasm_on_status,
+  NULL,
+  NULL,
   wasm_on_header_field,
   wasm_on_header_value,
+  NULL,
+  NULL,
   wasm_on_headers_complete_wrap,
   wasm_on_body,
   wasm_on_message_complete,
   NULL,
   NULL,
+  NULL,
+  NULL,
+  NULL,
+  NULL,
+  NULL,
+  NULL,
+  NULL,
+  NULL,
+  NULL,
 };
 
 
 llhttp_t* llhttp_alloc(llhttp_type_t type) {
   llhttp_t* parser = malloc(sizeof(llhttp_t));
   llhttp_init(parser, type, &wasm_settings);
   return parser;
 }
 
 void llhttp_free(llhttp_t* parser) {
   free(parser);
 }
 
+#endif  // defined(__wasm__)
+
 /* Some getters required to get stuff from the parser */
 
 uint8_t llhttp_get_type(llhttp_t* parser) {
   return parser->type;
 }
 
 uint8_t llhttp_get_http_major(llhttp_t* parser) {
@@ -102,16 +117,14 @@
   return parser->status_code;
 }
 
 uint8_t llhttp_get_upgrade(llhttp_t* parser) {
   return parser->upgrade;
 }
 
-#endif  // defined(__wasm__)
-
 
 void llhttp_reset(llhttp_t* parser) {
   llhttp_type_t type = parser->type;
   const llhttp_settings_t* settings = parser->settings;
   void* data = parser->data;
   uint8_t lenient_flags = parser->lenient_flags;
 
@@ -222,14 +235,23 @@
   switch (method) {
     HTTP_ALL_METHOD_MAP(HTTP_METHOD_GEN)
     default: abort();
   }
 #undef HTTP_METHOD_GEN
 }
 
+const char* llhttp_status_name(llhttp_status_t status) {
+#define HTTP_STATUS_GEN(NUM, NAME, STRING) case HTTP_STATUS_##NAME: return #STRING;
+  switch (status) {
+    HTTP_STATUS_MAP(HTTP_STATUS_GEN)
+    default: abort();
+  }
+#undef HTTP_STATUS_GEN
+}
+
 
 void llhttp_set_lenient_headers(llhttp_t* parser, int enabled) {
   if (enabled) {
     parser->lenient_flags |= LENIENT_HEADERS;
   } else {
     parser->lenient_flags &= ~LENIENT_HEADERS;
   }
@@ -295,14 +317,42 @@
 int llhttp__on_status_complete(llhttp_t* s, const char* p, const char* endp) {
   int err;
   CALLBACK_MAYBE(s, on_status_complete);
   return err;
 }
 
 
+int llhttp__on_method(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  SPAN_CALLBACK_MAYBE(s, on_method, p, endp - p);
+  return err;
+}
+
+
+int llhttp__on_method_complete(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  CALLBACK_MAYBE(s, on_method_complete);
+  return err;
+}
+
+
+int llhttp__on_version(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  SPAN_CALLBACK_MAYBE(s, on_version, p, endp - p);
+  return err;
+}
+
+
+int llhttp__on_version_complete(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  CALLBACK_MAYBE(s, on_version_complete);
+  return err;
+}
+
+
 int llhttp__on_header_field(llhttp_t* s, const char* p, const char* endp) {
   int err;
   SPAN_CALLBACK_MAYBE(s, on_header_field, p, endp - p);
   return err;
 }
 
 
@@ -351,21 +401,56 @@
 int llhttp__on_chunk_header(llhttp_t* s, const char* p, const char* endp) {
   int err;
   CALLBACK_MAYBE(s, on_chunk_header);
   return err;
 }
 
 
+int llhttp__on_chunk_extension_name(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  SPAN_CALLBACK_MAYBE(s, on_chunk_extension_name, p, endp - p);
+  return err;
+}
+
+
+int llhttp__on_chunk_extension_name_complete(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  CALLBACK_MAYBE(s, on_chunk_extension_name_complete);
+  return err;
+}
+
+
+int llhttp__on_chunk_extension_value(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  SPAN_CALLBACK_MAYBE(s, on_chunk_extension_value, p, endp - p);
+  return err;
+}
+
+
+int llhttp__on_chunk_extension_value_complete(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  CALLBACK_MAYBE(s, on_chunk_extension_value_complete);
+  return err;
+}
+
+
 int llhttp__on_chunk_complete(llhttp_t* s, const char* p, const char* endp) {
   int err;
   CALLBACK_MAYBE(s, on_chunk_complete);
   return err;
 }
 
 
+int llhttp__on_reset(llhttp_t* s, const char* p, const char* endp) {
+  int err;
+  CALLBACK_MAYBE(s, on_reset);
+  return err;
+}
+
+
 /* Private */
 
 
 void llhttp__debug(llhttp_t* s, const char* p, const char* endp,
                    const char* msg) {
   if (p == endp) {
     fprintf(stderr, "p=%p type=%d flags=%02x next=null debug=%s\n", s, s->type,
```

### Comparing `httptools-0.5.0/vendor/llhttp/src/http.c` & `httptools-0.6.0/vendor/llhttp/src/http.c`

 * *Files identical despite different names*

### Comparing `httptools-0.5.0/vendor/llhttp/src/llhttp.c` & `httptools-0.6.0/vendor/llhttp/src/llhttp.c`

 * *Files 19% similar despite different names*

```diff
@@ -335,49 +335,62 @@
   s_n_llhttp__internal__n_invoke_is_equal_upgrade,
   s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2,
   s_n_llhttp__internal__n_chunk_data_almost_done,
   s_n_llhttp__internal__n_consume_content_length,
   s_n_llhttp__internal__n_span_start_llhttp__on_body,
   s_n_llhttp__internal__n_invoke_is_equal_content_length,
   s_n_llhttp__internal__n_chunk_size_almost_done,
-  s_n_llhttp__internal__n_chunk_parameters,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete,
+  s_n_llhttp__internal__n_chunk_extension_quoted_value_done,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1,
+  s_n_llhttp__internal__n_error_21,
+  s_n_llhttp__internal__n_chunk_extension_quoted_value,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2,
+  s_n_llhttp__internal__n_error_23,
+  s_n_llhttp__internal__n_chunk_extension_value,
+  s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value,
+  s_n_llhttp__internal__n_error_24,
+  s_n_llhttp__internal__n_chunk_extension_name,
+  s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name,
+  s_n_llhttp__internal__n_chunk_extensions,
   s_n_llhttp__internal__n_chunk_size_otherwise,
   s_n_llhttp__internal__n_chunk_size,
   s_n_llhttp__internal__n_chunk_size_digit,
-  s_n_llhttp__internal__n_invoke_update_content_length,
+  s_n_llhttp__internal__n_invoke_update_content_length_1,
   s_n_llhttp__internal__n_consume_content_length_1,
   s_n_llhttp__internal__n_span_start_llhttp__on_body_1,
   s_n_llhttp__internal__n_eof,
   s_n_llhttp__internal__n_span_start_llhttp__on_body_2,
   s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete,
   s_n_llhttp__internal__n_headers_almost_done,
   s_n_llhttp__internal__n_header_field_colon_discard_ws,
-  s_n_llhttp__internal__n_error_19,
+  s_n_llhttp__internal__n_error_33,
   s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_value,
   s_n_llhttp__internal__n_header_value_discard_lws,
   s_n_llhttp__internal__n_header_value_discard_ws_almost_done,
   s_n_llhttp__internal__n_header_value_lws,
   s_n_llhttp__internal__n_header_value_almost_done,
   s_n_llhttp__internal__n_header_value_lenient,
-  s_n_llhttp__internal__n_error_23,
-  s_n_llhttp__internal__n_header_value_lenient_failed,
+  s_n_llhttp__internal__n_error_41,
   s_n_llhttp__internal__n_header_value_otherwise,
   s_n_llhttp__internal__n_header_value_connection_token,
   s_n_llhttp__internal__n_header_value_connection_ws,
   s_n_llhttp__internal__n_header_value_connection_1,
   s_n_llhttp__internal__n_header_value_connection_2,
   s_n_llhttp__internal__n_header_value_connection_3,
   s_n_llhttp__internal__n_header_value_connection,
-  s_n_llhttp__internal__n_error_26,
-  s_n_llhttp__internal__n_error_27,
+  s_n_llhttp__internal__n_error_43,
+  s_n_llhttp__internal__n_error_44,
   s_n_llhttp__internal__n_header_value_content_length_ws,
   s_n_llhttp__internal__n_header_value_content_length,
-  s_n_llhttp__internal__n_error_29,
-  s_n_llhttp__internal__n_error_28,
+  s_n_llhttp__internal__n_error_46,
+  s_n_llhttp__internal__n_error_45,
   s_n_llhttp__internal__n_header_value_te_token_ows,
   s_n_llhttp__internal__n_header_value,
   s_n_llhttp__internal__n_header_value_te_token,
   s_n_llhttp__internal__n_header_value_te_chunked_last,
   s_n_llhttp__internal__n_header_value_te_chunked,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1,
   s_n_llhttp__internal__n_header_value_discard_ws,
@@ -391,24 +404,32 @@
   s_n_llhttp__internal__n_header_field_1,
   s_n_llhttp__internal__n_header_field_5,
   s_n_llhttp__internal__n_header_field_6,
   s_n_llhttp__internal__n_header_field_7,
   s_n_llhttp__internal__n_header_field,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_field,
   s_n_llhttp__internal__n_header_field_start,
+  s_n_llhttp__internal__n_headers_start,
   s_n_llhttp__internal__n_url_to_http_09,
   s_n_llhttp__internal__n_url_skip_to_http09,
   s_n_llhttp__internal__n_url_skip_lf_to_http09_1,
   s_n_llhttp__internal__n_url_skip_lf_to_http09,
   s_n_llhttp__internal__n_req_pri_upgrade,
   s_n_llhttp__internal__n_req_http_complete_1,
   s_n_llhttp__internal__n_req_http_complete,
+  s_n_llhttp__internal__n_invoke_load_method_1,
+  s_n_llhttp__internal__n_invoke_llhttp__on_version_complete,
+  s_n_llhttp__internal__n_error_51,
+  s_n_llhttp__internal__n_error_56,
   s_n_llhttp__internal__n_req_http_minor,
+  s_n_llhttp__internal__n_error_57,
   s_n_llhttp__internal__n_req_http_dot,
+  s_n_llhttp__internal__n_error_58,
   s_n_llhttp__internal__n_req_http_major,
+  s_n_llhttp__internal__n_span_start_llhttp__on_version,
   s_n_llhttp__internal__n_req_http_start_1,
   s_n_llhttp__internal__n_req_http_start_2,
   s_n_llhttp__internal__n_req_http_start_3,
   s_n_llhttp__internal__n_req_http_start,
   s_n_llhttp__internal__n_url_to_http,
   s_n_llhttp__internal__n_url_skip_to_http,
   s_n_llhttp__internal__n_url_fragment,
@@ -428,126 +449,167 @@
   s_n_llhttp__internal__n_url_start,
   s_n_llhttp__internal__n_span_start_llhttp__on_url_1,
   s_n_llhttp__internal__n_url_entry_normal,
   s_n_llhttp__internal__n_span_start_llhttp__on_url,
   s_n_llhttp__internal__n_url_entry_connect,
   s_n_llhttp__internal__n_req_spaces_before_url,
   s_n_llhttp__internal__n_req_first_space_before_url,
-  s_n_llhttp__internal__n_start_req_2,
-  s_n_llhttp__internal__n_start_req_3,
-  s_n_llhttp__internal__n_start_req_1,
-  s_n_llhttp__internal__n_start_req_4,
-  s_n_llhttp__internal__n_start_req_6,
-  s_n_llhttp__internal__n_start_req_8,
-  s_n_llhttp__internal__n_start_req_9,
-  s_n_llhttp__internal__n_start_req_7,
-  s_n_llhttp__internal__n_start_req_5,
-  s_n_llhttp__internal__n_start_req_12,
-  s_n_llhttp__internal__n_start_req_13,
-  s_n_llhttp__internal__n_start_req_11,
-  s_n_llhttp__internal__n_start_req_10,
-  s_n_llhttp__internal__n_start_req_14,
-  s_n_llhttp__internal__n_start_req_17,
-  s_n_llhttp__internal__n_start_req_16,
-  s_n_llhttp__internal__n_start_req_15,
-  s_n_llhttp__internal__n_start_req_18,
-  s_n_llhttp__internal__n_start_req_20,
-  s_n_llhttp__internal__n_start_req_21,
-  s_n_llhttp__internal__n_start_req_19,
-  s_n_llhttp__internal__n_start_req_23,
-  s_n_llhttp__internal__n_start_req_24,
-  s_n_llhttp__internal__n_start_req_26,
-  s_n_llhttp__internal__n_start_req_28,
-  s_n_llhttp__internal__n_start_req_29,
-  s_n_llhttp__internal__n_start_req_27,
-  s_n_llhttp__internal__n_start_req_25,
-  s_n_llhttp__internal__n_start_req_30,
-  s_n_llhttp__internal__n_start_req_22,
-  s_n_llhttp__internal__n_start_req_31,
-  s_n_llhttp__internal__n_start_req_32,
-  s_n_llhttp__internal__n_start_req_35,
-  s_n_llhttp__internal__n_start_req_36,
-  s_n_llhttp__internal__n_start_req_34,
-  s_n_llhttp__internal__n_start_req_37,
-  s_n_llhttp__internal__n_start_req_38,
-  s_n_llhttp__internal__n_start_req_42,
-  s_n_llhttp__internal__n_start_req_43,
-  s_n_llhttp__internal__n_start_req_41,
-  s_n_llhttp__internal__n_start_req_40,
-  s_n_llhttp__internal__n_start_req_39,
-  s_n_llhttp__internal__n_start_req_45,
-  s_n_llhttp__internal__n_start_req_44,
-  s_n_llhttp__internal__n_start_req_33,
-  s_n_llhttp__internal__n_start_req_48,
-  s_n_llhttp__internal__n_start_req_49,
-  s_n_llhttp__internal__n_start_req_50,
-  s_n_llhttp__internal__n_start_req_51,
-  s_n_llhttp__internal__n_start_req_47,
-  s_n_llhttp__internal__n_start_req_46,
-  s_n_llhttp__internal__n_start_req_54,
-  s_n_llhttp__internal__n_start_req_56,
-  s_n_llhttp__internal__n_start_req_57,
-  s_n_llhttp__internal__n_start_req_55,
-  s_n_llhttp__internal__n_start_req_53,
-  s_n_llhttp__internal__n_start_req_58,
-  s_n_llhttp__internal__n_start_req_59,
-  s_n_llhttp__internal__n_start_req_52,
-  s_n_llhttp__internal__n_start_req_61,
-  s_n_llhttp__internal__n_start_req_62,
-  s_n_llhttp__internal__n_start_req_60,
-  s_n_llhttp__internal__n_start_req_65,
-  s_n_llhttp__internal__n_start_req_67,
-  s_n_llhttp__internal__n_start_req_68,
-  s_n_llhttp__internal__n_start_req_66,
-  s_n_llhttp__internal__n_start_req_69,
-  s_n_llhttp__internal__n_start_req_64,
-  s_n_llhttp__internal__n_start_req_63,
-  s_n_llhttp__internal__n_start_req,
+  s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1,
+  s_n_llhttp__internal__n_after_start_req_2,
+  s_n_llhttp__internal__n_after_start_req_3,
+  s_n_llhttp__internal__n_after_start_req_1,
+  s_n_llhttp__internal__n_after_start_req_4,
+  s_n_llhttp__internal__n_after_start_req_6,
+  s_n_llhttp__internal__n_after_start_req_8,
+  s_n_llhttp__internal__n_after_start_req_9,
+  s_n_llhttp__internal__n_after_start_req_7,
+  s_n_llhttp__internal__n_after_start_req_5,
+  s_n_llhttp__internal__n_after_start_req_12,
+  s_n_llhttp__internal__n_after_start_req_13,
+  s_n_llhttp__internal__n_after_start_req_11,
+  s_n_llhttp__internal__n_after_start_req_10,
+  s_n_llhttp__internal__n_after_start_req_14,
+  s_n_llhttp__internal__n_after_start_req_17,
+  s_n_llhttp__internal__n_after_start_req_16,
+  s_n_llhttp__internal__n_after_start_req_15,
+  s_n_llhttp__internal__n_after_start_req_18,
+  s_n_llhttp__internal__n_after_start_req_20,
+  s_n_llhttp__internal__n_after_start_req_21,
+  s_n_llhttp__internal__n_after_start_req_19,
+  s_n_llhttp__internal__n_after_start_req_23,
+  s_n_llhttp__internal__n_after_start_req_24,
+  s_n_llhttp__internal__n_after_start_req_26,
+  s_n_llhttp__internal__n_after_start_req_28,
+  s_n_llhttp__internal__n_after_start_req_29,
+  s_n_llhttp__internal__n_after_start_req_27,
+  s_n_llhttp__internal__n_after_start_req_25,
+  s_n_llhttp__internal__n_after_start_req_30,
+  s_n_llhttp__internal__n_after_start_req_22,
+  s_n_llhttp__internal__n_after_start_req_31,
+  s_n_llhttp__internal__n_after_start_req_32,
+  s_n_llhttp__internal__n_after_start_req_35,
+  s_n_llhttp__internal__n_after_start_req_36,
+  s_n_llhttp__internal__n_after_start_req_34,
+  s_n_llhttp__internal__n_after_start_req_37,
+  s_n_llhttp__internal__n_after_start_req_38,
+  s_n_llhttp__internal__n_after_start_req_42,
+  s_n_llhttp__internal__n_after_start_req_43,
+  s_n_llhttp__internal__n_after_start_req_41,
+  s_n_llhttp__internal__n_after_start_req_40,
+  s_n_llhttp__internal__n_after_start_req_39,
+  s_n_llhttp__internal__n_after_start_req_45,
+  s_n_llhttp__internal__n_after_start_req_44,
+  s_n_llhttp__internal__n_after_start_req_33,
+  s_n_llhttp__internal__n_after_start_req_48,
+  s_n_llhttp__internal__n_after_start_req_49,
+  s_n_llhttp__internal__n_after_start_req_50,
+  s_n_llhttp__internal__n_after_start_req_51,
+  s_n_llhttp__internal__n_after_start_req_47,
+  s_n_llhttp__internal__n_after_start_req_46,
+  s_n_llhttp__internal__n_after_start_req_54,
+  s_n_llhttp__internal__n_after_start_req_56,
+  s_n_llhttp__internal__n_after_start_req_57,
+  s_n_llhttp__internal__n_after_start_req_55,
+  s_n_llhttp__internal__n_after_start_req_53,
+  s_n_llhttp__internal__n_after_start_req_58,
+  s_n_llhttp__internal__n_after_start_req_59,
+  s_n_llhttp__internal__n_after_start_req_52,
+  s_n_llhttp__internal__n_after_start_req_61,
+  s_n_llhttp__internal__n_after_start_req_62,
+  s_n_llhttp__internal__n_after_start_req_60,
+  s_n_llhttp__internal__n_after_start_req_65,
+  s_n_llhttp__internal__n_after_start_req_67,
+  s_n_llhttp__internal__n_after_start_req_68,
+  s_n_llhttp__internal__n_after_start_req_66,
+  s_n_llhttp__internal__n_after_start_req_69,
+  s_n_llhttp__internal__n_after_start_req_64,
+  s_n_llhttp__internal__n_after_start_req_63,
+  s_n_llhttp__internal__n_after_start_req,
+  s_n_llhttp__internal__n_span_start_llhttp__on_method_1,
   s_n_llhttp__internal__n_invoke_llhttp__on_status_complete,
   s_n_llhttp__internal__n_res_line_almost_done,
   s_n_llhttp__internal__n_res_status,
   s_n_llhttp__internal__n_span_start_llhttp__on_status,
   s_n_llhttp__internal__n_res_status_start,
   s_n_llhttp__internal__n_res_status_code_otherwise,
-  s_n_llhttp__internal__n_res_status_code,
-  s_n_llhttp__internal__n_res_http_end,
+  s_n_llhttp__internal__n_res_status_code_digit_3,
+  s_n_llhttp__internal__n_res_status_code_digit_2,
+  s_n_llhttp__internal__n_res_status_code_digit_1,
+  s_n_llhttp__internal__n_res_after_version,
+  s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1,
+  s_n_llhttp__internal__n_error_73,
+  s_n_llhttp__internal__n_error_85,
   s_n_llhttp__internal__n_res_http_minor,
+  s_n_llhttp__internal__n_error_86,
   s_n_llhttp__internal__n_res_http_dot,
+  s_n_llhttp__internal__n_error_87,
   s_n_llhttp__internal__n_res_http_major,
+  s_n_llhttp__internal__n_span_start_llhttp__on_version_1,
   s_n_llhttp__internal__n_start_res,
+  s_n_llhttp__internal__n_invoke_llhttp__on_method_complete,
   s_n_llhttp__internal__n_req_or_res_method_2,
+  s_n_llhttp__internal__n_invoke_update_type_1,
   s_n_llhttp__internal__n_req_or_res_method_3,
   s_n_llhttp__internal__n_req_or_res_method_1,
   s_n_llhttp__internal__n_req_or_res_method,
+  s_n_llhttp__internal__n_span_start_llhttp__on_method,
   s_n_llhttp__internal__n_start_req_or_res,
   s_n_llhttp__internal__n_invoke_load_type,
+  s_n_llhttp__internal__n_invoke_update_finish,
   s_n_llhttp__internal__n_start,
 };
 typedef enum llparse_state_e llparse_state_t;
 
+int llhttp__on_method(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__on_url(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__on_version(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__on_header_field(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
 int llhttp__on_header_value(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
 int llhttp__on_body(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__on_chunk_extension_name(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
+int llhttp__on_chunk_extension_value(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__on_status(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__internal__c_load_initial_message_completed(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return state->initial_message_completed;
+}
+
+int llhttp__on_reset(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__internal__c_update_finish(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->finish = 2;
   return 0;
 }
@@ -568,14 +630,18 @@
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   state->method = match;
   return 0;
 }
 
+int llhttp__on_method_complete(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__internal__c_is_equal_method(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return state->method == 5;
 }
 
@@ -595,14 +661,21 @@
   return 0;
 }
 
 int llhttp__on_url_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__internal__c_test_lenient_flags(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return (state->lenient_flags & 1) == 1;
+}
+
 int llhttp__internal__c_test_flags(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->flags & 128) == 128;
 }
 
@@ -621,37 +694,53 @@
   return state->upgrade == 1;
 }
 
 int llhttp__after_message_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__internal__c_update_content_length(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  state->content_length = 0;
+  return 0;
+}
+
+int llhttp__internal__c_update_initial_message_completed(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  state->initial_message_completed = 1;
+  return 0;
+}
+
 int llhttp__internal__c_update_finish_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->finish = 0;
   return 0;
 }
 
-int llhttp__internal__c_test_lenient_flags(
+int llhttp__internal__c_test_lenient_flags_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->lenient_flags & 4) == 4;
 }
 
 int llhttp__internal__c_test_flags_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->flags & 544) == 544;
 }
 
-int llhttp__internal__c_test_lenient_flags_1(
+int llhttp__internal__c_test_lenient_flags_2(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->lenient_flags & 2) == 2;
 }
 
 int llhttp__before_headers_complete(
@@ -662,22 +751,14 @@
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
 int llhttp__after_headers_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
-int llhttp__internal__c_update_content_length(
-    llhttp__internal_t* state,
-    const unsigned char* p,
-    const unsigned char* endp) {
-  state->content_length = 0;
-  return 0;
-}
-
 int llhttp__internal__c_mul_add_content_length(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   /* Multiplication overflow */
   if (state->content_length > 0xffffffffffffffffULL / 16) {
@@ -715,14 +796,22 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 128;
   return 0;
 }
 
+int llhttp__on_chunk_extension_name_complete(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
+int llhttp__on_chunk_extension_value_complete(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__internal__c_update_finish_3(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->finish = 1;
   return 0;
 }
@@ -748,21 +837,14 @@
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   state->header_state = match;
   return 0;
 }
 
-int llhttp__internal__c_test_lenient_flags_2(
-    llhttp__internal_t* state,
-    const unsigned char* p,
-    const unsigned char* endp) {
-  return (state->lenient_flags & 1) == 1;
-}
-
 int llhttp__on_header_field_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
 int llhttp__internal__c_load_header_state(
     llhttp__internal_t* state,
     const unsigned char* p,
@@ -810,39 +892,39 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 8;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_2(
+int llhttp__internal__c_update_header_state_3(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 6;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_4(
+int llhttp__internal__c_update_header_state_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 0;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_5(
+int llhttp__internal__c_update_header_state_6(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 5;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_6(
+int llhttp__internal__c_update_header_state_7(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 7;
   return 0;
 }
 
@@ -890,15 +972,15 @@
 int llhttp__internal__c_test_flags_3(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->flags & 8) == 8;
 }
 
-int llhttp__internal__c_test_lenient_flags_4(
+int llhttp__internal__c_test_lenient_flags_8(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->lenient_flags & 8) == 8;
 }
 
 int llhttp__internal__c_or_flags_16(
@@ -913,15 +995,15 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags &= -9;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_7(
+int llhttp__internal__c_update_header_state_8(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 8;
   return 0;
 }
 
@@ -954,21 +1036,25 @@
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   state->http_minor = match;
   return 0;
 }
 
-int llhttp__internal__c_test_lenient_flags_6(
+int llhttp__internal__c_test_lenient_flags_10(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->lenient_flags & 16) == 16;
 }
 
+int llhttp__on_version_complete(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__internal__c_load_http_major(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return state->http_major;
 }
 
@@ -1006,19 +1092,14 @@
     }
   } else {
     if (state->status_code < 0 - match) {
       return 1;
     }
   }
   state->status_code += match;
-  
-  /* Enforce maximum */
-  if (state->status_code > 999) {
-    return 1;
-  }
   return 0;
 }
 
 int llhttp__on_status_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
@@ -1062,25 +1143,25 @@
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_closed;
         }
         default: {
           p++;
-          goto s_n_llhttp__internal__n_error_4;
+          goto s_n_llhttp__internal__n_error_7;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_llhttp__after_message_complete:
     s_n_llhttp__internal__n_invoke_llhttp__after_message_complete: {
       switch (llhttp__after_message_complete(state, p, endp)) {
         case 1:
-          goto s_n_llhttp__internal__n_invoke_update_finish_2;
+          goto s_n_llhttp__internal__n_invoke_update_content_length;
         default:
           goto s_n_llhttp__internal__n_invoke_update_finish_1;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_pause_1:
@@ -1106,17 +1187,17 @@
     }
     case s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2:
     s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2: {
       switch (llhttp__on_message_complete(state, p, endp)) {
         case 0:
           goto s_n_llhttp__internal__n_invoke_is_equal_upgrade;
         case 21:
-          goto s_n_llhttp__internal__n_pause_5;
+          goto s_n_llhttp__internal__n_pause_11;
         default:
-          goto s_n_llhttp__internal__n_error_14;
+          goto s_n_llhttp__internal__n_error_28;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_chunk_data_almost_done:
     s_n_llhttp__internal__n_chunk_data_almost_done: {
       llparse_match_t match_seq;
@@ -1131,15 +1212,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_complete;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_chunk_data_almost_done;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_8;
+          goto s_n_llhttp__internal__n_error_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_consume_content_length:
     s_n_llhttp__internal__n_consume_content_length: {
@@ -1188,54 +1269,302 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_header;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_9;
+          goto s_n_llhttp__internal__n_error_12;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete: {
+      switch (llhttp__on_chunk_extension_name_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_size_almost_done;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_5;
+        default:
+          goto s_n_llhttp__internal__n_error_15;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1: {
+      switch (llhttp__on_chunk_extension_name_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_extensions;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_6;
+        default:
+          goto s_n_llhttp__internal__n_error_16;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete: {
+      switch (llhttp__on_chunk_extension_value_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_size_almost_done;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_7;
+        default:
+          goto s_n_llhttp__internal__n_error_18;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extension_quoted_value_done:
+    s_n_llhttp__internal__n_chunk_extension_quoted_value_done: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_chunk_extension_quoted_value_done;
+      }
+      switch (*p) {
+        case 13: {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_size_almost_done;
+        }
+        case ';': {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_extensions;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_error_20;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_chunk_parameters:
-    s_n_llhttp__internal__n_chunk_parameters: {
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1: {
+      switch (llhttp__on_chunk_extension_value_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_extension_quoted_value_done;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_8;
+        default:
+          goto s_n_llhttp__internal__n_error_19;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_21:
+    s_n_llhttp__internal__n_error_21: {
+      state->error = 0x2;
+      state->reason = "Invalid character in chunk extensions quoted value";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extension_quoted_value:
+    s_n_llhttp__internal__n_chunk_extension_quoted_value: {
       static uint8_t lookup_table[] = {
-        0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 2, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0,
         0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        1, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+        1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
-        1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0,
-        1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1
       };
       if (p == endp) {
-        return s_n_llhttp__internal__n_chunk_parameters;
+        return s_n_llhttp__internal__n_chunk_extension_quoted_value;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_chunk_parameters;
+          goto s_n_llhttp__internal__n_chunk_extension_quoted_value;
         }
         case 2: {
           p++;
-          goto s_n_llhttp__internal__n_chunk_size_almost_done;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_10;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_2;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2: {
+      switch (llhttp__on_chunk_extension_value_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_size_otherwise;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_9;
+        default:
+          goto s_n_llhttp__internal__n_error_22;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_23:
+    s_n_llhttp__internal__n_error_23: {
+      state->error = 0x2;
+      state->reason = "Invalid character in chunk extensions value";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extension_value:
+    s_n_llhttp__internal__n_chunk_extension_value: {
+      static uint8_t lookup_table[] = {
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 2, 3, 2, 2, 2, 2, 2, 0, 0, 2, 2, 0, 2, 2, 0,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 4, 0, 0, 0, 0,
+        0, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 0, 0, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 2, 0, 2, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+      };
+      if (p == endp) {
+        return s_n_llhttp__internal__n_chunk_extension_value;
+      }
+      switch (lookup_table[(uint8_t) *p]) {
+        case 1: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value;
+        }
+        case 2: {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_extension_value;
+        }
+        case 3: {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_extension_quoted_value;
+        }
+        case 4: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_3;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_4;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value:
+    s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_chunk_extension_value;
+      goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_2;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_24:
+    s_n_llhttp__internal__n_error_24: {
+      state->error = 0x2;
+      state->reason = "Invalid character in chunk extensions name";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extension_name:
+    s_n_llhttp__internal__n_chunk_extension_name: {
+      static uint8_t lookup_table[] = {
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 2, 0, 2, 2, 2, 2, 2, 0, 0, 2, 2, 0, 2, 2, 0,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 3, 0, 4, 0, 0,
+        0, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 0, 0, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 2, 0, 2, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+      };
+      if (p == endp) {
+        return s_n_llhttp__internal__n_chunk_extension_name;
+      }
+      switch (lookup_table[(uint8_t) *p]) {
+        case 1: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name;
+        }
+        case 2: {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_extension_name;
+        }
+        case 3: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_1;
+        }
+        case 4: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_2;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_3;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name:
+    s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_chunk_extension_name;
+      goto s_n_llhttp__internal__n_chunk_extension_name;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extensions:
+    s_n_llhttp__internal__n_chunk_extensions: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_chunk_extensions;
+      }
+      switch (*p) {
+        case 13: {
+          p++;
+          goto s_n_llhttp__internal__n_error_13;
+        }
+        case ' ': {
+          p++;
+          goto s_n_llhttp__internal__n_error_14;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_chunk_size_otherwise:
     s_n_llhttp__internal__n_chunk_size_otherwise: {
@@ -1243,24 +1572,20 @@
         return s_n_llhttp__internal__n_chunk_size_otherwise;
       }
       switch (*p) {
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_chunk_size_almost_done;
         }
-        case ' ': {
-          p++;
-          goto s_n_llhttp__internal__n_chunk_parameters;
-        }
         case ';': {
           p++;
-          goto s_n_llhttp__internal__n_chunk_parameters;
+          goto s_n_llhttp__internal__n_chunk_extensions;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_11;
+          goto s_n_llhttp__internal__n_error_25;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_chunk_size:
     s_n_llhttp__internal__n_chunk_size: {
@@ -1498,22 +1823,22 @@
         }
         case 'f': {
           p++;
           match = 15;
           goto s_n_llhttp__internal__n_invoke_mul_add_content_length;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_13;
+          goto s_n_llhttp__internal__n_error_27;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_invoke_update_content_length:
-    s_n_llhttp__internal__n_invoke_update_content_length: {
+    case s_n_llhttp__internal__n_invoke_update_content_length_1:
+    s_n_llhttp__internal__n_invoke_update_content_length_1: {
       switch (llhttp__internal__c_update_content_length(state, p, endp)) {
         default:
           goto s_n_llhttp__internal__n_chunk_size_digit;
       }
       /* UNREACHABLE */;
       abort();
     }
@@ -1569,21 +1894,21 @@
     }
     case s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete:
     s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete: {
       switch (llhttp__after_headers_complete(state, p, endp)) {
         case 1:
           goto s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_1;
         case 2:
-          goto s_n_llhttp__internal__n_invoke_update_content_length;
+          goto s_n_llhttp__internal__n_invoke_update_content_length_1;
         case 3:
           goto s_n_llhttp__internal__n_span_start_llhttp__on_body_1;
         case 4:
           goto s_n_llhttp__internal__n_invoke_update_finish_3;
         case 5:
-          goto s_n_llhttp__internal__n_error_15;
+          goto s_n_llhttp__internal__n_error_29;
         default:
           goto s_n_llhttp__internal__n_invoke_llhttp__on_message_complete;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_headers_almost_done:
@@ -1593,15 +1918,15 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_invoke_test_flags;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_18;
+          goto s_n_llhttp__internal__n_error_32;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_colon_discard_ws:
     s_n_llhttp__internal__n_header_field_colon_discard_ws: {
@@ -1616,29 +1941,33 @@
         default: {
           goto s_n_llhttp__internal__n_header_field_colon;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_19:
-    s_n_llhttp__internal__n_error_19: {
+    case s_n_llhttp__internal__n_error_33:
+    s_n_llhttp__internal__n_error_33: {
       state->error = 0xa;
       state->reason = "Invalid header field char";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete:
     s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete: {
       switch (llhttp__on_header_value_complete(state, p, endp)) {
-        default:
+        case 0:
           goto s_n_llhttp__internal__n_header_field_start;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_14;
+        default:
+          goto s_n_llhttp__internal__n_error_37;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_header_value:
     s_n_llhttp__internal__n_span_start_llhttp__on_header_value: {
       if (p == endp) {
@@ -1654,19 +1983,19 @@
     s_n_llhttp__internal__n_header_value_discard_lws: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_discard_lws;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_ws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_5;
         }
         case ' ': {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_ws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_5;
         }
         default: {
           goto s_n_llhttp__internal__n_invoke_load_header_state;
         }
       }
       /* UNREACHABLE */;
       abort();
@@ -1678,34 +2007,34 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_lws;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_21;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_6;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_lws:
     s_n_llhttp__internal__n_header_value_lws: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_lws;
       }
       switch (*p) {
         case 9: {
-          goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
         }
         case ' ': {
-          goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_4;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_almost_done:
     s_n_llhttp__internal__n_header_value_almost_done: {
@@ -1714,15 +2043,15 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_header_value_lws;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_22;
+          goto s_n_llhttp__internal__n_error_40;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_lenient:
     s_n_llhttp__internal__n_header_value_lenient: {
@@ -1740,51 +2069,35 @@
           p++;
           goto s_n_llhttp__internal__n_header_value_lenient;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_23:
-    s_n_llhttp__internal__n_error_23: {
-      state->error = 0x19;
-      state->reason = "Missing expected CR after header value";
+    case s_n_llhttp__internal__n_error_41:
+    s_n_llhttp__internal__n_error_41: {
+      state->error = 0xa;
+      state->reason = "Invalid header value char";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_header_value_lenient_failed:
-    s_n_llhttp__internal__n_header_value_lenient_failed: {
-      if (p == endp) {
-        return s_n_llhttp__internal__n_header_value_lenient_failed;
-      }
-      switch (*p) {
-        case 10: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2;
-        }
-        default: {
-          goto s_n_llhttp__internal__n_error_24;
-        }
-      }
-      /* UNREACHABLE */;
-      abort();
-    }
     case s_n_llhttp__internal__n_header_value_otherwise:
     s_n_llhttp__internal__n_header_value_otherwise: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_otherwise;
       }
       switch (*p) {
         case 13: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_3;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_7;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_connection_token:
     s_n_llhttp__internal__n_header_value_connection_token: {
@@ -1839,18 +2152,18 @@
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_header_value_connection_ws;
         }
         case ',': {
           p++;
-          goto s_n_llhttp__internal__n_invoke_load_header_state_4;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_5;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_4;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_5;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_connection_1:
     s_n_llhttp__internal__n_header_value_connection_1: {
@@ -1860,15 +2173,15 @@
         return s_n_llhttp__internal__n_header_value_connection_1;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob3, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_2;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_3;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_1;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -1884,15 +2197,15 @@
         return s_n_llhttp__internal__n_header_value_connection_2;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob4, 9);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_5;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_6;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_2;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -1908,15 +2221,15 @@
         return s_n_llhttp__internal__n_header_value_connection_3;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob5, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_6;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_3;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -1953,26 +2266,26 @@
         default: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_26:
-    s_n_llhttp__internal__n_error_26: {
+    case s_n_llhttp__internal__n_error_43:
+    s_n_llhttp__internal__n_error_43: {
       state->error = 0xb;
       state->reason = "Content-Length overflow";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_27:
-    s_n_llhttp__internal__n_error_27: {
+    case s_n_llhttp__internal__n_error_44:
+    s_n_llhttp__internal__n_error_44: {
       state->error = 0xb;
       state->reason = "Invalid character in Content-Length";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
@@ -2059,26 +2372,26 @@
         default: {
           goto s_n_llhttp__internal__n_header_value_content_length_ws;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_29:
-    s_n_llhttp__internal__n_error_29: {
+    case s_n_llhttp__internal__n_error_46:
+    s_n_llhttp__internal__n_error_46: {
       state->error = 0xf;
       state->reason = "Invalid `Transfer-Encoding` header value";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_28:
-    s_n_llhttp__internal__n_error_28: {
+    case s_n_llhttp__internal__n_error_45:
+    s_n_llhttp__internal__n_error_45: {
       state->error = 0xf;
       state->reason = "Invalid `Transfer-Encoding` header value";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
@@ -2192,31 +2505,31 @@
           goto s_n_llhttp__internal__n_header_value_te_token;
         }
         case 2: {
           p++;
           goto s_n_llhttp__internal__n_header_value_te_token_ows;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_8;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_9;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_te_chunked_last:
     s_n_llhttp__internal__n_header_value_te_chunked_last: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_te_chunked_last;
       }
       switch (*p) {
         case 10: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_8;
         }
         case 13: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_8;
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_header_value_te_chunked_last;
         }
         case ',': {
           goto s_n_llhttp__internal__n_invoke_load_type_1;
@@ -2271,15 +2584,15 @@
       switch (*p) {
         case 9: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_ws;
         }
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_lws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_4;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_ws_almost_done;
         }
         case ' ': {
           p++;
@@ -2291,31 +2604,35 @@
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete:
     s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete: {
       switch (llhttp__on_header_field_complete(state, p, endp)) {
-        default:
+        case 0:
           goto s_n_llhttp__internal__n_header_value_discard_ws;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_15;
+        default:
+          goto s_n_llhttp__internal__n_error_34;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_general_otherwise:
     s_n_llhttp__internal__n_header_field_general_otherwise: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_field_general_otherwise;
       }
       switch (*p) {
         case ':': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field_2;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_30;
+          goto s_n_llhttp__internal__n_error_47;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_general:
     s_n_llhttp__internal__n_header_field_general: {
@@ -2391,21 +2708,21 @@
     case s_n_llhttp__internal__n_header_field_colon:
     s_n_llhttp__internal__n_header_field_colon: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_field_colon;
       }
       switch (*p) {
         case ' ': {
-          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_2;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_3;
         }
         case ':': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_9;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_3:
     s_n_llhttp__internal__n_header_field_3: {
@@ -2422,15 +2739,15 @@
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_4:
     s_n_llhttp__internal__n_header_field_4: {
@@ -2447,15 +2764,15 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_4;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_2:
     s_n_llhttp__internal__n_header_field_2: {
@@ -2468,15 +2785,15 @@
           goto s_n_llhttp__internal__n_header_field_3;
         }
         case 't': {
           p++;
           goto s_n_llhttp__internal__n_header_field_4;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_1:
     s_n_llhttp__internal__n_header_field_1: {
@@ -2492,15 +2809,15 @@
           p++;
           goto s_n_llhttp__internal__n_header_field_2;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_1;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_5:
     s_n_llhttp__internal__n_header_field_5: {
@@ -2517,15 +2834,15 @@
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_5;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_6:
     s_n_llhttp__internal__n_header_field_6: {
@@ -2542,15 +2859,15 @@
           match = 3;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_6;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_7:
     s_n_llhttp__internal__n_header_field_7: {
@@ -2567,15 +2884,15 @@
           match = 4;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_7;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field:
     s_n_llhttp__internal__n_header_field: {
@@ -2596,15 +2913,15 @@
           goto s_n_llhttp__internal__n_header_field_6;
         }
         case 'u': {
           p++;
           goto s_n_llhttp__internal__n_header_field_7;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_header_field:
     s_n_llhttp__internal__n_span_start_llhttp__on_header_field: {
@@ -2633,27 +2950,44 @@
         default: {
           goto s_n_llhttp__internal__n_span_start_llhttp__on_header_field;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_headers_start:
+    s_n_llhttp__internal__n_headers_start: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_headers_start;
+      }
+      switch (*p) {
+        case ' ': {
+          p++;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_header_field_start;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_url_to_http_09:
     s_n_llhttp__internal__n_url_to_http_09: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_to_http_09;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         default: {
           goto s_n_llhttp__internal__n_invoke_update_http_major;
         }
       }
       /* UNREACHABLE */;
       abort();
@@ -2662,19 +2996,19 @@
     s_n_llhttp__internal__n_url_skip_to_http09: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_skip_to_http09;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         default: {
           p++;
           goto s_n_llhttp__internal__n_url_to_http_09;
         }
       }
       /* UNREACHABLE */;
@@ -2687,40 +3021,40 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_url_to_http_09;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_31;
+          goto s_n_llhttp__internal__n_error_48;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_skip_lf_to_http09:
     s_n_llhttp__internal__n_url_skip_lf_to_http09: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_skip_lf_to_http09;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_url_skip_lf_to_http09_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_31;
+          goto s_n_llhttp__internal__n_error_48;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_pri_upgrade:
     s_n_llhttp__internal__n_req_pri_upgrade: {
@@ -2730,64 +3064,108 @@
         return s_n_llhttp__internal__n_req_pri_upgrade;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob15, 10);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_error_36;
+          goto s_n_llhttp__internal__n_error_54;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_pri_upgrade;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_37;
+          goto s_n_llhttp__internal__n_error_55;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_complete_1:
     s_n_llhttp__internal__n_req_http_complete_1: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_complete_1;
       }
       switch (*p) {
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_header_field_start;
+          goto s_n_llhttp__internal__n_headers_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_35;
+          goto s_n_llhttp__internal__n_error_53;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_complete:
     s_n_llhttp__internal__n_req_http_complete: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_complete;
       }
       switch (*p) {
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_header_field_start;
+          goto s_n_llhttp__internal__n_headers_start;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_req_http_complete_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_35;
+          goto s_n_llhttp__internal__n_error_53;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_load_method_1:
+    s_n_llhttp__internal__n_invoke_load_method_1: {
+      switch (llhttp__internal__c_load_method(state, p, endp)) {
+        case 34:
+          goto s_n_llhttp__internal__n_req_pri_upgrade;
+        default:
+          goto s_n_llhttp__internal__n_req_http_complete;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_version_complete:
+    s_n_llhttp__internal__n_invoke_llhttp__on_version_complete: {
+      switch (llhttp__on_version_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_invoke_load_method_1;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_17;
+        default:
+          goto s_n_llhttp__internal__n_error_52;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_51:
+    s_n_llhttp__internal__n_error_51: {
+      state->error = 0x9;
+      state->reason = "Invalid HTTP version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_56:
+    s_n_llhttp__internal__n_error_56: {
+      state->error = 0x9;
+      state->reason = "Invalid minor version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_http_minor:
     s_n_llhttp__internal__n_req_http_minor: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_minor;
       }
       switch (*p) {
         case '0': {
@@ -2837,37 +3215,57 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_40;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_2;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_57:
+    s_n_llhttp__internal__n_error_57: {
+      state->error = 0x9;
+      state->reason = "Expected dot";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_http_dot:
     s_n_llhttp__internal__n_req_http_dot: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_dot;
       }
       switch (*p) {
         case '.': {
           p++;
           goto s_n_llhttp__internal__n_req_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_41;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_3;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_58:
+    s_n_llhttp__internal__n_error_58: {
+      state->error = 0x9;
+      state->reason = "Invalid major version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_http_major:
     s_n_llhttp__internal__n_req_http_major: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_major;
       }
       switch (*p) {
         case '0': {
@@ -2917,20 +3315,31 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_major;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_42;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_4;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_version:
+    s_n_llhttp__internal__n_span_start_llhttp__on_version: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_version;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_version;
+      goto s_n_llhttp__internal__n_req_http_major;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_http_start_1:
     s_n_llhttp__internal__n_req_http_start_1: {
       llparse_match_t match_seq;
       
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_start_1;
       }
@@ -2941,15 +3350,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_1;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_61;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_2:
     s_n_llhttp__internal__n_req_http_start_2: {
@@ -2965,15 +3374,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method_2;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_2;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_61;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_3:
     s_n_llhttp__internal__n_req_http_start_3: {
@@ -2989,15 +3398,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method_3;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_61;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start:
     s_n_llhttp__internal__n_req_http_start: {
@@ -3018,33 +3427,33 @@
           goto s_n_llhttp__internal__n_req_http_start_2;
         }
         case 'R': {
           p++;
           goto s_n_llhttp__internal__n_req_http_start_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_61;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_to_http:
     s_n_llhttp__internal__n_url_to_http: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_to_http;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         default: {
           goto s_n_llhttp__internal__n_invoke_llhttp__on_url_complete_1;
         }
       }
       /* UNREACHABLE */;
       abort();
@@ -3053,19 +3462,19 @@
     s_n_llhttp__internal__n_url_skip_to_http: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_skip_to_http;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         default: {
           p++;
           goto s_n_llhttp__internal__n_url_to_http;
         }
       }
       /* UNREACHABLE */;
@@ -3093,15 +3502,15 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_fragment;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 2: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_6;
         }
         case 3: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_7;
         }
@@ -3109,15 +3518,15 @@
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_8;
         }
         case 5: {
           p++;
           goto s_n_llhttp__internal__n_url_fragment;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_62;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_end_stub_query_3:
     s_n_llhttp__internal__n_span_end_stub_query_3: {
@@ -3151,15 +3560,15 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_query;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 2: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_9;
         }
         case 3: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_10;
         }
@@ -3170,36 +3579,36 @@
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         case 6: {
           goto s_n_llhttp__internal__n_span_end_stub_query_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_47;
+          goto s_n_llhttp__internal__n_error_63;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_query_or_fragment:
     s_n_llhttp__internal__n_url_query_or_fragment: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_query_or_fragment;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 10: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_3;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 13: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_4;
         }
         case ' ': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_5;
         }
@@ -3208,15 +3617,15 @@
           goto s_n_llhttp__internal__n_url_fragment;
         }
         case '?': {
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_48;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_path:
     s_n_llhttp__internal__n_url_path: {
@@ -3240,15 +3649,15 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_path;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 2: {
           p++;
           goto s_n_llhttp__internal__n_url_path;
         }
         default: {
           goto s_n_llhttp__internal__n_url_query_or_fragment;
@@ -3309,15 +3718,15 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_server_with_at;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 2: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_12;
         }
         case 3: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_13;
         }
@@ -3333,18 +3742,18 @@
         }
         case 7: {
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         case 8: {
           p++;
-          goto s_n_llhttp__internal__n_error_49;
+          goto s_n_llhttp__internal__n_error_65;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_50;
+          goto s_n_llhttp__internal__n_error_66;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_server:
     s_n_llhttp__internal__n_url_server: {
@@ -3368,15 +3777,15 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_server;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 2: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url;
         }
         case 3: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_1;
         }
@@ -3395,15 +3804,15 @@
           goto s_n_llhttp__internal__n_url_query;
         }
         case 8: {
           p++;
           goto s_n_llhttp__internal__n_url_server_with_at;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_67;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_schema_delim_1:
     s_n_llhttp__internal__n_url_schema_delim_1: {
@@ -3412,52 +3821,52 @@
       }
       switch (*p) {
         case '/': {
           p++;
           goto s_n_llhttp__internal__n_url_server;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_53;
+          goto s_n_llhttp__internal__n_error_69;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_schema_delim:
     s_n_llhttp__internal__n_url_schema_delim: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_schema_delim;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_error_52;
+          goto s_n_llhttp__internal__n_error_68;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 13: {
           p++;
-          goto s_n_llhttp__internal__n_error_52;
+          goto s_n_llhttp__internal__n_error_68;
         }
         case ' ': {
           p++;
-          goto s_n_llhttp__internal__n_error_52;
+          goto s_n_llhttp__internal__n_error_68;
         }
         case '/': {
           p++;
           goto s_n_llhttp__internal__n_url_schema_delim_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_53;
+          goto s_n_llhttp__internal__n_error_69;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_end_stub_schema:
     s_n_llhttp__internal__n_span_end_stub_schema: {
@@ -3491,29 +3900,29 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_schema;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 2: {
           p++;
-          goto s_n_llhttp__internal__n_error_52;
+          goto s_n_llhttp__internal__n_error_68;
         }
         case 3: {
           goto s_n_llhttp__internal__n_span_end_stub_schema;
         }
         case 4: {
           p++;
           goto s_n_llhttp__internal__n_url_schema;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_54;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_start:
     s_n_llhttp__internal__n_url_start: {
@@ -3537,28 +3946,28 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_start;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 2: {
           p++;
-          goto s_n_llhttp__internal__n_error_52;
+          goto s_n_llhttp__internal__n_error_68;
         }
         case 3: {
           goto s_n_llhttp__internal__n_span_start_stub_path_2;
         }
         case 4: {
           goto s_n_llhttp__internal__n_url_schema;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_55;
+          goto s_n_llhttp__internal__n_error_71;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_url_1:
     s_n_llhttp__internal__n_span_start_llhttp__on_url_1: {
@@ -3575,19 +3984,19 @@
     s_n_llhttp__internal__n_url_entry_normal: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_entry_normal;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         default: {
           goto s_n_llhttp__internal__n_span_start_llhttp__on_url_1;
         }
       }
       /* UNREACHABLE */;
       abort();
@@ -3607,19 +4016,19 @@
     s_n_llhttp__internal__n_url_entry_connect: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_entry_connect;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         case 12: {
           p++;
-          goto s_n_llhttp__internal__n_error_1;
+          goto s_n_llhttp__internal__n_error_2;
         }
         default: {
           goto s_n_llhttp__internal__n_span_start_llhttp__on_url;
         }
       }
       /* UNREACHABLE */;
       abort();
@@ -3648,1717 +4057,1745 @@
       }
       switch (*p) {
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_req_spaces_before_url;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_56;
+          goto s_n_llhttp__internal__n_error_72;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_2:
-    s_n_llhttp__internal__n_start_req_2: {
+    case s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1:
+    s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1: {
+      switch (llhttp__on_method_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_req_first_space_before_url;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_22;
+        default:
+          goto s_n_llhttp__internal__n_error_89;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_after_start_req_2:
+    s_n_llhttp__internal__n_after_start_req_2: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_2;
+        return s_n_llhttp__internal__n_after_start_req_2;
       }
       switch (*p) {
         case 'L': {
           p++;
           match = 19;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_3:
-    s_n_llhttp__internal__n_start_req_3: {
+    case s_n_llhttp__internal__n_after_start_req_3:
+    s_n_llhttp__internal__n_after_start_req_3: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_3;
+        return s_n_llhttp__internal__n_after_start_req_3;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob18, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 36;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_3;
+          return s_n_llhttp__internal__n_after_start_req_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_1:
-    s_n_llhttp__internal__n_start_req_1: {
+    case s_n_llhttp__internal__n_after_start_req_1:
+    s_n_llhttp__internal__n_after_start_req_1: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_1;
+        return s_n_llhttp__internal__n_after_start_req_1;
       }
       switch (*p) {
         case 'C': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_2;
+          goto s_n_llhttp__internal__n_after_start_req_2;
         }
         case 'N': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_3;
+          goto s_n_llhttp__internal__n_after_start_req_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_4:
-    s_n_llhttp__internal__n_start_req_4: {
+    case s_n_llhttp__internal__n_after_start_req_4:
+    s_n_llhttp__internal__n_after_start_req_4: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_4;
+        return s_n_llhttp__internal__n_after_start_req_4;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob19, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 16;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_4;
+          return s_n_llhttp__internal__n_after_start_req_4;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_6:
-    s_n_llhttp__internal__n_start_req_6: {
+    case s_n_llhttp__internal__n_after_start_req_6:
+    s_n_llhttp__internal__n_after_start_req_6: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_6;
+        return s_n_llhttp__internal__n_after_start_req_6;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob20, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 22;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_6;
+          return s_n_llhttp__internal__n_after_start_req_6;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_8:
-    s_n_llhttp__internal__n_start_req_8: {
+    case s_n_llhttp__internal__n_after_start_req_8:
+    s_n_llhttp__internal__n_after_start_req_8: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_8;
+        return s_n_llhttp__internal__n_after_start_req_8;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob21, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 5;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_8;
+          return s_n_llhttp__internal__n_after_start_req_8;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_9:
-    s_n_llhttp__internal__n_start_req_9: {
+    case s_n_llhttp__internal__n_after_start_req_9:
+    s_n_llhttp__internal__n_after_start_req_9: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_9;
+        return s_n_llhttp__internal__n_after_start_req_9;
       }
       switch (*p) {
         case 'Y': {
           p++;
           match = 8;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_7:
-    s_n_llhttp__internal__n_start_req_7: {
+    case s_n_llhttp__internal__n_after_start_req_7:
+    s_n_llhttp__internal__n_after_start_req_7: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_7;
+        return s_n_llhttp__internal__n_after_start_req_7;
       }
       switch (*p) {
         case 'N': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_8;
+          goto s_n_llhttp__internal__n_after_start_req_8;
         }
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_9;
+          goto s_n_llhttp__internal__n_after_start_req_9;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_5:
-    s_n_llhttp__internal__n_start_req_5: {
+    case s_n_llhttp__internal__n_after_start_req_5:
+    s_n_llhttp__internal__n_after_start_req_5: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_5;
+        return s_n_llhttp__internal__n_after_start_req_5;
       }
       switch (*p) {
         case 'H': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_6;
+          goto s_n_llhttp__internal__n_after_start_req_6;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_7;
+          goto s_n_llhttp__internal__n_after_start_req_7;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_12:
-    s_n_llhttp__internal__n_start_req_12: {
+    case s_n_llhttp__internal__n_after_start_req_12:
+    s_n_llhttp__internal__n_after_start_req_12: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_12;
+        return s_n_llhttp__internal__n_after_start_req_12;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob22, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 0;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_12;
+          return s_n_llhttp__internal__n_after_start_req_12;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_13:
-    s_n_llhttp__internal__n_start_req_13: {
+    case s_n_llhttp__internal__n_after_start_req_13:
+    s_n_llhttp__internal__n_after_start_req_13: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_13;
+        return s_n_llhttp__internal__n_after_start_req_13;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob23, 5);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 35;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_13;
+          return s_n_llhttp__internal__n_after_start_req_13;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_11:
-    s_n_llhttp__internal__n_start_req_11: {
+    case s_n_llhttp__internal__n_after_start_req_11:
+    s_n_llhttp__internal__n_after_start_req_11: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_11;
+        return s_n_llhttp__internal__n_after_start_req_11;
       }
       switch (*p) {
         case 'L': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_12;
+          goto s_n_llhttp__internal__n_after_start_req_12;
         }
         case 'S': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_13;
+          goto s_n_llhttp__internal__n_after_start_req_13;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_10:
-    s_n_llhttp__internal__n_start_req_10: {
+    case s_n_llhttp__internal__n_after_start_req_10:
+    s_n_llhttp__internal__n_after_start_req_10: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_10;
+        return s_n_llhttp__internal__n_after_start_req_10;
       }
       switch (*p) {
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_11;
+          goto s_n_llhttp__internal__n_after_start_req_11;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_14:
-    s_n_llhttp__internal__n_start_req_14: {
+    case s_n_llhttp__internal__n_after_start_req_14:
+    s_n_llhttp__internal__n_after_start_req_14: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_14;
+        return s_n_llhttp__internal__n_after_start_req_14;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob24, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 45;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_14;
+          return s_n_llhttp__internal__n_after_start_req_14;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_17:
-    s_n_llhttp__internal__n_start_req_17: {
+    case s_n_llhttp__internal__n_after_start_req_17:
+    s_n_llhttp__internal__n_after_start_req_17: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_17;
+        return s_n_llhttp__internal__n_after_start_req_17;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob26, 9);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 41;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_17;
+          return s_n_llhttp__internal__n_after_start_req_17;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_16:
-    s_n_llhttp__internal__n_start_req_16: {
+    case s_n_llhttp__internal__n_after_start_req_16:
+    s_n_llhttp__internal__n_after_start_req_16: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_16;
+        return s_n_llhttp__internal__n_after_start_req_16;
       }
       switch (*p) {
         case '_': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_17;
+          goto s_n_llhttp__internal__n_after_start_req_17;
         }
         default: {
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_15:
-    s_n_llhttp__internal__n_start_req_15: {
+    case s_n_llhttp__internal__n_after_start_req_15:
+    s_n_llhttp__internal__n_after_start_req_15: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_15;
+        return s_n_llhttp__internal__n_after_start_req_15;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob25, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_start_req_16;
+          goto s_n_llhttp__internal__n_after_start_req_16;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_15;
+          return s_n_llhttp__internal__n_after_start_req_15;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_18:
-    s_n_llhttp__internal__n_start_req_18: {
+    case s_n_llhttp__internal__n_after_start_req_18:
+    s_n_llhttp__internal__n_after_start_req_18: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_18;
+        return s_n_llhttp__internal__n_after_start_req_18;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob27, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_18;
+          return s_n_llhttp__internal__n_after_start_req_18;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_20:
-    s_n_llhttp__internal__n_start_req_20: {
+    case s_n_llhttp__internal__n_after_start_req_20:
+    s_n_llhttp__internal__n_after_start_req_20: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_20;
+        return s_n_llhttp__internal__n_after_start_req_20;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob28, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 31;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_20;
+          return s_n_llhttp__internal__n_after_start_req_20;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_21:
-    s_n_llhttp__internal__n_start_req_21: {
+    case s_n_llhttp__internal__n_after_start_req_21:
+    s_n_llhttp__internal__n_after_start_req_21: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_21;
+        return s_n_llhttp__internal__n_after_start_req_21;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob29, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_21;
+          return s_n_llhttp__internal__n_after_start_req_21;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_19:
-    s_n_llhttp__internal__n_start_req_19: {
+    case s_n_llhttp__internal__n_after_start_req_19:
+    s_n_llhttp__internal__n_after_start_req_19: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_19;
+        return s_n_llhttp__internal__n_after_start_req_19;
       }
       switch (*p) {
         case 'I': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_20;
+          goto s_n_llhttp__internal__n_after_start_req_20;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_21;
+          goto s_n_llhttp__internal__n_after_start_req_21;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_23:
-    s_n_llhttp__internal__n_start_req_23: {
+    case s_n_llhttp__internal__n_after_start_req_23:
+    s_n_llhttp__internal__n_after_start_req_23: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_23;
+        return s_n_llhttp__internal__n_after_start_req_23;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob30, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 24;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_23;
+          return s_n_llhttp__internal__n_after_start_req_23;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_24:
-    s_n_llhttp__internal__n_start_req_24: {
+    case s_n_llhttp__internal__n_after_start_req_24:
+    s_n_llhttp__internal__n_after_start_req_24: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_24;
+        return s_n_llhttp__internal__n_after_start_req_24;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob31, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 23;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_24;
+          return s_n_llhttp__internal__n_after_start_req_24;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_26:
-    s_n_llhttp__internal__n_start_req_26: {
+    case s_n_llhttp__internal__n_after_start_req_26:
+    s_n_llhttp__internal__n_after_start_req_26: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_26;
+        return s_n_llhttp__internal__n_after_start_req_26;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob32, 7);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 21;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_26;
+          return s_n_llhttp__internal__n_after_start_req_26;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_28:
-    s_n_llhttp__internal__n_start_req_28: {
+    case s_n_llhttp__internal__n_after_start_req_28:
+    s_n_llhttp__internal__n_after_start_req_28: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_28;
+        return s_n_llhttp__internal__n_after_start_req_28;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob33, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 30;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_28;
+          return s_n_llhttp__internal__n_after_start_req_28;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_29:
-    s_n_llhttp__internal__n_start_req_29: {
+    case s_n_llhttp__internal__n_after_start_req_29:
+    s_n_llhttp__internal__n_after_start_req_29: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_29;
+        return s_n_llhttp__internal__n_after_start_req_29;
       }
       switch (*p) {
         case 'L': {
           p++;
           match = 10;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_27:
-    s_n_llhttp__internal__n_start_req_27: {
+    case s_n_llhttp__internal__n_after_start_req_27:
+    s_n_llhttp__internal__n_after_start_req_27: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_27;
+        return s_n_llhttp__internal__n_after_start_req_27;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_28;
+          goto s_n_llhttp__internal__n_after_start_req_28;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_29;
+          goto s_n_llhttp__internal__n_after_start_req_29;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_25:
-    s_n_llhttp__internal__n_start_req_25: {
+    case s_n_llhttp__internal__n_after_start_req_25:
+    s_n_llhttp__internal__n_after_start_req_25: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_25;
+        return s_n_llhttp__internal__n_after_start_req_25;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_26;
+          goto s_n_llhttp__internal__n_after_start_req_26;
         }
         case 'C': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_27;
+          goto s_n_llhttp__internal__n_after_start_req_27;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_30:
-    s_n_llhttp__internal__n_start_req_30: {
+    case s_n_llhttp__internal__n_after_start_req_30:
+    s_n_llhttp__internal__n_after_start_req_30: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_30;
+        return s_n_llhttp__internal__n_after_start_req_30;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob34, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 11;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_30;
+          return s_n_llhttp__internal__n_after_start_req_30;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_22:
-    s_n_llhttp__internal__n_start_req_22: {
+    case s_n_llhttp__internal__n_after_start_req_22:
+    s_n_llhttp__internal__n_after_start_req_22: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_22;
+        return s_n_llhttp__internal__n_after_start_req_22;
       }
       switch (*p) {
         case '-': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_23;
+          goto s_n_llhttp__internal__n_after_start_req_23;
         }
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_24;
+          goto s_n_llhttp__internal__n_after_start_req_24;
         }
         case 'K': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_25;
+          goto s_n_llhttp__internal__n_after_start_req_25;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_30;
+          goto s_n_llhttp__internal__n_after_start_req_30;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_31:
-    s_n_llhttp__internal__n_start_req_31: {
+    case s_n_llhttp__internal__n_after_start_req_31:
+    s_n_llhttp__internal__n_after_start_req_31: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_31;
+        return s_n_llhttp__internal__n_after_start_req_31;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob35, 5);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 25;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_31;
+          return s_n_llhttp__internal__n_after_start_req_31;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_32:
-    s_n_llhttp__internal__n_start_req_32: {
+    case s_n_llhttp__internal__n_after_start_req_32:
+    s_n_llhttp__internal__n_after_start_req_32: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_32;
+        return s_n_llhttp__internal__n_after_start_req_32;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob36, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 6;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_32;
+          return s_n_llhttp__internal__n_after_start_req_32;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_35:
-    s_n_llhttp__internal__n_start_req_35: {
+    case s_n_llhttp__internal__n_after_start_req_35:
+    s_n_llhttp__internal__n_after_start_req_35: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_35;
+        return s_n_llhttp__internal__n_after_start_req_35;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob37, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 28;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_35;
+          return s_n_llhttp__internal__n_after_start_req_35;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_36:
-    s_n_llhttp__internal__n_start_req_36: {
+    case s_n_llhttp__internal__n_after_start_req_36:
+    s_n_llhttp__internal__n_after_start_req_36: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_36;
+        return s_n_llhttp__internal__n_after_start_req_36;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob38, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 39;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_36;
+          return s_n_llhttp__internal__n_after_start_req_36;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_34:
-    s_n_llhttp__internal__n_start_req_34: {
+    case s_n_llhttp__internal__n_after_start_req_34:
+    s_n_llhttp__internal__n_after_start_req_34: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_34;
+        return s_n_llhttp__internal__n_after_start_req_34;
       }
       switch (*p) {
         case 'T': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_35;
+          goto s_n_llhttp__internal__n_after_start_req_35;
         }
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_36;
+          goto s_n_llhttp__internal__n_after_start_req_36;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_37:
-    s_n_llhttp__internal__n_start_req_37: {
+    case s_n_llhttp__internal__n_after_start_req_37:
+    s_n_llhttp__internal__n_after_start_req_37: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_37;
+        return s_n_llhttp__internal__n_after_start_req_37;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob39, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 38;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_37;
+          return s_n_llhttp__internal__n_after_start_req_37;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_38:
-    s_n_llhttp__internal__n_start_req_38: {
+    case s_n_llhttp__internal__n_after_start_req_38:
+    s_n_llhttp__internal__n_after_start_req_38: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_38;
+        return s_n_llhttp__internal__n_after_start_req_38;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob40, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 3;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_38;
+          return s_n_llhttp__internal__n_after_start_req_38;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_42:
-    s_n_llhttp__internal__n_start_req_42: {
+    case s_n_llhttp__internal__n_after_start_req_42:
+    s_n_llhttp__internal__n_after_start_req_42: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_42;
+        return s_n_llhttp__internal__n_after_start_req_42;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob41, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 12;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_42;
+          return s_n_llhttp__internal__n_after_start_req_42;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_43:
-    s_n_llhttp__internal__n_start_req_43: {
+    case s_n_llhttp__internal__n_after_start_req_43:
+    s_n_llhttp__internal__n_after_start_req_43: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_43;
+        return s_n_llhttp__internal__n_after_start_req_43;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob42, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 13;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_43;
+          return s_n_llhttp__internal__n_after_start_req_43;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_41:
-    s_n_llhttp__internal__n_start_req_41: {
+    case s_n_llhttp__internal__n_after_start_req_41:
+    s_n_llhttp__internal__n_after_start_req_41: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_41;
+        return s_n_llhttp__internal__n_after_start_req_41;
       }
       switch (*p) {
         case 'F': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_42;
+          goto s_n_llhttp__internal__n_after_start_req_42;
         }
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_43;
+          goto s_n_llhttp__internal__n_after_start_req_43;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_40:
-    s_n_llhttp__internal__n_start_req_40: {
+    case s_n_llhttp__internal__n_after_start_req_40:
+    s_n_llhttp__internal__n_after_start_req_40: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_40;
+        return s_n_llhttp__internal__n_after_start_req_40;
       }
       switch (*p) {
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_41;
+          goto s_n_llhttp__internal__n_after_start_req_41;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_39:
-    s_n_llhttp__internal__n_start_req_39: {
+    case s_n_llhttp__internal__n_after_start_req_39:
+    s_n_llhttp__internal__n_after_start_req_39: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_39;
+        return s_n_llhttp__internal__n_after_start_req_39;
       }
       switch (*p) {
         case 'I': {
           p++;
           match = 34;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_40;
+          goto s_n_llhttp__internal__n_after_start_req_40;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_45:
-    s_n_llhttp__internal__n_start_req_45: {
+    case s_n_llhttp__internal__n_after_start_req_45:
+    s_n_llhttp__internal__n_after_start_req_45: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_45;
+        return s_n_llhttp__internal__n_after_start_req_45;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob43, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 29;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_45;
+          return s_n_llhttp__internal__n_after_start_req_45;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_44:
-    s_n_llhttp__internal__n_start_req_44: {
+    case s_n_llhttp__internal__n_after_start_req_44:
+    s_n_llhttp__internal__n_after_start_req_44: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_44;
+        return s_n_llhttp__internal__n_after_start_req_44;
       }
       switch (*p) {
         case 'R': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_45;
+          goto s_n_llhttp__internal__n_after_start_req_45;
         }
         case 'T': {
           p++;
           match = 4;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_33:
-    s_n_llhttp__internal__n_start_req_33: {
+    case s_n_llhttp__internal__n_after_start_req_33:
+    s_n_llhttp__internal__n_after_start_req_33: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_33;
+        return s_n_llhttp__internal__n_after_start_req_33;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_34;
+          goto s_n_llhttp__internal__n_after_start_req_34;
         }
         case 'L': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_37;
+          goto s_n_llhttp__internal__n_after_start_req_37;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_38;
+          goto s_n_llhttp__internal__n_after_start_req_38;
         }
         case 'R': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_39;
+          goto s_n_llhttp__internal__n_after_start_req_39;
         }
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_44;
+          goto s_n_llhttp__internal__n_after_start_req_44;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_48:
-    s_n_llhttp__internal__n_start_req_48: {
+    case s_n_llhttp__internal__n_after_start_req_48:
+    s_n_llhttp__internal__n_after_start_req_48: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_48;
+        return s_n_llhttp__internal__n_after_start_req_48;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob44, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 17;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_48;
+          return s_n_llhttp__internal__n_after_start_req_48;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_49:
-    s_n_llhttp__internal__n_start_req_49: {
+    case s_n_llhttp__internal__n_after_start_req_49:
+    s_n_llhttp__internal__n_after_start_req_49: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_49;
+        return s_n_llhttp__internal__n_after_start_req_49;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob45, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 44;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_49;
+          return s_n_llhttp__internal__n_after_start_req_49;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_50:
-    s_n_llhttp__internal__n_start_req_50: {
+    case s_n_llhttp__internal__n_after_start_req_50:
+    s_n_llhttp__internal__n_after_start_req_50: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_50;
+        return s_n_llhttp__internal__n_after_start_req_50;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob46, 5);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 43;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_50;
+          return s_n_llhttp__internal__n_after_start_req_50;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_51:
-    s_n_llhttp__internal__n_start_req_51: {
+    case s_n_llhttp__internal__n_after_start_req_51:
+    s_n_llhttp__internal__n_after_start_req_51: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_51;
+        return s_n_llhttp__internal__n_after_start_req_51;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob47, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 20;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_51;
+          return s_n_llhttp__internal__n_after_start_req_51;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_47:
-    s_n_llhttp__internal__n_start_req_47: {
+    case s_n_llhttp__internal__n_after_start_req_47:
+    s_n_llhttp__internal__n_after_start_req_47: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_47;
+        return s_n_llhttp__internal__n_after_start_req_47;
       }
       switch (*p) {
         case 'B': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_48;
+          goto s_n_llhttp__internal__n_after_start_req_48;
         }
         case 'C': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_49;
+          goto s_n_llhttp__internal__n_after_start_req_49;
         }
         case 'D': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_50;
+          goto s_n_llhttp__internal__n_after_start_req_50;
         }
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_51;
+          goto s_n_llhttp__internal__n_after_start_req_51;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_46:
-    s_n_llhttp__internal__n_start_req_46: {
+    case s_n_llhttp__internal__n_after_start_req_46:
+    s_n_llhttp__internal__n_after_start_req_46: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_46;
+        return s_n_llhttp__internal__n_after_start_req_46;
       }
       switch (*p) {
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_47;
+          goto s_n_llhttp__internal__n_after_start_req_47;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_54:
-    s_n_llhttp__internal__n_start_req_54: {
+    case s_n_llhttp__internal__n_after_start_req_54:
+    s_n_llhttp__internal__n_after_start_req_54: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_54;
+        return s_n_llhttp__internal__n_after_start_req_54;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob48, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 14;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_54;
+          return s_n_llhttp__internal__n_after_start_req_54;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_56:
-    s_n_llhttp__internal__n_start_req_56: {
+    case s_n_llhttp__internal__n_after_start_req_56:
+    s_n_llhttp__internal__n_after_start_req_56: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_56;
+        return s_n_llhttp__internal__n_after_start_req_56;
       }
       switch (*p) {
         case 'P': {
           p++;
           match = 37;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_57:
-    s_n_llhttp__internal__n_start_req_57: {
+    case s_n_llhttp__internal__n_after_start_req_57:
+    s_n_llhttp__internal__n_after_start_req_57: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_57;
+        return s_n_llhttp__internal__n_after_start_req_57;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob49, 9);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 42;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_57;
+          return s_n_llhttp__internal__n_after_start_req_57;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_55:
-    s_n_llhttp__internal__n_start_req_55: {
+    case s_n_llhttp__internal__n_after_start_req_55:
+    s_n_llhttp__internal__n_after_start_req_55: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_55;
+        return s_n_llhttp__internal__n_after_start_req_55;
       }
       switch (*p) {
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_56;
+          goto s_n_llhttp__internal__n_after_start_req_56;
         }
         case '_': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_57;
+          goto s_n_llhttp__internal__n_after_start_req_57;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_53:
-    s_n_llhttp__internal__n_start_req_53: {
+    case s_n_llhttp__internal__n_after_start_req_53:
+    s_n_llhttp__internal__n_after_start_req_53: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_53;
+        return s_n_llhttp__internal__n_after_start_req_53;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_54;
+          goto s_n_llhttp__internal__n_after_start_req_54;
         }
         case 'T': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_55;
+          goto s_n_llhttp__internal__n_after_start_req_55;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_58:
-    s_n_llhttp__internal__n_start_req_58: {
+    case s_n_llhttp__internal__n_after_start_req_58:
+    s_n_llhttp__internal__n_after_start_req_58: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_58;
+        return s_n_llhttp__internal__n_after_start_req_58;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob50, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 33;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_58;
+          return s_n_llhttp__internal__n_after_start_req_58;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_59:
-    s_n_llhttp__internal__n_start_req_59: {
+    case s_n_llhttp__internal__n_after_start_req_59:
+    s_n_llhttp__internal__n_after_start_req_59: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_59;
+        return s_n_llhttp__internal__n_after_start_req_59;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob51, 7);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 26;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_59;
+          return s_n_llhttp__internal__n_after_start_req_59;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_52:
-    s_n_llhttp__internal__n_start_req_52: {
+    case s_n_llhttp__internal__n_after_start_req_52:
+    s_n_llhttp__internal__n_after_start_req_52: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_52;
+        return s_n_llhttp__internal__n_after_start_req_52;
       }
       switch (*p) {
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_53;
+          goto s_n_llhttp__internal__n_after_start_req_53;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_58;
+          goto s_n_llhttp__internal__n_after_start_req_58;
         }
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_59;
+          goto s_n_llhttp__internal__n_after_start_req_59;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_61:
-    s_n_llhttp__internal__n_start_req_61: {
+    case s_n_llhttp__internal__n_after_start_req_61:
+    s_n_llhttp__internal__n_after_start_req_61: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_61;
+        return s_n_llhttp__internal__n_after_start_req_61;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob52, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 40;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_61;
+          return s_n_llhttp__internal__n_after_start_req_61;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_62:
-    s_n_llhttp__internal__n_start_req_62: {
+    case s_n_llhttp__internal__n_after_start_req_62:
+    s_n_llhttp__internal__n_after_start_req_62: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_62;
+        return s_n_llhttp__internal__n_after_start_req_62;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob53, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 7;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_62;
+          return s_n_llhttp__internal__n_after_start_req_62;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_60:
-    s_n_llhttp__internal__n_start_req_60: {
+    case s_n_llhttp__internal__n_after_start_req_60:
+    s_n_llhttp__internal__n_after_start_req_60: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_60;
+        return s_n_llhttp__internal__n_after_start_req_60;
       }
       switch (*p) {
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_61;
+          goto s_n_llhttp__internal__n_after_start_req_61;
         }
         case 'R': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_62;
+          goto s_n_llhttp__internal__n_after_start_req_62;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_65:
-    s_n_llhttp__internal__n_start_req_65: {
+    case s_n_llhttp__internal__n_after_start_req_65:
+    s_n_llhttp__internal__n_after_start_req_65: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_65;
+        return s_n_llhttp__internal__n_after_start_req_65;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob54, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 18;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_65;
+          return s_n_llhttp__internal__n_after_start_req_65;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_67:
-    s_n_llhttp__internal__n_start_req_67: {
+    case s_n_llhttp__internal__n_after_start_req_67:
+    s_n_llhttp__internal__n_after_start_req_67: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_67;
+        return s_n_llhttp__internal__n_after_start_req_67;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob55, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 32;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_67;
+          return s_n_llhttp__internal__n_after_start_req_67;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_68:
-    s_n_llhttp__internal__n_start_req_68: {
+    case s_n_llhttp__internal__n_after_start_req_68:
+    s_n_llhttp__internal__n_after_start_req_68: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_68;
+        return s_n_llhttp__internal__n_after_start_req_68;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob56, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 15;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_68;
+          return s_n_llhttp__internal__n_after_start_req_68;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_66:
-    s_n_llhttp__internal__n_start_req_66: {
+    case s_n_llhttp__internal__n_after_start_req_66:
+    s_n_llhttp__internal__n_after_start_req_66: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_66;
+        return s_n_llhttp__internal__n_after_start_req_66;
       }
       switch (*p) {
         case 'I': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_67;
+          goto s_n_llhttp__internal__n_after_start_req_67;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_68;
+          goto s_n_llhttp__internal__n_after_start_req_68;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_69:
-    s_n_llhttp__internal__n_start_req_69: {
+    case s_n_llhttp__internal__n_after_start_req_69:
+    s_n_llhttp__internal__n_after_start_req_69: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_69;
+        return s_n_llhttp__internal__n_after_start_req_69;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob57, 8);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 27;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_69;
+          return s_n_llhttp__internal__n_after_start_req_69;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_64:
-    s_n_llhttp__internal__n_start_req_64: {
+    case s_n_llhttp__internal__n_after_start_req_64:
+    s_n_llhttp__internal__n_after_start_req_64: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_64;
+        return s_n_llhttp__internal__n_after_start_req_64;
       }
       switch (*p) {
         case 'B': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_65;
+          goto s_n_llhttp__internal__n_after_start_req_65;
         }
         case 'L': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_66;
+          goto s_n_llhttp__internal__n_after_start_req_66;
         }
         case 'S': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_69;
+          goto s_n_llhttp__internal__n_after_start_req_69;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_63:
-    s_n_llhttp__internal__n_start_req_63: {
+    case s_n_llhttp__internal__n_after_start_req_63:
+    s_n_llhttp__internal__n_after_start_req_63: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_63;
+        return s_n_llhttp__internal__n_after_start_req_63;
       }
       switch (*p) {
         case 'N': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_64;
+          goto s_n_llhttp__internal__n_after_start_req_64;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req:
-    s_n_llhttp__internal__n_start_req: {
+    case s_n_llhttp__internal__n_after_start_req:
+    s_n_llhttp__internal__n_after_start_req: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req;
+        return s_n_llhttp__internal__n_after_start_req;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_1;
+          goto s_n_llhttp__internal__n_after_start_req_1;
         }
         case 'B': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_4;
+          goto s_n_llhttp__internal__n_after_start_req_4;
         }
         case 'C': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_5;
+          goto s_n_llhttp__internal__n_after_start_req_5;
         }
         case 'D': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_10;
+          goto s_n_llhttp__internal__n_after_start_req_10;
         }
         case 'F': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_14;
+          goto s_n_llhttp__internal__n_after_start_req_14;
         }
         case 'G': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_15;
+          goto s_n_llhttp__internal__n_after_start_req_15;
         }
         case 'H': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_18;
+          goto s_n_llhttp__internal__n_after_start_req_18;
         }
         case 'L': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_19;
+          goto s_n_llhttp__internal__n_after_start_req_19;
         }
         case 'M': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_22;
+          goto s_n_llhttp__internal__n_after_start_req_22;
         }
         case 'N': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_31;
+          goto s_n_llhttp__internal__n_after_start_req_31;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_32;
+          goto s_n_llhttp__internal__n_after_start_req_32;
         }
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_33;
+          goto s_n_llhttp__internal__n_after_start_req_33;
         }
         case 'R': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_46;
+          goto s_n_llhttp__internal__n_after_start_req_46;
         }
         case 'S': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_52;
+          goto s_n_llhttp__internal__n_after_start_req_52;
         }
         case 'T': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_60;
+          goto s_n_llhttp__internal__n_after_start_req_60;
         }
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_63;
+          goto s_n_llhttp__internal__n_after_start_req_63;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_69;
+          goto s_n_llhttp__internal__n_error_90;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_method_1:
+    s_n_llhttp__internal__n_span_start_llhttp__on_method_1: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_method_1;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_method;
+      goto s_n_llhttp__internal__n_after_start_req;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_invoke_llhttp__on_status_complete:
     s_n_llhttp__internal__n_invoke_llhttp__on_status_complete: {
       switch (llhttp__on_status_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_headers_start;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_20;
         default:
-          goto s_n_llhttp__internal__n_header_field_start;
+          goto s_n_llhttp__internal__n_error_75;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_line_almost_done:
     s_n_llhttp__internal__n_res_line_almost_done: {
       if (p == endp) {
@@ -5366,15 +5803,15 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_invoke_llhttp__on_status_complete;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_60;
+          goto s_n_llhttp__internal__n_error_76;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_status:
     s_n_llhttp__internal__n_res_status: {
@@ -5441,24 +5878,150 @@
           goto s_n_llhttp__internal__n_res_status_start;
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_res_status_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_61;
+          goto s_n_llhttp__internal__n_error_77;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_res_status_code_digit_3:
+    s_n_llhttp__internal__n_res_status_code_digit_3: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_res_status_code_digit_3;
+      }
+      switch (*p) {
+        case '0': {
+          p++;
+          match = 0;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '1': {
+          p++;
+          match = 1;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '2': {
+          p++;
+          match = 2;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '3': {
+          p++;
+          match = 3;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '4': {
+          p++;
+          match = 4;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '5': {
+          p++;
+          match = 5;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '6': {
+          p++;
+          match = 6;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '7': {
+          p++;
+          match = 7;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '8': {
+          p++;
+          match = 8;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '9': {
+          p++;
+          match = 9;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_error_79;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_res_status_code_digit_2:
+    s_n_llhttp__internal__n_res_status_code_digit_2: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_res_status_code_digit_2;
+      }
+      switch (*p) {
+        case '0': {
+          p++;
+          match = 0;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '1': {
+          p++;
+          match = 1;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '2': {
+          p++;
+          match = 2;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '3': {
+          p++;
+          match = 3;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '4': {
+          p++;
+          match = 4;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '5': {
+          p++;
+          match = 5;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '6': {
+          p++;
+          match = 6;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '7': {
+          p++;
+          match = 7;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '8': {
+          p++;
+          match = 8;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '9': {
+          p++;
+          match = 9;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_error_81;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_res_status_code:
-    s_n_llhttp__internal__n_res_status_code: {
+    case s_n_llhttp__internal__n_res_status_code_digit_1:
+    s_n_llhttp__internal__n_res_status_code_digit_1: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_res_status_code;
+        return s_n_llhttp__internal__n_res_status_code_digit_1;
       }
       switch (*p) {
         case '0': {
           p++;
           match = 0;
           goto s_n_llhttp__internal__n_invoke_mul_add_status_code;
         }
@@ -5504,37 +6067,70 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_mul_add_status_code;
         }
         default: {
-          goto s_n_llhttp__internal__n_res_status_code_otherwise;
+          goto s_n_llhttp__internal__n_error_83;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_res_http_end:
-    s_n_llhttp__internal__n_res_http_end: {
+    case s_n_llhttp__internal__n_res_after_version:
+    s_n_llhttp__internal__n_res_after_version: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_res_http_end;
+        return s_n_llhttp__internal__n_res_after_version;
       }
       switch (*p) {
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_invoke_update_status_code;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1:
+    s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1: {
+      switch (llhttp__on_version_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_res_after_version;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_21;
+        default:
+          goto s_n_llhttp__internal__n_error_74;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_73:
+    s_n_llhttp__internal__n_error_73: {
+      state->error = 0x9;
+      state->reason = "Invalid HTTP version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_85:
+    s_n_llhttp__internal__n_error_85: {
+      state->error = 0x9;
+      state->reason = "Invalid minor version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_res_http_minor:
     s_n_llhttp__internal__n_res_http_minor: {
       if (p == endp) {
         return s_n_llhttp__internal__n_res_http_minor;
       }
       switch (*p) {
         case '0': {
@@ -5584,37 +6180,57 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_minor_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_65;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_7;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_86:
+    s_n_llhttp__internal__n_error_86: {
+      state->error = 0x9;
+      state->reason = "Expected dot";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_res_http_dot:
     s_n_llhttp__internal__n_res_http_dot: {
       if (p == endp) {
         return s_n_llhttp__internal__n_res_http_dot;
       }
       switch (*p) {
         case '.': {
           p++;
           goto s_n_llhttp__internal__n_res_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_66;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_8;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_87:
+    s_n_llhttp__internal__n_error_87: {
+      state->error = 0x9;
+      state->reason = "Invalid major version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_res_http_major:
     s_n_llhttp__internal__n_res_http_major: {
       if (p == endp) {
         return s_n_llhttp__internal__n_res_http_major;
       }
       switch (*p) {
         case '0': {
@@ -5664,44 +6280,68 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_major_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_67;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_9;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_version_1:
+    s_n_llhttp__internal__n_span_start_llhttp__on_version_1: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_version_1;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_version;
+      goto s_n_llhttp__internal__n_res_http_major;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_start_res:
     s_n_llhttp__internal__n_start_res: {
       llparse_match_t match_seq;
       
       if (p == endp) {
         return s_n_llhttp__internal__n_start_res;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob58, 5);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_res_http_major;
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_version_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_res;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_70;
+          goto s_n_llhttp__internal__n_error_91;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_method_complete:
+    s_n_llhttp__internal__n_invoke_llhttp__on_method_complete: {
+      switch (llhttp__on_method_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_req_first_space_before_url;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_19;
+        default:
+          goto s_n_llhttp__internal__n_error_1;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_or_res_method_2:
     s_n_llhttp__internal__n_req_or_res_method_2: {
       llparse_match_t match_seq;
       
       if (p == endp) {
         return s_n_llhttp__internal__n_req_or_res_method_2;
       }
@@ -5713,39 +6353,48 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_method;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_or_res_method_2;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_68;
+          goto s_n_llhttp__internal__n_error_88;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_update_type_1:
+    s_n_llhttp__internal__n_invoke_update_type_1: {
+      switch (llhttp__internal__c_update_type_1(state, p, endp)) {
+        default:
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_version_1;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_or_res_method_3:
     s_n_llhttp__internal__n_req_or_res_method_3: {
       llparse_match_t match_seq;
       
       if (p == endp) {
         return s_n_llhttp__internal__n_req_or_res_method_3;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob60, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_type_1;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_or_res_method_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_68;
+          goto s_n_llhttp__internal__n_error_88;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method_1:
     s_n_llhttp__internal__n_req_or_res_method_1: {
@@ -5758,15 +6407,15 @@
           goto s_n_llhttp__internal__n_req_or_res_method_2;
         }
         case 'T': {
           p++;
           goto s_n_llhttp__internal__n_req_or_res_method_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_68;
+          goto s_n_llhttp__internal__n_error_88;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method:
     s_n_llhttp__internal__n_req_or_res_method: {
@@ -5775,49 +6424,69 @@
       }
       switch (*p) {
         case 'H': {
           p++;
           goto s_n_llhttp__internal__n_req_or_res_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_68;
+          goto s_n_llhttp__internal__n_error_88;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_method:
+    s_n_llhttp__internal__n_span_start_llhttp__on_method: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_method;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_method;
+      goto s_n_llhttp__internal__n_req_or_res_method;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_start_req_or_res:
     s_n_llhttp__internal__n_start_req_or_res: {
       if (p == endp) {
         return s_n_llhttp__internal__n_start_req_or_res;
       }
       switch (*p) {
         case 'H': {
-          goto s_n_llhttp__internal__n_req_or_res_method;
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_method;
         }
         default: {
           goto s_n_llhttp__internal__n_invoke_update_type_2;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_load_type:
     s_n_llhttp__internal__n_invoke_load_type: {
       switch (llhttp__internal__c_load_type(state, p, endp)) {
         case 1:
-          goto s_n_llhttp__internal__n_start_req;
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_method_1;
         case 2:
           goto s_n_llhttp__internal__n_start_res;
         default:
           goto s_n_llhttp__internal__n_start_req_or_res;
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_update_finish:
+    s_n_llhttp__internal__n_invoke_update_finish: {
+      switch (llhttp__internal__c_update_finish(state, p, endp)) {
+        default:
+          goto s_n_llhttp__internal__n_invoke_llhttp__on_message_begin;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_start:
     s_n_llhttp__internal__n_start: {
       if (p == endp) {
         return s_n_llhttp__internal__n_start;
       }
       switch (*p) {
         case 10: {
@@ -5825,34 +6494,34 @@
           goto s_n_llhttp__internal__n_start;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_finish;
+          goto s_n_llhttp__internal__n_invoke_load_initial_message_completed;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     default:
       /* UNREACHABLE */
       abort();
   }
-  s_n_llhttp__internal__n_error_1: {
+  s_n_llhttp__internal__n_error_2: {
     state->error = 0x7;
     state->reason = "Invalid characters in url (strict mode)";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_52: {
+  s_n_llhttp__internal__n_error_68: {
     state->error = 0x7;
     state->reason = "Invalid characters in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -5861,90 +6530,106 @@
     switch (llhttp__internal__c_update_finish_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_start;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_4: {
+  s_n_llhttp__internal__n_invoke_update_initial_message_completed: {
+    switch (llhttp__internal__c_update_initial_message_completed(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_invoke_update_finish_2;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_content_length: {
+    switch (llhttp__internal__c_update_content_length(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_invoke_update_initial_message_completed;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_7: {
     state->error = 0x5;
     state->reason = "Data after `Connection: close`";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags: {
-    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_1: {
+    switch (llhttp__internal__c_test_lenient_flags_1(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_update_finish_2;
+        goto s_n_llhttp__internal__n_invoke_update_initial_message_completed;
       default:
         goto s_n_llhttp__internal__n_closed;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_update_finish_1: {
     switch (llhttp__internal__c_update_finish_1(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_pause_5: {
+  s_n_llhttp__internal__n_pause_11: {
     state->error = 0x15;
     state->reason = "on_message_complete pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_is_equal_upgrade;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_14: {
+  s_n_llhttp__internal__n_error_28: {
     state->error = 0x12;
     state->reason = "`on_message_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_pause_7: {
+  s_n_llhttp__internal__n_pause_13: {
     state->error = 0x15;
     state->reason = "on_chunk_complete pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_17: {
+  s_n_llhttp__internal__n_error_31: {
     state->error = 0x14;
     state->reason = "`on_chunk_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_chunk_complete_1: {
     switch (llhttp__on_chunk_complete(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2;
       case 21:
-        goto s_n_llhttp__internal__n_pause_7;
+        goto s_n_llhttp__internal__n_pause_13;
       default:
-        goto s_n_llhttp__internal__n_error_17;
+        goto s_n_llhttp__internal__n_error_31;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_16: {
+  s_n_llhttp__internal__n_error_30: {
     state->error = 0x4;
     state->reason = "Content-Length can't be present with Transfer-Encoding";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -5954,15 +6639,15 @@
     state->reason = "on_message_complete pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_pause_1;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_5: {
+  s_n_llhttp__internal__n_error_8: {
     state->error = 0x12;
     state->reason = "`on_message_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -5970,59 +6655,59 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_1: {
     switch (llhttp__on_message_complete(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_pause_1;
       case 21:
         goto s_n_llhttp__internal__n_pause_2;
       default:
-        goto s_n_llhttp__internal__n_error_5;
+        goto s_n_llhttp__internal__n_error_8;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_12: {
+  s_n_llhttp__internal__n_error_26: {
     state->error = 0xc;
     state->reason = "Chunk size overflow";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_pause_3: {
     state->error = 0x15;
     state->reason = "on_chunk_complete pause";
     state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_update_content_length;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_update_content_length_1;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_7: {
+  s_n_llhttp__internal__n_error_10: {
     state->error = 0x14;
     state->reason = "`on_chunk_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_chunk_complete: {
     switch (llhttp__on_chunk_complete(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_invoke_update_content_length;
+        goto s_n_llhttp__internal__n_invoke_update_content_length_1;
       case 21:
         goto s_n_llhttp__internal__n_pause_3;
       default:
-        goto s_n_llhttp__internal__n_error_7;
+        goto s_n_llhttp__internal__n_error_10;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_8: {
+  s_n_llhttp__internal__n_error_11: {
     state->error = 0x2;
     state->reason = "Expected CRLF after chunk";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6057,15 +6742,15 @@
     state->reason = "on_chunk_header pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_is_equal_content_length;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_6: {
+  s_n_llhttp__internal__n_error_9: {
     state->error = 0x13;
     state->reason = "`on_chunk_header` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6073,57 +6758,356 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_chunk_header: {
     switch (llhttp__on_chunk_header(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_is_equal_content_length;
       case 21:
         goto s_n_llhttp__internal__n_pause_4;
       default:
-        goto s_n_llhttp__internal__n_error_6;
+        goto s_n_llhttp__internal__n_error_9;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_9: {
+  s_n_llhttp__internal__n_error_12: {
     state->error = 0x2;
     state->reason = "Expected LF after chunk size";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_10: {
+  s_n_llhttp__internal__n_error_13: {
     state->error = 0x2;
-    state->reason = "Invalid character in chunk parameters";
+    state->reason = "Invalid character in chunk extensions";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_11: {
+  s_n_llhttp__internal__n_error_14: {
+    state->error = 0x2;
+    state->reason = "Invalid character in chunk extensions";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_5: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_name pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_size_almost_done;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_15: {
+    state->error = 0x22;
+    state->reason = "`on_chunk_extension_name` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_name(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_6: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_name pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_extensions;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_16: {
+    state->error = 0x22;
+    state->reason = "`on_chunk_extension_name` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_1: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_name(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_7: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_value pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_size_almost_done;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_18: {
+    state->error = 0x23;
+    state->reason = "`on_chunk_extension_value` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_20: {
+    state->error = 0x2;
+    state->reason = "Invalid character in chunk extensions quote value";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_8: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_value pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_extension_quoted_value_done;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_19: {
+    state->error = 0x23;
+    state->reason = "`on_chunk_extension_value` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_1: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_21;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_21;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_9: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_value pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_size_otherwise;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_22: {
+    state->error = 0x23;
+    state->reason = "`on_chunk_extension_value` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_3: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_4: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_23;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_23;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_10: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_name pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_extension_value;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_17: {
+    state->error = 0x22;
+    state->reason = "`on_chunk_extension_name` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_2: {
+    switch (llhttp__on_chunk_extension_name_complete(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_chunk_extension_value;
+      case 21:
+        goto s_n_llhttp__internal__n_pause_10;
+      default:
+        goto s_n_llhttp__internal__n_error_17;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_name(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_3: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_name(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_24;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_24;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_25: {
     state->error = 0xc;
     state->reason = "Invalid character in chunk size";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_mul_add_content_length: {
     switch (llhttp__internal__c_mul_add_content_length(state, p, endp, match)) {
       case 1:
-        goto s_n_llhttp__internal__n_error_12;
+        goto s_n_llhttp__internal__n_error_26;
       default:
         goto s_n_llhttp__internal__n_chunk_size;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_13: {
+  s_n_llhttp__internal__n_error_27: {
     state->error = 0xc;
     state->reason = "Invalid character in chunk size";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6149,15 +7133,15 @@
     switch (llhttp__internal__c_update_finish_3(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_span_start_llhttp__on_body_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_15: {
+  s_n_llhttp__internal__n_error_29: {
     state->error = 0xf;
     state->reason = "Request has invalid `Transfer-Encoding`";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6167,15 +7151,15 @@
     state->reason = "on_message_complete pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__after_message_complete;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_3: {
+  s_n_llhttp__internal__n_error_6: {
     state->error = 0x12;
     state->reason = "`on_message_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6183,15 +7167,15 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_message_complete: {
     switch (llhttp__on_message_complete(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_llhttp__after_message_complete;
       case 21:
         goto s_n_llhttp__internal__n_pause;
       default:
-        goto s_n_llhttp__internal__n_error_3;
+        goto s_n_llhttp__internal__n_error_6;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_1: {
     switch (llhttp__internal__c_or_flags_1(state, p, endp)) {
       default:
@@ -6212,24 +7196,24 @@
     switch (llhttp__internal__c_update_upgrade(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_or_flags_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_pause_6: {
+  s_n_llhttp__internal__n_pause_12: {
     state->error = 0x15;
     state->reason = "Paused by on_headers_complete";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_2: {
+  s_n_llhttp__internal__n_error_5: {
     state->error = 0x11;
     state->reason = "User callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6239,43 +7223,43 @@
       case 0:
         goto s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete;
       case 1:
         goto s_n_llhttp__internal__n_invoke_or_flags_1;
       case 2:
         goto s_n_llhttp__internal__n_invoke_update_upgrade;
       case 21:
-        goto s_n_llhttp__internal__n_pause_6;
+        goto s_n_llhttp__internal__n_pause_12;
       default:
-        goto s_n_llhttp__internal__n_error_2;
+        goto s_n_llhttp__internal__n_error_5;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__before_headers_complete: {
     switch (llhttp__before_headers_complete(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_headers_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_1: {
-    switch (llhttp__internal__c_test_lenient_flags_1(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_2: {
+    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_error_16;
+        goto s_n_llhttp__internal__n_error_30;
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__before_headers_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_test_flags_1: {
     switch (llhttp__internal__c_test_flags_1(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_1;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_2;
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__before_headers_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_test_flags: {
@@ -6284,15 +7268,15 @@
         goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_complete_1;
       default:
         goto s_n_llhttp__internal__n_invoke_test_flags_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_18: {
+  s_n_llhttp__internal__n_error_32: {
     state->error = 0x2;
     state->reason = "Expected LF after headers";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6303,41 +7287,78 @@
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_field(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) (p + 1);
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_19;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_33;
       return s_error;
     }
     p++;
-    goto s_n_llhttp__internal__n_error_19;
+    goto s_n_llhttp__internal__n_error_33;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_2: {
-    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_3: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
       case 1:
         goto s_n_llhttp__internal__n_header_field_colon_discard_ws;
       default:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_20: {
+  s_n_llhttp__internal__n_error_36: {
+    state->error = 0xa;
+    state->reason = "Invalid header value char";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_5: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_ws;
+      default:
+        goto s_n_llhttp__internal__n_error_36;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_38: {
     state->error = 0xb;
     state->reason = "Empty Content-Length";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_pause_14: {
+    state->error = 0x15;
+    state->reason = "on_header_value_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_header_field_start;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_37: {
+    state->error = 0x1d;
+    state->reason = "`on_header_value_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_value: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
@@ -6406,71 +7427,118 @@
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_header_state: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 2:
-        goto s_n_llhttp__internal__n_error_20;
+        goto s_n_llhttp__internal__n_error_38;
       default:
         goto s_n_llhttp__internal__n_invoke_load_header_state_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_21: {
+  s_n_llhttp__internal__n_error_35: {
+    state->error = 0xa;
+    state->reason = "Invalid header value char";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_4: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_lws;
+      default:
+        goto s_n_llhttp__internal__n_error_35;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_39: {
     state->error = 0x2;
     state->reason = "Expected LF after CR";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_6: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_lws;
+      default:
+        goto s_n_llhttp__internal__n_error_39;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_update_header_state_1: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_header_state_3: {
+    switch (llhttp__internal__c_load_header_state(state, p, endp)) {
+      case 8:
+        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+      default:
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_header_state_2: {
     switch (llhttp__internal__c_update_header_state(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_7: {
     switch (llhttp__internal__c_or_flags_3(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_8: {
     switch (llhttp__internal__c_or_flags_4(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_9: {
     switch (llhttp__internal__c_or_flags_5(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_10: {
     switch (llhttp__internal__c_or_flags_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_header_state_3: {
+  s_n_llhttp__internal__n_invoke_load_header_state_4: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 5:
         goto s_n_llhttp__internal__n_invoke_or_flags_7;
       case 6:
         goto s_n_llhttp__internal__n_invoke_or_flags_8;
       case 7:
         goto s_n_llhttp__internal__n_invoke_or_flags_9;
@@ -6478,15 +7546,15 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_10;
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_22: {
+  s_n_llhttp__internal__n_error_40: {
     state->error = 0x3;
     state->reason = "Missing expected LF after header value";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6549,83 +7617,73 @@
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
-      state->error_pos = (const char*) (p + 1);
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_23;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_41;
       return s_error;
     }
-    p++;
-    goto s_n_llhttp__internal__n_error_23;
-    /* UNREACHABLE */;
-    abort();
-  }
-  s_n_llhttp__internal__n_error_24: {
-    state->error = 0xa;
-    state->reason = "Invalid header value char";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+    goto s_n_llhttp__internal__n_error_41;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_3: {
-    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_7: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
       case 1:
         goto s_n_llhttp__internal__n_header_value_lenient;
       default:
-        goto s_n_llhttp__internal__n_header_value_lenient_failed;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_3: {
+  s_n_llhttp__internal__n_invoke_update_header_state_4: {
     switch (llhttp__internal__c_update_header_state(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_11: {
     switch (llhttp__internal__c_or_flags_3(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_12: {
     switch (llhttp__internal__c_or_flags_4(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_13: {
     switch (llhttp__internal__c_or_flags_5(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_14: {
     switch (llhttp__internal__c_or_flags_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_header_state_4: {
+  s_n_llhttp__internal__n_invoke_load_header_state_5: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 5:
         goto s_n_llhttp__internal__n_invoke_or_flags_11;
       case 6:
         goto s_n_llhttp__internal__n_invoke_or_flags_12;
       case 7:
         goto s_n_llhttp__internal__n_invoke_or_flags_13;
@@ -6633,40 +7691,40 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_14;
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_4: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_5: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_token;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_2: {
-    switch (llhttp__internal__c_update_header_state_2(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_3: {
+    switch (llhttp__internal__c_update_header_state_3(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_5: {
-    switch (llhttp__internal__c_update_header_state_5(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_6: {
+    switch (llhttp__internal__c_update_header_state_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_6: {
-    switch (llhttp__internal__c_update_header_state_6(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_7: {
+    switch (llhttp__internal__c_update_header_state_7(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5: {
@@ -6675,18 +7733,18 @@
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) p;
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_26;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_43;
       return s_error;
     }
-    goto s_n_llhttp__internal__n_error_26;
+    goto s_n_llhttp__internal__n_error_43;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_mul_add_content_length_1: {
     switch (llhttp__internal__c_mul_add_content_length_1(state, p, endp, match)) {
       case 1:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5;
@@ -6710,60 +7768,60 @@
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) p;
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_27;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_44;
       return s_error;
     }
-    goto s_n_llhttp__internal__n_error_27;
+    goto s_n_llhttp__internal__n_error_44;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_25: {
+  s_n_llhttp__internal__n_error_42: {
     state->error = 0x4;
     state->reason = "Duplicate Content-Length";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_test_flags_2: {
     switch (llhttp__internal__c_test_flags_2(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_header_value_content_length;
       default:
-        goto s_n_llhttp__internal__n_error_25;
+        goto s_n_llhttp__internal__n_error_42;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_value_8: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) (p + 1);
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_29;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_46;
       return s_error;
     }
     p++;
-    goto s_n_llhttp__internal__n_error_29;
+    goto s_n_llhttp__internal__n_error_46;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_7: {
-    switch (llhttp__internal__c_update_header_state_7(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_8: {
+    switch (llhttp__internal__c_update_header_state_8(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_otherwise;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_value_7: {
@@ -6772,44 +7830,44 @@
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) (p + 1);
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_28;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_45;
       return s_error;
     }
     p++;
-    goto s_n_llhttp__internal__n_error_28;
+    goto s_n_llhttp__internal__n_error_45;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_4: {
-    switch (llhttp__internal__c_test_lenient_flags_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_8: {
+    switch (llhttp__internal__c_test_lenient_flags_8(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_7;
       default:
         goto s_n_llhttp__internal__n_header_value_te_chunked;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_type_1: {
     switch (llhttp__internal__c_load_type(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_4;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_8;
       default:
         goto s_n_llhttp__internal__n_header_value_te_chunked;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_8: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_9: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_and_flags: {
@@ -6824,28 +7882,28 @@
     switch (llhttp__internal__c_or_flags_16(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_and_flags;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_5: {
-    switch (llhttp__internal__c_test_lenient_flags_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_9: {
+    switch (llhttp__internal__c_test_lenient_flags_8(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_8;
       default:
         goto s_n_llhttp__internal__n_invoke_or_flags_17;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_type_2: {
     switch (llhttp__internal__c_load_type(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_5;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_9;
       default:
         goto s_n_llhttp__internal__n_invoke_or_flags_17;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_16: {
@@ -6865,15 +7923,15 @@
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_18: {
     switch (llhttp__internal__c_or_flags_18(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_8;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_9;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_header_state_2: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 1:
@@ -6886,14 +7944,32 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_18;
       default:
         goto s_n_llhttp__internal__n_header_value;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_pause_15: {
+    state->error = 0x15;
+    state->reason = "on_header_field_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_header_value_discard_ws;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_34: {
+    state->error = 0x1c;
+    state->reason = "`on_header_field_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_field_1: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_field(state, start, p);
@@ -6922,51 +7998,92 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_30: {
+  s_n_llhttp__internal__n_error_47: {
     state->error = 0xa;
     state->reason = "Invalid header token";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_9: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_10: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_field_general;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_header_state: {
     switch (llhttp__internal__c_store_header_state(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_header_field_colon;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_10: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_11: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_field_general;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_error_4: {
+    state->error = 0x1e;
+    state->reason = "Unexpected space after start line";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_field_start;
+      default:
+        goto s_n_llhttp__internal__n_error_4;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_16: {
+    state->error = 0x15;
+    state->reason = "on_url_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_headers_start;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_3: {
+    state->error = 0x1a;
+    state->reason = "`on_url_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_llhttp__on_url_complete: {
     switch (llhttp__on_url_complete(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_headers_start;
+      case 21:
+        goto s_n_llhttp__internal__n_pause_16;
       default:
-        goto s_n_llhttp__internal__n_header_field_start;
+        goto s_n_llhttp__internal__n_error_3;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_update_http_minor: {
     switch (llhttp__internal__c_update_http_minor(state, p, endp)) {
       default:
@@ -6996,15 +8113,15 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http09;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http09;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_31: {
+  s_n_llhttp__internal__n_error_48: {
     state->error = 0x7;
     state->reason = "Expected CRLF";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7022,350 +8139,402 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_lf_to_http09;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_lf_to_http09;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_36: {
+  s_n_llhttp__internal__n_error_54: {
     state->error = 0x17;
     state->reason = "Pause on PRI/Upgrade";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_37: {
+  s_n_llhttp__internal__n_error_55: {
     state->error = 0x9;
     state->reason = "Expected HTTP/2 Connection Preface";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_35: {
+  s_n_llhttp__internal__n_error_53: {
     state->error = 0x9;
     state->reason = "Expected CRLF after version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_method_1: {
-    switch (llhttp__internal__c_load_method(state, p, endp)) {
-      case 34:
-        goto s_n_llhttp__internal__n_req_pri_upgrade;
-      default:
-        goto s_n_llhttp__internal__n_req_http_complete;
-    }
+  s_n_llhttp__internal__n_pause_17: {
+    state->error = 0x15;
+    state->reason = "on_version_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_load_method_1;
+    return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_34: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
+  s_n_llhttp__internal__n_error_52: {
+    state->error = 0x21;
+    state->reason = "`on_version_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_1: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_version_complete;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_version_complete;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_version: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_51;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_51;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_load_http_minor: {
     switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
       case 9:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       default:
-        goto s_n_llhttp__internal__n_error_34;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_38: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
-    /* UNREACHABLE */;
-    abort();
-  }
   s_n_llhttp__internal__n_invoke_load_http_minor_1: {
     switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       case 1:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       default:
-        goto s_n_llhttp__internal__n_error_38;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_39: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
-    /* UNREACHABLE */;
-    abort();
-  }
   s_n_llhttp__internal__n_invoke_load_http_minor_2: {
     switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       default:
-        goto s_n_llhttp__internal__n_error_39;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_33: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
-    /* UNREACHABLE */;
-    abort();
-  }
   s_n_llhttp__internal__n_invoke_load_http_major: {
     switch (llhttp__internal__c_load_http_major(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_load_http_minor;
       case 1:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_1;
       case 2:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_2;
       default:
-        goto s_n_llhttp__internal__n_error_33;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_6: {
-    switch (llhttp__internal__c_test_lenient_flags_6(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_10: {
+    switch (llhttp__internal__c_test_lenient_flags_10(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       default:
         goto s_n_llhttp__internal__n_invoke_load_http_major;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_http_minor: {
     switch (llhttp__internal__c_store_http_minor(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_6;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_10;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_40: {
-    state->error = 0x9;
-    state->reason = "Invalid minor version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_56;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_56;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_41: {
-    state->error = 0x9;
-    state->reason = "Expected dot";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_3: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_57;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_57;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_http_major: {
     switch (llhttp__internal__c_store_http_major(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_req_http_dot;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_42: {
-    state->error = 0x9;
-    state->reason = "Invalid major version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_4: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_58;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_58;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_32: {
+  s_n_llhttp__internal__n_error_50: {
     state->error = 0x8;
     state->reason = "Invalid method for HTTP/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_method: {
     switch (llhttp__internal__c_load_method(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 1:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 2:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 3:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 4:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 5:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 6:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 7:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 8:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 9:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 10:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 11:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 12:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 13:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 14:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 15:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 16:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 17:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 18:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 19:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 20:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 21:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 22:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 23:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 24:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 25:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 26:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 27:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 28:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 29:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 30:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 31:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 32:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 33:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 34:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       default:
-        goto s_n_llhttp__internal__n_error_32;
+        goto s_n_llhttp__internal__n_error_50;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_45: {
+  s_n_llhttp__internal__n_error_61: {
     state->error = 0x8;
     state->reason = "Expected HTTP/";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_43: {
+  s_n_llhttp__internal__n_error_59: {
     state->error = 0x8;
     state->reason = "Expected SOURCE method for ICE/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_method_2: {
     switch (llhttp__internal__c_load_method(state, p, endp)) {
       case 33:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       default:
-        goto s_n_llhttp__internal__n_error_43;
+        goto s_n_llhttp__internal__n_error_59;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_44: {
+  s_n_llhttp__internal__n_error_60: {
     state->error = 0x8;
     state->reason = "Invalid method for RTSP/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_method_3: {
     switch (llhttp__internal__c_load_method(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 3:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 6:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 35:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 36:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 37:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 38:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 39:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 40:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 41:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 42:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 43:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 44:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 45:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       default:
-        goto s_n_llhttp__internal__n_error_44;
+        goto s_n_llhttp__internal__n_error_60;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_pause_18: {
+    state->error = 0x15;
+    state->reason = "on_url_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_req_http_start;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_49: {
+    state->error = 0x1a;
+    state->reason = "`on_url_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_llhttp__on_url_complete_1: {
     switch (llhttp__on_url_complete(state, p, endp)) {
-      default:
+      case 0:
         goto s_n_llhttp__internal__n_req_http_start;
+      case 21:
+        goto s_n_llhttp__internal__n_pause_18;
+      default:
+        goto s_n_llhttp__internal__n_error_49;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_url_5: {
     const unsigned char* start;
     int err;
@@ -7430,15 +8599,15 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_46: {
+  s_n_llhttp__internal__n_error_62: {
     state->error = 0x7;
     state->reason = "Invalid char in url fragment start";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7490,24 +8659,24 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_47: {
+  s_n_llhttp__internal__n_error_63: {
     state->error = 0x7;
     state->reason = "Invalid char in url query";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_48: {
+  s_n_llhttp__internal__n_error_64: {
     state->error = 0x7;
     state->reason = "Invalid char in url path";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7610,60 +8779,60 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_49: {
+  s_n_llhttp__internal__n_error_65: {
     state->error = 0x7;
     state->reason = "Double @ in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_50: {
+  s_n_llhttp__internal__n_error_66: {
     state->error = 0x7;
     state->reason = "Unexpected char in url server";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_51: {
+  s_n_llhttp__internal__n_error_67: {
     state->error = 0x7;
     state->reason = "Unexpected char in url server";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_53: {
+  s_n_llhttp__internal__n_error_69: {
     state->error = 0x7;
     state->reason = "Unexpected char in url schema";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_54: {
+  s_n_llhttp__internal__n_error_70: {
     state->error = 0x7;
     state->reason = "Unexpected char in url schema";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_55: {
+  s_n_llhttp__internal__n_error_71: {
     state->error = 0x7;
     state->reason = "Unexpected start char in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7674,60 +8843,121 @@
         goto s_n_llhttp__internal__n_url_entry_normal;
       default:
         goto s_n_llhttp__internal__n_url_entry_connect;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_56: {
+  s_n_llhttp__internal__n_error_72: {
     state->error = 0x6;
     state->reason = "Expected space after method";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_pause_22: {
+    state->error = 0x15;
+    state->reason = "on_method_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_req_first_space_before_url;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_89: {
+    state->error = 0x20;
+    state->reason = "`on_method_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_method_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_method(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_store_method_1: {
     switch (llhttp__internal__c_store_method(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_req_first_space_before_url;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_method_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_69: {
+  s_n_llhttp__internal__n_error_90: {
     state->error = 0x6;
     state->reason = "Invalid method encountered";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_59: {
+  s_n_llhttp__internal__n_error_82: {
     state->error = 0xd;
-    state->reason = "Response overflow";
+    state->reason = "Invalid status code";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_mul_add_status_code: {
-    switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
-      case 1:
-        goto s_n_llhttp__internal__n_error_59;
-      default:
-        goto s_n_llhttp__internal__n_res_status_code;
-    }
+  s_n_llhttp__internal__n_error_80: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_60: {
+  s_n_llhttp__internal__n_error_78: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_20: {
+    state->error = 0x15;
+    state->reason = "on_status_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_headers_start;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_75: {
+    state->error = 0x1b;
+    state->reason = "`on_status_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_76: {
     state->error = 0x2;
     state->reason = "Expected LF after CR";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7764,226 +8994,367 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_res_line_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_61: {
+  s_n_llhttp__internal__n_error_77: {
     state->error = 0xd;
     state->reason = "Invalid response status";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_status_code: {
-    switch (llhttp__internal__c_update_status_code(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_mul_add_status_code_2: {
+    switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
+      case 1:
+        goto s_n_llhttp__internal__n_error_78;
       default:
-        goto s_n_llhttp__internal__n_res_status_code;
+        goto s_n_llhttp__internal__n_res_status_code_otherwise;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_62: {
-    state->error = 0x9;
-    state->reason = "Expected space after version";
+  s_n_llhttp__internal__n_error_79: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_58: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
+  s_n_llhttp__internal__n_invoke_mul_add_status_code_1: {
+    switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
+      case 1:
+        goto s_n_llhttp__internal__n_error_80;
+      default:
+        goto s_n_llhttp__internal__n_res_status_code_digit_3;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_81: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_http_minor_3: {
-    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
-      case 9:
-        goto s_n_llhttp__internal__n_res_http_end;
+  s_n_llhttp__internal__n_invoke_mul_add_status_code: {
+    switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
+      case 1:
+        goto s_n_llhttp__internal__n_error_82;
       default:
-        goto s_n_llhttp__internal__n_error_58;
+        goto s_n_llhttp__internal__n_res_status_code_digit_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_63: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
+  s_n_llhttp__internal__n_error_83: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_http_minor_4: {
-    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
-      case 0:
-        goto s_n_llhttp__internal__n_res_http_end;
-      case 1:
-        goto s_n_llhttp__internal__n_res_http_end;
+  s_n_llhttp__internal__n_invoke_update_status_code: {
+    switch (llhttp__internal__c_update_status_code(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_error_63;
+        goto s_n_llhttp__internal__n_res_status_code_digit_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_64: {
+  s_n_llhttp__internal__n_error_84: {
     state->error = 0x9;
-    state->reason = "Invalid HTTP version";
+    state->reason = "Expected space after version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_http_minor_5: {
+  s_n_llhttp__internal__n_pause_21: {
+    state->error = 0x15;
+    state->reason = "on_version_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_res_after_version;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_74: {
+    state->error = 0x21;
+    state->reason = "`on_version_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_6: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_5: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_73;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_73;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_3: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 9:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
+      default:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_5;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_4: {
     switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_res_http_end;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
+      case 1:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
       default:
-        goto s_n_llhttp__internal__n_error_64;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_5;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_57: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_invoke_load_http_minor_5: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
+      default:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_5;
+    }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_http_major_1: {
     switch (llhttp__internal__c_load_http_major(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_3;
       case 1:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_4;
       case 2:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_5;
       default:
-        goto s_n_llhttp__internal__n_error_57;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_5;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_7: {
-    switch (llhttp__internal__c_test_lenient_flags_6(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_11: {
+    switch (llhttp__internal__c_test_lenient_flags_10(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_res_http_end;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
       default:
         goto s_n_llhttp__internal__n_invoke_load_http_major_1;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_http_minor_1: {
     switch (llhttp__internal__c_store_http_minor(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_7;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_11;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_65: {
-    state->error = 0x9;
-    state->reason = "Invalid minor version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_7: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_85;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_85;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_66: {
-    state->error = 0x9;
-    state->reason = "Expected dot";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_8: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_86;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_86;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_http_major_1: {
     switch (llhttp__internal__c_store_http_major(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_res_http_dot;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_67: {
-    state->error = 0x9;
-    state->reason = "Invalid major version";
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_9: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_87;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_87;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_91: {
+    state->error = 0x8;
+    state->reason = "Expected HTTP/";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_70: {
-    state->error = 0x8;
-    state->reason = "Expected HTTP/";
+  s_n_llhttp__internal__n_pause_19: {
+    state->error = 0x15;
+    state->reason = "on_method_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_req_first_space_before_url;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_1: {
+    state->error = 0x20;
+    state->reason = "`on_method_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_span_end_llhttp__on_method: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_method(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_method_complete;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_method_complete;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_update_type: {
     switch (llhttp__internal__c_update_type(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_req_first_space_before_url;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_method;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_method: {
     switch (llhttp__internal__c_store_method(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_invoke_update_type;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_68: {
+  s_n_llhttp__internal__n_error_88: {
     state->error = 0x8;
     state->reason = "Invalid word encountered";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_type_1: {
-    switch (llhttp__internal__c_update_type_1(state, p, endp)) {
-      default:
-        goto s_n_llhttp__internal__n_res_http_major;
+  s_n_llhttp__internal__n_span_end_llhttp__on_method_1: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_method(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_update_type_1;
+      return s_error;
     }
+    goto s_n_llhttp__internal__n_invoke_update_type_1;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_update_type_2: {
     switch (llhttp__internal__c_update_type(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_start_req;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_method_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_pause_8: {
+  s_n_llhttp__internal__n_pause_23: {
     state->error = 0x15;
     state->reason = "on_message_begin pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_load_type;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7998,25 +9369,57 @@
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_message_begin: {
     switch (llhttp__on_message_begin(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_load_type;
       case 21:
-        goto s_n_llhttp__internal__n_pause_8;
+        goto s_n_llhttp__internal__n_pause_23;
       default:
         goto s_n_llhttp__internal__n_error;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_finish: {
-    switch (llhttp__internal__c_update_finish(state, p, endp)) {
+  s_n_llhttp__internal__n_pause_24: {
+    state->error = 0x15;
+    state->reason = "on_reset pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_update_finish;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_92: {
+    state->error = 0x1f;
+    state->reason = "`on_reset` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_llhttp__on_reset: {
+    switch (llhttp__on_reset(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_update_finish;
+      case 21:
+        goto s_n_llhttp__internal__n_pause_24;
       default:
-        goto s_n_llhttp__internal__n_invoke_llhttp__on_message_begin;
+        goto s_n_llhttp__internal__n_error_92;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_initial_message_completed: {
+    switch (llhttp__internal__c_load_initial_message_completed(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_llhttp__on_reset;
+      default:
+        goto s_n_llhttp__internal__n_invoke_update_finish;
     }
     /* UNREACHABLE */;
     abort();
   }
 }
 
 int llhttp__internal_execute(llhttp__internal_t* state, const char* p, const char* endp) {
@@ -8397,49 +9800,62 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2,
   s_n_llhttp__internal__n_chunk_data_almost_done_skip,
   s_n_llhttp__internal__n_chunk_data_almost_done,
   s_n_llhttp__internal__n_consume_content_length,
   s_n_llhttp__internal__n_span_start_llhttp__on_body,
   s_n_llhttp__internal__n_invoke_is_equal_content_length,
   s_n_llhttp__internal__n_chunk_size_almost_done,
-  s_n_llhttp__internal__n_chunk_parameters,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete,
+  s_n_llhttp__internal__n_chunk_extension_quoted_value_done,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1,
+  s_n_llhttp__internal__n_error_17,
+  s_n_llhttp__internal__n_chunk_extension_quoted_value,
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2,
+  s_n_llhttp__internal__n_error_19,
+  s_n_llhttp__internal__n_chunk_extension_value,
+  s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value,
+  s_n_llhttp__internal__n_error_20,
+  s_n_llhttp__internal__n_chunk_extension_name,
+  s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name,
+  s_n_llhttp__internal__n_chunk_extensions,
   s_n_llhttp__internal__n_chunk_size_otherwise,
   s_n_llhttp__internal__n_chunk_size,
   s_n_llhttp__internal__n_chunk_size_digit,
-  s_n_llhttp__internal__n_invoke_update_content_length,
+  s_n_llhttp__internal__n_invoke_update_content_length_1,
   s_n_llhttp__internal__n_consume_content_length_1,
   s_n_llhttp__internal__n_span_start_llhttp__on_body_1,
   s_n_llhttp__internal__n_eof,
   s_n_llhttp__internal__n_span_start_llhttp__on_body_2,
   s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete,
   s_n_llhttp__internal__n_headers_almost_done,
   s_n_llhttp__internal__n_header_field_colon_discard_ws,
-  s_n_llhttp__internal__n_error_14,
+  s_n_llhttp__internal__n_error_28,
   s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_value,
   s_n_llhttp__internal__n_header_value_discard_lws,
   s_n_llhttp__internal__n_header_value_discard_ws_almost_done,
   s_n_llhttp__internal__n_header_value_lws,
   s_n_llhttp__internal__n_header_value_almost_done,
   s_n_llhttp__internal__n_header_value_lenient,
-  s_n_llhttp__internal__n_error_17,
-  s_n_llhttp__internal__n_header_value_lenient_failed,
+  s_n_llhttp__internal__n_error_36,
   s_n_llhttp__internal__n_header_value_otherwise,
   s_n_llhttp__internal__n_header_value_connection_token,
   s_n_llhttp__internal__n_header_value_connection_ws,
   s_n_llhttp__internal__n_header_value_connection_1,
   s_n_llhttp__internal__n_header_value_connection_2,
   s_n_llhttp__internal__n_header_value_connection_3,
   s_n_llhttp__internal__n_header_value_connection,
-  s_n_llhttp__internal__n_error_20,
-  s_n_llhttp__internal__n_error_21,
+  s_n_llhttp__internal__n_error_38,
+  s_n_llhttp__internal__n_error_39,
   s_n_llhttp__internal__n_header_value_content_length_ws,
   s_n_llhttp__internal__n_header_value_content_length,
-  s_n_llhttp__internal__n_error_23,
-  s_n_llhttp__internal__n_error_22,
+  s_n_llhttp__internal__n_error_41,
+  s_n_llhttp__internal__n_error_40,
   s_n_llhttp__internal__n_header_value_te_token_ows,
   s_n_llhttp__internal__n_header_value,
   s_n_llhttp__internal__n_header_value_te_token,
   s_n_llhttp__internal__n_header_value_te_chunked_last,
   s_n_llhttp__internal__n_header_value_te_chunked,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1,
   s_n_llhttp__internal__n_header_value_discard_ws,
@@ -8453,22 +9869,30 @@
   s_n_llhttp__internal__n_header_field_1,
   s_n_llhttp__internal__n_header_field_5,
   s_n_llhttp__internal__n_header_field_6,
   s_n_llhttp__internal__n_header_field_7,
   s_n_llhttp__internal__n_header_field,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_field,
   s_n_llhttp__internal__n_header_field_start,
+  s_n_llhttp__internal__n_headers_start,
   s_n_llhttp__internal__n_url_skip_to_http09,
   s_n_llhttp__internal__n_url_skip_lf_to_http09,
   s_n_llhttp__internal__n_req_pri_upgrade,
   s_n_llhttp__internal__n_req_http_complete_1,
   s_n_llhttp__internal__n_req_http_complete,
+  s_n_llhttp__internal__n_invoke_load_method_1,
+  s_n_llhttp__internal__n_invoke_llhttp__on_version_complete,
+  s_n_llhttp__internal__n_error_46,
+  s_n_llhttp__internal__n_error_51,
   s_n_llhttp__internal__n_req_http_minor,
+  s_n_llhttp__internal__n_error_52,
   s_n_llhttp__internal__n_req_http_dot,
+  s_n_llhttp__internal__n_error_53,
   s_n_llhttp__internal__n_req_http_major,
+  s_n_llhttp__internal__n_span_start_llhttp__on_version,
   s_n_llhttp__internal__n_req_http_start_1,
   s_n_llhttp__internal__n_req_http_start_2,
   s_n_llhttp__internal__n_req_http_start_3,
   s_n_llhttp__internal__n_req_http_start,
   s_n_llhttp__internal__n_url_skip_to_http,
   s_n_llhttp__internal__n_url_fragment,
   s_n_llhttp__internal__n_span_end_stub_query_3,
@@ -8485,126 +9909,167 @@
   s_n_llhttp__internal__n_span_end_stub_schema,
   s_n_llhttp__internal__n_url_schema,
   s_n_llhttp__internal__n_url_start,
   s_n_llhttp__internal__n_span_start_llhttp__on_url_1,
   s_n_llhttp__internal__n_span_start_llhttp__on_url,
   s_n_llhttp__internal__n_req_spaces_before_url,
   s_n_llhttp__internal__n_req_first_space_before_url,
-  s_n_llhttp__internal__n_start_req_2,
-  s_n_llhttp__internal__n_start_req_3,
-  s_n_llhttp__internal__n_start_req_1,
-  s_n_llhttp__internal__n_start_req_4,
-  s_n_llhttp__internal__n_start_req_6,
-  s_n_llhttp__internal__n_start_req_8,
-  s_n_llhttp__internal__n_start_req_9,
-  s_n_llhttp__internal__n_start_req_7,
-  s_n_llhttp__internal__n_start_req_5,
-  s_n_llhttp__internal__n_start_req_12,
-  s_n_llhttp__internal__n_start_req_13,
-  s_n_llhttp__internal__n_start_req_11,
-  s_n_llhttp__internal__n_start_req_10,
-  s_n_llhttp__internal__n_start_req_14,
-  s_n_llhttp__internal__n_start_req_17,
-  s_n_llhttp__internal__n_start_req_16,
-  s_n_llhttp__internal__n_start_req_15,
-  s_n_llhttp__internal__n_start_req_18,
-  s_n_llhttp__internal__n_start_req_20,
-  s_n_llhttp__internal__n_start_req_21,
-  s_n_llhttp__internal__n_start_req_19,
-  s_n_llhttp__internal__n_start_req_23,
-  s_n_llhttp__internal__n_start_req_24,
-  s_n_llhttp__internal__n_start_req_26,
-  s_n_llhttp__internal__n_start_req_28,
-  s_n_llhttp__internal__n_start_req_29,
-  s_n_llhttp__internal__n_start_req_27,
-  s_n_llhttp__internal__n_start_req_25,
-  s_n_llhttp__internal__n_start_req_30,
-  s_n_llhttp__internal__n_start_req_22,
-  s_n_llhttp__internal__n_start_req_31,
-  s_n_llhttp__internal__n_start_req_32,
-  s_n_llhttp__internal__n_start_req_35,
-  s_n_llhttp__internal__n_start_req_36,
-  s_n_llhttp__internal__n_start_req_34,
-  s_n_llhttp__internal__n_start_req_37,
-  s_n_llhttp__internal__n_start_req_38,
-  s_n_llhttp__internal__n_start_req_42,
-  s_n_llhttp__internal__n_start_req_43,
-  s_n_llhttp__internal__n_start_req_41,
-  s_n_llhttp__internal__n_start_req_40,
-  s_n_llhttp__internal__n_start_req_39,
-  s_n_llhttp__internal__n_start_req_45,
-  s_n_llhttp__internal__n_start_req_44,
-  s_n_llhttp__internal__n_start_req_33,
-  s_n_llhttp__internal__n_start_req_48,
-  s_n_llhttp__internal__n_start_req_49,
-  s_n_llhttp__internal__n_start_req_50,
-  s_n_llhttp__internal__n_start_req_51,
-  s_n_llhttp__internal__n_start_req_47,
-  s_n_llhttp__internal__n_start_req_46,
-  s_n_llhttp__internal__n_start_req_54,
-  s_n_llhttp__internal__n_start_req_56,
-  s_n_llhttp__internal__n_start_req_57,
-  s_n_llhttp__internal__n_start_req_55,
-  s_n_llhttp__internal__n_start_req_53,
-  s_n_llhttp__internal__n_start_req_58,
-  s_n_llhttp__internal__n_start_req_59,
-  s_n_llhttp__internal__n_start_req_52,
-  s_n_llhttp__internal__n_start_req_61,
-  s_n_llhttp__internal__n_start_req_62,
-  s_n_llhttp__internal__n_start_req_60,
-  s_n_llhttp__internal__n_start_req_65,
-  s_n_llhttp__internal__n_start_req_67,
-  s_n_llhttp__internal__n_start_req_68,
-  s_n_llhttp__internal__n_start_req_66,
-  s_n_llhttp__internal__n_start_req_69,
-  s_n_llhttp__internal__n_start_req_64,
-  s_n_llhttp__internal__n_start_req_63,
-  s_n_llhttp__internal__n_start_req,
+  s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1,
+  s_n_llhttp__internal__n_after_start_req_2,
+  s_n_llhttp__internal__n_after_start_req_3,
+  s_n_llhttp__internal__n_after_start_req_1,
+  s_n_llhttp__internal__n_after_start_req_4,
+  s_n_llhttp__internal__n_after_start_req_6,
+  s_n_llhttp__internal__n_after_start_req_8,
+  s_n_llhttp__internal__n_after_start_req_9,
+  s_n_llhttp__internal__n_after_start_req_7,
+  s_n_llhttp__internal__n_after_start_req_5,
+  s_n_llhttp__internal__n_after_start_req_12,
+  s_n_llhttp__internal__n_after_start_req_13,
+  s_n_llhttp__internal__n_after_start_req_11,
+  s_n_llhttp__internal__n_after_start_req_10,
+  s_n_llhttp__internal__n_after_start_req_14,
+  s_n_llhttp__internal__n_after_start_req_17,
+  s_n_llhttp__internal__n_after_start_req_16,
+  s_n_llhttp__internal__n_after_start_req_15,
+  s_n_llhttp__internal__n_after_start_req_18,
+  s_n_llhttp__internal__n_after_start_req_20,
+  s_n_llhttp__internal__n_after_start_req_21,
+  s_n_llhttp__internal__n_after_start_req_19,
+  s_n_llhttp__internal__n_after_start_req_23,
+  s_n_llhttp__internal__n_after_start_req_24,
+  s_n_llhttp__internal__n_after_start_req_26,
+  s_n_llhttp__internal__n_after_start_req_28,
+  s_n_llhttp__internal__n_after_start_req_29,
+  s_n_llhttp__internal__n_after_start_req_27,
+  s_n_llhttp__internal__n_after_start_req_25,
+  s_n_llhttp__internal__n_after_start_req_30,
+  s_n_llhttp__internal__n_after_start_req_22,
+  s_n_llhttp__internal__n_after_start_req_31,
+  s_n_llhttp__internal__n_after_start_req_32,
+  s_n_llhttp__internal__n_after_start_req_35,
+  s_n_llhttp__internal__n_after_start_req_36,
+  s_n_llhttp__internal__n_after_start_req_34,
+  s_n_llhttp__internal__n_after_start_req_37,
+  s_n_llhttp__internal__n_after_start_req_38,
+  s_n_llhttp__internal__n_after_start_req_42,
+  s_n_llhttp__internal__n_after_start_req_43,
+  s_n_llhttp__internal__n_after_start_req_41,
+  s_n_llhttp__internal__n_after_start_req_40,
+  s_n_llhttp__internal__n_after_start_req_39,
+  s_n_llhttp__internal__n_after_start_req_45,
+  s_n_llhttp__internal__n_after_start_req_44,
+  s_n_llhttp__internal__n_after_start_req_33,
+  s_n_llhttp__internal__n_after_start_req_48,
+  s_n_llhttp__internal__n_after_start_req_49,
+  s_n_llhttp__internal__n_after_start_req_50,
+  s_n_llhttp__internal__n_after_start_req_51,
+  s_n_llhttp__internal__n_after_start_req_47,
+  s_n_llhttp__internal__n_after_start_req_46,
+  s_n_llhttp__internal__n_after_start_req_54,
+  s_n_llhttp__internal__n_after_start_req_56,
+  s_n_llhttp__internal__n_after_start_req_57,
+  s_n_llhttp__internal__n_after_start_req_55,
+  s_n_llhttp__internal__n_after_start_req_53,
+  s_n_llhttp__internal__n_after_start_req_58,
+  s_n_llhttp__internal__n_after_start_req_59,
+  s_n_llhttp__internal__n_after_start_req_52,
+  s_n_llhttp__internal__n_after_start_req_61,
+  s_n_llhttp__internal__n_after_start_req_62,
+  s_n_llhttp__internal__n_after_start_req_60,
+  s_n_llhttp__internal__n_after_start_req_65,
+  s_n_llhttp__internal__n_after_start_req_67,
+  s_n_llhttp__internal__n_after_start_req_68,
+  s_n_llhttp__internal__n_after_start_req_66,
+  s_n_llhttp__internal__n_after_start_req_69,
+  s_n_llhttp__internal__n_after_start_req_64,
+  s_n_llhttp__internal__n_after_start_req_63,
+  s_n_llhttp__internal__n_after_start_req,
+  s_n_llhttp__internal__n_span_start_llhttp__on_method_1,
   s_n_llhttp__internal__n_invoke_llhttp__on_status_complete,
   s_n_llhttp__internal__n_res_line_almost_done,
   s_n_llhttp__internal__n_res_status,
   s_n_llhttp__internal__n_span_start_llhttp__on_status,
   s_n_llhttp__internal__n_res_status_start,
   s_n_llhttp__internal__n_res_status_code_otherwise,
-  s_n_llhttp__internal__n_res_status_code,
-  s_n_llhttp__internal__n_res_http_end,
+  s_n_llhttp__internal__n_res_status_code_digit_3,
+  s_n_llhttp__internal__n_res_status_code_digit_2,
+  s_n_llhttp__internal__n_res_status_code_digit_1,
+  s_n_llhttp__internal__n_res_after_version,
+  s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1,
+  s_n_llhttp__internal__n_error_68,
+  s_n_llhttp__internal__n_error_79,
   s_n_llhttp__internal__n_res_http_minor,
+  s_n_llhttp__internal__n_error_80,
   s_n_llhttp__internal__n_res_http_dot,
+  s_n_llhttp__internal__n_error_81,
   s_n_llhttp__internal__n_res_http_major,
+  s_n_llhttp__internal__n_span_start_llhttp__on_version_1,
   s_n_llhttp__internal__n_start_res,
+  s_n_llhttp__internal__n_invoke_llhttp__on_method_complete,
   s_n_llhttp__internal__n_req_or_res_method_2,
+  s_n_llhttp__internal__n_invoke_update_type_1,
   s_n_llhttp__internal__n_req_or_res_method_3,
   s_n_llhttp__internal__n_req_or_res_method_1,
   s_n_llhttp__internal__n_req_or_res_method,
+  s_n_llhttp__internal__n_span_start_llhttp__on_method,
   s_n_llhttp__internal__n_start_req_or_res,
   s_n_llhttp__internal__n_invoke_load_type,
+  s_n_llhttp__internal__n_invoke_update_finish,
   s_n_llhttp__internal__n_start,
 };
 typedef enum llparse_state_e llparse_state_t;
 
+int llhttp__on_method(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__on_url(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__on_version(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__on_header_field(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
 int llhttp__on_header_value(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
 int llhttp__on_body(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__on_chunk_extension_name(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
+int llhttp__on_chunk_extension_value(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__on_status(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__internal__c_load_initial_message_completed(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return state->initial_message_completed;
+}
+
+int llhttp__on_reset(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__internal__c_update_finish(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->finish = 2;
   return 0;
 }
@@ -8625,14 +10090,18 @@
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   state->method = match;
   return 0;
 }
 
+int llhttp__on_method_complete(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__internal__c_is_equal_method(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return state->method == 5;
 }
 
@@ -8652,14 +10121,21 @@
   return 0;
 }
 
 int llhttp__on_url_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__internal__c_test_lenient_flags(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return (state->lenient_flags & 1) == 1;
+}
+
 int llhttp__internal__c_test_flags(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->flags & 128) == 128;
 }
 
@@ -8678,37 +10154,53 @@
   return state->upgrade == 1;
 }
 
 int llhttp__after_message_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
+int llhttp__internal__c_update_content_length(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  state->content_length = 0;
+  return 0;
+}
+
+int llhttp__internal__c_update_initial_message_completed(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  state->initial_message_completed = 1;
+  return 0;
+}
+
 int llhttp__internal__c_update_finish_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->finish = 0;
   return 0;
 }
 
-int llhttp__internal__c_test_lenient_flags(
+int llhttp__internal__c_test_lenient_flags_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->lenient_flags & 4) == 4;
 }
 
 int llhttp__internal__c_test_flags_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->flags & 544) == 544;
 }
 
-int llhttp__internal__c_test_lenient_flags_1(
+int llhttp__internal__c_test_lenient_flags_2(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->lenient_flags & 2) == 2;
 }
 
 int llhttp__before_headers_complete(
@@ -8719,22 +10211,14 @@
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
 int llhttp__after_headers_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
-int llhttp__internal__c_update_content_length(
-    llhttp__internal_t* state,
-    const unsigned char* p,
-    const unsigned char* endp) {
-  state->content_length = 0;
-  return 0;
-}
-
 int llhttp__internal__c_mul_add_content_length(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   /* Multiplication overflow */
   if (state->content_length > 0xffffffffffffffffULL / 16) {
@@ -8772,14 +10256,22 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 128;
   return 0;
 }
 
+int llhttp__on_chunk_extension_name_complete(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
+int llhttp__on_chunk_extension_value_complete(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__internal__c_update_finish_3(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->finish = 1;
   return 0;
 }
@@ -8805,21 +10297,14 @@
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   state->header_state = match;
   return 0;
 }
 
-int llhttp__internal__c_test_lenient_flags_2(
-    llhttp__internal_t* state,
-    const unsigned char* p,
-    const unsigned char* endp) {
-  return (state->lenient_flags & 1) == 1;
-}
-
 int llhttp__on_header_field_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
 int llhttp__internal__c_load_header_state(
     llhttp__internal_t* state,
     const unsigned char* p,
@@ -8867,39 +10352,39 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 8;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_2(
+int llhttp__internal__c_update_header_state_3(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 6;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_4(
+int llhttp__internal__c_update_header_state_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 0;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_5(
+int llhttp__internal__c_update_header_state_6(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 5;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_6(
+int llhttp__internal__c_update_header_state_7(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 7;
   return 0;
 }
 
@@ -8947,15 +10432,15 @@
 int llhttp__internal__c_test_flags_3(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->flags & 8) == 8;
 }
 
-int llhttp__internal__c_test_lenient_flags_4(
+int llhttp__internal__c_test_lenient_flags_8(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->lenient_flags & 8) == 8;
 }
 
 int llhttp__internal__c_or_flags_16(
@@ -8970,15 +10455,15 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags &= -9;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_7(
+int llhttp__internal__c_update_header_state_8(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 8;
   return 0;
 }
 
@@ -9011,21 +10496,25 @@
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   state->http_minor = match;
   return 0;
 }
 
-int llhttp__internal__c_test_lenient_flags_6(
+int llhttp__internal__c_test_lenient_flags_10(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return (state->lenient_flags & 16) == 16;
 }
 
+int llhttp__on_version_complete(
+    llhttp__internal_t* s, const unsigned char* p,
+    const unsigned char* endp);
+
 int llhttp__internal__c_load_http_major(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   return state->http_major;
 }
 
@@ -9063,19 +10552,14 @@
     }
   } else {
     if (state->status_code < 0 - match) {
       return 1;
     }
   }
   state->status_code += match;
-  
-  /* Enforce maximum */
-  if (state->status_code > 999) {
-    return 1;
-  }
   return 0;
 }
 
 int llhttp__on_status_complete(
     llhttp__internal_t* s, const unsigned char* p,
     const unsigned char* endp);
 
@@ -9117,15 +10601,15 @@
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_llhttp__after_message_complete:
     s_n_llhttp__internal__n_invoke_llhttp__after_message_complete: {
       switch (llhttp__after_message_complete(state, p, endp)) {
         case 1:
-          goto s_n_llhttp__internal__n_invoke_update_finish_2;
+          goto s_n_llhttp__internal__n_invoke_update_content_length;
         default:
           goto s_n_llhttp__internal__n_invoke_update_finish_1;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_pause_1:
@@ -9151,17 +10635,17 @@
     }
     case s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2:
     s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2: {
       switch (llhttp__on_message_complete(state, p, endp)) {
         case 0:
           goto s_n_llhttp__internal__n_invoke_is_equal_upgrade;
         case 21:
-          goto s_n_llhttp__internal__n_pause_5;
+          goto s_n_llhttp__internal__n_pause_11;
         default:
-          goto s_n_llhttp__internal__n_error_10;
+          goto s_n_llhttp__internal__n_error_24;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_chunk_data_almost_done_skip:
     s_n_llhttp__internal__n_chunk_data_almost_done_skip: {
       if (p == endp) {
@@ -9228,48 +10712,296 @@
         return s_n_llhttp__internal__n_chunk_size_almost_done;
       }
       p++;
       goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_header;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_chunk_parameters:
-    s_n_llhttp__internal__n_chunk_parameters: {
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete: {
+      switch (llhttp__on_chunk_extension_name_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_size_almost_done;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_5;
+        default:
+          goto s_n_llhttp__internal__n_error_11;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1: {
+      switch (llhttp__on_chunk_extension_name_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_extensions;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_6;
+        default:
+          goto s_n_llhttp__internal__n_error_12;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete: {
+      switch (llhttp__on_chunk_extension_value_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_size_almost_done;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_7;
+        default:
+          goto s_n_llhttp__internal__n_error_14;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extension_quoted_value_done:
+    s_n_llhttp__internal__n_chunk_extension_quoted_value_done: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_chunk_extension_quoted_value_done;
+      }
+      switch (*p) {
+        case 13: {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_size_almost_done;
+        }
+        case ';': {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_extensions;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_error_16;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1: {
+      switch (llhttp__on_chunk_extension_value_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_extension_quoted_value_done;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_8;
+        default:
+          goto s_n_llhttp__internal__n_error_15;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_17:
+    s_n_llhttp__internal__n_error_17: {
+      state->error = 0x2;
+      state->reason = "Invalid character in chunk extensions quoted value";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extension_quoted_value:
+    s_n_llhttp__internal__n_chunk_extension_quoted_value: {
       static uint8_t lookup_table[] = {
-        0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 2, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0,
         0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        1, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+        1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
-        1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0,
-        1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
         1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1
       };
       if (p == endp) {
-        return s_n_llhttp__internal__n_chunk_parameters;
+        return s_n_llhttp__internal__n_chunk_extension_quoted_value;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_chunk_parameters;
+          goto s_n_llhttp__internal__n_chunk_extension_quoted_value;
         }
         case 2: {
           p++;
-          goto s_n_llhttp__internal__n_chunk_size_almost_done;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_1;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_2;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2:
+    s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2: {
+      switch (llhttp__on_chunk_extension_value_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_chunk_size_otherwise;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_9;
+        default:
+          goto s_n_llhttp__internal__n_error_18;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_19:
+    s_n_llhttp__internal__n_error_19: {
+      state->error = 0x2;
+      state->reason = "Invalid character in chunk extensions value";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extension_value:
+    s_n_llhttp__internal__n_chunk_extension_value: {
+      static uint8_t lookup_table[] = {
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 2, 3, 2, 2, 2, 2, 2, 0, 0, 2, 2, 0, 2, 2, 0,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 4, 0, 0, 0, 0,
+        0, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 0, 0, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 2, 0, 2, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+      };
+      if (p == endp) {
+        return s_n_llhttp__internal__n_chunk_extension_value;
+      }
+      switch (lookup_table[(uint8_t) *p]) {
+        case 1: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value;
+        }
+        case 2: {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_extension_value;
+        }
+        case 3: {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_extension_quoted_value;
+        }
+        case 4: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_3;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_4;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value:
+    s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_chunk_extension_value;
+      goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_2;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_20:
+    s_n_llhttp__internal__n_error_20: {
+      state->error = 0x2;
+      state->reason = "Invalid character in chunk extensions name";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extension_name:
+    s_n_llhttp__internal__n_chunk_extension_name: {
+      static uint8_t lookup_table[] = {
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 2, 0, 2, 2, 2, 2, 2, 0, 0, 2, 2, 0, 2, 2, 0,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 3, 0, 4, 0, 0,
+        0, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 0, 0, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 0, 2, 0, 2, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+      };
+      if (p == endp) {
+        return s_n_llhttp__internal__n_chunk_extension_name;
+      }
+      switch (lookup_table[(uint8_t) *p]) {
+        case 1: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name;
+        }
+        case 2: {
+          p++;
+          goto s_n_llhttp__internal__n_chunk_extension_name;
+        }
+        case 3: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_1;
+        }
+        case 4: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_2;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_3;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name:
+    s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_chunk_extension_name;
+      goto s_n_llhttp__internal__n_chunk_extension_name;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_chunk_extensions:
+    s_n_llhttp__internal__n_chunk_extensions: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_chunk_extensions;
+      }
+      switch (*p) {
+        case 13: {
+          p++;
+          goto s_n_llhttp__internal__n_error_9;
+        }
+        case ' ': {
+          p++;
+          goto s_n_llhttp__internal__n_error_10;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_6;
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_name;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_chunk_size_otherwise:
     s_n_llhttp__internal__n_chunk_size_otherwise: {
@@ -9277,24 +11009,20 @@
         return s_n_llhttp__internal__n_chunk_size_otherwise;
       }
       switch (*p) {
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_chunk_size_almost_done;
         }
-        case ' ': {
-          p++;
-          goto s_n_llhttp__internal__n_chunk_parameters;
-        }
         case ';': {
           p++;
-          goto s_n_llhttp__internal__n_chunk_parameters;
+          goto s_n_llhttp__internal__n_chunk_extensions;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_7;
+          goto s_n_llhttp__internal__n_error_21;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_chunk_size:
     s_n_llhttp__internal__n_chunk_size: {
@@ -9532,22 +11260,22 @@
         }
         case 'f': {
           p++;
           match = 15;
           goto s_n_llhttp__internal__n_invoke_mul_add_content_length;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_9;
+          goto s_n_llhttp__internal__n_error_23;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_invoke_update_content_length:
-    s_n_llhttp__internal__n_invoke_update_content_length: {
+    case s_n_llhttp__internal__n_invoke_update_content_length_1:
+    s_n_llhttp__internal__n_invoke_update_content_length_1: {
       switch (llhttp__internal__c_update_content_length(state, p, endp)) {
         default:
           goto s_n_llhttp__internal__n_chunk_size_digit;
       }
       /* UNREACHABLE */;
       abort();
     }
@@ -9603,21 +11331,21 @@
     }
     case s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete:
     s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete: {
       switch (llhttp__after_headers_complete(state, p, endp)) {
         case 1:
           goto s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_1;
         case 2:
-          goto s_n_llhttp__internal__n_invoke_update_content_length;
+          goto s_n_llhttp__internal__n_invoke_update_content_length_1;
         case 3:
           goto s_n_llhttp__internal__n_span_start_llhttp__on_body_1;
         case 4:
           goto s_n_llhttp__internal__n_invoke_update_finish_3;
         case 5:
-          goto s_n_llhttp__internal__n_error_11;
+          goto s_n_llhttp__internal__n_error_25;
         default:
           goto s_n_llhttp__internal__n_invoke_llhttp__on_message_complete;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_headers_almost_done:
@@ -9643,29 +11371,33 @@
         default: {
           goto s_n_llhttp__internal__n_header_field_colon;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_14:
-    s_n_llhttp__internal__n_error_14: {
+    case s_n_llhttp__internal__n_error_28:
+    s_n_llhttp__internal__n_error_28: {
       state->error = 0xa;
       state->reason = "Invalid header field char";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete:
     s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete: {
       switch (llhttp__on_header_value_complete(state, p, endp)) {
-        default:
+        case 0:
           goto s_n_llhttp__internal__n_header_field_start;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_14;
+        default:
+          goto s_n_llhttp__internal__n_error_32;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_header_value:
     s_n_llhttp__internal__n_span_start_llhttp__on_header_value: {
       if (p == endp) {
@@ -9681,51 +11413,58 @@
     s_n_llhttp__internal__n_header_value_discard_lws: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_discard_lws;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_ws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_5;
         }
         case ' ': {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_ws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_5;
         }
         default: {
           goto s_n_llhttp__internal__n_invoke_load_header_state;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_discard_ws_almost_done:
     s_n_llhttp__internal__n_header_value_discard_ws_almost_done: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_discard_ws_almost_done;
       }
-      p++;
-      goto s_n_llhttp__internal__n_header_value_discard_lws;
+      switch (*p) {
+        case 10: {
+          p++;
+          goto s_n_llhttp__internal__n_header_value_discard_lws;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_6;
+        }
+      }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_lws:
     s_n_llhttp__internal__n_header_value_lws: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_lws;
       }
       switch (*p) {
         case 9: {
-          goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
         }
         case ' ': {
-          goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_4;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_almost_done:
     s_n_llhttp__internal__n_header_value_almost_done: {
@@ -9734,15 +11473,15 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_header_value_lws;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_16;
+          goto s_n_llhttp__internal__n_error_35;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_lenient:
     s_n_llhttp__internal__n_header_value_lenient: {
@@ -9760,51 +11499,35 @@
           p++;
           goto s_n_llhttp__internal__n_header_value_lenient;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_17:
-    s_n_llhttp__internal__n_error_17: {
-      state->error = 0x19;
-      state->reason = "Missing expected CR after header value";
+    case s_n_llhttp__internal__n_error_36:
+    s_n_llhttp__internal__n_error_36: {
+      state->error = 0xa;
+      state->reason = "Invalid header value char";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_header_value_lenient_failed:
-    s_n_llhttp__internal__n_header_value_lenient_failed: {
-      if (p == endp) {
-        return s_n_llhttp__internal__n_header_value_lenient_failed;
-      }
-      switch (*p) {
-        case 10: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2;
-        }
-        default: {
-          goto s_n_llhttp__internal__n_error_18;
-        }
-      }
-      /* UNREACHABLE */;
-      abort();
-    }
     case s_n_llhttp__internal__n_header_value_otherwise:
     s_n_llhttp__internal__n_header_value_otherwise: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_otherwise;
       }
       switch (*p) {
         case 13: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_3;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_7;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_connection_token:
     s_n_llhttp__internal__n_header_value_connection_token: {
@@ -9859,18 +11582,18 @@
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_header_value_connection_ws;
         }
         case ',': {
           p++;
-          goto s_n_llhttp__internal__n_invoke_load_header_state_4;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_5;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_4;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_5;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_connection_1:
     s_n_llhttp__internal__n_header_value_connection_1: {
@@ -9880,15 +11603,15 @@
         return s_n_llhttp__internal__n_header_value_connection_1;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob3, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_2;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_3;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_1;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -9904,15 +11627,15 @@
         return s_n_llhttp__internal__n_header_value_connection_2;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob4, 9);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_5;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_6;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_2;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -9928,15 +11651,15 @@
         return s_n_llhttp__internal__n_header_value_connection_3;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob5, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_6;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_3;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -9973,26 +11696,26 @@
         default: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_20:
-    s_n_llhttp__internal__n_error_20: {
+    case s_n_llhttp__internal__n_error_38:
+    s_n_llhttp__internal__n_error_38: {
       state->error = 0xb;
       state->reason = "Content-Length overflow";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_21:
-    s_n_llhttp__internal__n_error_21: {
+    case s_n_llhttp__internal__n_error_39:
+    s_n_llhttp__internal__n_error_39: {
       state->error = 0xb;
       state->reason = "Invalid character in Content-Length";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
@@ -10079,26 +11802,26 @@
         default: {
           goto s_n_llhttp__internal__n_header_value_content_length_ws;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_23:
-    s_n_llhttp__internal__n_error_23: {
+    case s_n_llhttp__internal__n_error_41:
+    s_n_llhttp__internal__n_error_41: {
       state->error = 0xf;
       state->reason = "Invalid `Transfer-Encoding` header value";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_22:
-    s_n_llhttp__internal__n_error_22: {
+    case s_n_llhttp__internal__n_error_40:
+    s_n_llhttp__internal__n_error_40: {
       state->error = 0xf;
       state->reason = "Invalid `Transfer-Encoding` header value";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
@@ -10212,31 +11935,31 @@
           goto s_n_llhttp__internal__n_header_value_te_token;
         }
         case 2: {
           p++;
           goto s_n_llhttp__internal__n_header_value_te_token_ows;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_8;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_9;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_te_chunked_last:
     s_n_llhttp__internal__n_header_value_te_chunked_last: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_te_chunked_last;
       }
       switch (*p) {
         case 10: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_8;
         }
         case 13: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_8;
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_header_value_te_chunked_last;
         }
         case ',': {
           goto s_n_llhttp__internal__n_invoke_load_type_1;
@@ -10291,15 +12014,15 @@
       switch (*p) {
         case 9: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_ws;
         }
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_lws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_4;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_ws_almost_done;
         }
         case ' ': {
           p++;
@@ -10311,31 +12034,35 @@
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete:
     s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete: {
       switch (llhttp__on_header_field_complete(state, p, endp)) {
-        default:
+        case 0:
           goto s_n_llhttp__internal__n_header_value_discard_ws;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_15;
+        default:
+          goto s_n_llhttp__internal__n_error_29;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_general_otherwise:
     s_n_llhttp__internal__n_header_field_general_otherwise: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_field_general_otherwise;
       }
       switch (*p) {
         case ':': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field_2;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_24;
+          goto s_n_llhttp__internal__n_error_42;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_general:
     s_n_llhttp__internal__n_header_field_general: {
@@ -10411,21 +12138,21 @@
     case s_n_llhttp__internal__n_header_field_colon:
     s_n_llhttp__internal__n_header_field_colon: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_field_colon;
       }
       switch (*p) {
         case ' ': {
-          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_2;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_3;
         }
         case ':': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_9;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_3:
     s_n_llhttp__internal__n_header_field_3: {
@@ -10442,15 +12169,15 @@
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_4:
     s_n_llhttp__internal__n_header_field_4: {
@@ -10467,15 +12194,15 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_4;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_2:
     s_n_llhttp__internal__n_header_field_2: {
@@ -10488,15 +12215,15 @@
           goto s_n_llhttp__internal__n_header_field_3;
         }
         case 't': {
           p++;
           goto s_n_llhttp__internal__n_header_field_4;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_1:
     s_n_llhttp__internal__n_header_field_1: {
@@ -10512,15 +12239,15 @@
           p++;
           goto s_n_llhttp__internal__n_header_field_2;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_1;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_5:
     s_n_llhttp__internal__n_header_field_5: {
@@ -10537,15 +12264,15 @@
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_5;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_6:
     s_n_llhttp__internal__n_header_field_6: {
@@ -10562,15 +12289,15 @@
           match = 3;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_6;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_7:
     s_n_llhttp__internal__n_header_field_7: {
@@ -10587,15 +12314,15 @@
           match = 4;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_7;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field:
     s_n_llhttp__internal__n_header_field: {
@@ -10616,15 +12343,15 @@
           goto s_n_llhttp__internal__n_header_field_6;
         }
         case 'u': {
           p++;
           goto s_n_llhttp__internal__n_header_field_7;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_header_field:
     s_n_llhttp__internal__n_span_start_llhttp__on_header_field: {
@@ -10653,14 +12380,31 @@
         default: {
           goto s_n_llhttp__internal__n_span_start_llhttp__on_header_field;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_headers_start:
+    s_n_llhttp__internal__n_headers_start: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_headers_start;
+      }
+      switch (*p) {
+        case ' ': {
+          p++;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_header_field_start;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_url_skip_to_http09:
     s_n_llhttp__internal__n_url_skip_to_http09: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_skip_to_http09;
       }
       p++;
       goto s_n_llhttp__internal__n_invoke_update_http_major;
@@ -10681,15 +12425,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_update_http_major;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_url_skip_lf_to_http09;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_25;
+          goto s_n_llhttp__internal__n_error_43;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_pri_upgrade:
     s_n_llhttp__internal__n_req_pri_upgrade: {
@@ -10699,64 +12443,108 @@
         return s_n_llhttp__internal__n_req_pri_upgrade;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob16, 10);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_error_30;
+          goto s_n_llhttp__internal__n_error_49;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_pri_upgrade;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_31;
+          goto s_n_llhttp__internal__n_error_50;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_complete_1:
     s_n_llhttp__internal__n_req_http_complete_1: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_complete_1;
       }
       switch (*p) {
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_header_field_start;
+          goto s_n_llhttp__internal__n_headers_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_29;
+          goto s_n_llhttp__internal__n_error_48;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_complete:
     s_n_llhttp__internal__n_req_http_complete: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_complete;
       }
       switch (*p) {
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_header_field_start;
+          goto s_n_llhttp__internal__n_headers_start;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_req_http_complete_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_29;
+          goto s_n_llhttp__internal__n_error_48;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_load_method_1:
+    s_n_llhttp__internal__n_invoke_load_method_1: {
+      switch (llhttp__internal__c_load_method(state, p, endp)) {
+        case 34:
+          goto s_n_llhttp__internal__n_req_pri_upgrade;
+        default:
+          goto s_n_llhttp__internal__n_req_http_complete;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_version_complete:
+    s_n_llhttp__internal__n_invoke_llhttp__on_version_complete: {
+      switch (llhttp__on_version_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_invoke_load_method_1;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_17;
+        default:
+          goto s_n_llhttp__internal__n_error_47;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_46:
+    s_n_llhttp__internal__n_error_46: {
+      state->error = 0x9;
+      state->reason = "Invalid HTTP version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_51:
+    s_n_llhttp__internal__n_error_51: {
+      state->error = 0x9;
+      state->reason = "Invalid minor version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_http_minor:
     s_n_llhttp__internal__n_req_http_minor: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_minor;
       }
       switch (*p) {
         case '0': {
@@ -10806,37 +12594,57 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_34;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_2;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_52:
+    s_n_llhttp__internal__n_error_52: {
+      state->error = 0x9;
+      state->reason = "Expected dot";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_http_dot:
     s_n_llhttp__internal__n_req_http_dot: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_dot;
       }
       switch (*p) {
         case '.': {
           p++;
           goto s_n_llhttp__internal__n_req_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_35;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_3;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_53:
+    s_n_llhttp__internal__n_error_53: {
+      state->error = 0x9;
+      state->reason = "Invalid major version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_http_major:
     s_n_llhttp__internal__n_req_http_major: {
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_major;
       }
       switch (*p) {
         case '0': {
@@ -10886,20 +12694,31 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_major;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_36;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_4;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_version:
+    s_n_llhttp__internal__n_span_start_llhttp__on_version: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_version;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_version;
+      goto s_n_llhttp__internal__n_req_http_major;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_http_start_1:
     s_n_llhttp__internal__n_req_http_start_1: {
       llparse_match_t match_seq;
       
       if (p == endp) {
         return s_n_llhttp__internal__n_req_http_start_1;
       }
@@ -10910,15 +12729,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_1;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_56;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_2:
     s_n_llhttp__internal__n_req_http_start_2: {
@@ -10934,15 +12753,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method_2;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_2;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_56;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_3:
     s_n_llhttp__internal__n_req_http_start_3: {
@@ -10958,15 +12777,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method_3;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_56;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start:
     s_n_llhttp__internal__n_req_http_start: {
@@ -10987,15 +12806,15 @@
           goto s_n_llhttp__internal__n_req_http_start_2;
         }
         case 'R': {
           p++;
           goto s_n_llhttp__internal__n_req_http_start_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_56;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_skip_to_http:
     s_n_llhttp__internal__n_url_skip_to_http: {
@@ -11041,15 +12860,15 @@
         case 3: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_7;
         }
         case 4: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_8;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_40;
+          goto s_n_llhttp__internal__n_error_57;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_end_stub_query_3:
     s_n_llhttp__internal__n_span_end_stub_query_3: {
@@ -11098,15 +12917,15 @@
         case 4: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_11;
         }
         case 5: {
           goto s_n_llhttp__internal__n_span_end_stub_query_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_41;
+          goto s_n_llhttp__internal__n_error_58;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_query_or_fragment:
     s_n_llhttp__internal__n_url_query_or_fragment: {
@@ -11128,15 +12947,15 @@
           goto s_n_llhttp__internal__n_url_fragment;
         }
         case '?': {
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_42;
+          goto s_n_llhttp__internal__n_error_59;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_path:
     s_n_llhttp__internal__n_url_path: {
@@ -11269,18 +13088,18 @@
         }
         case 6: {
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         case 7: {
           p++;
-          goto s_n_llhttp__internal__n_error_43;
+          goto s_n_llhttp__internal__n_error_60;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_44;
+          goto s_n_llhttp__internal__n_error_61;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_server:
     s_n_llhttp__internal__n_url_server: {
@@ -11327,15 +13146,15 @@
           goto s_n_llhttp__internal__n_url_query;
         }
         case 7: {
           p++;
           goto s_n_llhttp__internal__n_url_server_with_at;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_62;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_schema_delim_1:
     s_n_llhttp__internal__n_url_schema_delim_1: {
@@ -11344,44 +13163,44 @@
       }
       switch (*p) {
         case '/': {
           p++;
           goto s_n_llhttp__internal__n_url_server;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_47;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_schema_delim:
     s_n_llhttp__internal__n_url_schema_delim: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_schema_delim;
       }
       switch (*p) {
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_63;
         }
         case 13: {
           p++;
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_63;
         }
         case ' ': {
           p++;
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_63;
         }
         case '/': {
           p++;
           goto s_n_llhttp__internal__n_url_schema_delim_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_47;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_end_stub_schema:
     s_n_llhttp__internal__n_span_end_stub_schema: {
@@ -11415,25 +13234,25 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_schema;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_63;
         }
         case 2: {
           goto s_n_llhttp__internal__n_span_end_stub_schema;
         }
         case 3: {
           p++;
           goto s_n_llhttp__internal__n_url_schema;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_48;
+          goto s_n_llhttp__internal__n_error_65;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_start:
     s_n_llhttp__internal__n_url_start: {
@@ -11457,24 +13276,24 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_start;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_63;
         }
         case 2: {
           goto s_n_llhttp__internal__n_span_start_stub_path_2;
         }
         case 3: {
           goto s_n_llhttp__internal__n_url_schema;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_49;
+          goto s_n_llhttp__internal__n_error_66;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_url_1:
     s_n_llhttp__internal__n_span_start_llhttp__on_url_1: {
@@ -11522,1717 +13341,1745 @@
       }
       switch (*p) {
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_req_spaces_before_url;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_50;
+          goto s_n_llhttp__internal__n_error_67;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_2:
-    s_n_llhttp__internal__n_start_req_2: {
+    case s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1:
+    s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1: {
+      switch (llhttp__on_method_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_req_first_space_before_url;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_22;
+        default:
+          goto s_n_llhttp__internal__n_error_83;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_after_start_req_2:
+    s_n_llhttp__internal__n_after_start_req_2: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_2;
+        return s_n_llhttp__internal__n_after_start_req_2;
       }
       switch (*p) {
         case 'L': {
           p++;
           match = 19;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_3:
-    s_n_llhttp__internal__n_start_req_3: {
+    case s_n_llhttp__internal__n_after_start_req_3:
+    s_n_llhttp__internal__n_after_start_req_3: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_3;
+        return s_n_llhttp__internal__n_after_start_req_3;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob19, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 36;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_3;
+          return s_n_llhttp__internal__n_after_start_req_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_1:
-    s_n_llhttp__internal__n_start_req_1: {
+    case s_n_llhttp__internal__n_after_start_req_1:
+    s_n_llhttp__internal__n_after_start_req_1: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_1;
+        return s_n_llhttp__internal__n_after_start_req_1;
       }
       switch (*p) {
         case 'C': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_2;
+          goto s_n_llhttp__internal__n_after_start_req_2;
         }
         case 'N': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_3;
+          goto s_n_llhttp__internal__n_after_start_req_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_4:
-    s_n_llhttp__internal__n_start_req_4: {
+    case s_n_llhttp__internal__n_after_start_req_4:
+    s_n_llhttp__internal__n_after_start_req_4: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_4;
+        return s_n_llhttp__internal__n_after_start_req_4;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob20, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 16;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_4;
+          return s_n_llhttp__internal__n_after_start_req_4;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_6:
-    s_n_llhttp__internal__n_start_req_6: {
+    case s_n_llhttp__internal__n_after_start_req_6:
+    s_n_llhttp__internal__n_after_start_req_6: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_6;
+        return s_n_llhttp__internal__n_after_start_req_6;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob21, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 22;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_6;
+          return s_n_llhttp__internal__n_after_start_req_6;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_8:
-    s_n_llhttp__internal__n_start_req_8: {
+    case s_n_llhttp__internal__n_after_start_req_8:
+    s_n_llhttp__internal__n_after_start_req_8: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_8;
+        return s_n_llhttp__internal__n_after_start_req_8;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob22, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 5;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_8;
+          return s_n_llhttp__internal__n_after_start_req_8;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_9:
-    s_n_llhttp__internal__n_start_req_9: {
+    case s_n_llhttp__internal__n_after_start_req_9:
+    s_n_llhttp__internal__n_after_start_req_9: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_9;
+        return s_n_llhttp__internal__n_after_start_req_9;
       }
       switch (*p) {
         case 'Y': {
           p++;
           match = 8;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_7:
-    s_n_llhttp__internal__n_start_req_7: {
+    case s_n_llhttp__internal__n_after_start_req_7:
+    s_n_llhttp__internal__n_after_start_req_7: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_7;
+        return s_n_llhttp__internal__n_after_start_req_7;
       }
       switch (*p) {
         case 'N': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_8;
+          goto s_n_llhttp__internal__n_after_start_req_8;
         }
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_9;
+          goto s_n_llhttp__internal__n_after_start_req_9;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_5:
-    s_n_llhttp__internal__n_start_req_5: {
+    case s_n_llhttp__internal__n_after_start_req_5:
+    s_n_llhttp__internal__n_after_start_req_5: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_5;
+        return s_n_llhttp__internal__n_after_start_req_5;
       }
       switch (*p) {
         case 'H': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_6;
+          goto s_n_llhttp__internal__n_after_start_req_6;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_7;
+          goto s_n_llhttp__internal__n_after_start_req_7;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_12:
-    s_n_llhttp__internal__n_start_req_12: {
+    case s_n_llhttp__internal__n_after_start_req_12:
+    s_n_llhttp__internal__n_after_start_req_12: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_12;
+        return s_n_llhttp__internal__n_after_start_req_12;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob23, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 0;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_12;
+          return s_n_llhttp__internal__n_after_start_req_12;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_13:
-    s_n_llhttp__internal__n_start_req_13: {
+    case s_n_llhttp__internal__n_after_start_req_13:
+    s_n_llhttp__internal__n_after_start_req_13: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_13;
+        return s_n_llhttp__internal__n_after_start_req_13;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob24, 5);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 35;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_13;
+          return s_n_llhttp__internal__n_after_start_req_13;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_11:
-    s_n_llhttp__internal__n_start_req_11: {
+    case s_n_llhttp__internal__n_after_start_req_11:
+    s_n_llhttp__internal__n_after_start_req_11: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_11;
+        return s_n_llhttp__internal__n_after_start_req_11;
       }
       switch (*p) {
         case 'L': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_12;
+          goto s_n_llhttp__internal__n_after_start_req_12;
         }
         case 'S': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_13;
+          goto s_n_llhttp__internal__n_after_start_req_13;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_10:
-    s_n_llhttp__internal__n_start_req_10: {
+    case s_n_llhttp__internal__n_after_start_req_10:
+    s_n_llhttp__internal__n_after_start_req_10: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_10;
+        return s_n_llhttp__internal__n_after_start_req_10;
       }
       switch (*p) {
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_11;
+          goto s_n_llhttp__internal__n_after_start_req_11;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_14:
-    s_n_llhttp__internal__n_start_req_14: {
+    case s_n_llhttp__internal__n_after_start_req_14:
+    s_n_llhttp__internal__n_after_start_req_14: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_14;
+        return s_n_llhttp__internal__n_after_start_req_14;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob25, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 45;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_14;
+          return s_n_llhttp__internal__n_after_start_req_14;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_17:
-    s_n_llhttp__internal__n_start_req_17: {
+    case s_n_llhttp__internal__n_after_start_req_17:
+    s_n_llhttp__internal__n_after_start_req_17: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_17;
+        return s_n_llhttp__internal__n_after_start_req_17;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob27, 9);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 41;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_17;
+          return s_n_llhttp__internal__n_after_start_req_17;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_16:
-    s_n_llhttp__internal__n_start_req_16: {
+    case s_n_llhttp__internal__n_after_start_req_16:
+    s_n_llhttp__internal__n_after_start_req_16: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_16;
+        return s_n_llhttp__internal__n_after_start_req_16;
       }
       switch (*p) {
         case '_': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_17;
+          goto s_n_llhttp__internal__n_after_start_req_17;
         }
         default: {
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_15:
-    s_n_llhttp__internal__n_start_req_15: {
+    case s_n_llhttp__internal__n_after_start_req_15:
+    s_n_llhttp__internal__n_after_start_req_15: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_15;
+        return s_n_llhttp__internal__n_after_start_req_15;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob26, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_start_req_16;
+          goto s_n_llhttp__internal__n_after_start_req_16;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_15;
+          return s_n_llhttp__internal__n_after_start_req_15;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_18:
-    s_n_llhttp__internal__n_start_req_18: {
+    case s_n_llhttp__internal__n_after_start_req_18:
+    s_n_llhttp__internal__n_after_start_req_18: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_18;
+        return s_n_llhttp__internal__n_after_start_req_18;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob28, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_18;
+          return s_n_llhttp__internal__n_after_start_req_18;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_20:
-    s_n_llhttp__internal__n_start_req_20: {
+    case s_n_llhttp__internal__n_after_start_req_20:
+    s_n_llhttp__internal__n_after_start_req_20: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_20;
+        return s_n_llhttp__internal__n_after_start_req_20;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob29, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 31;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_20;
+          return s_n_llhttp__internal__n_after_start_req_20;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_21:
-    s_n_llhttp__internal__n_start_req_21: {
+    case s_n_llhttp__internal__n_after_start_req_21:
+    s_n_llhttp__internal__n_after_start_req_21: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_21;
+        return s_n_llhttp__internal__n_after_start_req_21;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob30, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_21;
+          return s_n_llhttp__internal__n_after_start_req_21;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_19:
-    s_n_llhttp__internal__n_start_req_19: {
+    case s_n_llhttp__internal__n_after_start_req_19:
+    s_n_llhttp__internal__n_after_start_req_19: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_19;
+        return s_n_llhttp__internal__n_after_start_req_19;
       }
       switch (*p) {
         case 'I': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_20;
+          goto s_n_llhttp__internal__n_after_start_req_20;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_21;
+          goto s_n_llhttp__internal__n_after_start_req_21;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_23:
-    s_n_llhttp__internal__n_start_req_23: {
+    case s_n_llhttp__internal__n_after_start_req_23:
+    s_n_llhttp__internal__n_after_start_req_23: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_23;
+        return s_n_llhttp__internal__n_after_start_req_23;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob31, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 24;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_23;
+          return s_n_llhttp__internal__n_after_start_req_23;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_24:
-    s_n_llhttp__internal__n_start_req_24: {
+    case s_n_llhttp__internal__n_after_start_req_24:
+    s_n_llhttp__internal__n_after_start_req_24: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_24;
+        return s_n_llhttp__internal__n_after_start_req_24;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob32, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 23;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_24;
+          return s_n_llhttp__internal__n_after_start_req_24;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_26:
-    s_n_llhttp__internal__n_start_req_26: {
+    case s_n_llhttp__internal__n_after_start_req_26:
+    s_n_llhttp__internal__n_after_start_req_26: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_26;
+        return s_n_llhttp__internal__n_after_start_req_26;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob33, 7);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 21;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_26;
+          return s_n_llhttp__internal__n_after_start_req_26;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_28:
-    s_n_llhttp__internal__n_start_req_28: {
+    case s_n_llhttp__internal__n_after_start_req_28:
+    s_n_llhttp__internal__n_after_start_req_28: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_28;
+        return s_n_llhttp__internal__n_after_start_req_28;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob34, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 30;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_28;
+          return s_n_llhttp__internal__n_after_start_req_28;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_29:
-    s_n_llhttp__internal__n_start_req_29: {
+    case s_n_llhttp__internal__n_after_start_req_29:
+    s_n_llhttp__internal__n_after_start_req_29: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_29;
+        return s_n_llhttp__internal__n_after_start_req_29;
       }
       switch (*p) {
         case 'L': {
           p++;
           match = 10;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_27:
-    s_n_llhttp__internal__n_start_req_27: {
+    case s_n_llhttp__internal__n_after_start_req_27:
+    s_n_llhttp__internal__n_after_start_req_27: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_27;
+        return s_n_llhttp__internal__n_after_start_req_27;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_28;
+          goto s_n_llhttp__internal__n_after_start_req_28;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_29;
+          goto s_n_llhttp__internal__n_after_start_req_29;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_25:
-    s_n_llhttp__internal__n_start_req_25: {
+    case s_n_llhttp__internal__n_after_start_req_25:
+    s_n_llhttp__internal__n_after_start_req_25: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_25;
+        return s_n_llhttp__internal__n_after_start_req_25;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_26;
+          goto s_n_llhttp__internal__n_after_start_req_26;
         }
         case 'C': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_27;
+          goto s_n_llhttp__internal__n_after_start_req_27;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_30:
-    s_n_llhttp__internal__n_start_req_30: {
+    case s_n_llhttp__internal__n_after_start_req_30:
+    s_n_llhttp__internal__n_after_start_req_30: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_30;
+        return s_n_llhttp__internal__n_after_start_req_30;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob35, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 11;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_30;
+          return s_n_llhttp__internal__n_after_start_req_30;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_22:
-    s_n_llhttp__internal__n_start_req_22: {
+    case s_n_llhttp__internal__n_after_start_req_22:
+    s_n_llhttp__internal__n_after_start_req_22: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_22;
+        return s_n_llhttp__internal__n_after_start_req_22;
       }
       switch (*p) {
         case '-': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_23;
+          goto s_n_llhttp__internal__n_after_start_req_23;
         }
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_24;
+          goto s_n_llhttp__internal__n_after_start_req_24;
         }
         case 'K': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_25;
+          goto s_n_llhttp__internal__n_after_start_req_25;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_30;
+          goto s_n_llhttp__internal__n_after_start_req_30;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_31:
-    s_n_llhttp__internal__n_start_req_31: {
+    case s_n_llhttp__internal__n_after_start_req_31:
+    s_n_llhttp__internal__n_after_start_req_31: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_31;
+        return s_n_llhttp__internal__n_after_start_req_31;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob36, 5);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 25;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_31;
+          return s_n_llhttp__internal__n_after_start_req_31;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_32:
-    s_n_llhttp__internal__n_start_req_32: {
+    case s_n_llhttp__internal__n_after_start_req_32:
+    s_n_llhttp__internal__n_after_start_req_32: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_32;
+        return s_n_llhttp__internal__n_after_start_req_32;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob37, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 6;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_32;
+          return s_n_llhttp__internal__n_after_start_req_32;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_35:
-    s_n_llhttp__internal__n_start_req_35: {
+    case s_n_llhttp__internal__n_after_start_req_35:
+    s_n_llhttp__internal__n_after_start_req_35: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_35;
+        return s_n_llhttp__internal__n_after_start_req_35;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob38, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 28;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_35;
+          return s_n_llhttp__internal__n_after_start_req_35;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_36:
-    s_n_llhttp__internal__n_start_req_36: {
+    case s_n_llhttp__internal__n_after_start_req_36:
+    s_n_llhttp__internal__n_after_start_req_36: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_36;
+        return s_n_llhttp__internal__n_after_start_req_36;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob39, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 39;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_36;
+          return s_n_llhttp__internal__n_after_start_req_36;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_34:
-    s_n_llhttp__internal__n_start_req_34: {
+    case s_n_llhttp__internal__n_after_start_req_34:
+    s_n_llhttp__internal__n_after_start_req_34: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_34;
+        return s_n_llhttp__internal__n_after_start_req_34;
       }
       switch (*p) {
         case 'T': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_35;
+          goto s_n_llhttp__internal__n_after_start_req_35;
         }
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_36;
+          goto s_n_llhttp__internal__n_after_start_req_36;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_37:
-    s_n_llhttp__internal__n_start_req_37: {
+    case s_n_llhttp__internal__n_after_start_req_37:
+    s_n_llhttp__internal__n_after_start_req_37: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_37;
+        return s_n_llhttp__internal__n_after_start_req_37;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob40, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 38;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_37;
+          return s_n_llhttp__internal__n_after_start_req_37;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_38:
-    s_n_llhttp__internal__n_start_req_38: {
+    case s_n_llhttp__internal__n_after_start_req_38:
+    s_n_llhttp__internal__n_after_start_req_38: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_38;
+        return s_n_llhttp__internal__n_after_start_req_38;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob41, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 3;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_38;
+          return s_n_llhttp__internal__n_after_start_req_38;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_42:
-    s_n_llhttp__internal__n_start_req_42: {
+    case s_n_llhttp__internal__n_after_start_req_42:
+    s_n_llhttp__internal__n_after_start_req_42: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_42;
+        return s_n_llhttp__internal__n_after_start_req_42;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob42, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 12;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_42;
+          return s_n_llhttp__internal__n_after_start_req_42;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_43:
-    s_n_llhttp__internal__n_start_req_43: {
+    case s_n_llhttp__internal__n_after_start_req_43:
+    s_n_llhttp__internal__n_after_start_req_43: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_43;
+        return s_n_llhttp__internal__n_after_start_req_43;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob43, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 13;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_43;
+          return s_n_llhttp__internal__n_after_start_req_43;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_41:
-    s_n_llhttp__internal__n_start_req_41: {
+    case s_n_llhttp__internal__n_after_start_req_41:
+    s_n_llhttp__internal__n_after_start_req_41: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_41;
+        return s_n_llhttp__internal__n_after_start_req_41;
       }
       switch (*p) {
         case 'F': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_42;
+          goto s_n_llhttp__internal__n_after_start_req_42;
         }
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_43;
+          goto s_n_llhttp__internal__n_after_start_req_43;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_40:
-    s_n_llhttp__internal__n_start_req_40: {
+    case s_n_llhttp__internal__n_after_start_req_40:
+    s_n_llhttp__internal__n_after_start_req_40: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_40;
+        return s_n_llhttp__internal__n_after_start_req_40;
       }
       switch (*p) {
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_41;
+          goto s_n_llhttp__internal__n_after_start_req_41;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_39:
-    s_n_llhttp__internal__n_start_req_39: {
+    case s_n_llhttp__internal__n_after_start_req_39:
+    s_n_llhttp__internal__n_after_start_req_39: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_39;
+        return s_n_llhttp__internal__n_after_start_req_39;
       }
       switch (*p) {
         case 'I': {
           p++;
           match = 34;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_40;
+          goto s_n_llhttp__internal__n_after_start_req_40;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_45:
-    s_n_llhttp__internal__n_start_req_45: {
+    case s_n_llhttp__internal__n_after_start_req_45:
+    s_n_llhttp__internal__n_after_start_req_45: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_45;
+        return s_n_llhttp__internal__n_after_start_req_45;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob44, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 29;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_45;
+          return s_n_llhttp__internal__n_after_start_req_45;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_44:
-    s_n_llhttp__internal__n_start_req_44: {
+    case s_n_llhttp__internal__n_after_start_req_44:
+    s_n_llhttp__internal__n_after_start_req_44: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_44;
+        return s_n_llhttp__internal__n_after_start_req_44;
       }
       switch (*p) {
         case 'R': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_45;
+          goto s_n_llhttp__internal__n_after_start_req_45;
         }
         case 'T': {
           p++;
           match = 4;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_33:
-    s_n_llhttp__internal__n_start_req_33: {
+    case s_n_llhttp__internal__n_after_start_req_33:
+    s_n_llhttp__internal__n_after_start_req_33: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_33;
+        return s_n_llhttp__internal__n_after_start_req_33;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_34;
+          goto s_n_llhttp__internal__n_after_start_req_34;
         }
         case 'L': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_37;
+          goto s_n_llhttp__internal__n_after_start_req_37;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_38;
+          goto s_n_llhttp__internal__n_after_start_req_38;
         }
         case 'R': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_39;
+          goto s_n_llhttp__internal__n_after_start_req_39;
         }
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_44;
+          goto s_n_llhttp__internal__n_after_start_req_44;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_48:
-    s_n_llhttp__internal__n_start_req_48: {
+    case s_n_llhttp__internal__n_after_start_req_48:
+    s_n_llhttp__internal__n_after_start_req_48: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_48;
+        return s_n_llhttp__internal__n_after_start_req_48;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob45, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 17;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_48;
+          return s_n_llhttp__internal__n_after_start_req_48;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_49:
-    s_n_llhttp__internal__n_start_req_49: {
+    case s_n_llhttp__internal__n_after_start_req_49:
+    s_n_llhttp__internal__n_after_start_req_49: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_49;
+        return s_n_llhttp__internal__n_after_start_req_49;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob46, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 44;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_49;
+          return s_n_llhttp__internal__n_after_start_req_49;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_50:
-    s_n_llhttp__internal__n_start_req_50: {
+    case s_n_llhttp__internal__n_after_start_req_50:
+    s_n_llhttp__internal__n_after_start_req_50: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_50;
+        return s_n_llhttp__internal__n_after_start_req_50;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob47, 5);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 43;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_50;
+          return s_n_llhttp__internal__n_after_start_req_50;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_51:
-    s_n_llhttp__internal__n_start_req_51: {
+    case s_n_llhttp__internal__n_after_start_req_51:
+    s_n_llhttp__internal__n_after_start_req_51: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_51;
+        return s_n_llhttp__internal__n_after_start_req_51;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob48, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 20;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_51;
+          return s_n_llhttp__internal__n_after_start_req_51;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_47:
-    s_n_llhttp__internal__n_start_req_47: {
+    case s_n_llhttp__internal__n_after_start_req_47:
+    s_n_llhttp__internal__n_after_start_req_47: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_47;
+        return s_n_llhttp__internal__n_after_start_req_47;
       }
       switch (*p) {
         case 'B': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_48;
+          goto s_n_llhttp__internal__n_after_start_req_48;
         }
         case 'C': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_49;
+          goto s_n_llhttp__internal__n_after_start_req_49;
         }
         case 'D': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_50;
+          goto s_n_llhttp__internal__n_after_start_req_50;
         }
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_51;
+          goto s_n_llhttp__internal__n_after_start_req_51;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_46:
-    s_n_llhttp__internal__n_start_req_46: {
+    case s_n_llhttp__internal__n_after_start_req_46:
+    s_n_llhttp__internal__n_after_start_req_46: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_46;
+        return s_n_llhttp__internal__n_after_start_req_46;
       }
       switch (*p) {
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_47;
+          goto s_n_llhttp__internal__n_after_start_req_47;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_54:
-    s_n_llhttp__internal__n_start_req_54: {
+    case s_n_llhttp__internal__n_after_start_req_54:
+    s_n_llhttp__internal__n_after_start_req_54: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_54;
+        return s_n_llhttp__internal__n_after_start_req_54;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob49, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 14;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_54;
+          return s_n_llhttp__internal__n_after_start_req_54;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_56:
-    s_n_llhttp__internal__n_start_req_56: {
+    case s_n_llhttp__internal__n_after_start_req_56:
+    s_n_llhttp__internal__n_after_start_req_56: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_56;
+        return s_n_llhttp__internal__n_after_start_req_56;
       }
       switch (*p) {
         case 'P': {
           p++;
           match = 37;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_57:
-    s_n_llhttp__internal__n_start_req_57: {
+    case s_n_llhttp__internal__n_after_start_req_57:
+    s_n_llhttp__internal__n_after_start_req_57: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_57;
+        return s_n_llhttp__internal__n_after_start_req_57;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob50, 9);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 42;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_57;
+          return s_n_llhttp__internal__n_after_start_req_57;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_55:
-    s_n_llhttp__internal__n_start_req_55: {
+    case s_n_llhttp__internal__n_after_start_req_55:
+    s_n_llhttp__internal__n_after_start_req_55: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_55;
+        return s_n_llhttp__internal__n_after_start_req_55;
       }
       switch (*p) {
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_56;
+          goto s_n_llhttp__internal__n_after_start_req_56;
         }
         case '_': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_57;
+          goto s_n_llhttp__internal__n_after_start_req_57;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_53:
-    s_n_llhttp__internal__n_start_req_53: {
+    case s_n_llhttp__internal__n_after_start_req_53:
+    s_n_llhttp__internal__n_after_start_req_53: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_53;
+        return s_n_llhttp__internal__n_after_start_req_53;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_54;
+          goto s_n_llhttp__internal__n_after_start_req_54;
         }
         case 'T': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_55;
+          goto s_n_llhttp__internal__n_after_start_req_55;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_58:
-    s_n_llhttp__internal__n_start_req_58: {
+    case s_n_llhttp__internal__n_after_start_req_58:
+    s_n_llhttp__internal__n_after_start_req_58: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_58;
+        return s_n_llhttp__internal__n_after_start_req_58;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob51, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 33;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_58;
+          return s_n_llhttp__internal__n_after_start_req_58;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_59:
-    s_n_llhttp__internal__n_start_req_59: {
+    case s_n_llhttp__internal__n_after_start_req_59:
+    s_n_llhttp__internal__n_after_start_req_59: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_59;
+        return s_n_llhttp__internal__n_after_start_req_59;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob52, 7);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 26;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_59;
+          return s_n_llhttp__internal__n_after_start_req_59;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_52:
-    s_n_llhttp__internal__n_start_req_52: {
+    case s_n_llhttp__internal__n_after_start_req_52:
+    s_n_llhttp__internal__n_after_start_req_52: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_52;
+        return s_n_llhttp__internal__n_after_start_req_52;
       }
       switch (*p) {
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_53;
+          goto s_n_llhttp__internal__n_after_start_req_53;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_58;
+          goto s_n_llhttp__internal__n_after_start_req_58;
         }
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_59;
+          goto s_n_llhttp__internal__n_after_start_req_59;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_61:
-    s_n_llhttp__internal__n_start_req_61: {
+    case s_n_llhttp__internal__n_after_start_req_61:
+    s_n_llhttp__internal__n_after_start_req_61: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_61;
+        return s_n_llhttp__internal__n_after_start_req_61;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob53, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 40;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_61;
+          return s_n_llhttp__internal__n_after_start_req_61;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_62:
-    s_n_llhttp__internal__n_start_req_62: {
+    case s_n_llhttp__internal__n_after_start_req_62:
+    s_n_llhttp__internal__n_after_start_req_62: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_62;
+        return s_n_llhttp__internal__n_after_start_req_62;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob54, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 7;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_62;
+          return s_n_llhttp__internal__n_after_start_req_62;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_60:
-    s_n_llhttp__internal__n_start_req_60: {
+    case s_n_llhttp__internal__n_after_start_req_60:
+    s_n_llhttp__internal__n_after_start_req_60: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_60;
+        return s_n_llhttp__internal__n_after_start_req_60;
       }
       switch (*p) {
         case 'E': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_61;
+          goto s_n_llhttp__internal__n_after_start_req_61;
         }
         case 'R': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_62;
+          goto s_n_llhttp__internal__n_after_start_req_62;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_65:
-    s_n_llhttp__internal__n_start_req_65: {
+    case s_n_llhttp__internal__n_after_start_req_65:
+    s_n_llhttp__internal__n_after_start_req_65: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_65;
+        return s_n_llhttp__internal__n_after_start_req_65;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob55, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 18;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_65;
+          return s_n_llhttp__internal__n_after_start_req_65;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_67:
-    s_n_llhttp__internal__n_start_req_67: {
+    case s_n_llhttp__internal__n_after_start_req_67:
+    s_n_llhttp__internal__n_after_start_req_67: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_67;
+        return s_n_llhttp__internal__n_after_start_req_67;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob56, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 32;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_67;
+          return s_n_llhttp__internal__n_after_start_req_67;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_68:
-    s_n_llhttp__internal__n_start_req_68: {
+    case s_n_llhttp__internal__n_after_start_req_68:
+    s_n_llhttp__internal__n_after_start_req_68: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_68;
+        return s_n_llhttp__internal__n_after_start_req_68;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob57, 2);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 15;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_68;
+          return s_n_llhttp__internal__n_after_start_req_68;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_66:
-    s_n_llhttp__internal__n_start_req_66: {
+    case s_n_llhttp__internal__n_after_start_req_66:
+    s_n_llhttp__internal__n_after_start_req_66: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_66;
+        return s_n_llhttp__internal__n_after_start_req_66;
       }
       switch (*p) {
         case 'I': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_67;
+          goto s_n_llhttp__internal__n_after_start_req_67;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_68;
+          goto s_n_llhttp__internal__n_after_start_req_68;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_69:
-    s_n_llhttp__internal__n_start_req_69: {
+    case s_n_llhttp__internal__n_after_start_req_69:
+    s_n_llhttp__internal__n_after_start_req_69: {
       llparse_match_t match_seq;
       
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_69;
+        return s_n_llhttp__internal__n_after_start_req_69;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob58, 8);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
           match = 27;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
-          return s_n_llhttp__internal__n_start_req_69;
+          return s_n_llhttp__internal__n_after_start_req_69;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_64:
-    s_n_llhttp__internal__n_start_req_64: {
+    case s_n_llhttp__internal__n_after_start_req_64:
+    s_n_llhttp__internal__n_after_start_req_64: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_64;
+        return s_n_llhttp__internal__n_after_start_req_64;
       }
       switch (*p) {
         case 'B': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_65;
+          goto s_n_llhttp__internal__n_after_start_req_65;
         }
         case 'L': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_66;
+          goto s_n_llhttp__internal__n_after_start_req_66;
         }
         case 'S': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_69;
+          goto s_n_llhttp__internal__n_after_start_req_69;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req_63:
-    s_n_llhttp__internal__n_start_req_63: {
+    case s_n_llhttp__internal__n_after_start_req_63:
+    s_n_llhttp__internal__n_after_start_req_63: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req_63;
+        return s_n_llhttp__internal__n_after_start_req_63;
       }
       switch (*p) {
         case 'N': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_64;
+          goto s_n_llhttp__internal__n_after_start_req_64;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_start_req:
-    s_n_llhttp__internal__n_start_req: {
+    case s_n_llhttp__internal__n_after_start_req:
+    s_n_llhttp__internal__n_after_start_req: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_start_req;
+        return s_n_llhttp__internal__n_after_start_req;
       }
       switch (*p) {
         case 'A': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_1;
+          goto s_n_llhttp__internal__n_after_start_req_1;
         }
         case 'B': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_4;
+          goto s_n_llhttp__internal__n_after_start_req_4;
         }
         case 'C': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_5;
+          goto s_n_llhttp__internal__n_after_start_req_5;
         }
         case 'D': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_10;
+          goto s_n_llhttp__internal__n_after_start_req_10;
         }
         case 'F': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_14;
+          goto s_n_llhttp__internal__n_after_start_req_14;
         }
         case 'G': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_15;
+          goto s_n_llhttp__internal__n_after_start_req_15;
         }
         case 'H': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_18;
+          goto s_n_llhttp__internal__n_after_start_req_18;
         }
         case 'L': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_19;
+          goto s_n_llhttp__internal__n_after_start_req_19;
         }
         case 'M': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_22;
+          goto s_n_llhttp__internal__n_after_start_req_22;
         }
         case 'N': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_31;
+          goto s_n_llhttp__internal__n_after_start_req_31;
         }
         case 'O': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_32;
+          goto s_n_llhttp__internal__n_after_start_req_32;
         }
         case 'P': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_33;
+          goto s_n_llhttp__internal__n_after_start_req_33;
         }
         case 'R': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_46;
+          goto s_n_llhttp__internal__n_after_start_req_46;
         }
         case 'S': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_52;
+          goto s_n_llhttp__internal__n_after_start_req_52;
         }
         case 'T': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_60;
+          goto s_n_llhttp__internal__n_after_start_req_60;
         }
         case 'U': {
           p++;
-          goto s_n_llhttp__internal__n_start_req_63;
+          goto s_n_llhttp__internal__n_after_start_req_63;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_62;
+          goto s_n_llhttp__internal__n_error_84;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_method_1:
+    s_n_llhttp__internal__n_span_start_llhttp__on_method_1: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_method_1;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_method;
+      goto s_n_llhttp__internal__n_after_start_req;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_invoke_llhttp__on_status_complete:
     s_n_llhttp__internal__n_invoke_llhttp__on_status_complete: {
       switch (llhttp__on_status_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_headers_start;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_20;
         default:
-          goto s_n_llhttp__internal__n_header_field_start;
+          goto s_n_llhttp__internal__n_error_70;
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_line_almost_done:
     s_n_llhttp__internal__n_res_line_almost_done: {
       if (p == endp) {
@@ -13308,24 +15155,150 @@
           goto s_n_llhttp__internal__n_res_status_start;
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_res_status_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_54;
+          goto s_n_llhttp__internal__n_error_71;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_res_status_code_digit_3:
+    s_n_llhttp__internal__n_res_status_code_digit_3: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_res_status_code_digit_3;
+      }
+      switch (*p) {
+        case '0': {
+          p++;
+          match = 0;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '1': {
+          p++;
+          match = 1;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '2': {
+          p++;
+          match = 2;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '3': {
+          p++;
+          match = 3;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '4': {
+          p++;
+          match = 4;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '5': {
+          p++;
+          match = 5;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '6': {
+          p++;
+          match = 6;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '7': {
+          p++;
+          match = 7;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '8': {
+          p++;
+          match = 8;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        case '9': {
+          p++;
+          match = 9;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_2;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_error_73;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_res_status_code_digit_2:
+    s_n_llhttp__internal__n_res_status_code_digit_2: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_res_status_code_digit_2;
+      }
+      switch (*p) {
+        case '0': {
+          p++;
+          match = 0;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '1': {
+          p++;
+          match = 1;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '2': {
+          p++;
+          match = 2;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '3': {
+          p++;
+          match = 3;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '4': {
+          p++;
+          match = 4;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '5': {
+          p++;
+          match = 5;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '6': {
+          p++;
+          match = 6;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '7': {
+          p++;
+          match = 7;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '8': {
+          p++;
+          match = 8;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        case '9': {
+          p++;
+          match = 9;
+          goto s_n_llhttp__internal__n_invoke_mul_add_status_code_1;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_error_75;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_res_status_code:
-    s_n_llhttp__internal__n_res_status_code: {
+    case s_n_llhttp__internal__n_res_status_code_digit_1:
+    s_n_llhttp__internal__n_res_status_code_digit_1: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_res_status_code;
+        return s_n_llhttp__internal__n_res_status_code_digit_1;
       }
       switch (*p) {
         case '0': {
           p++;
           match = 0;
           goto s_n_llhttp__internal__n_invoke_mul_add_status_code;
         }
@@ -13371,37 +15344,70 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_mul_add_status_code;
         }
         default: {
-          goto s_n_llhttp__internal__n_res_status_code_otherwise;
+          goto s_n_llhttp__internal__n_error_77;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_res_http_end:
-    s_n_llhttp__internal__n_res_http_end: {
+    case s_n_llhttp__internal__n_res_after_version:
+    s_n_llhttp__internal__n_res_after_version: {
       if (p == endp) {
-        return s_n_llhttp__internal__n_res_http_end;
+        return s_n_llhttp__internal__n_res_after_version;
       }
       switch (*p) {
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_invoke_update_status_code;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_55;
+          goto s_n_llhttp__internal__n_error_78;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1:
+    s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1: {
+      switch (llhttp__on_version_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_res_after_version;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_21;
+        default:
+          goto s_n_llhttp__internal__n_error_69;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_68:
+    s_n_llhttp__internal__n_error_68: {
+      state->error = 0x9;
+      state->reason = "Invalid HTTP version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_79:
+    s_n_llhttp__internal__n_error_79: {
+      state->error = 0x9;
+      state->reason = "Invalid minor version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_res_http_minor:
     s_n_llhttp__internal__n_res_http_minor: {
       if (p == endp) {
         return s_n_llhttp__internal__n_res_http_minor;
       }
       switch (*p) {
         case '0': {
@@ -13451,37 +15457,57 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_minor_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_7;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_80:
+    s_n_llhttp__internal__n_error_80: {
+      state->error = 0x9;
+      state->reason = "Expected dot";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_res_http_dot:
     s_n_llhttp__internal__n_res_http_dot: {
       if (p == endp) {
         return s_n_llhttp__internal__n_res_http_dot;
       }
       switch (*p) {
         case '.': {
           p++;
           goto s_n_llhttp__internal__n_res_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_59;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_8;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_81:
+    s_n_llhttp__internal__n_error_81: {
+      state->error = 0x9;
+      state->reason = "Invalid major version";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_res_http_major:
     s_n_llhttp__internal__n_res_http_major: {
       if (p == endp) {
         return s_n_llhttp__internal__n_res_http_major;
       }
       switch (*p) {
         case '0': {
@@ -13531,44 +15557,68 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_major_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_60;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_version_9;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_version_1:
+    s_n_llhttp__internal__n_span_start_llhttp__on_version_1: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_version_1;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_version;
+      goto s_n_llhttp__internal__n_res_http_major;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_start_res:
     s_n_llhttp__internal__n_start_res: {
       llparse_match_t match_seq;
       
       if (p == endp) {
         return s_n_llhttp__internal__n_start_res;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob59, 5);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_res_http_major;
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_version_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_res;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_63;
+          goto s_n_llhttp__internal__n_error_85;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_llhttp__on_method_complete:
+    s_n_llhttp__internal__n_invoke_llhttp__on_method_complete: {
+      switch (llhttp__on_method_complete(state, p, endp)) {
+        case 0:
+          goto s_n_llhttp__internal__n_req_first_space_before_url;
+        case 21:
+          goto s_n_llhttp__internal__n_pause_19;
+        default:
+          goto s_n_llhttp__internal__n_error_1;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_or_res_method_2:
     s_n_llhttp__internal__n_req_or_res_method_2: {
       llparse_match_t match_seq;
       
       if (p == endp) {
         return s_n_llhttp__internal__n_req_or_res_method_2;
       }
@@ -13580,39 +15630,48 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_method;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_or_res_method_2;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_61;
+          goto s_n_llhttp__internal__n_error_82;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_update_type_1:
+    s_n_llhttp__internal__n_invoke_update_type_1: {
+      switch (llhttp__internal__c_update_type_1(state, p, endp)) {
+        default:
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_version_1;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_req_or_res_method_3:
     s_n_llhttp__internal__n_req_or_res_method_3: {
       llparse_match_t match_seq;
       
       if (p == endp) {
         return s_n_llhttp__internal__n_req_or_res_method_3;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob61, 3);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_type_1;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_or_res_method_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_61;
+          goto s_n_llhttp__internal__n_error_82;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method_1:
     s_n_llhttp__internal__n_req_or_res_method_1: {
@@ -13625,15 +15684,15 @@
           goto s_n_llhttp__internal__n_req_or_res_method_2;
         }
         case 'T': {
           p++;
           goto s_n_llhttp__internal__n_req_or_res_method_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_61;
+          goto s_n_llhttp__internal__n_error_82;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method:
     s_n_llhttp__internal__n_req_or_res_method: {
@@ -13642,49 +15701,69 @@
       }
       switch (*p) {
         case 'H': {
           p++;
           goto s_n_llhttp__internal__n_req_or_res_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_61;
+          goto s_n_llhttp__internal__n_error_82;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_span_start_llhttp__on_method:
+    s_n_llhttp__internal__n_span_start_llhttp__on_method: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_span_start_llhttp__on_method;
+      }
+      state->_span_pos0 = (void*) p;
+      state->_span_cb0 = llhttp__on_method;
+      goto s_n_llhttp__internal__n_req_or_res_method;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_start_req_or_res:
     s_n_llhttp__internal__n_start_req_or_res: {
       if (p == endp) {
         return s_n_llhttp__internal__n_start_req_or_res;
       }
       switch (*p) {
         case 'H': {
-          goto s_n_llhttp__internal__n_req_or_res_method;
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_method;
         }
         default: {
           goto s_n_llhttp__internal__n_invoke_update_type_2;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_load_type:
     s_n_llhttp__internal__n_invoke_load_type: {
       switch (llhttp__internal__c_load_type(state, p, endp)) {
         case 1:
-          goto s_n_llhttp__internal__n_start_req;
+          goto s_n_llhttp__internal__n_span_start_llhttp__on_method_1;
         case 2:
           goto s_n_llhttp__internal__n_start_res;
         default:
           goto s_n_llhttp__internal__n_start_req_or_res;
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_invoke_update_finish:
+    s_n_llhttp__internal__n_invoke_update_finish: {
+      switch (llhttp__internal__c_update_finish(state, p, endp)) {
+        default:
+          goto s_n_llhttp__internal__n_invoke_llhttp__on_message_begin;
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_start:
     s_n_llhttp__internal__n_start: {
       if (p == endp) {
         return s_n_llhttp__internal__n_start;
       }
       switch (*p) {
         case 10: {
@@ -13692,25 +15771,25 @@
           goto s_n_llhttp__internal__n_start;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_finish;
+          goto s_n_llhttp__internal__n_invoke_load_initial_message_completed;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     default:
       /* UNREACHABLE */
       abort();
   }
-  s_n_llhttp__internal__n_error_46: {
+  s_n_llhttp__internal__n_error_63: {
     state->error = 0x7;
     state->reason = "Invalid characters in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13719,81 +15798,97 @@
     switch (llhttp__internal__c_update_finish_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_start;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags: {
-    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
-      case 1:
+  s_n_llhttp__internal__n_invoke_update_initial_message_completed: {
+    switch (llhttp__internal__c_update_initial_message_completed(state, p, endp)) {
+      default:
         goto s_n_llhttp__internal__n_invoke_update_finish_2;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_content_length: {
+    switch (llhttp__internal__c_update_content_length(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_invoke_update_initial_message_completed;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_1: {
+    switch (llhttp__internal__c_test_lenient_flags_1(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_update_initial_message_completed;
       default:
         goto s_n_llhttp__internal__n_closed;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_update_finish_1: {
     switch (llhttp__internal__c_update_finish_1(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_pause_5: {
+  s_n_llhttp__internal__n_pause_11: {
     state->error = 0x15;
     state->reason = "on_message_complete pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_is_equal_upgrade;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_10: {
+  s_n_llhttp__internal__n_error_24: {
     state->error = 0x12;
     state->reason = "`on_message_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_pause_7: {
+  s_n_llhttp__internal__n_pause_13: {
     state->error = 0x15;
     state->reason = "on_chunk_complete pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_13: {
+  s_n_llhttp__internal__n_error_27: {
     state->error = 0x14;
     state->reason = "`on_chunk_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_chunk_complete_1: {
     switch (llhttp__on_chunk_complete(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_2;
       case 21:
-        goto s_n_llhttp__internal__n_pause_7;
+        goto s_n_llhttp__internal__n_pause_13;
       default:
-        goto s_n_llhttp__internal__n_error_13;
+        goto s_n_llhttp__internal__n_error_27;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_12: {
+  s_n_llhttp__internal__n_error_26: {
     state->error = 0x4;
     state->reason = "Content-Length can't be present with Transfer-Encoding";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13803,15 +15898,15 @@
     state->reason = "on_message_complete pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_pause_1;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_3: {
+  s_n_llhttp__internal__n_error_6: {
     state->error = 0x12;
     state->reason = "`on_message_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13819,54 +15914,54 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_message_complete_1: {
     switch (llhttp__on_message_complete(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_pause_1;
       case 21:
         goto s_n_llhttp__internal__n_pause_2;
       default:
-        goto s_n_llhttp__internal__n_error_3;
+        goto s_n_llhttp__internal__n_error_6;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_8: {
+  s_n_llhttp__internal__n_error_22: {
     state->error = 0xc;
     state->reason = "Chunk size overflow";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_pause_3: {
     state->error = 0x15;
     state->reason = "on_chunk_complete pause";
     state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_update_content_length;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_update_content_length_1;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_5: {
+  s_n_llhttp__internal__n_error_8: {
     state->error = 0x14;
     state->reason = "`on_chunk_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_chunk_complete: {
     switch (llhttp__on_chunk_complete(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_invoke_update_content_length;
+        goto s_n_llhttp__internal__n_invoke_update_content_length_1;
       case 21:
         goto s_n_llhttp__internal__n_pause_3;
       default:
-        goto s_n_llhttp__internal__n_error_5;
+        goto s_n_llhttp__internal__n_error_8;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_body: {
     const unsigned char* start;
     int err;
@@ -13897,15 +15992,15 @@
     state->reason = "on_chunk_header pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_is_equal_content_length;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_4: {
+  s_n_llhttp__internal__n_error_7: {
     state->error = 0x13;
     state->reason = "`on_chunk_header` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13913,48 +16008,347 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_chunk_header: {
     switch (llhttp__on_chunk_header(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_is_equal_content_length;
       case 21:
         goto s_n_llhttp__internal__n_pause_4;
       default:
-        goto s_n_llhttp__internal__n_error_4;
+        goto s_n_llhttp__internal__n_error_7;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_6: {
+  s_n_llhttp__internal__n_error_9: {
     state->error = 0x2;
-    state->reason = "Invalid character in chunk parameters";
+    state->reason = "Invalid character in chunk extensions";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_7: {
+  s_n_llhttp__internal__n_error_10: {
+    state->error = 0x2;
+    state->reason = "Invalid character in chunk extensions";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_5: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_name pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_size_almost_done;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_11: {
+    state->error = 0x22;
+    state->reason = "`on_chunk_extension_name` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_name(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_6: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_name pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_extensions;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_12: {
+    state->error = 0x22;
+    state->reason = "`on_chunk_extension_name` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_1: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_name(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_1;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_7: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_value pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_size_almost_done;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_14: {
+    state->error = 0x23;
+    state->reason = "`on_chunk_extension_value` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_16: {
+    state->error = 0x2;
+    state->reason = "Invalid character in chunk extensions quote value";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_8: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_value pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_extension_quoted_value_done;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_15: {
+    state->error = 0x23;
+    state->reason = "`on_chunk_extension_value` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_1: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_1;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_17;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_17;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_9: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_value pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_size_otherwise;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_18: {
+    state->error = 0x23;
+    state->reason = "`on_chunk_extension_value` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_3: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_value_complete_2;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_value_4: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_19;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_19;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_10: {
+    state->error = 0x15;
+    state->reason = "on_chunk_extension_name pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_chunk_extension_value;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_13: {
+    state->error = 0x22;
+    state->reason = "`on_chunk_extension_name` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_llhttp__on_chunk_extension_name_complete_2: {
+    switch (llhttp__on_chunk_extension_name_complete(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_chunk_extension_value;
+      case 21:
+        goto s_n_llhttp__internal__n_pause_10;
+      default:
+        goto s_n_llhttp__internal__n_error_13;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_name(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_span_start_llhttp__on_chunk_extension_value;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_chunk_extension_name_3: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_chunk_extension_name(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_20;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_20;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_21: {
     state->error = 0xc;
     state->reason = "Invalid character in chunk size";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_mul_add_content_length: {
     switch (llhttp__internal__c_mul_add_content_length(state, p, endp, match)) {
       case 1:
-        goto s_n_llhttp__internal__n_error_8;
+        goto s_n_llhttp__internal__n_error_22;
       default:
         goto s_n_llhttp__internal__n_chunk_size;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_9: {
+  s_n_llhttp__internal__n_error_23: {
     state->error = 0xc;
     state->reason = "Invalid character in chunk size";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13980,15 +16374,15 @@
     switch (llhttp__internal__c_update_finish_3(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_span_start_llhttp__on_body_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_11: {
+  s_n_llhttp__internal__n_error_25: {
     state->error = 0xf;
     state->reason = "Request has invalid `Transfer-Encoding`";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13998,15 +16392,15 @@
     state->reason = "on_message_complete pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__after_message_complete;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_2: {
+  s_n_llhttp__internal__n_error_5: {
     state->error = 0x12;
     state->reason = "`on_message_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14014,15 +16408,15 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_message_complete: {
     switch (llhttp__on_message_complete(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_llhttp__after_message_complete;
       case 21:
         goto s_n_llhttp__internal__n_pause;
       default:
-        goto s_n_llhttp__internal__n_error_2;
+        goto s_n_llhttp__internal__n_error_5;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_1: {
     switch (llhttp__internal__c_or_flags_1(state, p, endp)) {
       default:
@@ -14043,24 +16437,24 @@
     switch (llhttp__internal__c_update_upgrade(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_or_flags_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_pause_6: {
+  s_n_llhttp__internal__n_pause_12: {
     state->error = 0x15;
     state->reason = "Paused by on_headers_complete";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_1: {
+  s_n_llhttp__internal__n_error_4: {
     state->error = 0x11;
     state->reason = "User callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14070,43 +16464,43 @@
       case 0:
         goto s_n_llhttp__internal__n_invoke_llhttp__after_headers_complete;
       case 1:
         goto s_n_llhttp__internal__n_invoke_or_flags_1;
       case 2:
         goto s_n_llhttp__internal__n_invoke_update_upgrade;
       case 21:
-        goto s_n_llhttp__internal__n_pause_6;
+        goto s_n_llhttp__internal__n_pause_12;
       default:
-        goto s_n_llhttp__internal__n_error_1;
+        goto s_n_llhttp__internal__n_error_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__before_headers_complete: {
     switch (llhttp__before_headers_complete(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_headers_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_1: {
-    switch (llhttp__internal__c_test_lenient_flags_1(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_2: {
+    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_error_12;
+        goto s_n_llhttp__internal__n_error_26;
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__before_headers_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_test_flags_1: {
     switch (llhttp__internal__c_test_flags_1(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_1;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_2;
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__before_headers_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_test_flags: {
@@ -14125,41 +16519,78 @@
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_field(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) (p + 1);
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_14;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_28;
       return s_error;
     }
     p++;
-    goto s_n_llhttp__internal__n_error_14;
+    goto s_n_llhttp__internal__n_error_28;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_2: {
-    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_3: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
       case 1:
         goto s_n_llhttp__internal__n_header_field_colon_discard_ws;
       default:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_15: {
+  s_n_llhttp__internal__n_error_31: {
+    state->error = 0xa;
+    state->reason = "Invalid header value char";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_5: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_ws;
+      default:
+        goto s_n_llhttp__internal__n_error_31;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_33: {
     state->error = 0xb;
     state->reason = "Empty Content-Length";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_pause_14: {
+    state->error = 0x15;
+    state->reason = "on_header_value_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_header_field_start;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_32: {
+    state->error = 0x1d;
+    state->reason = "`on_header_value_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_value: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
@@ -14228,62 +16659,118 @@
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_header_state: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 2:
-        goto s_n_llhttp__internal__n_error_15;
+        goto s_n_llhttp__internal__n_error_33;
       default:
         goto s_n_llhttp__internal__n_invoke_load_header_state_1;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_error_30: {
+    state->error = 0xa;
+    state->reason = "Invalid header value char";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_4: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_lws;
+      default:
+        goto s_n_llhttp__internal__n_error_30;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_34: {
+    state->error = 0x2;
+    state->reason = "Expected LF after CR";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_6: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_lws;
+      default:
+        goto s_n_llhttp__internal__n_error_34;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_update_header_state_1: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_header_state_3: {
+    switch (llhttp__internal__c_load_header_state(state, p, endp)) {
+      case 8:
+        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+      default:
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_header_state_2: {
     switch (llhttp__internal__c_update_header_state(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_7: {
     switch (llhttp__internal__c_or_flags_3(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_8: {
     switch (llhttp__internal__c_or_flags_4(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_9: {
     switch (llhttp__internal__c_or_flags_5(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_10: {
     switch (llhttp__internal__c_or_flags_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_header_state_3: {
+  s_n_llhttp__internal__n_invoke_load_header_state_4: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 5:
         goto s_n_llhttp__internal__n_invoke_or_flags_7;
       case 6:
         goto s_n_llhttp__internal__n_invoke_or_flags_8;
       case 7:
         goto s_n_llhttp__internal__n_invoke_or_flags_9;
@@ -14291,15 +16778,15 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_10;
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_16: {
+  s_n_llhttp__internal__n_error_35: {
     state->error = 0x3;
     state->reason = "Missing expected LF after header value";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14362,83 +16849,73 @@
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
-      state->error_pos = (const char*) (p + 1);
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_17;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_36;
       return s_error;
     }
-    p++;
-    goto s_n_llhttp__internal__n_error_17;
+    goto s_n_llhttp__internal__n_error_36;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_18: {
-    state->error = 0xa;
-    state->reason = "Invalid header value char";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
-    /* UNREACHABLE */;
-    abort();
-  }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_3: {
-    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_7: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
       case 1:
         goto s_n_llhttp__internal__n_header_value_lenient;
       default:
-        goto s_n_llhttp__internal__n_header_value_lenient_failed;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_3: {
+  s_n_llhttp__internal__n_invoke_update_header_state_4: {
     switch (llhttp__internal__c_update_header_state(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_11: {
     switch (llhttp__internal__c_or_flags_3(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_12: {
     switch (llhttp__internal__c_or_flags_4(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_13: {
     switch (llhttp__internal__c_or_flags_5(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_14: {
     switch (llhttp__internal__c_or_flags_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_header_state_4: {
+  s_n_llhttp__internal__n_invoke_load_header_state_5: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 5:
         goto s_n_llhttp__internal__n_invoke_or_flags_11;
       case 6:
         goto s_n_llhttp__internal__n_invoke_or_flags_12;
       case 7:
         goto s_n_llhttp__internal__n_invoke_or_flags_13;
@@ -14446,40 +16923,40 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_14;
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_4: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_5: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_token;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_2: {
-    switch (llhttp__internal__c_update_header_state_2(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_3: {
+    switch (llhttp__internal__c_update_header_state_3(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_5: {
-    switch (llhttp__internal__c_update_header_state_5(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_6: {
+    switch (llhttp__internal__c_update_header_state_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_6: {
-    switch (llhttp__internal__c_update_header_state_6(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_7: {
+    switch (llhttp__internal__c_update_header_state_7(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5: {
@@ -14488,18 +16965,18 @@
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) p;
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_20;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_38;
       return s_error;
     }
-    goto s_n_llhttp__internal__n_error_20;
+    goto s_n_llhttp__internal__n_error_38;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_mul_add_content_length_1: {
     switch (llhttp__internal__c_mul_add_content_length_1(state, p, endp, match)) {
       case 1:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5;
@@ -14523,60 +17000,60 @@
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) p;
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_21;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_39;
       return s_error;
     }
-    goto s_n_llhttp__internal__n_error_21;
+    goto s_n_llhttp__internal__n_error_39;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_19: {
+  s_n_llhttp__internal__n_error_37: {
     state->error = 0x4;
     state->reason = "Duplicate Content-Length";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_test_flags_2: {
     switch (llhttp__internal__c_test_flags_2(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_header_value_content_length;
       default:
-        goto s_n_llhttp__internal__n_error_19;
+        goto s_n_llhttp__internal__n_error_37;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_value_8: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) (p + 1);
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_23;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_41;
       return s_error;
     }
     p++;
-    goto s_n_llhttp__internal__n_error_23;
+    goto s_n_llhttp__internal__n_error_41;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_7: {
-    switch (llhttp__internal__c_update_header_state_7(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_8: {
+    switch (llhttp__internal__c_update_header_state_8(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_otherwise;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_value_7: {
@@ -14585,44 +17062,44 @@
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) (p + 1);
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_22;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_40;
       return s_error;
     }
     p++;
-    goto s_n_llhttp__internal__n_error_22;
+    goto s_n_llhttp__internal__n_error_40;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_4: {
-    switch (llhttp__internal__c_test_lenient_flags_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_8: {
+    switch (llhttp__internal__c_test_lenient_flags_8(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_7;
       default:
         goto s_n_llhttp__internal__n_header_value_te_chunked;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_type_1: {
     switch (llhttp__internal__c_load_type(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_4;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_8;
       default:
         goto s_n_llhttp__internal__n_header_value_te_chunked;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_8: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_9: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_and_flags: {
@@ -14637,28 +17114,28 @@
     switch (llhttp__internal__c_or_flags_16(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_and_flags;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_5: {
-    switch (llhttp__internal__c_test_lenient_flags_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_9: {
+    switch (llhttp__internal__c_test_lenient_flags_8(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_8;
       default:
         goto s_n_llhttp__internal__n_invoke_or_flags_17;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_type_2: {
     switch (llhttp__internal__c_load_type(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_5;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_9;
       default:
         goto s_n_llhttp__internal__n_invoke_or_flags_17;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_16: {
@@ -14678,15 +17155,15 @@
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_18: {
     switch (llhttp__internal__c_or_flags_18(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_8;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_9;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_header_state_2: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 1:
@@ -14699,14 +17176,32 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_18;
       default:
         goto s_n_llhttp__internal__n_header_value;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_pause_15: {
+    state->error = 0x15;
+    state->reason = "on_header_field_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_header_value_discard_ws;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_29: {
+    state->error = 0x1c;
+    state->reason = "`on_header_field_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_field_1: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_field(state, start, p);
@@ -14735,51 +17230,92 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_24: {
+  s_n_llhttp__internal__n_error_42: {
     state->error = 0xa;
     state->reason = "Invalid header token";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_9: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_10: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_field_general;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_header_state: {
     switch (llhttp__internal__c_store_header_state(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_header_field_colon;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_10: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_11: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_field_general;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_error_3: {
+    state->error = 0x1e;
+    state->reason = "Unexpected space after start line";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags: {
+    switch (llhttp__internal__c_test_lenient_flags(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_field_start;
+      default:
+        goto s_n_llhttp__internal__n_error_3;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_16: {
+    state->error = 0x15;
+    state->reason = "on_url_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_headers_start;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_2: {
+    state->error = 0x1a;
+    state->reason = "`on_url_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_llhttp__on_url_complete: {
     switch (llhttp__on_url_complete(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_headers_start;
+      case 21:
+        goto s_n_llhttp__internal__n_pause_16;
       default:
-        goto s_n_llhttp__internal__n_header_field_start;
+        goto s_n_llhttp__internal__n_error_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_update_http_minor: {
     switch (llhttp__internal__c_update_http_minor(state, p, endp)) {
       default:
@@ -14809,15 +17345,15 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http09;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http09;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_25: {
+  s_n_llhttp__internal__n_error_43: {
     state->error = 0x7;
     state->reason = "Expected CRLF";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14835,350 +17371,402 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_lf_to_http09;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_lf_to_http09;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_30: {
+  s_n_llhttp__internal__n_error_49: {
     state->error = 0x17;
     state->reason = "Pause on PRI/Upgrade";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_31: {
+  s_n_llhttp__internal__n_error_50: {
     state->error = 0x9;
     state->reason = "Expected HTTP/2 Connection Preface";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_29: {
+  s_n_llhttp__internal__n_error_48: {
     state->error = 0x9;
     state->reason = "Expected CRLF after version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_method_1: {
-    switch (llhttp__internal__c_load_method(state, p, endp)) {
-      case 34:
-        goto s_n_llhttp__internal__n_req_pri_upgrade;
-      default:
-        goto s_n_llhttp__internal__n_req_http_complete;
-    }
+  s_n_llhttp__internal__n_pause_17: {
+    state->error = 0x15;
+    state->reason = "on_version_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_load_method_1;
+    return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_28: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
+  s_n_llhttp__internal__n_error_47: {
+    state->error = 0x21;
+    state->reason = "`on_version_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_1: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_version_complete;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_version_complete;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_version: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_46;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_46;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_load_http_minor: {
     switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
       case 9:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       default:
-        goto s_n_llhttp__internal__n_error_28;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_32: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
-    /* UNREACHABLE */;
-    abort();
-  }
   s_n_llhttp__internal__n_invoke_load_http_minor_1: {
     switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       case 1:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       default:
-        goto s_n_llhttp__internal__n_error_32;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_33: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
-    /* UNREACHABLE */;
-    abort();
-  }
   s_n_llhttp__internal__n_invoke_load_http_minor_2: {
     switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       default:
-        goto s_n_llhttp__internal__n_error_33;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_27: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
-    /* UNREACHABLE */;
-    abort();
-  }
   s_n_llhttp__internal__n_invoke_load_http_major: {
     switch (llhttp__internal__c_load_http_major(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_load_http_minor;
       case 1:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_1;
       case 2:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_2;
       default:
-        goto s_n_llhttp__internal__n_error_27;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_6: {
-    switch (llhttp__internal__c_test_lenient_flags_6(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_10: {
+    switch (llhttp__internal__c_test_lenient_flags_10(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_1;
       default:
         goto s_n_llhttp__internal__n_invoke_load_http_major;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_http_minor: {
     switch (llhttp__internal__c_store_http_minor(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_6;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_10;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_34: {
-    state->error = 0x9;
-    state->reason = "Invalid minor version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_51;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_51;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_35: {
-    state->error = 0x9;
-    state->reason = "Expected dot";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_3: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_52;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_52;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_http_major: {
     switch (llhttp__internal__c_store_http_major(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_req_http_dot;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_36: {
-    state->error = 0x9;
-    state->reason = "Invalid major version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_4: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_53;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_53;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_26: {
+  s_n_llhttp__internal__n_error_45: {
     state->error = 0x8;
     state->reason = "Invalid method for HTTP/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_method: {
     switch (llhttp__internal__c_load_method(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 1:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 2:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 3:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 4:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 5:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 6:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 7:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 8:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 9:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 10:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 11:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 12:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 13:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 14:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 15:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 16:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 17:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 18:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 19:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 20:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 21:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 22:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 23:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 24:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 25:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 26:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 27:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 28:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 29:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 30:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 31:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 32:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 33:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 34:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       default:
-        goto s_n_llhttp__internal__n_error_26;
+        goto s_n_llhttp__internal__n_error_45;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_39: {
+  s_n_llhttp__internal__n_error_56: {
     state->error = 0x8;
     state->reason = "Expected HTTP/";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_37: {
+  s_n_llhttp__internal__n_error_54: {
     state->error = 0x8;
     state->reason = "Expected SOURCE method for ICE/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_method_2: {
     switch (llhttp__internal__c_load_method(state, p, endp)) {
       case 33:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       default:
-        goto s_n_llhttp__internal__n_error_37;
+        goto s_n_llhttp__internal__n_error_54;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_38: {
+  s_n_llhttp__internal__n_error_55: {
     state->error = 0x8;
     state->reason = "Invalid method for RTSP/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_method_3: {
     switch (llhttp__internal__c_load_method(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 3:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 6:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 35:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 36:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 37:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 38:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 39:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 40:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 41:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 42:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 43:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 44:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       case 45:
-        goto s_n_llhttp__internal__n_req_http_major;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_version;
       default:
-        goto s_n_llhttp__internal__n_error_38;
+        goto s_n_llhttp__internal__n_error_55;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_pause_18: {
+    state->error = 0x15;
+    state->reason = "on_url_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_req_http_start;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_44: {
+    state->error = 0x1a;
+    state->reason = "`on_url_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_llhttp__on_url_complete_1: {
     switch (llhttp__on_url_complete(state, p, endp)) {
-      default:
+      case 0:
         goto s_n_llhttp__internal__n_req_http_start;
+      case 21:
+        goto s_n_llhttp__internal__n_pause_18;
+      default:
+        goto s_n_llhttp__internal__n_error_44;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_url_5: {
     const unsigned char* start;
     int err;
@@ -15243,15 +17831,15 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_40: {
+  s_n_llhttp__internal__n_error_57: {
     state->error = 0x7;
     state->reason = "Invalid char in url fragment start";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -15303,24 +17891,24 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_41: {
+  s_n_llhttp__internal__n_error_58: {
     state->error = 0x7;
     state->reason = "Invalid char in url query";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_42: {
+  s_n_llhttp__internal__n_error_59: {
     state->error = 0x7;
     state->reason = "Invalid char in url path";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -15423,60 +18011,60 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_43: {
+  s_n_llhttp__internal__n_error_60: {
     state->error = 0x7;
     state->reason = "Double @ in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_44: {
+  s_n_llhttp__internal__n_error_61: {
     state->error = 0x7;
     state->reason = "Unexpected char in url server";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_45: {
+  s_n_llhttp__internal__n_error_62: {
     state->error = 0x7;
     state->reason = "Unexpected char in url server";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_47: {
+  s_n_llhttp__internal__n_error_64: {
     state->error = 0x7;
     state->reason = "Unexpected char in url schema";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_48: {
+  s_n_llhttp__internal__n_error_65: {
     state->error = 0x7;
     state->reason = "Unexpected char in url schema";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_49: {
+  s_n_llhttp__internal__n_error_66: {
     state->error = 0x7;
     state->reason = "Unexpected start char in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -15487,56 +18075,117 @@
         goto s_n_llhttp__internal__n_span_start_llhttp__on_url_1;
       default:
         goto s_n_llhttp__internal__n_span_start_llhttp__on_url;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_50: {
+  s_n_llhttp__internal__n_error_67: {
     state->error = 0x6;
     state->reason = "Expected space after method";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_pause_22: {
+    state->error = 0x15;
+    state->reason = "on_method_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_req_first_space_before_url;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_83: {
+    state->error = 0x20;
+    state->reason = "`on_method_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_method_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_method(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_method_complete_1;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_store_method_1: {
     switch (llhttp__internal__c_store_method(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_req_first_space_before_url;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_method_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_62: {
+  s_n_llhttp__internal__n_error_84: {
     state->error = 0x6;
     state->reason = "Invalid method encountered";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_53: {
+  s_n_llhttp__internal__n_error_76: {
     state->error = 0xd;
-    state->reason = "Response overflow";
+    state->reason = "Invalid status code";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_mul_add_status_code: {
-    switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
-      case 1:
-        goto s_n_llhttp__internal__n_error_53;
-      default:
-        goto s_n_llhttp__internal__n_res_status_code;
-    }
+  s_n_llhttp__internal__n_error_74: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_72: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_pause_20: {
+    state->error = 0x15;
+    state->reason = "on_status_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_headers_start;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_70: {
+    state->error = 0x1b;
+    state->reason = "`on_status_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_status: {
     const unsigned char* start;
     int err;
     
@@ -15568,226 +18217,367 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_res_line_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_54: {
+  s_n_llhttp__internal__n_error_71: {
     state->error = 0xd;
     state->reason = "Invalid response status";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_status_code: {
-    switch (llhttp__internal__c_update_status_code(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_mul_add_status_code_2: {
+    switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
+      case 1:
+        goto s_n_llhttp__internal__n_error_72;
       default:
-        goto s_n_llhttp__internal__n_res_status_code;
+        goto s_n_llhttp__internal__n_res_status_code_otherwise;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_55: {
-    state->error = 0x9;
-    state->reason = "Expected space after version";
+  s_n_llhttp__internal__n_error_73: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_52: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
+  s_n_llhttp__internal__n_invoke_mul_add_status_code_1: {
+    switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
+      case 1:
+        goto s_n_llhttp__internal__n_error_74;
+      default:
+        goto s_n_llhttp__internal__n_res_status_code_digit_3;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_75: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_http_minor_3: {
-    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
-      case 9:
-        goto s_n_llhttp__internal__n_res_http_end;
+  s_n_llhttp__internal__n_invoke_mul_add_status_code: {
+    switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
+      case 1:
+        goto s_n_llhttp__internal__n_error_76;
       default:
-        goto s_n_llhttp__internal__n_error_52;
+        goto s_n_llhttp__internal__n_res_status_code_digit_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_56: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
+  s_n_llhttp__internal__n_error_77: {
+    state->error = 0xd;
+    state->reason = "Invalid status code";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_http_minor_4: {
-    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
-      case 0:
-        goto s_n_llhttp__internal__n_res_http_end;
-      case 1:
-        goto s_n_llhttp__internal__n_res_http_end;
+  s_n_llhttp__internal__n_invoke_update_status_code: {
+    switch (llhttp__internal__c_update_status_code(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_error_56;
+        goto s_n_llhttp__internal__n_res_status_code_digit_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_57: {
+  s_n_llhttp__internal__n_error_78: {
     state->error = 0x9;
-    state->reason = "Invalid HTTP version";
+    state->reason = "Expected space after version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_http_minor_5: {
+  s_n_llhttp__internal__n_pause_21: {
+    state->error = 0x15;
+    state->reason = "on_version_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_res_after_version;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_69: {
+    state->error = 0x21;
+    state->reason = "`on_version_complete` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_6: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_version_complete_1;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_5: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_68;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_68;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_3: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 9:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
+      default:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_5;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_4: {
     switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
       case 0:
-        goto s_n_llhttp__internal__n_res_http_end;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
+      case 1:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
       default:
-        goto s_n_llhttp__internal__n_error_57;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_5;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_51: {
-    state->error = 0x9;
-    state->reason = "Invalid HTTP version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_invoke_load_http_minor_5: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
+      default:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_5;
+    }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_http_major_1: {
     switch (llhttp__internal__c_load_http_major(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_3;
       case 1:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_4;
       case 2:
         goto s_n_llhttp__internal__n_invoke_load_http_minor_5;
       default:
-        goto s_n_llhttp__internal__n_error_51;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_5;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_7: {
-    switch (llhttp__internal__c_test_lenient_flags_6(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_11: {
+    switch (llhttp__internal__c_test_lenient_flags_10(state, p, endp)) {
       case 1:
-        goto s_n_llhttp__internal__n_res_http_end;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_version_6;
       default:
         goto s_n_llhttp__internal__n_invoke_load_http_major_1;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_http_minor_1: {
     switch (llhttp__internal__c_store_http_minor(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_7;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_11;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_58: {
-    state->error = 0x9;
-    state->reason = "Invalid minor version";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_7: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_79;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_79;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_59: {
-    state->error = 0x9;
-    state->reason = "Expected dot";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_8: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_80;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_80;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_http_major_1: {
     switch (llhttp__internal__c_store_http_major(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_res_http_dot;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_60: {
-    state->error = 0x9;
-    state->reason = "Invalid major version";
+  s_n_llhttp__internal__n_span_end_llhttp__on_version_9: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_version(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_81;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_81;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_85: {
+    state->error = 0x8;
+    state->reason = "Expected HTTP/";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_63: {
-    state->error = 0x8;
-    state->reason = "Expected HTTP/";
+  s_n_llhttp__internal__n_pause_19: {
+    state->error = 0x15;
+    state->reason = "on_method_complete pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_req_first_space_before_url;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_1: {
+    state->error = 0x20;
+    state->reason = "`on_method_complete` callback error";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_span_end_llhttp__on_method: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_method(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_llhttp__on_method_complete;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_invoke_llhttp__on_method_complete;
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_update_type: {
     switch (llhttp__internal__c_update_type(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_req_first_space_before_url;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_method;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_method: {
     switch (llhttp__internal__c_store_method(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_invoke_update_type;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_61: {
+  s_n_llhttp__internal__n_error_82: {
     state->error = 0x8;
     state->reason = "Invalid word encountered";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_type_1: {
-    switch (llhttp__internal__c_update_type_1(state, p, endp)) {
-      default:
-        goto s_n_llhttp__internal__n_res_http_major;
+  s_n_llhttp__internal__n_span_end_llhttp__on_method_1: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_method(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_update_type_1;
+      return s_error;
     }
+    goto s_n_llhttp__internal__n_invoke_update_type_1;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_update_type_2: {
     switch (llhttp__internal__c_update_type(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_start_req;
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_method_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_pause_8: {
+  s_n_llhttp__internal__n_pause_23: {
     state->error = 0x15;
     state->reason = "on_message_begin pause";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_load_type;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -15802,25 +18592,57 @@
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_message_begin: {
     switch (llhttp__on_message_begin(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_invoke_load_type;
       case 21:
-        goto s_n_llhttp__internal__n_pause_8;
+        goto s_n_llhttp__internal__n_pause_23;
       default:
         goto s_n_llhttp__internal__n_error;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_finish: {
-    switch (llhttp__internal__c_update_finish(state, p, endp)) {
+  s_n_llhttp__internal__n_pause_24: {
+    state->error = 0x15;
+    state->reason = "on_reset pause";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_invoke_update_finish;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_86: {
+    state->error = 0x1f;
+    state->reason = "`on_reset` callback error";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_llhttp__on_reset: {
+    switch (llhttp__on_reset(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_update_finish;
+      case 21:
+        goto s_n_llhttp__internal__n_pause_24;
+      default:
+        goto s_n_llhttp__internal__n_error_86;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_initial_message_completed: {
+    switch (llhttp__internal__c_load_initial_message_completed(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_llhttp__on_reset;
       default:
-        goto s_n_llhttp__internal__n_invoke_llhttp__on_message_begin;
+        goto s_n_llhttp__internal__n_invoke_update_finish;
     }
     /* UNREACHABLE */;
     abort();
   }
 }
 
 int llhttp__internal_execute(llhttp__internal_t* state, const char* p, const char* endp) {
```

