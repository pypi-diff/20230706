# Comparing `tmp/discotoolkit-1.1.2.tar.gz` & `tmp/discotoolkit-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.1.2.tar", last modified: Tue May 23 12:19:36 2023, max compression
+gzip compressed data, was "discotoolkit-1.1.3.tar", last modified: Thu Jul  6 08:58:58 2023, max compression
```

## Comparing `discotoolkit-1.1.2.tar` & `discotoolkit-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-23 12:19:24.847714 discotoolkit-1.1.2/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.1.2/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-23 12:19:24.847714 discotoolkit-1.1.2/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)     2618 2023-05-23 12:09:46.000000 discotoolkit-1.1.2/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-23 12:19:24.803714 discotoolkit-1.1.2/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)    18674 2023-05-23 12:15:25.000000 discotoolkit-1.1.2/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.1.2/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.1.2/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     7361 2023-05-18 08:03:41.000000 discotoolkit-1.1.2/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     4372 2023-05-22 02:26:21.000000 discotoolkit-1.1.2/discotoolkit/GeneSearch.py
--rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.1.2/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.1.2/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      156 2023-05-23 12:10:04.000000 discotoolkit-1.1.2/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-23 12:19:24.839714 discotoolkit-1.1.2/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-23 12:19:24.000000 discotoolkit-1.1.2/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      431 2023-05-23 12:19:24.000000 discotoolkit-1.1.2/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-23 12:19:24.000000 discotoolkit-1.1.2/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)      122 2023-05-23 12:19:24.000000 discotoolkit-1.1.2/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-23 12:19:24.000000 discotoolkit-1.1.2/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-23 12:19:24.851714 discotoolkit-1.1.2/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1052 2023-05-23 12:09:36.000000 discotoolkit-1.1.2/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-07-06 08:58:42.757437 discotoolkit-1.1.3/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.1.3/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-07-06 08:58:42.757437 discotoolkit-1.1.3/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2618 2023-07-06 08:53:57.000000 discotoolkit-1.1.3/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-07-06 08:58:42.725437 discotoolkit-1.1.3/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    18674 2023-05-23 12:29:40.000000 discotoolkit-1.1.3/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.1.3/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.1.3/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     7361 2023-07-06 02:05:18.000000 discotoolkit-1.1.3/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     4372 2023-05-22 02:26:21.000000 discotoolkit-1.1.3/discotoolkit/GeneSearch.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    13211 2023-07-06 08:49:58.000000 discotoolkit-1.1.3/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.1.3/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      156 2023-07-06 08:53:52.000000 discotoolkit-1.1.3/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-07-06 08:58:42.753437 discotoolkit-1.1.3/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-07-06 08:58:42.000000 discotoolkit-1.1.3/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      431 2023-07-06 08:58:42.000000 discotoolkit-1.1.3/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-07-06 08:58:42.000000 discotoolkit-1.1.3/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)      122 2023-07-06 08:58:42.000000 discotoolkit-1.1.3/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-07-06 08:58:42.000000 discotoolkit-1.1.3/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-07-06 08:58:42.761437 discotoolkit-1.1.3/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1052 2023-07-06 08:53:59.000000 discotoolkit-1.1.3/setup.py
```

### Comparing `discotoolkit-1.1.2/README.md` & `discotoolkit-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
  * @Author: Mengwei Li
  * @Date: 2023-04-16 21:20:42
  * @LastEditors: Mengwei Li
  * @LastEditTime: 2023-04-16 21:22:03
 -->
 [![Documentation Status](https://readthedocs.org/projects/discotoolkit-py/badge/?version=latest)](https://discotoolkit-py.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/discotoolkit?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/discotoolkit) [![PyPI version](https://img.shields.io/pypi/v/discotoolkit)](https://pypi.org/project/discotoolkit)
 
-# DISCOtoolkit 1.1.2
+# DISCOtoolkit 1.1.3
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). Read the documentation [DISCOtoolkit](https://discotoolkit-py.readthedocs.io/en/latest/). It provides the following functions:
 
 - Filter and download DISCO data based on sample metadata and cell type information
 - CELLiD: cell type annotation
 - scEnrichment: geneset enrichment using DISCO DEGs
```

### Comparing `discotoolkit-1.1.2/discotoolkit/CELLiD.py` & `discotoolkit-1.1.3/discotoolkit/CELLiD.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.2/discotoolkit/DiscoClass.py` & `discotoolkit-1.1.3/discotoolkit/DiscoClass.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.2/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.1.3/discotoolkit/DownloadDiscoData.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.2/discotoolkit/GeneSearch.py` & `discotoolkit-1.1.3/discotoolkit/GeneSearch.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.2/discotoolkit/GetMetadata.py` & `discotoolkit-1.1.3/discotoolkit/GetMetadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 # import libraries
 import requests
 import json
 import pandas as pd
 import re
+import numpy as np
 from typing import Union
 
 # import variable and class from other script
 from .GlobalVariable import logging, prefix_disco_url
 from .DiscoClass import FilterData, Filter
 
 def get_json(url : str, info_msg: str, error_msg: str, prefix : bool = True):
@@ -220,16 +221,17 @@
     metadata = metadata[retain_field]
 
     # checking for the specific cell type
     if filter.cell_type is None:
         sample_ct_info = sample_ct_info.iloc[check_in_list(sample_ct_info["sampleId"], metadata["sampleId"])]
         sample_cell_count = pd.DataFrame(sample_ct_info.groupby(["sampleId"])["cellNumber"].agg("sum")) # get the total number of cells
         sample_cell_count.columns = ["x"] # assigning different column name
-        
-        metadata["cell_number"] = list(sample_cell_count.loc[list(metadata["sampleId"])]["x"]) # assigning to the metadata
+        filtered_index = np.intersect1d(sample_cell_count.index, list(metadata["sampleId"])) # getting the common sampleId from the ct info and metadata info
+        metadata = metadata.loc[metadata['sampleId'].isin(filtered_index)] # filtering to only the common sampleId
+        metadata["cell_number"] = list(sample_cell_count.loc[filtered_index]["x"]) # assigning to the metadata
         metadata = metadata[metadata["cell_number"] > filter.min_cell_per_sample] # filter by the minimum cell per sample
 
         # condiition for none
         if len(metadata) == 0:
             logging.warn("Sorry, no samples passed the applied filters.")
             return None
```

### Comparing `discotoolkit-1.1.2/discotoolkit/GlobalVariable.py` & `discotoolkit-1.1.3/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.2/setup.py` & `discotoolkit-1.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='discotoolkit',
-    version="1.1.2",
+    version="1.1.3",
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
     install_requires=requirements,
     python_requires = '>=3.8.16',
```

