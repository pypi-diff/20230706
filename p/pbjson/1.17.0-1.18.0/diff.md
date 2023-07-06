# Comparing `tmp/pbjson-1.17.0.tar.gz` & `tmp/pbjson-1.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbjson-1.17.0.tar", last modified: Thu Jul  6 06:14:49 2023, max compression
+gzip compressed data, was "pbjson-1.18.0.tar", last modified: Thu Jul  6 06:29:02 2023, max compression
```

## Comparing `pbjson-1.17.0.tar` & `pbjson-1.18.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:14:49.733837 pbjson-1.17.0/
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      282 2023-07-05 18:34:23.000000 pbjson-1.17.0/CHANGES.txt
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7280 2023-07-06 05:39:50.000000 pbjson-1.17.0/DESCRIPTION.rst
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10373 2023-07-04 20:51:52.000000 pbjson-1.17.0/LICENSE
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       61 2023-07-04 20:51:52.000000 pbjson-1.17.0/MANIFEST.in
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     8775 2023-07-06 06:14:49.733909 pbjson-1.17.0/PKG-INFO
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7092 2023-07-06 05:34:52.000000 pbjson-1.17.0/README.md
-drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:14:49.721456 pbjson-1.17.0/pbjson/
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7780 2023-07-06 05:31:22.000000 pbjson-1.17.0/pbjson/__init__.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3815 2023-07-06 06:09:49.000000 pbjson-1.17.0/pbjson/__main__.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    50064 2023-07-06 05:53:53.000000 pbjson-1.17.0/pbjson/_speedups.c
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      893 2023-07-04 21:26:22.000000 pbjson-1.17.0/pbjson/compat.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     4738 2023-07-06 05:03:08.000000 pbjson-1.17.0/pbjson/decoder.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10968 2023-07-06 05:03:08.000000 pbjson-1.17.0/pbjson/encoder.py
-drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:14:49.733698 pbjson-1.17.0/pbjson/tests/
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     2709 2023-07-06 05:49:10.000000 pbjson-1.17.0/pbjson/tests/__init__.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      594 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_check_circular.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1015 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_custom.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10841 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_decode.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      259 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_default.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10067 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_encode.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1434 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_float.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3054 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_for_json.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1217 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_item_sort_key.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3723 2023-07-04 20:57:40.000000 pbjson-1.17.0/pbjson/tests/test_mapping.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1804 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_pass1.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      420 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_pass2.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      453 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_speedups.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      846 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_tuple.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1314 2023-07-04 20:51:52.000000 pbjson-1.17.0/pbjson/tests/test_unicode.py
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      774 2023-07-04 21:18:30.000000 pbjson-1.17.0/pbjson/tokens.py
-drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:14:49.730889 pbjson-1.17.0/pbjson.egg-info/
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     8775 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/PKG-INFO
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      820 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/SOURCES.txt
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        1 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/dependency_links.txt
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       48 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/entry_points.txt
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        1 2023-07-04 20:58:41.000000 pbjson-1.17.0/pbjson.egg-info/not-zip-safe
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        7 2023-07-06 06:14:49.000000 pbjson-1.17.0/pbjson.egg-info/top_level.txt
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       79 2023-07-06 06:14:49.734584 pbjson-1.17.0/setup.cfg
--rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     4495 2023-07-06 05:53:00.000000 pbjson-1.17.0/setup.py
+drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:29:02.445421 pbjson-1.18.0/
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      282 2023-07-05 18:34:23.000000 pbjson-1.18.0/CHANGES.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7671 2023-07-06 06:27:59.000000 pbjson-1.18.0/DESCRIPTION.rst
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10373 2023-07-04 20:51:52.000000 pbjson-1.18.0/LICENSE
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       61 2023-07-04 20:51:52.000000 pbjson-1.18.0/MANIFEST.in
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     9166 2023-07-06 06:29:02.445490 pbjson-1.18.0/PKG-INFO
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7433 2023-07-06 06:26:39.000000 pbjson-1.18.0/README.md
+drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:29:02.441517 pbjson-1.18.0/pbjson/
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     7780 2023-07-06 06:24:01.000000 pbjson-1.18.0/pbjson/__init__.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3815 2023-07-06 06:09:49.000000 pbjson-1.18.0/pbjson/__main__.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    50064 2023-07-06 05:53:53.000000 pbjson-1.18.0/pbjson/_speedups.c
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      893 2023-07-04 21:26:22.000000 pbjson-1.18.0/pbjson/compat.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     4738 2023-07-06 05:03:08.000000 pbjson-1.18.0/pbjson/decoder.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10968 2023-07-06 05:03:08.000000 pbjson-1.18.0/pbjson/encoder.py
+drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:29:02.445270 pbjson-1.18.0/pbjson/tests/
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     2709 2023-07-06 05:49:10.000000 pbjson-1.18.0/pbjson/tests/__init__.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      594 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_check_circular.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1015 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_custom.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10841 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_decode.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      259 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_default.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)    10067 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_encode.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1434 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_float.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3054 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_for_json.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1217 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_item_sort_key.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     3723 2023-07-04 20:57:40.000000 pbjson-1.18.0/pbjson/tests/test_mapping.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1804 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_pass1.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      420 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_pass2.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      453 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_speedups.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      846 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_tuple.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     1314 2023-07-04 20:51:52.000000 pbjson-1.18.0/pbjson/tests/test_unicode.py
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      774 2023-07-04 21:18:30.000000 pbjson-1.18.0/pbjson/tokens.py
+drwxr-xr-x   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        0 2023-07-06 06:29:02.442604 pbjson-1.18.0/pbjson.egg-info/
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     9166 2023-07-06 06:29:02.000000 pbjson-1.18.0/pbjson.egg-info/PKG-INFO
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)      820 2023-07-06 06:29:02.000000 pbjson-1.18.0/pbjson.egg-info/SOURCES.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        1 2023-07-06 06:29:02.000000 pbjson-1.18.0/pbjson.egg-info/dependency_links.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       48 2023-07-06 06:29:02.000000 pbjson-1.18.0/pbjson.egg-info/entry_points.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        1 2023-07-04 20:58:41.000000 pbjson-1.18.0/pbjson.egg-info/not-zip-safe
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)        7 2023-07-06 06:29:02.000000 pbjson-1.18.0/pbjson.egg-info/top_level.txt
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)       79 2023-07-06 06:29:02.445715 pbjson-1.18.0/setup.cfg
+-rw-r--r--   0 smaxwell (1726680969) ZOOXLABS\Domain Users (1950283502)     4495 2023-07-06 05:53:00.000000 pbjson-1.18.0/setup.py
```

### Comparing `pbjson-1.17.0/DESCRIPTION.rst` & `pbjson-1.18.0/DESCRIPTION.rst`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,27 @@
 
 The decoder can handle incoming JSON strings of any specified encoding
 (UTF-8 by default). It can also be specialized to post-process JSON
 objects with the ``object_hook`` or ``object_pairs_hook`` kwargs. This
 is particularly useful for implementing protocols that have a richer
 type system than JSON itself.
 
+Using the API
+-------------
+
+The ``pbjson`` module works ust like the ``json`` module. You can ``pbjson.load``,
+``pbjson.loads``, ``pbjson.dump``, and ``pbjson.dumps``.
+
+Command-Line Tool
+-----------------
+
+After you have installed ``pbjson``, you can use the ``pbjson`` command-line tool to
+convert files to or from ``pbjson``. Run ``pbjson -h`` for details.
+
+
 What is Packed Binary JSON (``PBJSON``)
 ---------------------------------------
 
 Packed Binary JSON is not the same as ``BSON``. ``BSON`` is a format
 used primarily in MongoDB and is meant for efficient parsing. ``PBJSON``
 is meant for efficient conversion from a dict or list, transmission and
 conversion back to a dict or list on the other end. ``BSON`` has
@@ -110,15 +123,15 @@
        }
    }
 
 ::
 
    E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
    08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
-   0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
+   0A 'dimensions' E2 09 'thickness' 61 d7 05 'width' 62 4d5d
 
 Let's break that out:
 
 -  00: E5 - dict with 5 elements
 -  01: 05 - key with 5 characters
 -  02-06: toast
 -  07: 01 - true
@@ -139,23 +152,22 @@
 -  32: 86 - string with 6 characters
 -  33-38: butter
 -  39: 0A - key with 10 bytes
 -  3A-43: dimensions
 -  44: E3 - dict with 2 elements
 -  45: 09 - key with 9 characters
 -  46-4E: thickness
--  4F: 68 - float with 8 bytes
--  50-57: IEEE representation of .7
--  58: 05 - key with 5 characters
--  59-5D: width
--  5E: 62 - float with 2 bytes
--  5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes
-   were all zeros.
+-  4F: 61 - float with 1 bytes
+-  50: first byte of IEEE representation of .7. Remaining 7 bytes were all zeros.
+-  51: 05 - key with 5 characters
+-  52-56: width
+-  57: 62 - float with 2 bytes
+-  58-59: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes were all zeros.
 
-Total 97 bytes. The tightest ``JSON`` representation requires 126 bytes.
+Total 90 bytes. The tightest ``JSON`` representation requires 126 bytes.
 Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
 
 Now here is an example with repeating data:
 
 .. code:: javascript
 
    {
```

### Comparing `pbjson-1.17.0/LICENSE` & `pbjson-1.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/PKG-INFO` & `pbjson-1.18.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbjson
-Version: 1.17.0
+Version: 1.18.0
 Summary: Packed Binary JSON encoder/decoder for Python
 Home-page: https://github.com/scottkmaxwell/pbjson
 Author: Scott Maxwell
 Author-email: scott@codecobblers.com
 License: MIT License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,14 +53,27 @@
 
 The decoder can handle incoming JSON strings of any specified encoding
 (UTF-8 by default). It can also be specialized to post-process JSON
 objects with the ``object_hook`` or ``object_pairs_hook`` kwargs. This
 is particularly useful for implementing protocols that have a richer
 type system than JSON itself.
 
+Using the API
+-------------
+
+The ``pbjson`` module works ust like the ``json`` module. You can ``pbjson.load``,
+``pbjson.loads``, ``pbjson.dump``, and ``pbjson.dumps``.
+
+Command-Line Tool
+-----------------
+
+After you have installed ``pbjson``, you can use the ``pbjson`` command-line tool to
+convert files to or from ``pbjson``. Run ``pbjson -h`` for details.
+
+
 What is Packed Binary JSON (``PBJSON``)
 ---------------------------------------
 
 Packed Binary JSON is not the same as ``BSON``. ``BSON`` is a format
 used primarily in MongoDB and is meant for efficient parsing. ``PBJSON``
 is meant for efficient conversion from a dict or list, transmission and
 conversion back to a dict or list on the other end. ``BSON`` has
@@ -144,15 +157,15 @@
        }
    }
 
 ::
 
    E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
    08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
-   0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
+   0A 'dimensions' E2 09 'thickness' 61 d7 05 'width' 62 4d5d
 
 Let's break that out:
 
 -  00: E5 - dict with 5 elements
 -  01: 05 - key with 5 characters
 -  02-06: toast
 -  07: 01 - true
@@ -173,23 +186,22 @@
 -  32: 86 - string with 6 characters
 -  33-38: butter
 -  39: 0A - key with 10 bytes
 -  3A-43: dimensions
 -  44: E3 - dict with 2 elements
 -  45: 09 - key with 9 characters
 -  46-4E: thickness
--  4F: 68 - float with 8 bytes
--  50-57: IEEE representation of .7
--  58: 05 - key with 5 characters
--  59-5D: width
--  5E: 62 - float with 2 bytes
--  5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes
-   were all zeros.
+-  4F: 61 - float with 1 bytes
+-  50: first byte of IEEE representation of .7. Remaining 7 bytes were all zeros.
+-  51: 05 - key with 5 characters
+-  52-56: width
+-  57: 62 - float with 2 bytes
+-  58-59: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes were all zeros.
 
-Total 97 bytes. The tightest ``JSON`` representation requires 126 bytes.
+Total 90 bytes. The tightest ``JSON`` representation requires 126 bytes.
 Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
 
 Now here is an example with repeating data:
 
 .. code:: javascript
 
    {
```

### Comparing `pbjson-1.17.0/README.md` & `pbjson-1.18.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,25 @@
 <http://simplejson.readthedocs.org/>
 
 The encoder can be specialized to provide serialization in any kind of situation, without any special support by the objects to be serialized (somewhat like pickle). This is best done with the `default` kwarg to dumps.
 
 The decoder can handle incoming JSON strings of any specified encoding (UTF-8 by default). It can also be specialized to post-process JSON objects with the `object_hook` or `object_pairs_hook` kwargs. This
 is particularly useful for implementing protocols that have a richer type system than JSON itself.
 
+Using the API
+-------------
+
+The `pbjson` module works ust like the `json` module. You can `pbjson.load`, `pbjson.loads`, `pbjson.dump`, and `pbjson.dumps`.
+
+Command-Line Tool
+-----------------
+
+After you have installed `pbjson`, you can use the `pbjson` command-line tool to convert files to or from `pbjson`.
+Run `pbjson -h` for details.
+
 What is Packed Binary JSON (`PBJSON`)
 -----------------------------------
 
 Packed Binary JSON is not the same as `BSON`. `BSON` is a format used primarily in MongoDB and is meant for efficient parsing. `PBJSON` is meant for efficient conversion from a dict or list, transmission and conversion back to a dict or list on the other end. `BSON` has explicit support for several types not available in standard JSON. PBJSON supports only those types supported by normal JSON, plus binary data blobs and set collections.
 
 Unlike `BSON`, `PBJSON` is almost always smaller than the equivalent JSON. Like `BSON`, `PBJSON` can be very quickly encoded and decoded since all elements are length encoded.
```

### Comparing `pbjson-1.17.0/pbjson/__init__.py` & `pbjson-1.18.0/pbjson/__init__.py`

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
-__version__ = '1.17.0'
+__version__ = '1.18.0'
 __all__ = [
     'dump', 'dumps', 'load', 'loads',
     'PBJSONDecodeError',
 ]
 
 __author__ = 'Scott Maxwell <scott@codecobblers.com>'
```

### Comparing `pbjson-1.17.0/pbjson/__main__.py` & `pbjson-1.18.0/pbjson/__main__.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/_speedups.c` & `pbjson-1.18.0/pbjson/_speedups.c`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/compat.py` & `pbjson-1.18.0/pbjson/compat.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/decoder.py` & `pbjson-1.18.0/pbjson/decoder.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/encoder.py` & `pbjson-1.18.0/pbjson/encoder.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/__init__.py` & `pbjson-1.18.0/pbjson/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_check_circular.py` & `pbjson-1.18.0/pbjson/tests/test_check_circular.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_custom.py` & `pbjson-1.18.0/pbjson/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_decode.py` & `pbjson-1.18.0/pbjson/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_encode.py` & `pbjson-1.18.0/pbjson/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_float.py` & `pbjson-1.18.0/pbjson/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_for_json.py` & `pbjson-1.18.0/pbjson/tests/test_for_json.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_item_sort_key.py` & `pbjson-1.18.0/pbjson/tests/test_item_sort_key.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_mapping.py` & `pbjson-1.18.0/pbjson/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_pass1.py` & `pbjson-1.18.0/pbjson/tests/test_pass1.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_tuple.py` & `pbjson-1.18.0/pbjson/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tests/test_unicode.py` & `pbjson-1.18.0/pbjson/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson/tokens.py` & `pbjson-1.18.0/pbjson/tokens.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/pbjson.egg-info/PKG-INFO` & `pbjson-1.18.0/pbjson.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbjson
-Version: 1.17.0
+Version: 1.18.0
 Summary: Packed Binary JSON encoder/decoder for Python
 Home-page: https://github.com/scottkmaxwell/pbjson
 Author: Scott Maxwell
 Author-email: scott@codecobblers.com
 License: MIT License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,14 +53,27 @@
 
 The decoder can handle incoming JSON strings of any specified encoding
 (UTF-8 by default). It can also be specialized to post-process JSON
 objects with the ``object_hook`` or ``object_pairs_hook`` kwargs. This
 is particularly useful for implementing protocols that have a richer
 type system than JSON itself.
 
+Using the API
+-------------
+
+The ``pbjson`` module works ust like the ``json`` module. You can ``pbjson.load``,
+``pbjson.loads``, ``pbjson.dump``, and ``pbjson.dumps``.
+
+Command-Line Tool
+-----------------
+
+After you have installed ``pbjson``, you can use the ``pbjson`` command-line tool to
+convert files to or from ``pbjson``. Run ``pbjson -h`` for details.
+
+
 What is Packed Binary JSON (``PBJSON``)
 ---------------------------------------
 
 Packed Binary JSON is not the same as ``BSON``. ``BSON`` is a format
 used primarily in MongoDB and is meant for efficient parsing. ``PBJSON``
 is meant for efficient conversion from a dict or list, transmission and
 conversion back to a dict or list on the other end. ``BSON`` has
@@ -144,15 +157,15 @@
        }
    }
 
 ::
 
    E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
    08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
-   0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
+   0A 'dimensions' E2 09 'thickness' 61 d7 05 'width' 62 4d5d
 
 Let's break that out:
 
 -  00: E5 - dict with 5 elements
 -  01: 05 - key with 5 characters
 -  02-06: toast
 -  07: 01 - true
@@ -173,23 +186,22 @@
 -  32: 86 - string with 6 characters
 -  33-38: butter
 -  39: 0A - key with 10 bytes
 -  3A-43: dimensions
 -  44: E3 - dict with 2 elements
 -  45: 09 - key with 9 characters
 -  46-4E: thickness
--  4F: 68 - float with 8 bytes
--  50-57: IEEE representation of .7
--  58: 05 - key with 5 characters
--  59-5D: width
--  5E: 62 - float with 2 bytes
--  5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes
-   were all zeros.
+-  4F: 61 - float with 1 bytes
+-  50: first byte of IEEE representation of .7. Remaining 7 bytes were all zeros.
+-  51: 05 - key with 5 characters
+-  52-56: width
+-  57: 62 - float with 2 bytes
+-  58-59: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes were all zeros.
 
-Total 97 bytes. The tightest ``JSON`` representation requires 126 bytes.
+Total 90 bytes. The tightest ``JSON`` representation requires 126 bytes.
 Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
 
 Now here is an example with repeating data:
 
 .. code:: javascript
 
    {
```

### Comparing `pbjson-1.17.0/pbjson.egg-info/SOURCES.txt` & `pbjson-1.18.0/pbjson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pbjson-1.17.0/setup.py` & `pbjson-1.18.0/setup.py`

 * *Files identical despite different names*

