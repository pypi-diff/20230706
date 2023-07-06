# Comparing `tmp/tkintertoy-1.5.0.tar.gz` & `tmp/tkintertoy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertoy-1.5.0.tar", last modified: Sat Jun 10 18:15:05 2023, max compression
+gzip compressed data, was "tkintertoy-1.6.0.tar", last modified: Thu Jul  6 16:58:02 2023, max compression
```

## Comparing `tkintertoy-1.5.0.tar` & `tkintertoy-1.6.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/
--rw-rw-rw-   0        0        0     1080 2020-01-12 00:42:26.000000 tkintertoy-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     2522 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2023-05-08 23:33:42.000000 tkintertoy-1.5.0/README.md
--rw-rw-rw-   0        0        0      857 2023-06-10 18:06:12.000000 tkintertoy-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 18:15:05.926439 tkintertoy-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/src/tkintertoy/
--rw-rw-rw-   0        0        0  2190126 2019-07-15 23:19:56.000000 tkintertoy-1.5.0/src/tkintertoy/Shipman_tkinter8_5.pdf
--rw-rw-rw-   0        0        0       32 2019-02-19 20:11:06.000000 tkintertoy-1.5.0/src/tkintertoy/__init__.py
--rw-rw-rw-   0        0        0    73560 2023-06-04 18:20:58.000000 tkintertoy-1.5.0/src/tkintertoy/tt.py
--rw-rw-rw-   0        0        0    13129 2023-06-04 02:15:07.000000 tkintertoy-1.5.0/src/tkintertoy/ttgallery.py
-drwxrwxrwx   0        0        0        0 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/src/tkintertoy.egg-info/
--rw-rw-rw-   0        0        0     2522 2023-06-10 18:15:05.000000 tkintertoy-1.5.0/src/tkintertoy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-10 18:15:05.000000 tkintertoy-1.5.0/src/tkintertoy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 18:15:05.000000 tkintertoy-1.5.0/src/tkintertoy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-10 18:15:05.000000 tkintertoy-1.5.0/src/tkintertoy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 16:58:02.729923 tkintertoy-1.6.0/
+-rw-rw-rw-   0        0        0     1080 2020-01-12 00:42:26.000000 tkintertoy-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2522 2023-07-06 16:58:02.729923 tkintertoy-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2023-05-08 23:33:42.000000 tkintertoy-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 16:58:02.714297 tkintertoy-1.6.0/dist/
+-rw-rw-rw-   0        0        0  1603093 2023-07-06 16:56:26.000000 tkintertoy-1.6.0/dist/tkintertoy-1.5.0-py3-none-any.whl
+-rw-rw-rw-   0        0        0  4802896 2023-07-06 16:56:19.000000 tkintertoy-1.6.0/dist/tkintertoy-1.5.0.tar.gz
+-rw-rw-rw-   0        0        0      857 2023-07-06 16:57:24.000000 tkintertoy-1.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 16:58:02.729923 tkintertoy-1.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 16:58:02.698668 tkintertoy-1.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 16:58:02.729923 tkintertoy-1.6.0/src/tkintertoy/
+-rw-rw-rw-   0        0        0  2190126 2019-07-15 23:19:56.000000 tkintertoy-1.6.0/src/tkintertoy/Shipman_tkinter8_5.pdf
+-rw-rw-rw-   0        0        0       32 2019-02-19 20:11:06.000000 tkintertoy-1.6.0/src/tkintertoy/__init__.py
+-rw-rw-rw-   0        0        0    73560 2023-06-04 18:20:58.000000 tkintertoy-1.6.0/src/tkintertoy/tt.py
+-rw-rw-rw-   0        0        0    13129 2023-06-04 02:15:07.000000 tkintertoy-1.6.0/src/tkintertoy/ttgallery.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:58:02.729923 tkintertoy-1.6.0/src/tkintertoy.egg-info/
+-rw-rw-rw-   0        0        0     2522 2023-07-06 16:58:02.000000 tkintertoy-1.6.0/src/tkintertoy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-06 16:58:02.000000 tkintertoy-1.6.0/src/tkintertoy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 16:58:02.000000 tkintertoy-1.6.0/src/tkintertoy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 16:58:02.000000 tkintertoy-1.6.0/src/tkintertoy.egg-info/top_level.txt
```

### Comparing `tkintertoy-1.5.0/LICENSE` & `tkintertoy-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkintertoy-1.5.0/PKG-INFO` & `tkintertoy-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertoy
-Version: 1.5.0
+Version: 1.6.0
 Summary: A simple GUI package based on Tkinter
 Author-email: Mike Callahan <mcalla@twc.com>
 Project-URL: Homepage, https://github.com/mcalla314/tkintertoy
 Project-URL: Documentation, https://tkintertoy.readthedocs.io
 Keywords: GUI,novice
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tkintertoy-1.5.0/README.md` & `tkintertoy-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tkintertoy-1.5.0/pyproject.toml` & `tkintertoy-1.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tkintertoy"
-version = "1.5.0"
+version = "1.6.0"
 authors = [
     { name="Mike Callahan", email="mcalla@twc.com"},
 ]
 description = "A simple GUI package based on Tkinter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers=[
```

### Comparing `tkintertoy-1.5.0/src/tkintertoy/Shipman_tkinter8_5.pdf` & `tkintertoy-1.6.0/src/tkintertoy/Shipman_tkinter8_5.pdf`

 * *Files identical despite different names*

### Comparing `tkintertoy-1.5.0/src/tkintertoy/tt.py` & `tkintertoy-1.6.0/src/tkintertoy/tt.py`

 * *Files identical despite different names*

### Comparing `tkintertoy-1.5.0/src/tkintertoy/ttgallery.py` & `tkintertoy-1.6.0/src/tkintertoy/ttgallery.py`

 * *Files identical despite different names*

### Comparing `tkintertoy-1.5.0/src/tkintertoy.egg-info/PKG-INFO` & `tkintertoy-1.6.0/src/tkintertoy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertoy
-Version: 1.5.0
+Version: 1.6.0
 Summary: A simple GUI package based on Tkinter
 Author-email: Mike Callahan <mcalla@twc.com>
 Project-URL: Homepage, https://github.com/mcalla314/tkintertoy
 Project-URL: Documentation, https://tkintertoy.readthedocs.io
 Keywords: GUI,novice
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
```

