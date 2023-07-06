# Comparing `tmp/refineGEMs-1.0.1.tar.gz` & `tmp/refineGEMs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineGEMs-1.0.1.tar", last modified: Tue May  9 14:59:15 2023, max compression
+gzip compressed data, was "refineGEMs-1.1.0.tar", last modified: Thu Jul  6 14:37:56 2023, max compression
```

## Comparing `refineGEMs-1.0.1.tar` & `refineGEMs-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.832120 refineGEMs-1.0.1/
--rw-r--r--   0 root         (0) staff       (20)     1068 2022-05-04 13:39:38.000000 refineGEMs-1.0.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     3117 2023-05-09 14:59:15.831723 refineGEMs-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2735 2023-05-09 14:56:11.000000 refineGEMs-1.0.1/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.819773 refineGEMs-1.0.1/data/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.822757 refineGEMs-1.0.1/data/database/
--rw-r--r--   0 root         (0) staff       (20)   353015 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/data/database/sbo_media_db.sql
--rw-r--r--   0 root         (0) staff       (20)      140 2023-05-04 11:55:59.000000 refineGEMs-1.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.824968 refineGEMs-1.0.1/refineGEMs.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     3117 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      693 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-04 12:05:30.000000 refineGEMs-1.0.1/refineGEMs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)      292 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       11 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.831015 refineGEMs-1.0.1/refinegems/
--rw-r--r--   0 root         (0) staff       (20)      595 2023-05-04 11:40:57.000000 refineGEMs-1.0.1/refinegems/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    22498 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/analysis_biocyc.py
--rw-r--r--   0 root         (0) staff       (20)    14987 2023-05-04 09:57:20.000000 refineGEMs-1.0.1/refinegems/analysis_db.py
--rw-r--r--   0 root         (0) staff       (20)     6328 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/analysis_kegg.py
--rw-r--r--   0 root         (0) staff       (20)     3167 2023-03-14 15:27:23.000000 refineGEMs-1.0.1/refinegems/charges.py
--rw-r--r--   0 root         (0) staff       (20)    10352 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/comparison.py
--rw-r--r--   0 root         (0) staff       (20)     5672 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/curate.py
--rw-r--r--   0 root         (0) staff       (20)     8936 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/cvterms.py
--rw-r--r--   0 root         (0) staff       (20)     9537 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/databases.py
--rw-r--r--   0 root         (0) staff       (20)    10350 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/entities.py
--rw-r--r--   0 root         (0) staff       (20)    12891 2023-05-04 09:57:20.000000 refineGEMs-1.0.1/refinegems/gapfill.py
--rw-r--r--   0 root         (0) staff       (20)    15225 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/growth.py
--rw-r--r--   0 root         (0) staff       (20)    11765 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/investigate.py
--rw-r--r--   0 root         (0) staff       (20)    20824 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/io.py
--rw-r--r--   0 root         (0) staff       (20)     7224 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/modelseed.py
--rw-r--r--   0 root         (0) staff       (20)     7042 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/pathways.py
--rw-r--r--   0 root         (0) staff       (20)    41756 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/polish.py
--rw-r--r--   0 root         (0) staff       (20)    23740 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/sboann.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-09 14:59:15.832211 refineGEMs-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1234 2023-05-09 14:59:04.000000 refineGEMs-1.0.1/setup.py
+drwxr-xr-x   0 gusak      (505) staff       (20)        0 2023-07-06 14:37:56.892967 refineGEMs-1.1.0/
+-rw-r--r--   0 gusak      (505) staff       (20)     1068 2023-03-03 18:29:17.000000 refineGEMs-1.1.0/LICENSE
+-rw-r--r--   0 gusak      (505) staff       (20)     3630 2023-07-06 14:37:56.892364 refineGEMs-1.1.0/PKG-INFO
+-rw-r--r--   0 gusak      (505) staff       (20)     3248 2023-07-06 13:47:18.000000 refineGEMs-1.1.0/README.md
+-rw-r--r--   0 gusak      (505) staff       (20)      140 2023-03-03 18:29:17.000000 refineGEMs-1.1.0/pyproject.toml
+drwxr-xr-x   0 gusak      (505) staff       (20)        0 2023-07-06 14:37:56.854461 refineGEMs-1.1.0/refineGEMs.egg-info/
+-rw-r--r--   0 gusak      (505) staff       (20)     3630 2023-07-06 14:37:56.000000 refineGEMs-1.1.0/refineGEMs.egg-info/PKG-INFO
+-rw-r--r--   0 gusak      (505) staff       (20)      684 2023-07-06 14:37:56.000000 refineGEMs-1.1.0/refineGEMs.egg-info/SOURCES.txt
+-rw-r--r--   0 gusak      (505) staff       (20)        1 2023-07-06 14:37:56.000000 refineGEMs-1.1.0/refineGEMs.egg-info/dependency_links.txt
+-rw-r--r--   0 gusak      (505) staff       (20)        1 2023-03-06 13:24:40.000000 refineGEMs-1.1.0/refineGEMs.egg-info/not-zip-safe
+-rw-r--r--   0 gusak      (505) staff       (20)      292 2023-07-06 14:37:56.000000 refineGEMs-1.1.0/refineGEMs.egg-info/requires.txt
+-rw-r--r--   0 gusak      (505) staff       (20)       11 2023-07-06 14:37:56.000000 refineGEMs-1.1.0/refineGEMs.egg-info/top_level.txt
+drwxr-xr-x   0 gusak      (505) staff       (20)        0 2023-07-06 14:37:56.890343 refineGEMs-1.1.0/refinegems/
+-rw-r--r--   0 gusak      (505) staff       (20)      621 2023-07-06 09:38:27.000000 refineGEMs-1.1.0/refinegems/__init__.py
+-rw-r--r--   0 gusak      (505) staff       (20)    22498 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/analysis_biocyc.py
+-rw-r--r--   0 gusak      (505) staff       (20)    14987 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/analysis_db.py
+-rw-r--r--   0 gusak      (505) staff       (20)     6328 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/analysis_kegg.py
+-rw-r--r--   0 gusak      (505) staff       (20)     7844 2023-07-06 09:38:27.000000 refineGEMs-1.1.0/refinegems/biomass.py
+-rw-r--r--   0 gusak      (505) staff       (20)     3167 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/charges.py
+-rw-r--r--   0 gusak      (505) staff       (20)    10352 2023-06-27 12:14:59.000000 refineGEMs-1.1.0/refinegems/comparison.py
+-rw-r--r--   0 gusak      (505) staff       (20)     5672 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/curate.py
+-rw-r--r--   0 gusak      (505) staff       (20)     8936 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/cvterms.py
+-rw-r--r--   0 gusak      (505) staff       (20)     9537 2023-06-27 13:26:33.000000 refineGEMs-1.1.0/refinegems/databases.py
+-rw-r--r--   0 gusak      (505) staff       (20)    10350 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/entities.py
+-rw-r--r--   0 gusak      (505) staff       (20)    12891 2023-07-06 12:58:41.000000 refineGEMs-1.1.0/refinegems/gapfill.py
+-rw-r--r--   0 gusak      (505) staff       (20)    15225 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/growth.py
+-rw-r--r--   0 gusak      (505) staff       (20)    11765 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/investigate.py
+-rw-r--r--   0 gusak      (505) staff       (20)    21121 2023-07-06 12:58:41.000000 refineGEMs-1.1.0/refinegems/io.py
+-rw-r--r--   0 gusak      (505) staff       (20)     7224 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/modelseed.py
+-rw-r--r--   0 gusak      (505) staff       (20)     7042 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/pathways.py
+-rw-r--r--   0 gusak      (505) staff       (20)    42104 2023-07-06 12:58:41.000000 refineGEMs-1.1.0/refinegems/polish.py
+-rw-r--r--   0 gusak      (505) staff       (20)    23740 2023-06-12 12:35:18.000000 refineGEMs-1.1.0/refinegems/sboann.py
+-rw-r--r--   0 gusak      (505) staff       (20)       38 2023-07-06 14:37:56.893153 refineGEMs-1.1.0/setup.cfg
+-rw-r--r--   0 gusak      (505) staff       (20)     1234 2023-07-06 09:38:27.000000 refineGEMs-1.1.0/setup.py
```

### Comparing `refineGEMs-1.0.1/LICENSE` & `refineGEMs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/PKG-INFO` & `refineGEMs-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 Metadata-Version: 2.1
 Name: refineGEMs
-Version: 1.0.1
+Version: 1.1.0
 Summary: refineGEMs is a python package inteded to help with the curation of genome-scale metabolic models (GEMS)
 Home-page: https://github.com/draeger-lab/refinegems
 Author: Famke Baeuerle and Gwendolyn O. Gusak
 Author-email: famke.baeuerle@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7915766.svg)](https://doi.org/10.5281/zenodo.7915766) [![Documentation Status](https://readthedocs.org/projects/refinegems/badge/?version=latest)](https://refinegems.readthedocs.io/en/latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/draeger-lab/refinegems/refinegems)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Documentation Status](https://readthedocs.org/projects/refinegems/badge/?version=latest)](https://refinegems.readthedocs.io/en/latest/?badge=latest)
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/draeger-lab/refinegems/main)
+[![PyPI version](https://badge.fury.io/py/refineGEMs.svg)](https://badge.fury.io/py/refineGEMs)
+![PyPI - Format](https://img.shields.io/pypi/format/refinegems)
+[![PyPI downloads](https://img.shields.io/pypi/dm/refinegems.svg)](https://pypistats.org/packages/refinegems)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7915766.svg)](https://doi.org/10.5281/zenodo.7915766)
 
 <p align="center">
 <img src="https://github.com/draeger-lab/refinegems/raw/main/docs/source/images/refineGEMs_logo.png" height="200"/>
 </p>
 
 # refineGEMs
 `refineGEMs` is a python package inteded to help with the curation of genome-scale metabolic models (GEMS).
```

### Comparing `refineGEMs-1.0.1/README.md` & `refineGEMs-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7915766.svg)](https://doi.org/10.5281/zenodo.7915766) [![Documentation Status](https://readthedocs.org/projects/refinegems/badge/?version=latest)](https://refinegems.readthedocs.io/en/latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/draeger-lab/refinegems/refinegems)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Documentation Status](https://readthedocs.org/projects/refinegems/badge/?version=latest)](https://refinegems.readthedocs.io/en/latest/?badge=latest)
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/draeger-lab/refinegems/main)
+[![PyPI version](https://badge.fury.io/py/refineGEMs.svg)](https://badge.fury.io/py/refineGEMs)
+![PyPI - Format](https://img.shields.io/pypi/format/refinegems)
+[![PyPI downloads](https://img.shields.io/pypi/dm/refinegems.svg)](https://pypistats.org/packages/refinegems)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7915766.svg)](https://doi.org/10.5281/zenodo.7915766)
 
 <p align="center">
 <img src="https://github.com/draeger-lab/refinegems/raw/main/docs/source/images/refineGEMs_logo.png" height="200"/>
 </p>
 
 # refineGEMs
 `refineGEMs` is a python package inteded to help with the curation of genome-scale metabolic models (GEMS).
```

### Comparing `refineGEMs-1.0.1/refineGEMs.egg-info/PKG-INFO` & `refineGEMs-1.1.0/refineGEMs.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 Metadata-Version: 2.1
 Name: refineGEMs
-Version: 1.0.1
+Version: 1.1.0
 Summary: refineGEMs is a python package inteded to help with the curation of genome-scale metabolic models (GEMS)
 Home-page: https://github.com/draeger-lab/refinegems
 Author: Famke Baeuerle and Gwendolyn O. Gusak
 Author-email: famke.baeuerle@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7915766.svg)](https://doi.org/10.5281/zenodo.7915766) [![Documentation Status](https://readthedocs.org/projects/refinegems/badge/?version=latest)](https://refinegems.readthedocs.io/en/latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/draeger-lab/refinegems/refinegems)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Documentation Status](https://readthedocs.org/projects/refinegems/badge/?version=latest)](https://refinegems.readthedocs.io/en/latest/?badge=latest)
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/draeger-lab/refinegems/main)
+[![PyPI version](https://badge.fury.io/py/refineGEMs.svg)](https://badge.fury.io/py/refineGEMs)
+![PyPI - Format](https://img.shields.io/pypi/format/refinegems)
+[![PyPI downloads](https://img.shields.io/pypi/dm/refinegems.svg)](https://pypistats.org/packages/refinegems)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7915766.svg)](https://doi.org/10.5281/zenodo.7915766)
 
 <p align="center">
 <img src="https://github.com/draeger-lab/refinegems/raw/main/docs/source/images/refineGEMs_logo.png" height="200"/>
 </p>
 
 # refineGEMs
 `refineGEMs` is a python package inteded to help with the curation of genome-scale metabolic models (GEMS).
```

### Comparing `refineGEMs-1.0.1/refinegems/__init__.py` & `refineGEMs-1.1.0/refinegems/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # declares public API for this module
 # loads functions from subscripts which are needed in main.py
 import refinegems.databases
+import refinegems.biomass
 import refinegems.growth
 import refinegems.modelseed
 import refinegems.sboann
 import refinegems.charges
 import refinegems.pathways
 import refinegems.curate
 import refinegems.polish
```

### Comparing `refineGEMs-1.0.1/refinegems/analysis_biocyc.py` & `refineGEMs-1.1.0/refinegems/analysis_biocyc.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/analysis_db.py` & `refineGEMs-1.1.0/refinegems/analysis_db.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/analysis_kegg.py` & `refineGEMs-1.1.0/refinegems/analysis_kegg.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/charges.py` & `refineGEMs-1.1.0/refinegems/charges.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/comparison.py` & `refineGEMs-1.1.0/refinegems/comparison.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/curate.py` & `refineGEMs-1.1.0/refinegems/curate.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/cvterms.py` & `refineGEMs-1.1.0/refinegems/cvterms.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/databases.py` & `refineGEMs-1.1.0/refinegems/databases.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/entities.py` & `refineGEMs-1.1.0/refinegems/entities.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/gapfill.py` & `refineGEMs-1.1.0/refinegems/gapfill.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/growth.py` & `refineGEMs-1.1.0/refinegems/growth.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/investigate.py` & `refineGEMs-1.1.0/refinegems/investigate.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/io.py` & `refineGEMs-1.1.0/refinegems/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 """ Provides functions to load and write models, media definitions and the manual annotation table
 
-Depending on the application the model needs to be loaded with cobra (memote)
-or with libSBML (activation of groups). The media definitions are denoted in a csv within the data folder of this repository, thus the functions will only work if the user clones the repository. The manual_annotations table has to follow the specific layout given in the data folder in order to work with this module.
+Depending on the application the model needs to be loaded with cobra (memote) or with libSBML (activation of groups). 
+The media definitions are denoted in a csv within the data folder of this repository, thus the functions will only work if the user clones the repository. 
+The manual_annotations table has to follow the specific layout given in the data folder in order to work with this module.
 """
 
 import cobra
 import click
 import yaml
 import os
 import re
@@ -447,15 +448,14 @@
             while not_valid:
                 model = click.prompt('Path to your model file.')
                 if os.path.isfile(model):
                     user_input['model'] = model
                     not_valid = False
                 else:
                     print('File does not exist. Please enter a valid file path')
-        
             user_input['memote'] = click.confirm('Do you want to run MEMOTE (takes some time)?')    
             user_input['modelseed'] = click.confirm('Do you want to compare your model entities to the ModelSEED database?')
         
             gap_analysis = click.confirm('Do you want to run a gap analysis?') 
             user_input['gap_analysis'] = gap_analysis
             if gap_analysis:
                 gap_analysis_params = {}
@@ -477,18 +477,20 @@
                 
                 new_path = click.confirm('Do you want to save your modified model to ' + user_input['out_path'] + '<model.id>_modified_<today>.xml?')
                 if new_path:
                     user_input['model_out'] = 'stdout'
                 else:
                     user_input['model_out'] = click.prompt('Enter path and filename to where to save the modified model')
                 
-                user_input['gapfill_model'] = click.confirm('Do you want to fill gaps in your model?')
+                gapfill_model = click.confirm('Do you want to fill gaps in your model?')
+                user_input['gapfill_model'] = gapfill_model
                 
-                if not gap_analysis:
-                    user_input['gap_analysis_file'] = click.prompt('Enter path to Excel file with which gaps should be filled')
+                if gapfill_model:
+                    if not gap_analysis:
+                        user_input['gap_analysis_file'] = click.prompt('Enter path to Excel file with which gaps should be filled')
                 
                 user_input['keggpathways'] = click.confirm('Do you want to add KEGG Pathways?')
                     
                 user_input['sboterms'] = click.confirm('Do you want to update the SBO Terms?')
                 
                 user_input['charge_corr'] = click.confirm('Do you want to add charges to uncharged metabolites?')
                     
@@ -512,17 +514,21 @@
                     id_db = click.prompt('What database is your model based on? BIGG|VMH')
                     user_input['id_db'] = id_db
                     lab_strain = not click.confirm('Does your modeled organism have a database entry?', default=True)
                     user_input['lab_strain'] = lab_strain
                     protein_fasta = click.prompt('If possible, provide the path to your Protein FASTA file used for CarveMe')
                     user_input['protein_fasta'] = protein_fasta
                     
+                biomass = click.confirm('Do you want to check & normalise the biomass function(s)?')
+                user_input['biomass'] = biomass
+                    
             else:
                 user_input['keggpathways'] = False
                 user_input['polish'] = False
+                user_input['biomass'] = False
                 user_input['sboterms'] = False
                 user_input['charge_corr'] = False
                 user_input['gapfill_model'] = False
                 user_input['man_cur'] = False
             
         today = date.today().strftime("%Y%m%d")
```

### Comparing `refineGEMs-1.0.1/refinegems/modelseed.py` & `refineGEMs-1.1.0/refinegems/modelseed.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/pathways.py` & `refineGEMs-1.1.0/refinegems/pathways.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/refinegems/polish.py` & `refineGEMs-1.1.0/refinegems/polish.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         notes_string = species.getNotesString().split('\n')
         for elem in notes_string:
             for db in metabol_db_dict.keys():
                 if '<p>' + db in elem:
                     elem_used.append(elem)
                     #print(elem.strip()[:-4].split(': ')[1])
                     fill_in = re.split(':\s*', elem.strip()[:-4])[1]
-                    if (';') in fill_in and db != 'INCHI':
+                    if (';') in fill_in and not re.search('inchi', db, re.IGNORECASE):
                         entries = fill_in.split(';')
                         for entry in entries:
                             add_cv_term_metabolites(entry.strip(), db, species)
                     else:
                         add_cv_term_metabolites(fill_in, db, species)
 
         for elem in notes_string:
@@ -536,17 +536,22 @@
             extracted_curie = curie.split(OLD_MIRIAM)[1]
         
         # Get CURIEs irrespective of pattern
         if '/' in extracted_curie:
             extracted_curie = extracted_curie.split('/')
             
             # Check for certain special cases
-            if re.fullmatch('^inchi$', extracted_curie[0], re.IGNORECASE):  # Check for inchi as splitting by '/' splits too much
-                prefix = extracted_curie[0].lower()
-                identifier = '/'.join(extracted_curie[1:len(extracted_curie)])
+            if re.search('inchi', extracted_curie[0], re.IGNORECASE):  # Check for inchi as splitting by '/' splits too much
+                if re.fullmatch('^inchi$', extracted_curie[0], re.IGNORECASE):
+                    prefix = extracted_curie[0].lower()
+                    identifier = '/'.join(extracted_curie[1:len(extracted_curie)])
+                else:
+                    wrong_prefix = extracted_curie[0].split(':')
+                    prefix = wrong_prefix[0]
+                    identifier = f'{wrong_prefix[1]}/{"/".join(extracted_curie[1:len(extracted_curie)])}'
             elif re.fullmatch('^brenda$', extracted_curie[0], re.IGNORECASE):
                 prefix = 'ec-code'
                 identifier = extracted_curie[1]
             elif re.fullmatch('^biocyc$', extracted_curie[0], re.IGNORECASE) or ('metacyc.' in extracted_curie[0]):  # Check for bio- & metacyc
                 prefix = 'biocyc'
                 identifier = extracted_curie[1].replace('META:', '')
```

### Comparing `refineGEMs-1.0.1/refinegems/sboann.py` & `refineGEMs-1.1.0/refinegems/sboann.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.1/setup.py` & `refineGEMs-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # needed for installation of refinegems
 from setuptools import setup
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(name='refineGEMs',
-      version='1.0.1',
+      version='1.1.0',
       description='refineGEMs is a python package inteded to help with the curation of genome-scale metabolic models (GEMS)',
       long_description=readme,
       long_description_content_type='text/markdown',
       author='Famke Baeuerle and Gwendolyn O. Gusak',
       author_email='famke.baeuerle@gmail.com',
       url='https://github.com/draeger-lab/refinegems',
       license='MIT',
```

