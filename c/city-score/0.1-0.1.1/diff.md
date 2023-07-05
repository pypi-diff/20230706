# Comparing `tmp/city_score-0.1.tar.gz` & `tmp/city_score-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "city_score-0.1.tar", last modified: Tue Jul  4 21:02:56 2023, max compression
+gzip compressed data, was "city_score-0.1.1.tar", last modified: Wed Jul  5 21:33:57 2023, max compression
```

## Comparing `city_score-0.1.tar` & `city_score-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-04 21:02:56.145399 city_score-0.1/
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1071 2023-07-04 20:59:48.000000 city_score-0.1/LICENSE
--rw-r--r--   0 jacobbudin   (501) staff       (20)     5152 2023-07-04 21:02:56.145281 city_score-0.1/PKG-INFO
--rw-r--r--   0 jacobbudin   (501) staff       (20)     3040 2023-07-04 20:59:48.000000 city_score-0.1/README.md
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1128 2023-07-04 20:59:48.000000 city_score-0.1/pyproject.toml
--rw-r--r--   0 jacobbudin   (501) staff       (20)       38 2023-07-04 21:02:56.145433 city_score-0.1/setup.cfg
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-04 21:02:56.142423 city_score-0.1/src/
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-04 21:02:56.143862 city_score-0.1/src/city_score/
--rw-r--r--   0 jacobbudin   (501) staff       (20)       27 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/__init__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)       20 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/__version__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1683 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/app.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      155 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/cache.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1739 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/city.py
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-04 21:02:56.144455 city_score-0.1/src/city_score/city_score.egg-info/
--rw-r--r--   0 jacobbudin   (501) staff       (20)     5152 2023-07-04 21:02:56.000000 city_score-0.1/src/city_score/city_score.egg-info/PKG-INFO
--rw-r--r--   0 jacobbudin   (501) staff       (20)      688 2023-07-04 21:02:56.000000 city_score-0.1/src/city_score/city_score.egg-info/SOURCES.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)        1 2023-07-04 21:02:56.000000 city_score-0.1/src/city_score/city_score.egg-info/dependency_links.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)       75 2023-07-04 21:02:56.000000 city_score-0.1/src/city_score/city_score.egg-info/requires.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)       71 2023-07-04 21:02:56.000000 city_score-0.1/src/city_score/city_score.egg-info/top_level.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1478 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/decorators.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2663 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/printers.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1499 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/source.py
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-04 21:02:56.145124 city_score-0.1/src/city_score/sources/
--rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/sources/__init__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1108 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/sources/core.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1509 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/sources/peopleforbikes.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2786 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/sources/snowpak.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1269 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/sources/yelp.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2048 2023-07-04 20:59:48.000000 city_score-0.1/src/city_score/sources/zillow.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.294854 city_score-0.1.1/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1071 2023-07-04 20:59:48.000000 city_score-0.1.1/LICENSE
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     5154 2023-07-05 21:33:57.294729 city_score-0.1.1/PKG-INFO
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     3040 2023-07-04 20:59:48.000000 city_score-0.1.1/README.md
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1217 2023-07-05 21:19:40.000000 city_score-0.1.1/pyproject.toml
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       38 2023-07-05 21:33:57.294890 city_score-0.1.1/setup.cfg
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.291664 city_score-0.1.1/src/
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.293224 city_score-0.1.1/src/city_score/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       27 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/__init__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       22 2023-07-05 21:33:46.000000 city_score-0.1.1/src/city_score/__version__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1683 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/app.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      155 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/cache.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1739 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/city.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1478 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/decorators.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     2663 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/printers.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1499 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/source.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.294551 city_score-0.1.1/src/city_score/sources/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/__init__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1108 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/core.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1509 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/peopleforbikes.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     2786 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/snowpak.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1269 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/yelp.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     2048 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/zillow.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.293801 city_score-0.1.1/src/city_score.egg-info/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     5154 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/PKG-INFO
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      633 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        1 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       75 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/requires.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       11 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/top_level.txt
```

### Comparing `city_score-0.1/LICENSE` & `city_score-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `city_score-0.1/PKG-INFO` & `city_score-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: city_score
-Version: 0.1
+Version: 0.1.1
 Summary: A command-line application for scoring US cities and towns.
 Maintainer-email: Jacob Budin <self@jacobbudin.com>
 License: The MIT License
         
         Copyright (c) 2023 Jacob Budin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: city_score Version: 0.1 Summary: A command-line
+Metadata-Version: 2.1 Name: city_score Version: 0.1.1 Summary: A command-line
 application for scoring US cities and towns. Maintainer-email: Jacob Budin
 jacobbudin.com> License: The MIT License Copyright (c) 2023 Jacob Budin
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `city_score-0.1/README.md` & `city_score-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `city_score-0.1/pyproject.toml` & `city_score-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
 [project]
 name = "city_score"
 description = "A command-line application for scoring US cities and towns."
 readme = "README.md"
 keywords = ["cli", "geography", "reading", "epub", "instapaper"]
 license = {file = "LICENSE"}
 maintainers = [{name = "Jacob Budin", email = "self@jacobbudin.com"}]
@@ -26,11 +30,11 @@
     "requests>=2.31.0",
     "rich>=13.4.2",
     "yelpapi>=2.5.0",
 ]
 dynamic = ["version"]
 
 [tool.setuptools]
-package-dir = {"" = "src/city_score"}
+package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
-version = {attr = "__version__.__version__"}
+version = {attr = "city_score.__version__.__version__"}
```

### Comparing `city_score-0.1/src/city_score/app.py` & `city_score-0.1.1/src/city_score/app.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/city.py` & `city_score-0.1.1/src/city_score/city.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/city_score.egg-info/PKG-INFO` & `city_score-0.1.1/src/city_score.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: city-score
-Version: 0.1
+Version: 0.1.1
 Summary: A command-line application for scoring US cities and towns.
 Maintainer-email: Jacob Budin <self@jacobbudin.com>
 License: The MIT License
         
         Copyright (c) 2023 Jacob Budin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: city-score Version: 0.1 Summary: A command-line
+Metadata-Version: 2.1 Name: city-score Version: 0.1.1 Summary: A command-line
 application for scoring US cities and towns. Maintainer-email: Jacob Budin
 jacobbudin.com> License: The MIT License Copyright (c) 2023 Jacob Budin
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `city_score-0.1/src/city_score/city_score.egg-info/SOURCES.txt` & `city_score-0.1.1/src/city_score.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 src/city_score/__version__.py
 src/city_score/app.py
 src/city_score/cache.py
 src/city_score/city.py
 src/city_score/decorators.py
 src/city_score/printers.py
 src/city_score/source.py
-src/city_score/city_score.egg-info/PKG-INFO
-src/city_score/city_score.egg-info/SOURCES.txt
-src/city_score/city_score.egg-info/dependency_links.txt
-src/city_score/city_score.egg-info/requires.txt
-src/city_score/city_score.egg-info/top_level.txt
+src/city_score.egg-info/PKG-INFO
+src/city_score.egg-info/SOURCES.txt
+src/city_score.egg-info/dependency_links.txt
+src/city_score.egg-info/requires.txt
+src/city_score.egg-info/top_level.txt
 src/city_score/sources/__init__.py
 src/city_score/sources/core.py
 src/city_score/sources/peopleforbikes.py
 src/city_score/sources/snowpak.py
 src/city_score/sources/yelp.py
 src/city_score/sources/zillow.py
```

### Comparing `city_score-0.1/src/city_score/decorators.py` & `city_score-0.1.1/src/city_score/decorators.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/printers.py` & `city_score-0.1.1/src/city_score/printers.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/source.py` & `city_score-0.1.1/src/city_score/source.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/sources/core.py` & `city_score-0.1.1/src/city_score/sources/core.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/sources/peopleforbikes.py` & `city_score-0.1.1/src/city_score/sources/peopleforbikes.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/sources/snowpak.py` & `city_score-0.1.1/src/city_score/sources/snowpak.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/sources/yelp.py` & `city_score-0.1.1/src/city_score/sources/yelp.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1/src/city_score/sources/zillow.py` & `city_score-0.1.1/src/city_score/sources/zillow.py`

 * *Files identical despite different names*

