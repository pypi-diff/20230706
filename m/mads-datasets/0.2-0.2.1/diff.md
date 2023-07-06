# Comparing `tmp/mads_datasets-0.2.tar.gz` & `tmp/mads_datasets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.2.tar", last modified: Thu Jul  6 14:17:48 2023, max compression
+gzip compressed data, was "mads_datasets-0.2.1.tar", last modified: Thu Jul  6 14:29:49 2023, max compression
```

## Comparing `mads_datasets-0.2.tar` & `mads_datasets-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1408 2023-06-21 07:02:25.478815 mads_datasets-0.2/README.md
--rw-r--r--   0        0        0     1770 2023-07-06 14:17:36.250742 mads_datasets-0.2/mads_datasets/__init__.py
--rw-r--r--   0        0        0     5660 2023-07-06 14:17:36.250970 mads_datasets-0.2/mads_datasets/base.py
--rw-r--r--   0        0        0      396 2023-07-06 14:17:36.251215 mads_datasets-0.2/mads_datasets/datasets/__init__.py
--rw-r--r--   0        0        0     1608 2023-07-06 14:17:36.251500 mads_datasets-0.2/mads_datasets/datasets/basicdatasets.py
--rw-r--r--   0        0        0     3784 2023-07-06 14:17:36.251757 mads_datasets-0.2/mads_datasets/datasets/torchdatasets.py
--rw-r--r--   0        0        0     4757 2023-07-06 14:17:36.252046 mads_datasets-0.2/mads_datasets/datatools.py
--rw-r--r--   0        0        0      511 2023-07-06 14:17:36.252279 mads_datasets-0.2/mads_datasets/factories/__init__.py
--rw-r--r--   0        0        0     3070 2023-07-06 14:17:36.252470 mads_datasets-0.2/mads_datasets/factories/basicfactories.py
--rw-r--r--   0        0        0     4666 2023-07-06 14:17:36.252668 mads_datasets-0.2/mads_datasets/factories/torchfactories.py
--rw-r--r--   0        0        0     4028 2023-07-06 14:17:36.252928 mads_datasets-0.2/mads_datasets/settings.py
--rw-r--r--   0        0        0     1094 2023-07-06 14:17:48.994010 mads_datasets-0.2/pyproject.toml
--rw-r--r--   0        0        0     2932 2023-06-05 11:35:08.197025 mads_datasets-0.2/tests/test_data.py
--rw-r--r--   0        0        0      134 2023-06-05 13:30:33.572743 mads_datasets-0.2/tests/test_tokenizer.py
--rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 mads_datasets-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1408 2023-06-21 07:02:25.478815 mads_datasets-0.2.1/README.md
+-rw-r--r--   0        0        0     1772 2023-07-06 14:28:27.216097 mads_datasets-0.2.1/mads_datasets/__init__.py
+-rw-r--r--   0        0        0     5660 2023-07-06 14:17:36.250970 mads_datasets-0.2.1/mads_datasets/base.py
+-rw-r--r--   0        0        0      396 2023-07-06 14:17:36.251215 mads_datasets-0.2.1/mads_datasets/datasets/__init__.py
+-rw-r--r--   0        0        0     1608 2023-07-06 14:17:36.251500 mads_datasets-0.2.1/mads_datasets/datasets/basicdatasets.py
+-rw-r--r--   0        0        0     3784 2023-07-06 14:17:36.251757 mads_datasets-0.2.1/mads_datasets/datasets/torchdatasets.py
+-rw-r--r--   0        0        0     4949 2023-07-06 14:28:51.194758 mads_datasets-0.2.1/mads_datasets/datatools.py
+-rw-r--r--   0        0        0      511 2023-07-06 14:17:36.252279 mads_datasets-0.2.1/mads_datasets/factories/__init__.py
+-rw-r--r--   0        0        0     3070 2023-07-06 14:17:36.252470 mads_datasets-0.2.1/mads_datasets/factories/basicfactories.py
+-rw-r--r--   0        0        0     4666 2023-07-06 14:17:36.252668 mads_datasets-0.2.1/mads_datasets/factories/torchfactories.py
+-rw-r--r--   0        0        0     4028 2023-07-06 14:17:36.252928 mads_datasets-0.2.1/mads_datasets/settings.py
+-rw-r--r--   0        0        0     1096 2023-07-06 14:29:49.064092 mads_datasets-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2932 2023-06-05 11:35:08.197025 mads_datasets-0.2.1/tests/test_data.py
+-rw-r--r--   0        0        0      134 2023-06-05 13:30:33.572743 mads_datasets-0.2.1/tests/test_tokenizer.py
+-rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 mads_datasets-0.2.1/PKG-INFO
```

### Comparing `mads_datasets-0.2/README.md` & `mads_datasets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.2/mads_datasets/__init__.py` & `mads_datasets-0.2.1/mads_datasets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     irissettings,
     penguinssettings,
     sunspotsettings,
 )
 
 __all__ = ["DatasetFactoryProvider", "DatasetType"]
 
-__version__ = "0.2"
+__version__ = "0.2.1"
 
 
 class DatasetFactoryProvider:
     @staticmethod
     def create_factory(dataset_type: DatasetType, **kwargs) -> AbstractDatasetFactory:
         datadir = Path(kwargs.get("datadir", Path.home() / ".cache/mads_datasets"))
         if dataset_type == DatasetType.FLOWERS:
```

### Comparing `mads_datasets-0.2/mads_datasets/base.py` & `mads_datasets-0.2.1/mads_datasets/base.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.2/mads_datasets/datasets/basicdatasets.py` & `mads_datasets-0.2.1/mads_datasets/datasets/basicdatasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.2/mads_datasets/datasets/torchdatasets.py` & `mads_datasets-0.2.1/mads_datasets/datasets/torchdatasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.2/mads_datasets/datatools.py` & `mads_datasets-0.2.1/mads_datasets/datatools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 import shutil
 import tarfile
 import zipfile
 from datetime import datetime
 from pathlib import Path
-from typing import Iterator, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Iterator, List, Optional, Tuple, Union
 
 import requests
-import torch
 from loguru import logger
 from tqdm import tqdm
 
+from mads_datasets.base import import_torch
 from mads_datasets.settings import FileTypes
 
-Tensor = torch.Tensor
+if TYPE_CHECKING:
+    import torch
+
+    Tensor = torch.Tensor
 
 
 def walk_dir(path: Path) -> Iterator:
     """loops recursively through a folder
 
     Args:
         path (Path): folder to loop trough. If a directory
@@ -125,33 +128,34 @@
     if dir.exists():
         logger.info(f"Clean out {dir}")
         shutil.rmtree(dir)
     else:
         dir.mkdir(parents=True)
 
 
-def window(x: Tensor, n_time: int) -> Tensor:
+def window(x: "Tensor", n_time: int) -> "Tensor":
     """
     Generates and index that can be used to window a timeseries.
     E.g. the single series [0, 1, 2, 3, 4, 5] can be windowed into 4 timeseries with
     length 3 like this:
 
     [0, 1, 2]
     [1, 2, 3]
     [2, 3, 4]
     [3, 4, 5]
 
     We now can feed 4 different timeseries into the model, instead of 1, all
     with the same length.
     """
-    n_window = len(x) - n_time + 1
-    time = torch.arange(0, n_time).reshape(1, -1)
-    window = torch.arange(0, n_window).reshape(-1, 1)
-    idx = time + window
-    return idx
+    with import_torch() as torch:  # type: ignore
+        n_window = len(x) - n_time + 1
+        time = torch.arange(0, n_time).reshape(1, -1)  # type: ignore
+        window = torch.arange(0, n_window).reshape(-1, 1)  # type: ignore
+        idx = time + window
+        return idx
 
 
 def dir_add_timestamp(log_dir: Optional[Path] = None) -> Path:
     if log_dir is None:
         log_dir = Path(".")
     log_dir = Path(log_dir)
     timestamp = datetime.now().strftime("%Y%m%d-%H%M")
```

### Comparing `mads_datasets-0.2/mads_datasets/factories/basicfactories.py` & `mads_datasets-0.2.1/mads_datasets/factories/basicfactories.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.2/mads_datasets/factories/torchfactories.py` & `mads_datasets-0.2.1/mads_datasets/factories/torchfactories.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.2/mads_datasets/settings.py` & `mads_datasets-0.2.1/mads_datasets/settings.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.2/pyproject.toml` & `mads_datasets-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mads-datasets"
-version = "0.2"
+version = "0.2.1"
 description = "Datasets for the master applied data science"
 authors = [
     { name = "Raoul Grouls", email = "Raoul.Grouls@han.nl" },
 ]
 dependencies = [
     "tqdm>=4.65.0",
     "requests>=2.31.0",
```

### Comparing `mads_datasets-0.2/tests/test_data.py` & `mads_datasets-0.2.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.2/PKG-INFO` & `mads_datasets-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mads-datasets
-Version: 0.2
+Version: 0.2.1
 Summary: Datasets for the master applied data science
 Author-Email: Raoul Grouls <Raoul.Grouls@han.nl>
 License: MIT
 Project-URL: Github, https://github.com/raoulg/mads_datasets
 Requires-Python: >=3.8
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: requests>=2.31.0
```

