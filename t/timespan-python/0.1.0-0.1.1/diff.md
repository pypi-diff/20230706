# Comparing `tmp/timespan-python-0.1.0.tar.gz` & `tmp/timespan-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timespan-python-0.1.0.tar", last modified: Thu Jul  6 08:04:04 2023, max compression
+gzip compressed data, was "timespan-python-0.1.1.tar", last modified: Thu Jul  6 09:03:34 2023, max compression
```

## Comparing `timespan-python-0.1.0.tar` & `timespan-python-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:04:04.700173 timespan-python-0.1.0/
--rw-rw-rw-   0        0        0     1162 2023-07-05 13:54:28.000000 timespan-python-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2190 2023-07-06 08:04:04.700173 timespan-python-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2023-07-05 14:59:53.000000 timespan-python-0.1.0/README.md
--rw-rw-rw-   0        0        0      571 2023-07-06 08:04:04.700173 timespan-python-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-07-06 07:04:21.000000 timespan-python-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:04:04.683538 timespan-python-0.1.0/src/
--rw-rw-rw-   0        0        0        0 2023-07-05 14:04:50.000000 timespan-python-0.1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:04:04.693347 timespan-python-0.1.0/src/package/
--rw-rw-rw-   0        0        0        0 2023-07-05 14:04:50.000000 timespan-python-0.1.0/src/package/__init__.py
--rw-rw-rw-   0        0        0     7822 2023-07-05 14:04:50.000000 timespan-python-0.1.0/src/package/timespan.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:04:04.693347 timespan-python-0.1.0/test/
--rw-rw-rw-   0        0        0     1542 2023-07-05 14:04:50.000000 timespan-python-0.1.0/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:04:04.700173 timespan-python-0.1.0/timespan_python.egg-info/
--rw-rw-rw-   0        0        0     2190 2023-07-06 08:04:04.000000 timespan-python-0.1.0/timespan_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-06 08:04:04.000000 timespan-python-0.1.0/timespan_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:04:04.000000 timespan-python-0.1.0/timespan_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 08:04:04.000000 timespan-python-0.1.0/timespan_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-07-06 08:04:04.000000 timespan-python-0.1.0/timespan_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.054846 timespan-python-0.1.1/
+-rw-rw-rw-   0        0        0     1162 2023-07-05 13:54:28.000000 timespan-python-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2254 2023-07-06 09:03:34.054846 timespan-python-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2023-07-06 08:43:38.000000 timespan-python-0.1.1/README.md
+-rw-rw-rw-   0        0        0      630 2023-07-06 09:03:34.056568 timespan-python-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-07-06 08:43:38.000000 timespan-python-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.045339 timespan-python-0.1.1/src/
+-rw-rw-rw-   0        0        0        0 2023-07-06 08:43:38.000000 timespan-python-0.1.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.047339 timespan-python-0.1.1/src/package/
+-rw-rw-rw-   0        0        0        0 2023-07-05 14:04:50.000000 timespan-python-0.1.1/src/package/__init__.py
+-rw-rw-rw-   0        0        0     7822 2023-07-06 08:43:38.000000 timespan-python-0.1.1/src/package/timespan.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.047339 timespan-python-0.1.1/test/
+-rw-rw-rw-   0        0        0     1542 2023-07-05 14:04:50.000000 timespan-python-0.1.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.053845 timespan-python-0.1.1/timespan_python.egg-info/
+-rw-rw-rw-   0        0        0     2254 2023-07-06 09:03:34.000000 timespan-python-0.1.1/timespan_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-06 09:03:34.000000 timespan-python-0.1.1/timespan_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 09:03:34.000000 timespan-python-0.1.1/timespan_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 09:03:33.000000 timespan-python-0.1.1/timespan_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2023-07-06 09:03:34.000000 timespan-python-0.1.1/timespan_python.egg-info/top_level.txt
```

### Comparing `timespan-python-0.1.0/LICENSE` & `timespan-python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timespan-python-0.1.0/PKG-INFO` & `timespan-python-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: timespan-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python module for conversion between .NET TimeSpan objects and Python datetime.timedelta objects
+Home-page: https://github.com/microsoft/dotnet-timespan-python
 Author: Mattan Serry
 Author-email: maserry@microsoft.com
 License: MIT License
 Keywords: TimeSpan
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `timespan-python-0.1.0/README.md` & `timespan-python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `timespan-python-0.1.0/setup.cfg` & `timespan-python-0.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 00000150: 6e73 650d 0a63 6c61 7373 6966 6965 7273  nse..classifiers
 00000160: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
 00000170: 7420 5374 6174 7573 203a 3a20 3420 2d20  t Status :: 4 - 
 00000180: 4265 7461 0d0a 0950 726f 6772 616d 6d69  Beta...Programmi
 00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000001a0: 7974 686f 6e20 3a3a 2033 0d0a 0954 6f70  ython :: 3...Top
 000001b0: 6963 203a 3a20 5574 696c 6974 6965 730d  ic :: Utilities.
-000001c0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7a69  ...[options]..zi
-000001d0: 705f 7361 6665 203d 2046 616c 7365 0d0a  p_safe = False..
-000001e0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-000001f0: 6461 7461 203d 2054 7275 650d 0a70 6163  data = True..pac
-00000200: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a0d  kages = find:...
-00000210: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000220: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000230: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+000001c0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+000001d0: 6974 6875 622e 636f 6d2f 6d69 6372 6f73  ithub.com/micros
+000001e0: 6f66 742f 646f 746e 6574 2d74 696d 6573  oft/dotnet-times
+000001f0: 7061 6e2d 7079 7468 6f6e 0d0a 0d0a 5b6f  pan-python....[o
+00000200: 7074 696f 6e73 5d0d 0a7a 6970 5f73 6166  ptions]..zip_saf
+00000210: 6520 3d20 4661 6c73 650d 0a69 6e63 6c75  e = False..inclu
+00000220: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000230: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
+00000240: 203d 2066 696e 643a 0d0a 0d0a 5b65 6767   = find:....[egg
+00000250: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000260: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000270: 2030 0d0a 0d0a                            0....
```

### Comparing `timespan-python-0.1.0/src/package/timespan.py` & `timespan-python-0.1.1/src/package/timespan.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import locale
 import os
 import re
 from functools import partial
 
 __author__ = "Mattan Serry"
 __email__ = "maserry@microsoft.com"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 """
 
 Module to convert between .NET 7.0 TimeSpan objects (with format specifiers) and Python's datetime.timedelta objects.
 
 References:
 https://learn.microsoft.com/en-us/dotnet/api/system.timespan?view=net-7.0
```

### Comparing `timespan-python-0.1.0/test/test.py` & `timespan-python-0.1.1/test/test.py`

 * *Files identical despite different names*

### Comparing `timespan-python-0.1.0/timespan_python.egg-info/PKG-INFO` & `timespan-python-0.1.1/timespan_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: timespan-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python module for conversion between .NET TimeSpan objects and Python datetime.timedelta objects
+Home-page: https://github.com/microsoft/dotnet-timespan-python
 Author: Mattan Serry
 Author-email: maserry@microsoft.com
 License: MIT License
 Keywords: TimeSpan
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

