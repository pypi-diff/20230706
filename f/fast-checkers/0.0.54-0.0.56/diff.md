# Comparing `tmp/fast-checkers-0.0.54.tar.gz` & `tmp/fast-checkers-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-checkers-0.0.54.tar", last modified: Thu Jul  6 13:08:10 2023, max compression
+gzip compressed data, was "fast-checkers-0.0.56.tar", last modified: Thu Jul  6 13:09:36 2023, max compression
```

## Comparing `fast-checkers-0.0.54.tar` & `fast-checkers-0.0.56.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 13:08:10.010141 fast-checkers-0.0.54/
--rw-rw-rw-   0        0        0       17 2023-07-06 12:35:59.000000 fast-checkers-0.0.54/MANIFEST.in
--rw-rw-rw-   0        0        0     4570 2023-07-06 13:08:10.010141 fast-checkers-0.0.54/PKG-INFO
--rw-rw-rw-   0        0        0     4027 2023-07-06 13:00:06.000000 fast-checkers-0.0.54/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 13:08:09.997027 fast-checkers-0.0.54/checkers/
--rw-rw-rw-   0        0        0      889 2023-07-06 11:33:52.000000 fast-checkers-0.0.54/checkers/__init__.py
--rw-rw-rw-   0        0        0     3735 2023-07-06 12:28:19.000000 fast-checkers-0.0.54/checkers/american.py
--rw-rw-rw-   0        0        0     5062 2023-07-06 12:21:56.000000 fast-checkers-0.0.54/checkers/base.py
--rw-rw-rw-   0        0        0     1147 2023-07-06 11:33:52.000000 fast-checkers-0.0.54/checkers/main.py
--rw-rw-rw-   0        0        0     3838 2023-07-06 12:21:42.000000 fast-checkers-0.0.54/checkers/models.py
--rw-rw-rw-   0        0        0       65 2023-06-18 11:52:25.000000 fast-checkers-0.0.54/checkers/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:08:10.007146 fast-checkers-0.0.54/fast_checkers.egg-info/
--rw-rw-rw-   0        0        0     4570 2023-07-06 13:08:09.000000 fast-checkers-0.0.54/fast_checkers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-06 13:08:09.000000 fast-checkers-0.0.54/fast_checkers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 13:08:09.000000 fast-checkers-0.0.54/fast_checkers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 13:08:09.000000 fast-checkers-0.0.54/fast_checkers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 13:08:10.010141 fast-checkers-0.0.54/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-07-06 13:08:05.000000 fast-checkers-0.0.54/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:08:10.008142 fast-checkers-0.0.54/test/
--rw-rw-rw-   0        0        0     2387 2023-07-06 11:33:52.000000 fast-checkers-0.0.54/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:09:36.340021 fast-checkers-0.0.56/
+-rw-rw-rw-   0        0        0       17 2023-07-06 12:35:59.000000 fast-checkers-0.0.56/MANIFEST.in
+-rw-rw-rw-   0        0        0     4570 2023-07-06 13:09:36.340021 fast-checkers-0.0.56/PKG-INFO
+-rw-rw-rw-   0        0        0     4027 2023-07-06 13:00:06.000000 fast-checkers-0.0.56/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 13:09:36.326023 fast-checkers-0.0.56/checkers/
+-rw-rw-rw-   0        0        0      889 2023-07-06 11:33:52.000000 fast-checkers-0.0.56/checkers/__init__.py
+-rw-rw-rw-   0        0        0     3735 2023-07-06 12:28:19.000000 fast-checkers-0.0.56/checkers/american.py
+-rw-rw-rw-   0        0        0     5062 2023-07-06 12:21:56.000000 fast-checkers-0.0.56/checkers/base.py
+-rw-rw-rw-   0        0        0     1147 2023-07-06 11:33:52.000000 fast-checkers-0.0.56/checkers/main.py
+-rw-rw-rw-   0        0        0     3838 2023-07-06 12:21:42.000000 fast-checkers-0.0.56/checkers/models.py
+-rw-rw-rw-   0        0        0       65 2023-06-18 11:52:25.000000 fast-checkers-0.0.56/checkers/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:09:36.335021 fast-checkers-0.0.56/fast_checkers.egg-info/
+-rw-rw-rw-   0        0        0     4570 2023-07-06 13:09:36.000000 fast-checkers-0.0.56/fast_checkers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-06 13:09:36.000000 fast-checkers-0.0.56/fast_checkers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:09:36.000000 fast-checkers-0.0.56/fast_checkers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 13:09:36.000000 fast-checkers-0.0.56/fast_checkers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:09:36.341022 fast-checkers-0.0.56/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-07-06 13:09:27.000000 fast-checkers-0.0.56/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:09:36.338022 fast-checkers-0.0.56/test/
+-rw-rw-rw-   0        0        0     2387 2023-07-06 11:33:52.000000 fast-checkers-0.0.56/test/test_board.py
```

### Comparing `fast-checkers-0.0.54/PKG-INFO` & `fast-checkers-0.0.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.0.54
+Version: 0.0.56
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fast-checkers-0.0.54/README.md` & `fast-checkers-0.0.56/README.md`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.54/checkers/__init__.py` & `fast-checkers-0.0.56/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.54/checkers/american.py` & `fast-checkers-0.0.56/checkers/american.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.54/checkers/base.py` & `fast-checkers-0.0.56/checkers/base.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.54/checkers/main.py` & `fast-checkers-0.0.56/checkers/main.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.54/checkers/models.py` & `fast-checkers-0.0.56/checkers/models.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.54/fast_checkers.egg-info/PKG-INFO` & `fast-checkers-0.0.56/fast_checkers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.0.54
+Version: 0.0.56
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fast-checkers-0.0.54/setup.py` & `fast-checkers-0.0.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "readme.md").read_text()
 
 setuptools.setup(
     name="fast-checkers",
-    version="0.0.54",
+    version="0.0.56",
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     files_to_include=["checkers"],
     description=__doc__.replace("\n", " ").strip(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

### Comparing `fast-checkers-0.0.54/test/test_board.py` & `fast-checkers-0.0.56/test/test_board.py`

 * *Files identical despite different names*

