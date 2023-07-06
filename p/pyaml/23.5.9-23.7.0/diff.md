# Comparing `tmp/pyaml-23.5.9.tar.gz` & `tmp/pyaml-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaml-23.5.9.tar", last modified: Thu May 11 09:29:24 2023, max compression
+gzip compressed data, was "pyaml-23.7.0.tar", last modified: Thu Jul  6 06:26:00 2023, max compression
```

## Comparing `pyaml-23.5.9.tar` & `pyaml-23.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-11 09:29:24.741461 pyaml-23.5.9/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.5.9/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.5.9/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9777 2023-05-11 09:29:24.741461 pyaml-23.5.9/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9028 2023-05-11 09:26:12.000000 pyaml-23.5.9/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-11 09:29:24.740461 pyaml-23.5.9/pyaml/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8977 2023-05-06 07:43:09.000000 pyaml-23.5.9/pyaml/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.5.9/pyaml/__main__.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-11 09:29:24.741461 pyaml-23.5.9/pyaml/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.5.9/pyaml/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17672 2023-05-06 07:43:17.000000 pyaml-23.5.9/pyaml/tests/test_dump.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-11 09:29:24.741461 pyaml-23.5.9/pyaml.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9777 2023-05-11 09:29:24.000000 pyaml-23.5.9/pyaml.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-05-11 09:29:24.000000 pyaml-23.5.9/pyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-11 09:29:24.000000 pyaml-23.5.9/pyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-05-11 09:29:24.000000 pyaml-23.5.9/pyaml.egg-info/requires.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-05-11 09:29:24.000000 pyaml-23.5.9/pyaml.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      829 2023-05-11 09:28:10.000000 pyaml-23.5.9/pyproject.toml
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-05-11 09:29:24.741461 pyaml-23.5.9/setup.cfg
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       96 2023-05-05 00:23:33.000000 pyaml-23.5.9/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-07-06 06:26:00.007076 pyaml-23.7.0/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.7.0/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.7.0/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9908 2023-07-06 06:26:00.007076 pyaml-23.7.0/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9028 2023-05-11 09:26:12.000000 pyaml-23.7.0/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-07-06 06:26:00.007076 pyaml-23.7.0/pyaml/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8977 2023-05-06 07:43:09.000000 pyaml-23.7.0/pyaml/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.7.0/pyaml/__main__.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-07-06 06:26:00.007076 pyaml-23.7.0/pyaml/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.7.0/pyaml/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17672 2023-05-06 07:43:17.000000 pyaml-23.7.0/pyaml/tests/test_dump.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-07-06 06:26:00.007076 pyaml-23.7.0/pyaml.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9908 2023-07-06 06:26:00.000000 pyaml-23.7.0/pyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-07-06 06:26:00.000000 pyaml-23.7.0/pyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-07-06 06:26:00.000000 pyaml-23.7.0/pyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-07-06 06:26:00.000000 pyaml-23.7.0/pyaml.egg-info/requires.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-07-06 06:26:00.000000 pyaml-23.7.0/pyaml.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      895 2023-07-06 06:20:15.000000 pyaml-23.7.0/pyproject.toml
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-07-06 06:26:00.007076 pyaml-23.7.0/setup.cfg
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1193 2023-07-06 06:21:28.000000 pyaml-23.7.0/setup.py
```

### Comparing `pyaml-23.5.9/PKG-INFO` & `pyaml-23.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.5.9
+Version: 23.7.0
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
+Home-page: https://github.com/mk-fg/pretty-yaml
+Author: Mike Kazantsev
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
+Project-URL: Homepage, https://github.com/mk-fg/pretty-yaml
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
```

### Comparing `pyaml-23.5.9/README.rst` & `pyaml-23.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.9/pyaml/__init__.py` & `pyaml-23.7.0/pyaml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.9/pyaml/__main__.py` & `pyaml-23.7.0/pyaml/__main__.py`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.9/pyaml/tests/test_dump.py` & `pyaml-23.7.0/pyaml/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pyaml-23.5.9/pyaml.egg-info/PKG-INFO` & `pyaml-23.7.0/pyaml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.5.9
+Version: 23.7.0
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
+Home-page: https://github.com/mk-fg/pretty-yaml
+Author: Mike Kazantsev
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
+Project-URL: Homepage, https://github.com/mk-fg/pretty-yaml
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
```

### Comparing `pyaml-23.5.9/pyproject.toml` & `pyaml-23.7.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pyaml"
-version = "23.5.9"
+version = "23.7.0"
 
 description = "PyYAML-based module to produce a bit more pretty and readable YAML-serialized data"
 authors = [{name="Mike Kazantsev", email="mk.fraggod@gmail.com"}]
 license = {text="WTFPL"}
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
@@ -17,12 +17,15 @@
 	"Topic :: Utilities" ]
 keywords = ["yaml", "serialization", "pretty-print", "formatter", "human", "readability"]
 
 requires-python = ">=3.8"
 dependencies = ["PyYAML"]
 dynamic = ["readme"]
 
+[project.urls]
+Homepage = "https://github.com/mk-fg/pretty-yaml"
+
 [tool.setuptools.dynamic]
 readme = {file="README.rst"}
 
 [project.optional-dependencies]
 anchors = ["unidecode"]
```

