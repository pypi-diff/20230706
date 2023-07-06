# Comparing `tmp/paraclient-1.36.6.tar.gz` & `tmp/paraclient-1.36.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paraclient-1.36.6.tar", last modified: Tue Oct  5 19:22:52 2021, max compression
+gzip compressed data, was "paraclient-1.36.8.tar", last modified: Thu Jul  6 14:06:42 2023, max compression
```

## Comparing `paraclient-1.36.6.tar` & `paraclient-1.36.8.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2021-10-05 19:22:52.000000 paraclient-1.36.6/
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      972 2021-10-05 19:22:52.000000 paraclient-1.36.6/PKG-INFO
--rw-r--r--   0 alexb     (1000) alexb     (1000)     1613 2019-11-14 15:52:51.000000 paraclient-1.36.6/README.md
-drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2021-10-05 19:22:52.000000 paraclient-1.36.6/paraclient/
--rw-rw-r--   0 alexb     (1000) alexb     (1000)        0 2019-11-14 12:33:37.000000 paraclient-1.36.6/paraclient/__init__.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     2045 2021-02-07 09:10:47.000000 paraclient-1.36.6/paraclient/auth.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     2814 2021-02-07 09:10:47.000000 paraclient-1.36.6/paraclient/constraint.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     1326 2021-06-11 19:39:01.000000 paraclient-1.36.6/paraclient/pager.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)    47430 2021-10-05 19:22:22.000000 paraclient-1.36.6/paraclient/paraclient.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     2050 2021-10-03 12:27:07.000000 paraclient-1.36.6/paraclient/paraobject.py
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      101 2021-10-05 19:22:48.000000 paraclient-1.36.6/paraclient/version.py
-drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2021-10-05 19:22:52.000000 paraclient-1.36.6/paraclient.egg-info/
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      972 2021-10-05 19:22:52.000000 paraclient-1.36.6/paraclient.egg-info/PKG-INFO
--rw-rw-r--   0 alexb     (1000) alexb     (1000)      313 2021-10-05 19:22:52.000000 paraclient-1.36.6/paraclient.egg-info/SOURCES.txt
--rw-rw-r--   0 alexb     (1000) alexb     (1000)        1 2021-10-05 19:22:52.000000 paraclient-1.36.6/paraclient.egg-info/dependency_links.txt
--rw-rw-r--   0 alexb     (1000) alexb     (1000)       11 2021-10-05 19:22:52.000000 paraclient-1.36.6/paraclient.egg-info/top_level.txt
--rw-rw-r--   0 alexb     (1000) alexb     (1000)       38 2021-10-05 19:22:52.000000 paraclient-1.36.6/setup.cfg
--rw-rw-r--   0 alexb     (1000) alexb     (1000)     3513 2020-02-24 22:03:01.000000 paraclient-1.36.6/setup.py
+drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2023-07-06 14:06:42.472936 paraclient-1.36.8/
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)    11363 2023-07-06 14:02:43.000000 paraclient-1.36.8/LICENSE
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)      964 2023-07-06 14:06:42.472936 paraclient-1.36.8/PKG-INFO
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)     1613 2019-11-14 15:52:51.000000 paraclient-1.36.8/README.md
+drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2023-07-06 14:06:42.472936 paraclient-1.36.8/paraclient/
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)      782 2023-07-06 14:02:43.000000 paraclient-1.36.8/paraclient/__init__.py
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)     2045 2023-07-06 14:02:43.000000 paraclient-1.36.8/paraclient/auth.py
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)     2814 2023-07-06 14:02:43.000000 paraclient-1.36.8/paraclient/constraint.py
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)     1326 2023-07-06 14:02:43.000000 paraclient-1.36.8/paraclient/pager.py
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)    47430 2023-07-06 14:02:43.000000 paraclient-1.36.8/paraclient/paraclient.py
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)     2050 2023-07-06 14:02:43.000000 paraclient-1.36.8/paraclient/paraobject.py
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)      101 2023-07-06 14:06:34.000000 paraclient-1.36.8/paraclient/version.py
+drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2023-07-06 14:06:42.472936 paraclient-1.36.8/paraclient.egg-info/
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)      964 2023-07-06 14:06:42.000000 paraclient-1.36.8/paraclient.egg-info/PKG-INFO
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)      371 2023-07-06 14:06:42.000000 paraclient-1.36.8/paraclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)        1 2023-07-06 14:06:42.000000 paraclient-1.36.8/paraclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)       11 2023-07-06 14:06:42.000000 paraclient-1.36.8/paraclient.egg-info/top_level.txt
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)       38 2023-07-06 14:06:42.472936 paraclient-1.36.8/setup.cfg
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)     3513 2020-02-24 22:03:01.000000 paraclient-1.36.8/setup.py
+drwxrwxr-x   0 alexb     (1000) alexb     (1000)        0 2023-07-06 14:06:42.472936 paraclient-1.36.8/tests/
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)    19888 2020-02-24 21:36:45.000000 paraclient-1.36.8/tests/test_paraclient.py
+-rw-rw-r--   0 alexb     (1000) alexb     (1000)      885 2020-02-24 21:06:17.000000 paraclient-1.36.8/tests/test_paraobject.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `paraclient-1.36.6/PKG-INFO` & `paraclient-1.36.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: paraclient
-Version: 1.36.6
+Version: 1.36.8
 Summary: Python client for Para
 Home-page: https://github.com/Erudika/para-client-python
 Author: Alexander Bogdanovski
 Author-email: alex@erudika.com
 License: Apache 2.0
-Description: **Para** was designed as a simple and modular backend framework for object persistence and retrieval. It helps you build applications faster by taking care of the backend. It works on three levels - objects are stored in a NoSQL data store or any old relational database, then automatically indexed by a search engine and finally, cached. This is the Python client for Para.
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+**Para** was designed as a simple and modular backend framework for object persistence and retrieval. It helps you build applications faster by taking care of the backend. It works on three levels - objects are stored in a NoSQL data store or any old relational database, then automatically indexed by a search engine and finally, cached. This is the Python client for Para.
```

### Comparing `paraclient-1.36.6/README.md` & `paraclient-1.36.8/README.md`

 * *Files identical despite different names*

### Comparing `paraclient-1.36.6/paraclient/auth.py` & `paraclient-1.36.8/paraclient/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- * Copyright 2013-2021 Erudika. https://erudika.com
+ * Copyright 2013-2023 Erudika. https://erudika.com
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *      http://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `paraclient-1.36.6/paraclient/constraint.py` & `paraclient-1.36.8/paraclient/constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- * Copyright 2013-2021 Erudika. https://erudika.com
+ * Copyright 2013-2023 Erudika. https://erudika.com
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *      http://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `paraclient-1.36.6/paraclient/pager.py` & `paraclient-1.36.8/paraclient/pager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- * Copyright 2013-2021 Erudika. https://erudika.com
+ * Copyright 2013-2023 Erudika. https://erudika.com
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *      http://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `paraclient-1.36.6/paraclient/paraclient.py` & `paraclient-1.36.8/paraclient/paraclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- * Copyright 2013-2021 Erudika. https://erudika.com
+ * Copyright 2013-2023 Erudika. https://erudika.com
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *      http://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `paraclient-1.36.6/paraclient/paraobject.py` & `paraclient-1.36.8/paraclient/paraobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- * Copyright 2013-2021 Erudika. https://erudika.com
+ * Copyright 2013-2023 Erudika. https://erudika.com
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *      http://www.apache.org/licenses/LICENSE-2.0
  *
```

### Comparing `paraclient-1.36.6/paraclient.egg-info/PKG-INFO` & `paraclient-1.36.8/paraclient.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: paraclient
-Version: 1.36.6
+Version: 1.36.8
 Summary: Python client for Para
 Home-page: https://github.com/Erudika/para-client-python
 Author: Alexander Bogdanovski
 Author-email: alex@erudika.com
 License: Apache 2.0
-Description: **Para** was designed as a simple and modular backend framework for object persistence and retrieval. It helps you build applications faster by taking care of the backend. It works on three levels - objects are stored in a NoSQL data store or any old relational database, then automatically indexed by a search engine and finally, cached. This is the Python client for Para.
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+**Para** was designed as a simple and modular backend framework for object persistence and retrieval. It helps you build applications faster by taking care of the backend. It works on three levels - objects are stored in a NoSQL data store or any old relational database, then automatically indexed by a search engine and finally, cached. This is the Python client for Para.
```

### Comparing `paraclient-1.36.6/setup.py` & `paraclient-1.36.8/setup.py`

 * *Files identical despite different names*

