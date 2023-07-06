# Comparing `tmp/pbjson-1.15.tar.gz` & `tmp/pbjson-1.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pbjson-1.15.tar", last modified: Mon Apr 29 19:53:29 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pbjson-1.15.tar` & `pbjson-1.16.0.tar`

### file list

```diff
@@ -1,40 +1,27 @@
-drwxr-xr-x   0 smaxwell (362104396) ANT\Domain Users (1896053708)        0 2019-04-29 19:53:29.000000 pbjson-1.15/
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      215 2019-04-29 17:06:09.000000 pbjson-1.15/CHANGES.txt
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     7286 2019-04-29 19:52:45.000000 pbjson-1.15/DESCRIPTION.rst
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)    10373 2019-04-26 17:09:05.000000 pbjson-1.15/LICENSE.txt
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)       61 2019-04-26 17:09:05.000000 pbjson-1.15/MANIFEST.in
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)    10206 2019-04-29 19:53:29.000000 pbjson-1.15/PKG-INFO
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     7060 2019-04-29 00:32:18.000000 pbjson-1.15/README.md
-drwxr-xr-x   0 smaxwell (362104396) ANT\Domain Users (1896053708)        0 2019-04-29 19:53:29.000000 pbjson-1.15/pbjson/
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     7737 2019-04-29 16:26:26.000000 pbjson-1.15/pbjson/__init__.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)    50123 2019-04-29 16:33:52.000000 pbjson-1.15/pbjson/_speedups.c
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      754 2019-04-29 16:27:24.000000 pbjson-1.15/pbjson/compat.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     4716 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/decoder.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)    11000 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/encoder.py
-drwxr-xr-x   0 smaxwell (362104396) ANT\Domain Users (1896053708)        0 2019-04-29 19:53:29.000000 pbjson-1.15/pbjson/tests/
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     2253 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/__init__.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      594 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_check_circular.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     1015 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_custom.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)    10841 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_decode.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      259 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_default.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)    10067 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_encode.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     1434 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_float.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     3054 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_for_json.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     1217 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_item_sort_key.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     3716 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_mapping.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     1804 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_pass1.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      420 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_pass2.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      453 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_speedups.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      846 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_tuple.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     1314 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tests/test_unicode.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      774 2019-04-26 17:09:05.000000 pbjson-1.15/pbjson/tokens.py
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     3862 2019-04-29 16:55:18.000000 pbjson-1.15/pbjson/tool.py
-drwxr-xr-x   0 smaxwell (362104396) ANT\Domain Users (1896053708)        0 2019-04-29 19:53:29.000000 pbjson-1.15/pbjson.egg-info/
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)    10206 2019-04-29 19:53:29.000000 pbjson-1.15/pbjson.egg-info/PKG-INFO
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)      820 2019-04-29 19:53:29.000000 pbjson-1.15/pbjson.egg-info/SOURCES.txt
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)        1 2019-04-29 19:53:29.000000 pbjson-1.15/pbjson.egg-info/dependency_links.txt
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)       74 2019-04-29 19:53:29.000000 pbjson-1.15/pbjson.egg-info/entry_points.txt
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)        1 2019-04-29 16:32:35.000000 pbjson-1.15/pbjson.egg-info/not-zip-safe
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)        7 2019-04-29 19:53:29.000000 pbjson-1.15/pbjson.egg-info/top_level.txt
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)       79 2019-04-29 19:53:29.000000 pbjson-1.15/setup.cfg
--rw-r--r--   0 smaxwell (362104396) ANT\Domain Users (1896053708)     4075 2019-04-29 19:53:23.000000 pbjson-1.15/setup.py
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/__init__.py
+-rw-r--r--   0        0        0    50123 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/_speedups.c
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/compat.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/decoder.py
+-rw-r--r--   0        0        0    10968 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/encoder.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tokens.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tool.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/__init__.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_check_circular.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_custom.py
+-rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_decode.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_default.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_encode.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_float.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_for_json.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_item_sort_key.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_mapping.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_pass1.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_pass2.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_speedups.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_tuple.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 pbjson-1.16.0/pbjson/tests/test_unicode.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pbjson-1.16.0/.gitignore
+-rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 pbjson-1.16.0/LICENSE
+-rw-r--r--   0        0        0     7060 2020-02-02 00:00:00.000000 pbjson-1.16.0/README.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 pbjson-1.16.0/pyproject.toml
+-rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 pbjson-1.16.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pbjson-1.15/DESCRIPTION.rst` & `pbjson-1.16.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,217 +1,165 @@
 pbjson
 ======
 
 Packed Binary JSON extension for Python
 
-``pbjson`` is a packed binary JSON encoder and decoder for Python 2.5+
-and Python 3.3+. It is pure Python code with no dependencies, but
-includes an optional C extension for a serious speed boost.
-
-``pbjson`` can be used standalone or as an extension to the standard
-``json`` module or to ``simplejson``, from which code was heavily
-borrowed. The latest documentation for ``simplejson`` can be read online
-here: http://simplejson.readthedocs.org/
-
-The encoder can be specialized to provide serialization in any kind of
-situation, without any special support by the objects to be serialized
-(somewhat like pickle). This is best done with the ``default`` kwarg to
-dumps.
-
-The decoder can handle incoming JSON strings of any specified encoding
-(UTF-8 by default). It can also be specialized to post-process JSON
-objects with the ``object_hook`` or ``object_pairs_hook`` kwargs. This
-is particularly useful for implementing protocols that have a richer
-type system than JSON itself.
-
-What is Packed Binary JSON (``PBJSON``)
----------------------------------------
-
-Packed Binary JSON is not the same as ``BSON``. ``BSON`` is a format
-used primarily in MongoDB and is meant for efficient parsing. ``PBJSON``
-is meant for efficient conversion from a dict or list, transmission and
-conversion back to a dict or list on the other end. ``BSON`` has
-explicit support for several types not available in standard JSON.
-PBJSON supports only those types supported by normal JSON, plus binary
-data blobs and set collections.
-
-Unlike ``BSON``, ``PBJSON`` is almost always smaller than the equivalent
-JSON. Like ``BSON``, ``PBJSON`` can be very quickly encoded and decoded
-since all elements are length encoded.
-
-There are two types of tokens in ``PBJSON``: data and key. Data tokens
-can be zero length fundamental types (``false``, ``true``, ``null``),
-variable length fundamental types (``int``, ``float``, ``string``,
-``binary``) or containers (``set``, ``array``, ``dict``).
-
-The type for the data token is generally stored in the top 3 bits (bits
-5-7). Type zero is a special type to represent the zero length
-fundamental types. The lower bits indicate the actual value. These are:
+`pbjson` is a packed binary JSON encoder and decoder for Python 2.5+ and Python 3.3+. It is pure Python code with no dependencies, but includes an optional C extension for a serious speed boost.
+
+`pbjson` can be used standalone or as an extension to the standard `json` module or to `simplejson`, from which code was heavily borrowed. The latest documentation for `simplejson` can be read online here:
+<http://simplejson.readthedocs.org/>
+
+The encoder can be specialized to provide serialization in any kind of situation, without any special support by the objects to be serialized (somewhat like pickle). This is best done with the `default` kwarg to dumps.
+
+The decoder can handle incoming JSON strings of any specified encoding (UTF-8 by default). It can also be specialized to post-process JSON objects with the `object_hook` or `object_pairs_hook` kwargs. This
+is particularly useful for implementing protocols that have a richer type system than JSON itself.
+
+What is Packed Binary JSON (`PBJSON`)
+-----------------------------------
+
+Packed Binary JSON is not the same as `BSON`. `BSON` is a format used primarily in MongoDB and is meant for efficient parsing. `PBJSON` is meant for efficient conversion from a dict or list, transmission and conversion back to a dict or list on the other end. `BSON` has explicit support for several types not available in standard JSON. PBJSON supports only those types supported by normal JSON, plus binary data blobs and set collections.
+
+Unlike `BSON`, `PBJSON` is almost always smaller than the equivalent JSON. Like `BSON`, `PBJSON` can be very quickly encoded and decoded since all elements are length encoded.
+
+There are two types of tokens in `PBJSON`: data and key. Data tokens can be zero length fundamental types (`false`, `true`, `null`), variable length fundamental types (`int`, `float`, `string`, `binary`) or containers (`set`, `array`, `dict`).
+
+The type for the data token is generally stored in the top 3 bits (bits 5-7). Type zero is a special type to represent the zero length fundamental types. The lower bits indicate the actual value. These are:
 
 Zero-length Data Types:
 
--  00 - false
--  01 - true
--  02 - null
-
-All other types are variable length. If the length is between 0 and 15,
-that length is stored in bits 0-3. For lengths in the 16-2047 range, bit
-4 is set and bits 0-2 are combined with the next byte to make an 11-bit
-length. If bits 4 and 3 are both set, then the value in bits 0-2 are
-combined with the next 2 bytes to create a 19-bit length. However, if
-bits 4-0 are all set, this indicates that the following 4 bytes are
-simply used as a size. So the token plus length is, one byte (length of
-0-15), two bytes (16-2047), three bytes (2048-458751) or five bytes
-(458876-4294967295).
+- 00 - false
+- 01 - true
+- 02 - null
+
+All other types are variable length. If the length is between 0 and 15, that length is stored in bits 0-3. For lengths in the 16-2047 range, bit 4 is set and bits 0-2 are combined with the next byte to make an 11-bit length. If bits 4 and 3 are both set, then the value in bits 0-2 are combined with the next 2 bytes to create a 19-bit length. However, if bits 4-0 are all set, this indicates that the following 4 bytes are simply used as a size. So the token plus length is, one byte (length of 0-15), two bytes (16-2047), three bytes (2048-458751) or five bytes (458876-4294967295).
 
 Variable-length Data types:
 
--  2x - int (bytes stored big endian with leading zero bytes removed)
--  4x - negative int (bytes stored big endian as a positive number with
-   leading zero bytes removed)
--  6x - float (stored as big endian double precision with trailing zero
-   bytes removed)
--  8x - string
--  Ax - binary
+- 2x - int (bytes stored big endian with leading zero bytes removed)
+- 4x - negative int (bytes stored big endian as a positive number with leading zero bytes removed)
+- 6x - float (stored as big endian double precision with trailing zero bytes removed)
+- 8x - string
+- Ax - binary
 
 Collection types: (length is number of elements)
 
--  Cx - array
--  Ex - object
--  0C - terminated array
--  0F - terminator
-
-The final entry, the "terminated array" works a bit differently. This is
-for use when the length is not known when writing begins. Instead, a
-terminator (0F) is written to the stream when the last element of the
-array has been written.
-
-Object keys must be text and are a maximum of 127 bytes in length. They
-are stored as a (7-bit length, followed by the actual key. The first 128
-keys are remembered by index. If the same key is used again, it can be
-represented as a single byte consisting of the high bit and the index
-number of the key.
-
-In other words, if the recurring key is "toast", it should be encoded as
-05 toast. The next time the key "toast" is needed, it can be encoded as
-simply 80, since it was the first key.
+- Cx - array
+- Ex - object
+- 0C - terminated array
+- 0F - terminator
 
-Here is an example of a simple structure:
+The final entry, the "terminated array" works a bit differently. This is for use when the length is not known when writing begins. Instead, a terminator (0F) is written to the stream when the last element of the array has been written.
 
-.. code:: javascript
+Object keys must be text and are a maximum of 127 bytes in length. They are stored as a (7-bit length, followed by the actual key. The first 128 keys are remembered by index. If the same key is used again, it can be represented as a single byte consisting of the high bit and the index number of the key.
 
-   {
-       "toast": true,
-       "burned": false,
-       "name": "the best",
-       "toppings": ["jelly","jam","butter"],
-       "dimensions": {
-           "thickness": 0.7,
-           "width": 4.5
-       }
-   }
-
-::
-
-   E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
-   08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
-   0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
-
-Let’s break that out:
-
--  00: E5 - dict with 5 elements
--  01: 05 - key with 5 characters
--  02-06: toast
--  07: 01 - true
--  08: 06 - key with 6 characters
--  09-0E: burned
--  0F: 00 - false
--  10: 04 - key with 4 characters
--  11-14: name
--  15: 88 - string with 8 characters
--  16-1D: the best
--  1E: 08 - key with 8 bytes
--  1F-26: toppings
--  27: C3 - array with 3 elements
--  28: 85 - string with 5 characters
--  29-2D: jelly
--  2E: 83 - string with 3 characters
--  2F-31: jam
--  32: 86 - string with 6 characters
--  33-38: butter
--  39: 0A - key with 10 bytes
--  3A-43: dimensions
--  44: E3 - dict with 2 elements
--  45: 09 - key with 9 characters
--  46-4E: thickness
--  4F: 68 - float with 8 bytes
--  50-57: IEEE representation of .7
--  58: 05 - key with 5 characters
--  59-5D: width
--  5E: 62 - float with 2 bytes
--  5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes
-   were all zeros.
+In other words, if the recurring key is "toast", it should be encoded as 05 toast. The next time the key "toast" is needed, it can be encoded as simply 80, since it was the first key.
 
-Total 97 bytes. The tightest ``JSON`` representation requires 126 bytes.
-Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
+Here is an example of a simple structure:
 
-Now here is an example with repeating data:
+```javascript
+{
+    "toast": true,
+    "burned": false,
+    "name": "the best",
+    "toppings": ["jelly","jam","butter"],
+    "dimensions": {
+        "thickness": 0.7,
+        "width": 4.5
+    }
+}
+```
+
+    E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
+    08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
+    0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
+
+Let's break that out:
+
+- 00: E5 - dict with 5 elements
+- 01: 05 - key with 5 characters
+- 02-06: toast
+- 07: 01 - true
+- 08: 06 - key with 6 characters
+- 09-0E: burned
+- 0F: 00 - false
+- 10: 04 - key with 4 characters
+- 11-14: name
+- 15: 88 - string with 8 characters
+- 16-1D: the best
+- 1E: 08 - key with 8 bytes
+- 1F-26: toppings
+- 27: C3 - array with 3 elements
+- 28: 85 - string with 5 characters
+- 29-2D: jelly
+- 2E: 83 - string with 3 characters
+- 2F-31: jam
+- 32: 86 - string with 6 characters
+- 33-38: butter
+- 39: 0A - key with 10 bytes
+- 3A-43: dimensions
+- 44: E3 - dict with 2 elements
+- 45: 09 - key with 9 characters
+- 46-4E: thickness
+- 4F: 68 - float with 8 bytes
+- 50-57: IEEE representation of .7
+- 58: 05 - key with 5 characters
+- 59-5D: width
+- 5E: 62 - float with 2 bytes
+- 5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes were all zeros.
 
-.. code:: javascript
+Total 97 bytes. The tightest `JSON` representation requires 126 bytes. Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
 
-   {
-       "region": 3,
-       "countries": [
-           {"code": "us", "name": "United States"},
-           {"code": "ca", "name": "Canada"},
-           {"code": "mx", "name": "Mexico"}
-       ]
-   }
-
-::
-
-   E2 06 region 21 03 09 countries C3
-   E2 04 code 82 us 04 name 8D United States
-   E2 82 82 ca 83 86 Canada
-   E2 82 82 mx 83 86 Mexico
+Now here is an example with repeating data:
+
+```javascript
+{
+    "region": 3,
+    "countries": [
+        {"code": "us", "name": "United States"},
+        {"code": "ca", "name": "Canada"},
+        {"code": "mx", "name": "Mexico"}
+    ]
+}
+```
+
+    E2 06 region 21 03 09 countries C3
+    E2 04 code 82 us 04 name 8D United States
+    E2 82 82 ca 83 86 Canada
+    E2 82 82 mx 83 86 Mexico
 
 This breaks down thus:
 
--  00: E2 - dict with 2 elements
--  01: 06 - key with 6 characters
--  02-07: region
--  08: 21 - int with 1 byte
--  09: 03 - the int for 3. Only a single byte is required.
--  0A: 09 - key with 9 bytes
--  0B-13: countries
--  14: C3 - array with 3 elements
--  15: E2 - dict with 2 elements
--  16: 04 - key with 4 characters
--  17-1A: code
--  19: 82 - string with 2 characters
--  1A-1B: us
--  1C: 04 - key with 4 characters
--  1E-21: name
--  22: 8D - string with 13 characters
--  23-2F: United States
--  30: E2 - dict with 2 elements
--  31: 82 - recurring key 2. Since ‘code’ was the 3rd key, it has an
-   index of 2.
--  32: 82 - string with 2 characters
--  33-34: ca
--  35: 83 - recurring key 3
--  36: 86 - string with 6 characters
--  37-3C: Canada
--  3D: E2 - dict with 2 elements
--  3E: 82 - recurring key 0
--  3F: 82 - string with 2 characters
--  40-41: mx
--  42: 83 - recurring key 1
--  43: 86 - string with 6 characters
--  44-49: Mexico
-
-Total 74 bytes. The tightest ``JSON`` representation requires 123 bytes.
-Marshal takes 158 bytes and Pickle takes 162. BSON takes 154 bytes.
-
-``Packed Binary JSON`` is available now in the ``pbjson`` Python module.
-That module includes a command line utility to convert between normal
-``JSON`` files and ``PBJSON``.
+- 00: E2 - dict with 2 elements
+- 01: 06 - key with 6 characters
+- 02-07: region
+- 08: 21 - int with 1 byte
+- 09: 03 - the int for 3. Only a single byte is required.
+- 0A: 09 - key with 9 bytes
+- 0B-13: countries
+- 14: C3 - array with 3 elements
+- 15: E2 - dict with 2 elements
+- 16: 04 - key with 4 characters
+- 17-1A: code
+- 19: 82 - string with 2 characters
+- 1A-1B: us
+- 1C: 04 - key with 4 characters
+- 1E-21: name
+- 22: 8D - string with 13 characters
+- 23-2F: United States
+- 30: E2 - dict with 2 elements
+- 31: 82 - recurring key 2. Since 'code' was the 3rd key, it has an index of 2.
+- 32: 82 - string with 2 characters
+- 33-34: ca
+- 35: 83 - recurring key 3
+- 36: 86 - string with 6 characters
+- 37-3C: Canada
+- 3D: E2 - dict with 2 elements
+- 3E: 82 - recurring key 0
+- 3F: 82 - string with 2 characters
+- 40-41: mx
+- 42: 83 - recurring key 1
+- 43: 86 - string with 6 characters
+- 44-49: Mexico
+
+Total 74 bytes. The tightest `JSON` representation requires 123 bytes. Marshal takes 158 bytes and Pickle takes 162. BSON takes 154 bytes.
+
+`Packed Binary JSON` is available now in the `pbjson` Python module. That module includes a command line utility to convert between normal `JSON` files and `PBJSON`.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pbjson-1.15/LICENSE.txt` & `pbjson-1.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/PKG-INFO` & `pbjson-1.16.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,244 +1,197 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pbjson
-Version: 1.15
+Version: 1.16.0
 Summary: Packed Binary JSON encoder/decoder for Python
-Home-page: https://github.com/scottkmaxwell/pbjson
-Author: Scott Maxwell
-Author-email: scott@codecobblers.com
-License: MIT License
-Description: pbjson
-        ======
-        
-        Packed Binary JSON extension for Python
-        
-        ``pbjson`` is a packed binary JSON encoder and decoder for Python 2.5+
-        and Python 3.3+. It is pure Python code with no dependencies, but
-        includes an optional C extension for a serious speed boost.
-        
-        ``pbjson`` can be used standalone or as an extension to the standard
-        ``json`` module or to ``simplejson``, from which code was heavily
-        borrowed. The latest documentation for ``simplejson`` can be read online
-        here: http://simplejson.readthedocs.org/
-        
-        The encoder can be specialized to provide serialization in any kind of
-        situation, without any special support by the objects to be serialized
-        (somewhat like pickle). This is best done with the ``default`` kwarg to
-        dumps.
-        
-        The decoder can handle incoming JSON strings of any specified encoding
-        (UTF-8 by default). It can also be specialized to post-process JSON
-        objects with the ``object_hook`` or ``object_pairs_hook`` kwargs. This
-        is particularly useful for implementing protocols that have a richer
-        type system than JSON itself.
-        
-        What is Packed Binary JSON (``PBJSON``)
-        ---------------------------------------
-        
-        Packed Binary JSON is not the same as ``BSON``. ``BSON`` is a format
-        used primarily in MongoDB and is meant for efficient parsing. ``PBJSON``
-        is meant for efficient conversion from a dict or list, transmission and
-        conversion back to a dict or list on the other end. ``BSON`` has
-        explicit support for several types not available in standard JSON.
-        PBJSON supports only those types supported by normal JSON, plus binary
-        data blobs and set collections.
-        
-        Unlike ``BSON``, ``PBJSON`` is almost always smaller than the equivalent
-        JSON. Like ``BSON``, ``PBJSON`` can be very quickly encoded and decoded
-        since all elements are length encoded.
-        
-        There are two types of tokens in ``PBJSON``: data and key. Data tokens
-        can be zero length fundamental types (``false``, ``true``, ``null``),
-        variable length fundamental types (``int``, ``float``, ``string``,
-        ``binary``) or containers (``set``, ``array``, ``dict``).
-        
-        The type for the data token is generally stored in the top 3 bits (bits
-        5-7). Type zero is a special type to represent the zero length
-        fundamental types. The lower bits indicate the actual value. These are:
-        
-        Zero-length Data Types:
-        
-        -  00 - false
-        -  01 - true
-        -  02 - null
-        
-        All other types are variable length. If the length is between 0 and 15,
-        that length is stored in bits 0-3. For lengths in the 16-2047 range, bit
-        4 is set and bits 0-2 are combined with the next byte to make an 11-bit
-        length. If bits 4 and 3 are both set, then the value in bits 0-2 are
-        combined with the next 2 bytes to create a 19-bit length. However, if
-        bits 4-0 are all set, this indicates that the following 4 bytes are
-        simply used as a size. So the token plus length is, one byte (length of
-        0-15), two bytes (16-2047), three bytes (2048-458751) or five bytes
-        (458876-4294967295).
-        
-        Variable-length Data types:
-        
-        -  2x - int (bytes stored big endian with leading zero bytes removed)
-        -  4x - negative int (bytes stored big endian as a positive number with
-           leading zero bytes removed)
-        -  6x - float (stored as big endian double precision with trailing zero
-           bytes removed)
-        -  8x - string
-        -  Ax - binary
-        
-        Collection types: (length is number of elements)
-        
-        -  Cx - array
-        -  Ex - object
-        -  0C - terminated array
-        -  0F - terminator
-        
-        The final entry, the "terminated array" works a bit differently. This is
-        for use when the length is not known when writing begins. Instead, a
-        terminator (0F) is written to the stream when the last element of the
-        array has been written.
-        
-        Object keys must be text and are a maximum of 127 bytes in length. They
-        are stored as a (7-bit length, followed by the actual key. The first 128
-        keys are remembered by index. If the same key is used again, it can be
-        represented as a single byte consisting of the high bit and the index
-        number of the key.
-        
-        In other words, if the recurring key is "toast", it should be encoded as
-        05 toast. The next time the key "toast" is needed, it can be encoded as
-        simply 80, since it was the first key.
-        
-        Here is an example of a simple structure:
-        
-        .. code:: javascript
-        
-           {
-               "toast": true,
-               "burned": false,
-               "name": "the best",
-               "toppings": ["jelly","jam","butter"],
-               "dimensions": {
-                   "thickness": 0.7,
-                   "width": 4.5
-               }
-           }
-        
-        ::
-        
-           E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
-           08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
-           0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
-        
-        Let’s break that out:
-        
-        -  00: E5 - dict with 5 elements
-        -  01: 05 - key with 5 characters
-        -  02-06: toast
-        -  07: 01 - true
-        -  08: 06 - key with 6 characters
-        -  09-0E: burned
-        -  0F: 00 - false
-        -  10: 04 - key with 4 characters
-        -  11-14: name
-        -  15: 88 - string with 8 characters
-        -  16-1D: the best
-        -  1E: 08 - key with 8 bytes
-        -  1F-26: toppings
-        -  27: C3 - array with 3 elements
-        -  28: 85 - string with 5 characters
-        -  29-2D: jelly
-        -  2E: 83 - string with 3 characters
-        -  2F-31: jam
-        -  32: 86 - string with 6 characters
-        -  33-38: butter
-        -  39: 0A - key with 10 bytes
-        -  3A-43: dimensions
-        -  44: E3 - dict with 2 elements
-        -  45: 09 - key with 9 characters
-        -  46-4E: thickness
-        -  4F: 68 - float with 8 bytes
-        -  50-57: IEEE representation of .7
-        -  58: 05 - key with 5 characters
-        -  59-5D: width
-        -  5E: 62 - float with 2 bytes
-        -  5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes
-           were all zeros.
-        
-        Total 97 bytes. The tightest ``JSON`` representation requires 126 bytes.
-        Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
-        
-        Now here is an example with repeating data:
-        
-        .. code:: javascript
-        
-           {
-               "region": 3,
-               "countries": [
-                   {"code": "us", "name": "United States"},
-                   {"code": "ca", "name": "Canada"},
-                   {"code": "mx", "name": "Mexico"}
-               ]
-           }
-        
-        ::
-        
-           E2 06 region 21 03 09 countries C3
-           E2 04 code 82 us 04 name 8D United States
-           E2 82 82 ca 83 86 Canada
-           E2 82 82 mx 83 86 Mexico
-        
-        This breaks down thus:
-        
-        -  00: E2 - dict with 2 elements
-        -  01: 06 - key with 6 characters
-        -  02-07: region
-        -  08: 21 - int with 1 byte
-        -  09: 03 - the int for 3. Only a single byte is required.
-        -  0A: 09 - key with 9 bytes
-        -  0B-13: countries
-        -  14: C3 - array with 3 elements
-        -  15: E2 - dict with 2 elements
-        -  16: 04 - key with 4 characters
-        -  17-1A: code
-        -  19: 82 - string with 2 characters
-        -  1A-1B: us
-        -  1C: 04 - key with 4 characters
-        -  1E-21: name
-        -  22: 8D - string with 13 characters
-        -  23-2F: United States
-        -  30: E2 - dict with 2 elements
-        -  31: 82 - recurring key 2. Since ‘code’ was the 3rd key, it has an
-           index of 2.
-        -  32: 82 - string with 2 characters
-        -  33-34: ca
-        -  35: 83 - recurring key 3
-        -  36: 86 - string with 6 characters
-        -  37-3C: Canada
-        -  3D: E2 - dict with 2 elements
-        -  3E: 82 - recurring key 0
-        -  3F: 82 - string with 2 characters
-        -  40-41: mx
-        -  42: 83 - recurring key 1
-        -  43: 86 - string with 6 characters
-        -  44-49: Mexico
-        
-        Total 74 bytes. The tightest ``JSON`` representation requires 123 bytes.
-        Marshal takes 158 bytes and Pickle takes 162. BSON takes 154 bytes.
-        
-        ``Packed Binary JSON`` is available now in the ``pbjson`` Python module.
-        That module includes a command line utility to convert between normal
-        ``JSON`` files and ``PBJSON``.
-        
-Platform: any
+Project-URL: Homepage, https://github.com/scottkmaxwell/pbjson
+Project-URL: Bug Tracker, https://github.com/scottkmaxwell/pbjson/issues
+Author-email: Scott Maxwell <scott@codecobblers.com>
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+
+pbjson
+======
+
+Packed Binary JSON extension for Python
+
+`pbjson` is a packed binary JSON encoder and decoder for Python 2.5+ and Python 3.3+. It is pure Python code with no dependencies, but includes an optional C extension for a serious speed boost.
+
+`pbjson` can be used standalone or as an extension to the standard `json` module or to `simplejson`, from which code was heavily borrowed. The latest documentation for `simplejson` can be read online here:
+<http://simplejson.readthedocs.org/>
+
+The encoder can be specialized to provide serialization in any kind of situation, without any special support by the objects to be serialized (somewhat like pickle). This is best done with the `default` kwarg to dumps.
+
+The decoder can handle incoming JSON strings of any specified encoding (UTF-8 by default). It can also be specialized to post-process JSON objects with the `object_hook` or `object_pairs_hook` kwargs. This
+is particularly useful for implementing protocols that have a richer type system than JSON itself.
+
+What is Packed Binary JSON (`PBJSON`)
+-----------------------------------
+
+Packed Binary JSON is not the same as `BSON`. `BSON` is a format used primarily in MongoDB and is meant for efficient parsing. `PBJSON` is meant for efficient conversion from a dict or list, transmission and conversion back to a dict or list on the other end. `BSON` has explicit support for several types not available in standard JSON. PBJSON supports only those types supported by normal JSON, plus binary data blobs and set collections.
+
+Unlike `BSON`, `PBJSON` is almost always smaller than the equivalent JSON. Like `BSON`, `PBJSON` can be very quickly encoded and decoded since all elements are length encoded.
+
+There are two types of tokens in `PBJSON`: data and key. Data tokens can be zero length fundamental types (`false`, `true`, `null`), variable length fundamental types (`int`, `float`, `string`, `binary`) or containers (`set`, `array`, `dict`).
+
+The type for the data token is generally stored in the top 3 bits (bits 5-7). Type zero is a special type to represent the zero length fundamental types. The lower bits indicate the actual value. These are:
+
+Zero-length Data Types:
+
+- 00 - false
+- 01 - true
+- 02 - null
+
+All other types are variable length. If the length is between 0 and 15, that length is stored in bits 0-3. For lengths in the 16-2047 range, bit 4 is set and bits 0-2 are combined with the next byte to make an 11-bit length. If bits 4 and 3 are both set, then the value in bits 0-2 are combined with the next 2 bytes to create a 19-bit length. However, if bits 4-0 are all set, this indicates that the following 4 bytes are simply used as a size. So the token plus length is, one byte (length of 0-15), two bytes (16-2047), three bytes (2048-458751) or five bytes (458876-4294967295).
+
+Variable-length Data types:
+
+- 2x - int (bytes stored big endian with leading zero bytes removed)
+- 4x - negative int (bytes stored big endian as a positive number with leading zero bytes removed)
+- 6x - float (stored as big endian double precision with trailing zero bytes removed)
+- 8x - string
+- Ax - binary
+
+Collection types: (length is number of elements)
+
+- Cx - array
+- Ex - object
+- 0C - terminated array
+- 0F - terminator
+
+The final entry, the "terminated array" works a bit differently. This is for use when the length is not known when writing begins. Instead, a terminator (0F) is written to the stream when the last element of the array has been written.
+
+Object keys must be text and are a maximum of 127 bytes in length. They are stored as a (7-bit length, followed by the actual key. The first 128 keys are remembered by index. If the same key is used again, it can be represented as a single byte consisting of the high bit and the index number of the key.
+
+In other words, if the recurring key is "toast", it should be encoded as 05 toast. The next time the key "toast" is needed, it can be encoded as simply 80, since it was the first key.
+
+Here is an example of a simple structure:
+
+```javascript
+{
+    "toast": true,
+    "burned": false,
+    "name": "the best",
+    "toppings": ["jelly","jam","butter"],
+    "dimensions": {
+        "thickness": 0.7,
+        "width": 4.5
+    }
+}
+```
+
+    E5 05 'toast' 01 06 'burned' 00 04 'name' 88 'the best'
+    08 'toppings' C3 85 'jelly' 83 'jam' 86 'butter'
+    0A 'dimensions' E2 09 'thickness' 68 3FE6666666666666 05 'width' 62 4012
+
+Let's break that out:
+
+- 00: E5 - dict with 5 elements
+- 01: 05 - key with 5 characters
+- 02-06: toast
+- 07: 01 - true
+- 08: 06 - key with 6 characters
+- 09-0E: burned
+- 0F: 00 - false
+- 10: 04 - key with 4 characters
+- 11-14: name
+- 15: 88 - string with 8 characters
+- 16-1D: the best
+- 1E: 08 - key with 8 bytes
+- 1F-26: toppings
+- 27: C3 - array with 3 elements
+- 28: 85 - string with 5 characters
+- 29-2D: jelly
+- 2E: 83 - string with 3 characters
+- 2F-31: jam
+- 32: 86 - string with 6 characters
+- 33-38: butter
+- 39: 0A - key with 10 bytes
+- 3A-43: dimensions
+- 44: E3 - dict with 2 elements
+- 45: 09 - key with 9 characters
+- 46-4E: thickness
+- 4F: 68 - float with 8 bytes
+- 50-57: IEEE representation of .7
+- 58: 05 - key with 5 characters
+- 59-5D: width
+- 5E: 62 - float with 2 bytes
+- 5F-60: first 2 bytes of IEEE representation of 4.5. Remaining 6 bytes were all zeros.
+
+Total 97 bytes. The tightest `JSON` representation requires 126 bytes. Marshal takes 153 bytes. Pickle takes 184 bytes. BSON takes 145 bytes.
+
+Now here is an example with repeating data:
+
+```javascript
+{
+    "region": 3,
+    "countries": [
+        {"code": "us", "name": "United States"},
+        {"code": "ca", "name": "Canada"},
+        {"code": "mx", "name": "Mexico"}
+    ]
+}
+```
+
+    E2 06 region 21 03 09 countries C3
+    E2 04 code 82 us 04 name 8D United States
+    E2 82 82 ca 83 86 Canada
+    E2 82 82 mx 83 86 Mexico
+
+This breaks down thus:
+
+- 00: E2 - dict with 2 elements
+- 01: 06 - key with 6 characters
+- 02-07: region
+- 08: 21 - int with 1 byte
+- 09: 03 - the int for 3. Only a single byte is required.
+- 0A: 09 - key with 9 bytes
+- 0B-13: countries
+- 14: C3 - array with 3 elements
+- 15: E2 - dict with 2 elements
+- 16: 04 - key with 4 characters
+- 17-1A: code
+- 19: 82 - string with 2 characters
+- 1A-1B: us
+- 1C: 04 - key with 4 characters
+- 1E-21: name
+- 22: 8D - string with 13 characters
+- 23-2F: United States
+- 30: E2 - dict with 2 elements
+- 31: 82 - recurring key 2. Since 'code' was the 3rd key, it has an index of 2.
+- 32: 82 - string with 2 characters
+- 33-34: ca
+- 35: 83 - recurring key 3
+- 36: 86 - string with 6 characters
+- 37-3C: Canada
+- 3D: E2 - dict with 2 elements
+- 3E: 82 - recurring key 0
+- 3F: 82 - string with 2 characters
+- 40-41: mx
+- 42: 83 - recurring key 1
+- 43: 86 - string with 6 characters
+- 44-49: Mexico
+
+Total 74 bytes. The tightest `JSON` representation requires 123 bytes. Marshal takes 158 bytes and Pickle takes 162. BSON takes 154 bytes.
+
+`Packed Binary JSON` is available now in the `pbjson` Python module. That module includes a command line utility to convert between normal `JSON` files and `PBJSON`.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pbjson-1.15/pbjson/__init__.py` & `pbjson-1.16.0/pbjson/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-r"""JSON (JavaScript Object Notation) <http://json.org> is a subset of
+r"""JSON (JavaScript Object Notation) <https://json.org> is a subset of
 JavaScript syntax (ECMA-262 3rd edition) used as a lightweight data
 interchange format. PBJSON is a binary encoding for JSON.
 
 :mod:`pbjson` exposes an API familiar to users of the standard library
 :mod:`marshal` and :mod:`pickle` modules.
 
 Encoding basic Python object hierarchies::
@@ -52,15 +52,15 @@
 
 Specializing JSON object encoding::
 
     >>> import pbjson
     >>> def encode_complex(obj):
     ...     if isinstance(obj, complex):
     ...         return [obj.real, obj.imag]
-    ...     raise TypeError(repr(o) + " is not JSON serializable")
+    ...     raise TypeError(repr(obj) + " is not JSON serializable")
     ...
     >>> pbjson.dumps(2 + 1j, converter=encode_complex)
     '[2.0, 1.0]'
 
 
 Using pbjson.tool from the shell to validate and pretty-print::
 
@@ -68,24 +68,25 @@
     {
         "json": "obj"
     }
     $ echo '{ 1.2:3.4}' | python -m simplejson.tool
     Expecting property name: line 1 column 3 (char 2)
 """
 from __future__ import absolute_import
-__version__ = '1.0.0'
+__version__ = '1.16.0'
 __all__ = [
     'dump', 'dumps', 'load', 'loads',
     'PBJSONDecodeError',
 ]
 
 __author__ = 'Scott Maxwell <scott@codecobblers.com>'
 
 from . import decoder
 from . import encoder
+from .decoder import PBJSONDecodeError
 
 
 def dump(obj, fp, skip_illegal_keys=False, check_circular=True, sort_keys=False, custom=None, convert=None, use_for_json=False):
     """Serialize ``obj`` as a Packed Binary JSON stream to ``fp`` (a
     ``.write()``-supporting file-like object).
 
     If *skip_illegal_keys* is true then ``dict`` keys that are not basic types
```

### Comparing `pbjson-1.15/pbjson/_speedups.c` & `pbjson-1.16.0/pbjson/_speedups.c`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/decoder.py` & `pbjson-1.16.0/pbjson/decoder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import absolute_import
-
 __author__ = 'Scott Maxwell'
-__all__ = ['decode']
+__all__ = ['decode', "PBJSONDecodeError"]
 
 # noinspection PyStatementEffect
 """Implementation of PBJSONDecoder"""
 import struct
 from .tokens import *
 
 
@@ -117,29 +115,29 @@
 def py_decoder(data, document_class=None, float_class=None, custom=None, unicode_errors='strict'):
     if isinstance(data, memoryview):
         data = data.tobytes()
     float_class = float_class or float
     document_class = document_class or dict
     keys = []
     context = {
-        FALSE: lambda context, data: (False, data),
-        TRUE: lambda context, data: (True, data),
-        NULL: lambda context, data: (None, data),
-        INF: lambda context, data: (float_class('inf'), data),
-        NEGINF: lambda context, data: (float_class('-inf'), data),
-        NAN: lambda context, data: (float_class('nan'), data),
+        FALSE: lambda _context, _data: (False, _data),
+        TRUE: lambda _context, _data: (True, _data),
+        NULL: lambda _context, _data: (None, _data),
+        INF: lambda _context, _data: (float_class('inf'), _data),
+        NEGINF: lambda _context, _data: (float_class('-inf'), _data),
+        NAN: lambda _context, _data: (float_class('nan'), _data),
         TERMINATED_LIST: _decode_list,
-        INT: lambda context, data: _decode_int(data),
-        NEGINT: lambda context, data: -_decode_int(data),
-        FLOAT: lambda context, data: _decode_float(float_class, data),
-        STRING: lambda context, data: data.decode(errors=unicode_errors),
-        BINARY: lambda context, data: data,
+        INT: lambda _context, _data: _decode_int(_data),
+        NEGINT: lambda _context, _data: -_decode_int(_data),
+        FLOAT: lambda _context, _data: _decode_float(float_class, _data),
+        STRING: lambda _context, _data: _data.decode(errors=unicode_errors),
+        BINARY: lambda _context, _data: _data,
         LIST: _decode_list,
-        DICT: lambda context, data, length: _decode_dict(context, document_class, keys, data, length),
-        CUSTOM: lambda context, data: _decode_custom(context, data, custom),
+        DICT: lambda _context, _data, length: _decode_dict(_context, document_class, keys, _data, length),
+        CUSTOM: lambda _context, _data: _decode_custom(_context, _data, custom),
     }
     return _decode_one(context, data)[0]
 
 
 # Use speedup if available
 c_decoder = _import_speedups()
 decode = c_decoder or py_decoder
```

### Comparing `pbjson-1.15/pbjson/encoder.py` & `pbjson-1.16.0/pbjson/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 # noinspection PyStatementEffect
 """Implementation of PBJSON encoder"""
 
 from operator import itemgetter
 from decimal import Decimal
 from struct import pack
-from .compat import text_type, binary_type, string_types, integer_types, PY3
+from .compat import text_type, binary_type, string_types, integer_types, Mapping, PY3
 from .tokens import *
-from collections import Mapping
 
 
 def _import_speedups():
     try:
         # noinspection PyUnresolvedReferences
         from . import _speedups
         return _speedups.encode
@@ -86,23 +85,23 @@
     convert = convert or default_converter
     for i in iterencoder(obj, Decimal, Mapping, skip_illegal_keys, check_circular, sort_keys, custom, convert, use_for_json):
         yield i
 
 
 # noinspection PyShadowingBuiltins
 def py_iterencoder(obj, Decimal, Mapping, skip_illegal_keys, check_circular, sort_keys, custom, convert, use_for_json,
-                    ## HACK: hand-optimized bytecode; turn globals into locals
-                    _PY3=PY3,
-                    ValueError=ValueError,
-                    string_types=string_types,
-                    float=float,
-                    id=id,
-                    integer_types=integer_types,
-                    isinstance=isinstance,
-                    str=str):
+                   # HACK: hand-optimized bytecode; turn globals into locals
+                   _PY3=PY3,
+                   ValueError=ValueError,
+                   string_types=string_types,
+                   float=float,
+                   id=id,
+                   integer_types=integer_types,
+                   isinstance=isinstance,
+                   str=str):
     key_cache = {}
     markers = {} if check_circular else None
     if custom and isinstance(custom[0], type):
         custom = (custom, )
     custom_types = tuple(c[0] for c in custom) if custom else None
 
     def _iterencode_list(lst):
@@ -294,9 +293,10 @@
                         yield chunk
                     if check_circular:
                         # noinspection PyUnboundLocalVariable
                         del markers[markerid]
 
     return _iterencode(obj)
 
+
 c_iterencoder = _import_speedups()
 iterencoder = c_iterencoder or py_iterencoder
```

### Comparing `pbjson-1.15/pbjson/tests/__init__.py` & `pbjson-1.16.0/pbjson/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from __future__ import absolute_import
 import unittest
 import sys
 
 
 class OptionalExtensionTestSuite(unittest.TestSuite):
-    def run(self, result, debug=False):
+    def __init__(self, suite, test_no_speedups=False):
+        super(OptionalExtensionTestSuite, self).__init__(suite)
+        self.test_no_speedups = test_no_speedups
+
+    def run(self, result, test_no_speedups=False):
         import pbjson
         run = unittest.TestSuite.run
-        for i in range(1):
+        if not self.test_no_speedups:
+            run(self, result)
+            return result
+
+        if not pbjson._has_encoder_speedups() and not pbjson._has_decoder_speedups():
+            print("Testing with missing speedups")
+            TestMissingSpeedups().run(result)
+        else:
+            pbjson._toggle_speedups(False)
             run(self, result)
-            if not pbjson._has_encoder_speedups() and not pbjson._has_decoder_speedups():
-                TestMissingSpeedups().run(result)
-            else:
-                pbjson._toggle_speedups(False)
-                run(self, result)
-                pbjson._toggle_speedups(True)
+            pbjson._toggle_speedups(True)
         return result
 
 
 class TestMissingSpeedups(unittest.TestCase):
     def runTest(self):
         if hasattr(sys, 'pypy_translation_info'):
             "PyPy doesn't need speedups! :)"
@@ -34,15 +41,15 @@
 #         suite = unittest.TestSuite()
 #     for mod in (pbjson, pbjson.encoder, pbjson.decoder):
 #         suite.addTest(doctest.DocTestSuite(mod))
 #     suite.addTest(doctest.DocFileSuite('../../index.rst'))
 #     return suite
 
 
-def all_tests_suite():
+def all_tests_suite(test_no_speedups=False):
     suite = unittest.TestLoader().loadTestsFromNames([
         'pbjson.tests.test_check_circular',
         'pbjson.tests.test_custom',
         # 'pbjson.tests.test_decimal',
         'pbjson.tests.test_decode',
         'pbjson.tests.test_default',
         'pbjson.tests.test_encode',
@@ -52,20 +59,23 @@
         'pbjson.tests.test_pass1',
         'pbjson.tests.test_pass2',
         # 'pbjson.tests.test_recursion',
         'pbjson.tests.test_speedups',
         'pbjson.tests.test_tuple',
     ])
     # suite = additional_tests(suite)
-    return OptionalExtensionTestSuite([suite])
+    return OptionalExtensionTestSuite([suite], test_no_speedups=test_no_speedups)
 
 
 def main():
     runner = unittest.TextTestRunner(verbosity=1 + sys.argv.count('-v'))
     suite = all_tests_suite()
+    if not runner.run(suite).wasSuccessful():
+        raise SystemExit(1)
+    suite = all_tests_suite(True)
     raise SystemExit(not runner.run(suite).wasSuccessful())
 
 
 if __name__ == '__main__':
     import os
     import sys
     sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
```

### Comparing `pbjson-1.15/pbjson/tests/test_check_circular.py` & `pbjson-1.16.0/pbjson/tests/test_check_circular.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_custom.py` & `pbjson-1.16.0/pbjson/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_decode.py` & `pbjson-1.16.0/pbjson/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_encode.py` & `pbjson-1.16.0/pbjson/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_float.py` & `pbjson-1.16.0/pbjson/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_for_json.py` & `pbjson-1.16.0/pbjson/tests/test_for_json.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_item_sort_key.py` & `pbjson-1.16.0/pbjson/tests/test_item_sort_key.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_mapping.py` & `pbjson-1.16.0/pbjson/tests/test_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 __author__ = 'Scott Maxwell'
 
-import collections
 import pbjson
+from pbjson.compat import Mapping, MutableMapping
 from operator import itemgetter
 from unittest import TestCase, main
 
 
-class CaseInsensitiveDict(collections.MutableMapping):
+class CaseInsensitiveDict(MutableMapping):
     """
     A case-insensitive ``dict``-like object.
 
     Implements all methods and operations of
     ``collections.MutableMapping`` as well as dict's ``copy``. Also
     provides ``lower_items``.
 
@@ -62,15 +62,15 @@
         return (
             (lowerkey, keyval[1])
             for (lowerkey, keyval)
             in self._store.items()
         )
 
     def __eq__(self, other):
-        if isinstance(other, collections.Mapping):
+        if isinstance(other, Mapping):
             other = CaseInsensitiveDict(other)
         else:
             return NotImplemented
         # Compare insensitively
         return dict(self.lower_items()) == dict(other.lower_items())
 
     # Copy is required
```

### Comparing `pbjson-1.15/pbjson/tests/test_pass1.py` & `pbjson-1.16.0/pbjson/tests/test_pass1.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_tuple.py` & `pbjson-1.16.0/pbjson/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tests/test_unicode.py` & `pbjson-1.16.0/pbjson/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tokens.py` & `pbjson-1.16.0/pbjson/tokens.py`

 * *Files identical despite different names*

### Comparing `pbjson-1.15/pbjson/tool.py` & `pbjson-1.16.0/pbjson/tool.py`

 * *Files identical despite different names*

