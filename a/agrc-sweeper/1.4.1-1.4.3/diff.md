# Comparing `tmp/agrc-sweeper-1.4.1.tar.gz` & `tmp/agrc-sweeper-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agrc-sweeper-1.4.1.tar", last modified: Thu Jul  6 19:50:45 2023, max compression
+gzip compressed data, was "agrc-sweeper-1.4.3.tar", last modified: Thu Jul  6 21:04:23 2023, max compression
```

## Comparing `agrc-sweeper-1.4.1.tar` & `agrc-sweeper-1.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/sweeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/credentials_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/street_types.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/sweeper/sweepers/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/UseLimitations.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/empties.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/invalids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/sweeper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/tests/test_address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/tests/test_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/workspace_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.235008 agrc-sweeper-1.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/src/sweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/credentials_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/street_types.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/src/sweeper/sweepers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/UseLimitations.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/empties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/invalids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/src/sweeper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/tests/test_address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/tests/test_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/workspace_info.py
```

### Comparing `agrc-sweeper-1.4.1/setup.py` & `agrc-sweeper-1.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import glob
 import io
 from os.path import basename, dirname, join, splitext
+from pathlib import Path
 
 from setuptools import find_packages, setup
 
 
 def read(*names, **kwargs):
     return io.open(
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ).read()
 
 
 setup(
     name="agrc-sweeper",
-    version="1.4.1",
+    version="1.4.3",
     license="MIT",
     description="CLI tool for making good data",
-    long_description="",
-    author="AGRC",
-    author_email="agrc@utah.gov",
+    long_description=(Path(__file__).parent / "readme.md").read_text(),
+    long_description_content_type="text/markdown",
+    author="UGRC",
+    author_email="ugrc-developers@utah.gov",
     url="https://github.com/agrc/sweeper",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[splitext(basename(i))[0] for i in glob.glob("src/*.py")],
     python_requires=">=3",
     include_package_data=True,
     zip_safe=False,
```

### Comparing `agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/SOURCES.txt` & `agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/__main__.py` & `agrc-sweeper-1.4.3/src/sweeper/__main__.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/address_parser.py` & `agrc-sweeper-1.4.3/src/sweeper/address_parser.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/backup.py` & `agrc-sweeper-1.4.3/src/sweeper/backup.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/credentials_template.py` & `agrc-sweeper-1.4.3/src/sweeper/credentials_template.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/report.py` & `agrc-sweeper-1.4.3/src/sweeper/report.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/street_types.json` & `agrc-sweeper-1.4.3/src/sweeper/street_types.json`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/sweepers/UseLimitations.html` & `agrc-sweeper-1.4.3/src/sweeper/sweepers/UseLimitations.html`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/sweepers/addresses.py` & `agrc-sweeper-1.4.3/src/sweeper/sweepers/addresses.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/sweepers/duplicates.py` & `agrc-sweeper-1.4.3/src/sweeper/sweepers/duplicates.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/sweepers/empties.py` & `agrc-sweeper-1.4.3/src/sweeper/sweepers/empties.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/sweepers/invalids.py` & `agrc-sweeper-1.4.3/src/sweeper/sweepers/invalids.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/sweepers/metadata.py` & `agrc-sweeper-1.4.3/src/sweeper/sweepers/metadata.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/tests/test_address_parser.py` & `agrc-sweeper-1.4.3/src/sweeper/tests/test_address_parser.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/tests/test_metadata.py` & `agrc-sweeper-1.4.3/src/sweeper/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.1/src/sweeper/workspace_info.py` & `agrc-sweeper-1.4.3/src/sweeper/workspace_info.py`

 * *Files identical despite different names*

