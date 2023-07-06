# Comparing `tmp/mads_datasets-0.1.6.tar.gz` & `tmp/mads_datasets-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.1.6.tar", last modified: Wed Jul  5 12:27:32 2023, max compression
+gzip compressed data, was "mads_datasets-0.2.tar", last modified: Thu Jul  6 14:17:48 2023, max compression
```

## Comparing `mads_datasets-0.1.6.tar` & `mads_datasets-0.2.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0     1408 2023-06-21 07:02:25.478815 mads_datasets-0.1.6/README.md
--rw-r--r--   0        0        0      187 2023-07-05 12:26:35.859652 mads_datasets-0.1.6/mads_datasets/__init__.py
--rw-r--r--   0        0        0    17872 2023-07-04 15:26:46.051334 mads_datasets-0.1.6/mads_datasets/datasetfactory.py
--rw-r--r--   0        0        0     5708 2023-07-04 15:18:06.790943 mads_datasets-0.1.6/mads_datasets/datasets.py
--rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.6/mads_datasets/datatools.py
--rw-r--r--   0        0        0     4003 2023-06-21 07:28:25.959229 mads_datasets-0.1.6/mads_datasets/settings.py
--rw-r--r--   0        0        0     1111 2023-07-05 12:27:32.349985 mads_datasets-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2932 2023-06-05 11:35:08.197025 mads_datasets-0.1.6/tests/test_data.py
--rw-r--r--   0        0        0      134 2023-06-05 13:30:33.572743 mads_datasets-0.1.6/tests/test_tokenizer.py
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 mads_datasets-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1408 2023-06-21 07:02:25.478815 mads_datasets-0.2/README.md
+-rw-r--r--   0        0        0     1770 2023-07-06 14:17:36.250742 mads_datasets-0.2/mads_datasets/__init__.py
+-rw-r--r--   0        0        0     5660 2023-07-06 14:17:36.250970 mads_datasets-0.2/mads_datasets/base.py
+-rw-r--r--   0        0        0      396 2023-07-06 14:17:36.251215 mads_datasets-0.2/mads_datasets/datasets/__init__.py
+-rw-r--r--   0        0        0     1608 2023-07-06 14:17:36.251500 mads_datasets-0.2/mads_datasets/datasets/basicdatasets.py
+-rw-r--r--   0        0        0     3784 2023-07-06 14:17:36.251757 mads_datasets-0.2/mads_datasets/datasets/torchdatasets.py
+-rw-r--r--   0        0        0     4757 2023-07-06 14:17:36.252046 mads_datasets-0.2/mads_datasets/datatools.py
+-rw-r--r--   0        0        0      511 2023-07-06 14:17:36.252279 mads_datasets-0.2/mads_datasets/factories/__init__.py
+-rw-r--r--   0        0        0     3070 2023-07-06 14:17:36.252470 mads_datasets-0.2/mads_datasets/factories/basicfactories.py
+-rw-r--r--   0        0        0     4666 2023-07-06 14:17:36.252668 mads_datasets-0.2/mads_datasets/factories/torchfactories.py
+-rw-r--r--   0        0        0     4028 2023-07-06 14:17:36.252928 mads_datasets-0.2/mads_datasets/settings.py
+-rw-r--r--   0        0        0     1094 2023-07-06 14:17:48.994010 mads_datasets-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2932 2023-06-05 11:35:08.197025 mads_datasets-0.2/tests/test_data.py
+-rw-r--r--   0        0        0      134 2023-06-05 13:30:33.572743 mads_datasets-0.2/tests/test_tokenizer.py
+-rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 mads_datasets-0.2/PKG-INFO
```

### Comparing `mads_datasets-0.1.6/README.md` & `mads_datasets-0.2/README.md`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.6/mads_datasets/datatools.py` & `mads_datasets-0.2/mads_datasets/datatools.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """Download a file from url to location data_dir / filename
 
     Args:
         data_dir (Path): dir to store file
         filename (Path): filename
         url (str): url to obtain filename
         unzip (bool, optional): If the file needs unzipping
-        overwrite (bool, optional): If the file needs to be overwritten, if it already exists.
+        overwrite (bool, optional): overwrite file, if it already exists.
 
     Returns:
         Path: _description_
     """
 
     path = data_dir / filename
     if path.exists() and not overwrite:
```

### Comparing `mads_datasets-0.1.6/mads_datasets/settings.py` & `mads_datasets-0.2/mads_datasets/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,23 @@
     window_size: int
 
 
 class PdDatasetSettings(DatasetSettings):
     target: str
     features: List[str]
 
+
 penguinssettings = DatasetSettings(
-    dataset_url=cast(HttpUrl, "https://github.com/raoulg/juliaintro/raw/main/data/palmerpenguins.parq"),
+    dataset_url=cast(
+        HttpUrl,
+        "https://github.com/raoulg/juliaintro/raw/main/data/palmerpenguins.parq",
+    ),
     filename=Path("penguins.parq"),
     name="penguins",
-    digest="675e2a75750d0e076df810893e675476"
+    digest="675e2a75750d0e076df810893e675476",
 )
 
 irissettings = PdDatasetSettings(
     dataset_url=cast(
         HttpUrl, "https://github.com/raoulg/data_assets/raw/main/iris_dirty.csv"
     ),
     filename=Path("iris.csv"),
```

### Comparing `mads_datasets-0.1.6/pyproject.toml` & `mads_datasets-0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 [project]
 name = "mads-datasets"
-version = "0.1.6"
+version = "0.2"
 description = "Datasets for the master applied data science"
 authors = [
     { name = "Raoul Grouls", email = "Raoul.Grouls@han.nl" },
 ]
 dependencies = [
-    "torch>=2.0.1",
     "tqdm>=4.65.0",
     "requests>=2.31.0",
     "loguru>=0.7.0",
     "numpy>=1.24.3",
     "pydantic>=1.10.8",
     "pillow>=9.5.0",
-    "torchtext>=0.15.2",
     "pandas>=2.0.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 GitHub = "https://github.com/raoulg/mads_datasets"
 
 [project.optional-dependencies]
-pandas = [
-    "pandas>=2.0.2",
+torch = [
+    "torch>=2.0.1",
 ]
 
 [project.group.tests.dependencies]
 responses = "^0.23.1"
 
 [tool.pdm.dev-dependencies]
 lint = [
     "ruff>=0.0.277",
     "black>=23.3.0",
     "mypy>=1.4.1",
     "isort>=5.12.0",
+    "types-requests>=2.31.0.1",
 ]
 tests = [
     "pytest>=7.4.0",
     "jupyter>=1.0.0",
     "responses>=0.23.1",
 ]
```

### Comparing `mads_datasets-0.1.6/tests/test_data.py` & `mads_datasets-0.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.6/PKG-INFO` & `mads_datasets-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: mads-datasets
-Version: 0.1.6
+Version: 0.2
 Summary: Datasets for the master applied data science
 Author-Email: Raoul Grouls <Raoul.Grouls@han.nl>
 License: MIT
 Project-URL: Github, https://github.com/raoulg/mads_datasets
 Requires-Python: >=3.8
-Requires-Dist: torch>=2.0.1
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: loguru>=0.7.0
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: pydantic>=1.10.8
 Requires-Dist: pillow>=9.5.0
-Requires-Dist: torchtext>=0.15.2
 Requires-Dist: pandas>=2.0.3
-Requires-Dist: pandas>=2.0.2; extra == "pandas"
-Provides-Extra: pandas
+Requires-Dist: torch>=2.0.1; extra == "torch"
+Provides-Extra: torch
 Description-Content-Type: text/markdown
 
 # MADS Datasets Library
 
 This library provides the functionality to download, process, and stream several datasets.
 
 ## Installation
```

