# Comparing `tmp/timespan-python-0.1.1.tar.gz` & `tmp/timespan-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timespan-python-0.1.1.tar", last modified: Thu Jul  6 09:03:34 2023, max compression
+gzip compressed data, was "timespan-python-0.1.2.tar", last modified: Thu Jul  6 13:13:18 2023, max compression
```

## Comparing `timespan-python-0.1.1.tar` & `timespan-python-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.054846 timespan-python-0.1.1/
--rw-rw-rw-   0        0        0     1162 2023-07-05 13:54:28.000000 timespan-python-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2254 2023-07-06 09:03:34.054846 timespan-python-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2023-07-06 08:43:38.000000 timespan-python-0.1.1/README.md
--rw-rw-rw-   0        0        0      630 2023-07-06 09:03:34.056568 timespan-python-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-07-06 08:43:38.000000 timespan-python-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.045339 timespan-python-0.1.1/src/
--rw-rw-rw-   0        0        0        0 2023-07-06 08:43:38.000000 timespan-python-0.1.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.047339 timespan-python-0.1.1/src/package/
--rw-rw-rw-   0        0        0        0 2023-07-05 14:04:50.000000 timespan-python-0.1.1/src/package/__init__.py
--rw-rw-rw-   0        0        0     7822 2023-07-06 08:43:38.000000 timespan-python-0.1.1/src/package/timespan.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.047339 timespan-python-0.1.1/test/
--rw-rw-rw-   0        0        0     1542 2023-07-05 14:04:50.000000 timespan-python-0.1.1/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:03:34.053845 timespan-python-0.1.1/timespan_python.egg-info/
--rw-rw-rw-   0        0        0     2254 2023-07-06 09:03:34.000000 timespan-python-0.1.1/timespan_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-06 09:03:34.000000 timespan-python-0.1.1/timespan_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 09:03:34.000000 timespan-python-0.1.1/timespan_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 09:03:33.000000 timespan-python-0.1.1/timespan_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-07-06 09:03:34.000000 timespan-python-0.1.1/timespan_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 13:13:18.485697 timespan-python-0.1.2/
+-rw-rw-rw-   0        0        0      550 2023-07-06 13:13:18.485697 timespan-python-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-06 12:52:51.000000 timespan-python-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-07-06 13:13:18.491701 timespan-python-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 13:13:18.471850 timespan-python-0.1.2/timespan/
+-rw-rw-rw-   0        0        0      116 2023-07-06 13:12:26.000000 timespan-python-0.1.2/timespan/__init__.py
+-rw-rw-rw-   0        0        0     7735 2023-07-06 12:45:29.000000 timespan-python-0.1.2/timespan/timespan.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:13:18.485697 timespan-python-0.1.2/timespan_python.egg-info/
+-rw-rw-rw-   0        0        0      550 2023-07-06 13:13:18.000000 timespan-python-0.1.2/timespan_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-07-06 13:13:18.000000 timespan-python-0.1.2/timespan_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:13:18.000000 timespan-python-0.1.2/timespan_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 13:13:18.000000 timespan-python-0.1.2/timespan_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-06 13:13:18.000000 timespan-python-0.1.2/timespan_python.egg-info/top_level.txt
```

### Comparing `timespan-python-0.1.1/setup.cfg` & `timespan-python-0.1.2/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 696d 6573 7061 6e2d 7079 7468   = timespan-pyth
 00000020: 6f6e 0d0a 7665 7273 696f 6e20 3d20 6174  on..version = at
-00000030: 7472 3a20 7372 632e 7061 636b 6167 652e  tr: src.package.
-00000040: 7469 6d65 7370 616e 2e5f 5f76 6572 7369  timespan.__versi
-00000050: 6f6e 5f5f 0d0a 6175 7468 6f72 203d 204d  on__..author = M
-00000060: 6174 7461 6e20 5365 7272 790d 0a61 7574  attan Serry..aut
-00000070: 686f 725f 656d 6169 6c20 3d20 6d61 7365  hor_email = mase
-00000080: 7272 7940 6d69 6372 6f73 6f66 742e 636f  rry@microsoft.co
-00000090: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
-000000a0: 2041 2050 7974 686f 6e20 6d6f 6475 6c65   A Python module
-000000b0: 2066 6f72 2063 6f6e 7665 7273 696f 6e20   for conversion 
-000000c0: 6265 7477 6565 6e20 2e4e 4554 2054 696d  between .NET Tim
-000000d0: 6553 7061 6e20 6f62 6a65 6374 7320 616e  eSpan objects an
-000000e0: 6420 5079 7468 6f6e 2064 6174 6574 696d  d Python datetim
-000000f0: 652e 7469 6d65 6465 6c74 6120 6f62 6a65  e.timedelta obje
-00000100: 6374 730d 0a6c 6f6e 675f 6465 7363 7269  cts..long_descri
-00000110: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-00000120: 4144 4d45 2e6d 640d 0a6b 6579 776f 7264  ADME.md..keyword
-00000130: 7320 3d20 5469 6d65 5370 616e 0d0a 6c69  s = TimeSpan..li
-00000140: 6365 6e73 6520 3d20 4d49 5420 4c69 6365  cense = MIT Lice
-00000150: 6e73 650d 0a63 6c61 7373 6966 6965 7273  nse..classifiers
-00000160: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
-00000170: 7420 5374 6174 7573 203a 3a20 3420 2d20  t Status :: 4 - 
-00000180: 4265 7461 0d0a 0950 726f 6772 616d 6d69  Beta...Programmi
-00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001a0: 7974 686f 6e20 3a3a 2033 0d0a 0954 6f70  ython :: 3...Top
-000001b0: 6963 203a 3a20 5574 696c 6974 6965 730d  ic :: Utilities.
-000001c0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
-000001d0: 6974 6875 622e 636f 6d2f 6d69 6372 6f73  ithub.com/micros
-000001e0: 6f66 742f 646f 746e 6574 2d74 696d 6573  oft/dotnet-times
-000001f0: 7061 6e2d 7079 7468 6f6e 0d0a 0d0a 5b6f  pan-python....[o
-00000200: 7074 696f 6e73 5d0d 0a7a 6970 5f73 6166  ptions]..zip_saf
-00000210: 6520 3d20 4661 6c73 650d 0a69 6e63 6c75  e = False..inclu
-00000220: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-00000230: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
-00000240: 203d 2066 696e 643a 0d0a 0d0a 5b65 6767   = find:....[egg
-00000250: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000260: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000270: 2030 0d0a 0d0a                            0....
+00000030: 7472 3a20 7469 6d65 7370 616e 2e5f 5f76  tr: timespan.__v
+00000040: 6572 7369 6f6e 5f5f 0d0a 6175 7468 6f72  ersion__..author
+00000050: 203d 204d 6174 7461 6e20 5365 7272 790d   = Mattan Serry.
+00000060: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000070: 6d61 7365 7272 7940 6d69 6372 6f73 6f66  maserry@microsof
+00000080: 742e 636f 6d0d 0a64 6573 6372 6970 7469  t.com..descripti
+00000090: 6f6e 203d 2041 2050 7974 686f 6e20 6d6f  on = A Python mo
+000000a0: 6475 6c65 2066 6f72 2063 6f6e 7665 7273  dule for convers
+000000b0: 696f 6e20 6265 7477 6565 6e20 2e4e 4554  ion between .NET
+000000c0: 2054 696d 6553 7061 6e20 6f62 6a65 6374   TimeSpan object
+000000d0: 7320 616e 6420 5079 7468 6f6e 2064 6174  s and Python dat
+000000e0: 6574 696d 652e 7469 6d65 6465 6c74 6120  etime.timedelta 
+000000f0: 6f62 6a65 6374 730d 0a6c 6f6e 675f 6465  objects..long_de
+00000100: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+00000110: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+00000120: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+00000130: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+00000140: 742f 6d61 726b 646f 776e 0d0a 6b65 7977  t/markdown..keyw
+00000150: 6f72 6473 203d 2054 696d 6553 7061 6e0d  ords = TimeSpan.
+00000160: 0a6c 6963 656e 7365 203d 204d 4954 204c  .license = MIT L
+00000170: 6963 656e 7365 0d0a 636c 6173 7369 6669  icense..classifi
+00000180: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
+00000190: 6d65 6e74 2053 7461 7475 7320 3a3a 2034  ment Status :: 4
+000001a0: 202d 2042 6574 610d 0a09 5072 6f67 7261   - Beta...Progra
+000001b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001c0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
+000001d0: 546f 7069 6320 3a3a 2055 7469 6c69 7469  Topic :: Utiliti
+000001e0: 6573 0d0a 094f 7065 7261 7469 6e67 2053  es...Operating S
+000001f0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000200: 7065 6e64 656e 740d 0a75 726c 203d 2068  pendent..url = h
+00000210: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000220: 6d2f 6d69 6372 6f73 6f66 742f 646f 746e  m/microsoft/dotn
+00000230: 6574 2d74 696d 6573 7061 6e2d 7079 7468  et-timespan-pyth
+00000240: 6f6e 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  on....[options].
+00000250: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
+00000260: 650d 0a69 6e63 6c75 6465 5f70 6163 6b61  e..include_packa
+00000270: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
+00000280: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+00000290: 093d 202e 0d0a 7061 636b 6167 6573 203d  .= ...packages =
+000002a0: 2066 696e 643a 0d0a 0d0a 5b65 6767 5f69   find:....[egg_i
+000002b0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000002c0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000002d0: 0d0a 0d0a                                ....
```

### Comparing `timespan-python-0.1.1/src/package/timespan.py` & `timespan-python-0.1.2/timespan/timespan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import datetime
 import locale
 import os
 import re
 from functools import partial
 
-__author__ = "Mattan Serry"
-__email__ = "maserry@microsoft.com"
-__version__ = "0.1.1"
+
 
 """
 
 Module to convert between .NET 7.0 TimeSpan objects (with format specifiers) and Python's datetime.timedelta objects.
 
 References:
 https://learn.microsoft.com/en-us/dotnet/api/system.timespan?view=net-7.0
```

