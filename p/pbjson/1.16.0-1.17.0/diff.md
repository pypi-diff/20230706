# Comparing `tmp/pbjson-1.16.0.tar.gz` & `tmp/pbjson-1.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pbjson-1.17.0.tar", last modified: Thu Jul  6 06:14:49 2023, max compression
```

## Comparing `pbjson-1.16.0.tar` & `pbjson-1.17.0.tar`

### file list

```diff
@@ -1,27 +1,40 @@
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/__init__.py
--rw-r--r--   0        0        0    50123 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/_speedups.c
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/compat.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/decoder.py
--rw-r--r--   0        0        0    10968 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/encoder.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tokens.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tool.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/__init__.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_check_circular.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_custom.py
--rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_decode.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_default.py
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_encode.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_float.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_for_json.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_item_sort_key.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_mapping.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_pass1.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_pass2.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_speedups.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_tuple.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_unicode.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pbjson-1.16.0/.gitignore
--rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 pbjson-1.16.0/LICENSE
--rw-r--r--   0        0        0     7060 2020-02-02 00:00:00.000000 pbjson-1.16.0/README.md
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 pbjson-1.16.0/pyproject.toml
--rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 pbjson-1.16.0/PKG-INFO
+drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:14:49.733837 pbjson-1.17.0/
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      282 2023-07-05 18:34:23.000000 pbjson-1.17.0/CHANGES.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7280 2023-07-06 05:39:50.000000 pbjson-1.17.0/DESCRIPTION.rst
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10373 2023-07-04 20:51:52.000000 pbjson-1.17.0/LICENSE
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       61 2023-07-04 20:51:52.000000 pbjson-1.17.0/MANIFEST.in
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     8775 2023-07-06 06:14:49.733909 pbjson-1.17.0/PKG-INFO
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7092 2023-07-06 05:34:52.000000 pbjson-1.17.0/README.md
+drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:14:49.721456 pbjson-1.17.0/pbjson/
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7780 2023-07-06 05:31:22.000000 pbjson-1.17.0/pbjson/__init__.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3815 2023-07-06 06:09:49.000000 pbjson-1.17.0/pbjson/__main__.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    50064 2023-07-06 05:53:53.000000 pbjson-1.17.0/pbjson/_speedups.c
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      893 2023-07-04 21:26:22.000000 pbjson-1.17.0/pbjson/compat.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     4738 2023-07-06 05:03:08.000000 pbjson-1.17.0/pbjson/decoder.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10968 2023-07-06 05:03:08.000000 pbjson-1.17.0/pbjson/encoder.py
+drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:14:49.733698 pbjson-1.17.0/pbjson/tests/
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     2709 2023-07-06 05:49:10.000000 pbjson-1.17.0/pbjson/tests/__init__.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      594 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_check_circular.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1015 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_custom.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10841 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_decode.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      259 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_default.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10067 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_encode.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1434 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_float.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3054 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_for_json.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1217 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_item_sort_key.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3723 2023-07-04 20:57:40.000000 pbjson-1.17.0/pbjson/tests/test_mapping.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1804 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_pass1.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      420 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_pass2.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      453 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_speedups.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      846 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_tuple.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1314 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_unicode.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      774 2023-07-04 21:18:30.000000 pbjson-1.17.0/pbjson/tokens.py
+drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:14:49.730889 pbjson-1.17.0/pbjson.egg-info/
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     8775 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/PKG-INFO
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      820 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/SOURCES.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        1 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/dependency_links.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       48 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/entry_points.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        1 2023-07-04 20:58:41.000000 pbjson-1.17.0/pbjson.egg-info/not-zip-safe
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        7 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/top_level.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       79 2023-07-06 06:14:49.734584 pbjson-1.17.0/setup.cfg
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     4495 2023-07-06 05:53:00.000000 pbjson-1.17.0/setup.py
```

### Comparing `pbjson-1.16.0/pbjson/__init__.py` & `pbjson-1.17.0/pbjson/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     {
         "json": "obj"
     }
     $ echo '{ 1.2:3.4}' | python -m simplejson.tool
     Expecting property name: line 1 column 3 (char 2)
 """
 from __future__ import absolute_import
-__version__ = '1.16.0'
+__version__ = '1.17.0'
 __all__ = [
     'dump', 'dumps', 'load', 'loads',
     'PBJSONDecodeError',
 ]
 
 __author__ = 'Scott Maxwell <scott@codecobblers.com>'
```

### Comparing `pbjson-1.16.0/pbjson/_speedups.c` & `pbjson-1.17.0/pbjson/_speedups.c`

 * *Files 0% similar despite different names*

```diff
@@ -1456,15 +1456,14 @@
     /* Encode Python dict dct a JSON term */
     PyObject *kstr = NULL;
     PyObject *ident = NULL;
     PyObject *iter = NULL;
     PyObject *item = NULL;
     PyObject *items = NULL;
     PyObject *encoded = NULL;
-    Py_ssize_t idx;
 
     int len = PyMapping_Size(dct);
     if (encode_type_and_length(encoder, Enc_DICT, len)) {
         return -1;
     }
 
     if (len) {
@@ -1472,15 +1471,14 @@
             goto bail;
         }
         
         iter = encode_dict_items(encoder, dct);
         if (iter == NULL)
             goto bail;
         
-        idx = 0;
         while ((item = PyIter_Next(iter))) {
             PyObject *encoded, *key, *value;
             if (!PyTuple_Check(item) || Py_SIZE(item) != 2) {
                 PyErr_SetString(PyExc_ValueError, "items must return 2-tuples");
                 goto bail;
             }
             key = PyTuple_GET_ITEM(item, 0);
@@ -1499,15 +1497,14 @@
                 }
             } else if (encode_key(encoder, key)) {
                 goto bail;
             }
             if (encode_one(encoder, value))
                 goto bail;
             Py_CLEAR(item);
-            idx += 1;
         }
         Py_CLEAR(iter);
         if (PyErr_Occurred())
             goto bail;
         if (ident != NULL) {
             if (PyDict_DelItem(encoder->markers, ident))
                 goto bail;
```

### Comparing `pbjson-1.16.0/pbjson/compat.py` & `pbjson-1.17.0/pbjson/compat.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/decoder.py` & `pbjson-1.17.0/pbjson/decoder.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/encoder.py` & `pbjson-1.17.0/pbjson/encoder.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tokens.py` & `pbjson-1.17.0/pbjson/tokens.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tool.py` & `pbjson-1.17.0/pbjson/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     parser = argparse.ArgumentParser(
         description='Convert between pbjson and json',
         epilog='If converting a PBJSON file with binary elements, you may need to use `--repr` since JSON cannot handle binary data.')
     parser.add_argument('-r', '--repr', action='store_true', help='instead of converting to JSON, just output the `repr` of the object')
     parser.add_argument('-p', '--pretty', action='store_true', help='make it nice for humans')
     if yaml is not None:
         parser.add_argument('-y', '--yaml', action='store_true', help='input or output is YAML instead of JSON')
-    parser.add_argument('infile', nargs='?', type=argparse.FileType('rb'), default=sys.stdin, help='filename to convert from or to pbjson (default: stdin)')
+    parser.add_argument('infile', type=argparse.FileType('rb'), help='filename to convert from or to pbjson')
     parser.add_argument('outfile', nargs='?', type=argparse.FileType('wb'), default=sys.stdout, help='filename to write the converted file to (default: stdout)')
     args = parser.parse_args()
 
     contents = args.infile.read()
     try:
         text = contents.decode()
     except Exception:
```

### Comparing `pbjson-1.16.0/pbjson/tests/__init__.py` & `pbjson-1.17.0/pbjson/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
             return result
 
         if not pbjson._has_encoder_speedups() and not pbjson._has_decoder_speedups():
             print("Testing with missing speedups")
             TestMissingSpeedups().run(result)
         else:
             pbjson._toggle_speedups(False)
+            print("Testing without speedups")
             run(self, result)
             pbjson._toggle_speedups(True)
         return result
 
 
 class TestMissingSpeedups(unittest.TestCase):
     def runTest(self):
```

### Comparing `pbjson-1.16.0/pbjson/tests/test_check_circular.py` & `pbjson-1.17.0/pbjson/tests/test_check_circular.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_custom.py` & `pbjson-1.17.0/pbjson/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_decode.py` & `pbjson-1.17.0/pbjson/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_encode.py` & `pbjson-1.17.0/pbjson/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_float.py` & `pbjson-1.17.0/pbjson/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_for_json.py` & `pbjson-1.17.0/pbjson/tests/test_for_json.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_item_sort_key.py` & `pbjson-1.17.0/pbjson/tests/test_item_sort_key.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_mapping.py` & `pbjson-1.17.0/pbjson/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_pass1.py` & `pbjson-1.17.0/pbjson/tests/test_pass1.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_tuple.py` & `pbjson-1.17.0/pbjson/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/pbjson/tests/test_unicode.py` & `pbjson-1.17.0/pbjson/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/LICENSE` & `pbjson-1.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbjson-1.16.0/README.md` & `pbjson-1.17.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pbjson
 ======
 
 Packed Binary JSON extension for Python
 
-`pbjson` is a packed binary JSON encoder and decoder for Python 2.5+ and Python 3.3+. It is pure Python code with no dependencies, but includes an optional C extension for a serious speed boost.
+`pbjson` is a packed binary JSON encoder and decoder for Python 2.6+ and Python 3.3+. It is pure Python code with no dependencies, but includes an optional C extension for a serious speed boost.
 
 `pbjson` can be used standalone or as an extension to the standard `json` module or to `simplejson`, from which code was heavily borrowed. The latest documentation for `simplejson` can be read online here:
 <http://simplejson.readthedocs.org/>
 
 The encoder can be specialized to provide serialization in any kind of situation, without any special support by the objects to be serialized (somewhat like pickle). This is best done with the `default` kwarg to dumps.
 
 The decoder can handle incoming JSON strings of any specified encoding (UTF-8 by default). It can also be specialized to post-process JSON objects with the `object_hook` or `object_pairs_hook` kwargs. This
@@ -66,15 +66,15 @@
         "width": 4.5
     }
 }
 ```
 
     E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
     08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
-    0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
+    0A 'dimensions' E2 09 'thickness' 61 d7 05 'width' 62 4d5d
 
 Let's break that out:
 
 - 00: E5 - dict with 5 elements
 - 01: 05 - key with 5 characters
 - 02-06: toast
 - 07: 01 - true
@@ -95,22 +95,22 @@
 - 32: 86 - string with 6 characters
 - 33-38: butter
 - 39: 0A - key with 10 bytes
 - 3A-43: dimensions
 - 44: E3 - dict with 2 elements
 - 45: 09 - key with 9 characters
 - 46-4E: thickness
-- 4F: 68 - float with 8 bytes
-- 50-57: IEEE representation of .7
-- 58: 05 - key with 5 characters
-- 59-5D: width
-- 5E: 62 - float with 2 bytes
-- 5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes were all zeros.
+- 4F: 61 - float with 1 bytes
+- 50: first byte of IEEE representation of .7. Remaining 7 bytes were all zeros.
+- 51: 05 - key with 5 characters
+- 52-56: width
+- 57: 62 - float with 2 bytes
+- 58-59: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes were all zeros.
 
-Total 97 bytes. The tightest `JSON` representation requires 126 bytes. Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
+Total 90 bytes. The tightest `JSON` representation requires 126 bytes. Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
 
 Now here is an example with repeating data:
 
 ```javascript
 {
     "region": 3,
     "countries": [
```

### Comparing `pbjson-1.16.0/PKG-INFO` & `pbjson-1.17.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pbjson
-Version: 1.16.0
+Version: 1.17.0
 Summary: Packed Binary JSON encoder/decoder for Python
-Project-URL: Homepage, https://github.com/scottkmaxwell/pbjson
-Project-URL: Bug Tracker, https://github.com/scottkmaxwell/pbjson/issues
-Author-email: Scott Maxwell <scott@codecobblers.com>
-License-File: LICENSE
+Home-page: https://github.com/scottkmaxwell/pbjson
+Author: Scott Maxwell
+Author-email: scott@codecobblers.com
+License: MIT License
+Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -24,174 +24,228 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
+Classifier: Operating System :: OS Independent
+Requires-Python: >=2.5, !=3.0.*, !=3.1.*, !=3.2.*
+License-File: LICENSE
 
 pbjson
 ======
 
 Packed Binary JSON extension for Python
 
-`pbjson` is a packed binary JSON encoder and decoder for Python 2.5+ and Python 3.3+. It is pure Python code with no dependencies, but includes an optional C extension for a serious speed boost.
-
-`pbjson` can be used standalone or as an extension to the standard `json` module or to `simplejson`, from which code was heavily borrowed. The latest documentation for `simplejson` can be read online here:
-<http://simplejson.readthedocs.org/>
-
-The encoder can be specialized to provide serialization in any kind of situation, without any special support by the objects to be serialized (somewhat like pickle). This is best done with the `default` kwarg to dumps.
-
-The decoder can handle incoming JSON strings of any specified encoding (UTF-8 by default). It can also be specialized to post-process JSON objects with the `object_hook` or `object_pairs_hook` kwargs. This
-is particularly useful for implementing protocols that have a richer type system than JSON itself.
-
-What is Packed Binary JSON (`PBJSON`)
------------------------------------
-
-Packed Binary JSON is not the same as `BSON`. `BSON` is a format used primarily in MongoDB and is meant for efficient parsing. `PBJSON` is meant for efficient conversion from a dict or list, transmission and conversion back to a dict or list on the other end. `BSON` has explicit support for several types not available in standard JSON. PBJSON supports only those types supported by normal JSON, plus binary data blobs and set collections.
-
-Unlike `BSON`, `PBJSON` is almost always smaller than the equivalent JSON. Like `BSON`, `PBJSON` can be very quickly encoded and decoded since all elements are length encoded.
-
-There are two types of tokens in `PBJSON`: data and key. Data tokens can be zero length fundamental types (`false`, `true`, `null`), variable length fundamental types (`int`, `float`, `string`, `binary`) or containers (`set`, `array`, `dict`).
-
-The type for the data token is generally stored in the top 3 bits (bits 5-7). Type zero is a special type to represent the zero length fundamental types. The lower bits indicate the actual value. These are:
+``pbjson`` is a packed binary JSON encoder and decoder for Python 2.5+
+and Python 3.3+. It is pure Python code with no dependencies, but
+includes an optional C extension for a serious speed boost.
+
+``pbjson`` can be used standalone or as an extension to the standard
+``json`` module or to ``simplejson``, from which code was heavily
+borrowed. The latest documentation for ``simplejson`` can be read online
+here: http://simplejson.readthedocs.org/
+
+The encoder can be specialized to provide serialization in any kind of
+situation, without any special support by the objects to be serialized
+(somewhat like pickle). This is best done with the ``default`` kwarg to
+dumps.
+
+The decoder can handle incoming JSON strings of any specified encoding
+(UTF-8 by default). It can also be specialized to post-process JSON
+objects with the ``object_hook`` or ``object_pairs_hook`` kwargs. This
+is particularly useful for implementing protocols that have a richer
+type system than JSON itself.
+
+What is Packed Binary JSON (``PBJSON``)
+---------------------------------------
+
+Packed Binary JSON is not the same as ``BSON``. ``BSON`` is a format
+used primarily in MongoDB and is meant for efficient parsing. ``PBJSON``
+is meant for efficient conversion from a dict or list, transmission and
+conversion back to a dict or list on the other end. ``BSON`` has
+explicit support for several types not available in standard JSON.
+PBJSON supports only those types supported by normal JSON, plus binary
+data blobs and set collections.
+
+Unlike ``BSON``, ``PBJSON`` is almost always smaller than the equivalent
+JSON. Like ``BSON``, ``PBJSON`` can be very quickly encoded and decoded
+since all elements are length encoded.
+
+There are two types of tokens in ``PBJSON``: data and key. Data tokens
+can be zero length fundamental types (``false``, ``true``, ``null``),
+variable length fundamental types (``int``, ``float``, ``string``,
+``binary``) or containers (``set``, ``array``, ``dict``).
+
+The type for the data token is generally stored in the top 3 bits (bits
+5-7). Type zero is a special type to represent the zero length
+fundamental types. The lower bits indicate the actual value. These are:
 
 Zero-length Data Types:
 
-- 00 - false
-- 01 - true
-- 02 - null
-
-All other types are variable length. If the length is between 0 and 15, that length is stored in bits 0-3. For lengths in the 16-2047 range, bit 4 is set and bits 0-2 are combined with the next byte to make an 11-bit length. If bits 4 and 3 are both set, then the value in bits 0-2 are combined with the next 2 bytes to create a 19-bit length. However, if bits 4-0 are all set, this indicates that the following 4 bytes are simply used as a size. So the token plus length is, one byte (length of 0-15), two bytes (16-2047), three bytes (2048-458751) or five bytes (458876-4294967295).
+-  00 - false
+-  01 - true
+-  02 - null
+
+All other types are variable length. If the length is between 0 and 15,
+that length is stored in bits 0-3. For lengths in the 16-2047 range, bit
+4 is set and bits 0-2 are combined with the next byte to make an 11-bit
+length. If bits 4 and 3 are both set, then the value in bits 0-2 are
+combined with the next 2 bytes to create a 19-bit length. However, if
+bits 4-0 are all set, this indicates that the following 4 bytes are
+simply used as a size. So the token plus length is, one byte (length of
+0-15), two bytes (16-2047), three bytes (2048-458751) or five bytes
+(458876-4294967295).
 
 Variable-length Data types:
 
-- 2x - int (bytes stored big endian with leading zero bytes removed)
-- 4x - negative int (bytes stored big endian as a positive number with leading zero bytes removed)
-- 6x - float (stored as big endian double precision with trailing zero bytes removed)
-- 8x - string
-- Ax - binary
+-  2x - int (bytes stored big endian with leading zero bytes removed)
+-  4x - negative int (bytes stored big endian as a positive number with
+   leading zero bytes removed)
+-  6x - float (stored as big endian double precision with trailing zero
+   bytes removed)
+-  8x - string
+-  Ax - binary
 
 Collection types: (length is number of elements)
 
-- Cx - array
-- Ex - object
-- 0C - terminated array
-- 0F - terminator
-
-The final entry, the "terminated array" works a bit differently. This is for use when the length is not known when writing begins. Instead, a terminator (0F) is written to the stream when the last element of the array has been written.
-
-Object keys must be text and are a maximum of 127 bytes in length. They are stored as a (7-bit length, followed by the actual key. The first 128 keys are remembered by index. If the same key is used again, it can be represented as a single byte consisting of the high bit and the index number of the key.
-
-In other words, if the recurring key is "toast", it should be encoded as 05 toast. The next time the key "toast" is needed, it can be encoded as simply 80, since it was the first key.
+-  Cx - array
+-  Ex - object
+-  0C - terminated array
+-  0F - terminator
+
+The final entry, the "terminated array" works a bit differently. This is
+for use when the length is not known when writing begins. Instead, a
+terminator (0F) is written to the stream when the last element of the
+array has been written.
+
+Object keys must be text and are a maximum of 127 bytes in length. They
+are stored as a (7-bit length, followed by the actual key. The first 128
+keys are remembered by index. If the same key is used again, it can be
+represented as a single byte consisting of the high bit and the index
+number of the key.
+
+In other words, if the recurring key is "toast", it should be encoded as
+05 toast. The next time the key "toast" is needed, it can be encoded as
+simply 80, since it was the first key.
 
 Here is an example of a simple structure:
 
-```javascript
-{
-    "toast": true,
-    "burned": false,
-    "name": "the best",
-    "toppings": ["jelly","jam","butter"],
-    "dimensions": {
-        "thickness": 0.7,
-        "width": 4.5
-    }
-}
-```
-
-    E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
-    08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
-    0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
+.. code:: javascript
+
+   {
+       "toast": true,
+       "burned": false,
+       "name": "the best",
+       "toppings": ["jelly","jam","butter"],
+       "dimensions": {
+           "thickness": 0.7,
+           "width": 4.5
+       }
+   }
+
+::
+
+   E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
+   08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
+   0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
 
 Let's break that out:
 
-- 00: E5 - dict with 5 elements
-- 01: 05 - key with 5 characters
-- 02-06: toast
-- 07: 01 - true
-- 08: 06 - key with 6 characters
-- 09-0E: burned
-- 0F: 00 - false
-- 10: 04 - key with 4 characters
-- 11-14: name
-- 15: 88 - string with 8 characters
-- 16-1D: the best
-- 1E: 08 - key with 8 bytes
-- 1F-26: toppings
-- 27: C3 - array with 3 elements
-- 28: 85 - string with 5 characters
-- 29-2D: jelly
-- 2E: 83 - string with 3 characters
-- 2F-31: jam
-- 32: 86 - string with 6 characters
-- 33-38: butter
-- 39: 0A - key with 10 bytes
-- 3A-43: dimensions
-- 44: E3 - dict with 2 elements
-- 45: 09 - key with 9 characters
-- 46-4E: thickness
-- 4F: 68 - float with 8 bytes
-- 50-57: IEEE representation of .7
-- 58: 05 - key with 5 characters
-- 59-5D: width
-- 5E: 62 - float with 2 bytes
-- 5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes were all zeros.
+-  00: E5 - dict with 5 elements
+-  01: 05 - key with 5 characters
+-  02-06: toast
+-  07: 01 - true
+-  08: 06 - key with 6 characters
+-  09-0E: burned
+-  0F: 00 - false
+-  10: 04 - key with 4 characters
+-  11-14: name
+-  15: 88 - string with 8 characters
+-  16-1D: the best
+-  1E: 08 - key with 8 bytes
+-  1F-26: toppings
+-  27: C3 - array with 3 elements
+-  28: 85 - string with 5 characters
+-  29-2D: jelly
+-  2E: 83 - string with 3 characters
+-  2F-31: jam
+-  32: 86 - string with 6 characters
+-  33-38: butter
+-  39: 0A - key with 10 bytes
+-  3A-43: dimensions
+-  44: E3 - dict with 2 elements
+-  45: 09 - key with 9 characters
+-  46-4E: thickness
+-  4F: 68 - float with 8 bytes
+-  50-57: IEEE representation of .7
+-  58: 05 - key with 5 characters
+-  59-5D: width
+-  5E: 62 - float with 2 bytes
+-  5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes
+   were all zeros.
 
-Total 97 bytes. The tightest `JSON` representation requires 126 bytes. Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
+Total 97 bytes. The tightest ``JSON`` representation requires 126 bytes.
+Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
 
 Now here is an example with repeating data:
 
-```javascript
-{
-    "region": 3,
-    "countries": [
-        {"code": "us", "name": "United States"},
-        {"code": "ca", "name": "Canada"},
-        {"code": "mx", "name": "Mexico"}
-    ]
-}
-```
-
-    E2 06 region 21 03 09 countries C3
-    E2 04 code 82 us 04 name 8D United States
-    E2 82 82 ca 83 86 Canada
-    E2 82 82 mx 83 86 Mexico
+.. code:: javascript
 
-This breaks down thus:
+   {
+       "region": 3,
+       "countries": [
+           {"code": "us", "name": "United States"},
+           {"code": "ca", "name": "Canada"},
+           {"code": "mx", "name": "Mexico"}
+       ]
+   }
+
+::
+
+   E2 06 region 21 03 09 countries C3
+   E2 04 code 82 us 04 name 8D United States
+   E2 82 82 ca 83 86 Canada
+   E2 82 82 mx 83 86 Mexico
 
-- 00: E2 - dict with 2 elements
-- 01: 06 - key with 6 characters
-- 02-07: region
-- 08: 21 - int with 1 byte
-- 09: 03 - the int for 3. Only a single byte is required.
-- 0A: 09 - key with 9 bytes
-- 0B-13: countries
-- 14: C3 - array with 3 elements
-- 15: E2 - dict with 2 elements
-- 16: 04 - key with 4 characters
-- 17-1A: code
-- 19: 82 - string with 2 characters
-- 1A-1B: us
-- 1C: 04 - key with 4 characters
-- 1E-21: name
-- 22: 8D - string with 13 characters
-- 23-2F: United States
-- 30: E2 - dict with 2 elements
-- 31: 82 - recurring key 2. Since 'code' was the 3rd key, it has an index of 2.
-- 32: 82 - string with 2 characters
-- 33-34: ca
-- 35: 83 - recurring key 3
-- 36: 86 - string with 6 characters
-- 37-3C: Canada
-- 3D: E2 - dict with 2 elements
-- 3E: 82 - recurring key 0
-- 3F: 82 - string with 2 characters
-- 40-41: mx
-- 42: 83 - recurring key 1
-- 43: 86 - string with 6 characters
-- 44-49: Mexico
-
-Total 74 bytes. The tightest `JSON` representation requires 123 bytes. Marshal takes 158 bytes and Pickle takes 162. BSON takes 154 bytes.
+This breaks down thus:
 
-`Packed Binary JSON` is available now in the `pbjson` Python module. That module includes a command line utility to convert between normal `JSON` files and `PBJSON`.
+-  00: E2 - dict with 2 elements
+-  01: 06 - key with 6 characters
+-  02-07: region
+-  08: 21 - int with 1 byte
+-  09: 03 - the int for 3. Only a single byte is required.
+-  0A: 09 - key with 9 bytes
+-  0B-13: countries
+-  14: C3 - array with 3 elements
+-  15: E2 - dict with 2 elements
+-  16: 04 - key with 4 characters
+-  17-1A: code
+-  19: 82 - string with 2 characters
+-  1A-1B: us
+-  1C: 04 - key with 4 characters
+-  1E-21: name
+-  22: 8D - string with 13 characters
+-  23-2F: United States
+-  30: E2 - dict with 2 elements
+-  31: 82 - recurring key 2. Since 'code' was the 3rd key, it has an
+   index of 2.
+-  32: 82 - string with 2 characters
+-  33-34: ca
+-  35: 83 - recurring key 3
+-  36: 86 - string with 6 characters
+-  37-3C: Canada
+-  3D: E2 - dict with 2 elements
+-  3E: 82 - recurring key 0
+-  3F: 82 - string with 2 characters
+-  40-41: mx
+-  42: 83 - recurring key 1
+-  43: 86 - string with 6 characters
+-  44-49: Mexico
+
+Total 74 bytes. The tightest ``JSON`` representation requires 123 bytes.
+Marshal takes 158 bytes and Pickle takes 162. BSON takes 154 bytes.
+
+``Packed Binary JSON`` is available now in the ``pbjson`` Python module.
+That module includes a command line utility to convert between normal
+``JSON`` files and ``PBJSON``.
```

