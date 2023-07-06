# Comparing `tmp/pyrarecomb-0.0.1.tar.gz` & `tmp/pyrarecomb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrarecomb-0.0.1.tar", last modified: Thu Jul  6 16:24:20 2023, max compression
+gzip compressed data, was "pyrarecomb-0.0.2.tar", last modified: Thu Jul  6 17:30:56 2023, max compression
```

## Comparing `pyrarecomb-0.0.1.tar` & `pyrarecomb-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 16:24:20.154061 pyrarecomb-0.0.1/
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     1072 2023-07-05 20:39:51.000000 pyrarecomb-0.0.1/LICENSE
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       18 2023-07-06 16:16:04.000000 pyrarecomb-0.0.1/MANIFEST.in
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3507 2023-07-06 16:24:20.156283 pyrarecomb-0.0.1/PKG-INFO
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3025 2023-07-06 16:21:36.000000 pyrarecomb-0.0.1/README.md
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      107 2023-07-06 16:23:38.000000 pyrarecomb-0.0.1/pyproject.toml
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      651 2023-07-06 16:24:20.164936 pyrarecomb-0.0.1/setup.cfg
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 16:24:19.992896 pyrarecomb-0.0.1/src/
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 16:24:20.097577 pyrarecomb-0.0.1/src/pyrarecomb/
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-05 21:01:50.000000 pyrarecomb-0.0.1/src/pyrarecomb/__init__.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)    10379 2023-07-05 19:32:05.000000 pyrarecomb-0.0.1/src/pyrarecomb/compare_enrichment.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     9576 2023-07-05 19:31:26.000000 pyrarecomb-0.0.1/src/pyrarecomb/compare_enrichment_depletion.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)    10423 2023-07-05 19:30:47.000000 pyrarecomb-0.0.1/src/pyrarecomb/compare_enrichment_modifiers.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     6483 2023-07-03 16:24:22.000000 pyrarecomb-0.0.1/src/pyrarecomb/helpers.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     2766 2023-07-05 17:25:55.000000 pyrarecomb-0.0.1/src/pyrarecomb/run_apriori_freqitems.py
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 16:24:20.145944 pyrarecomb-0.0.1/src/pyrarecomb.egg-info/
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3507 2023-07-06 16:24:19.000000 pyrarecomb-0.0.1/src/pyrarecomb.egg-info/PKG-INFO
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      467 2023-07-06 16:24:19.000000 pyrarecomb-0.0.1/src/pyrarecomb.egg-info/SOURCES.txt
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        1 2023-07-06 16:24:19.000000 pyrarecomb-0.0.1/src/pyrarecomb.egg-info/dependency_links.txt
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       27 2023-07-06 16:24:19.000000 pyrarecomb-0.0.1/src/pyrarecomb.egg-info/requires.txt
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       11 2023-07-06 16:24:19.000000 pyrarecomb-0.0.1/src/pyrarecomb.egg-info/top_level.txt
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:30:56.251485 pyrarecomb-0.0.2/
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     1072 2023-07-05 20:39:51.000000 pyrarecomb-0.0.2/LICENSE
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       18 2023-07-06 16:16:04.000000 pyrarecomb-0.0.2/MANIFEST.in
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3555 2023-07-06 17:30:56.253662 pyrarecomb-0.0.2/PKG-INFO
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3074 2023-07-06 16:28:15.000000 pyrarecomb-0.0.2/README.md
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      107 2023-07-06 16:23:38.000000 pyrarecomb-0.0.2/pyproject.toml
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      651 2023-07-06 17:30:56.262014 pyrarecomb-0.0.2/setup.cfg
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:30:56.092705 pyrarecomb-0.0.2/src/
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:30:56.171525 pyrarecomb-0.0.2/src/pyrarecomb/
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-05 21:01:50.000000 pyrarecomb-0.0.2/src/pyrarecomb/__init__.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)    10396 2023-07-06 17:29:34.000000 pyrarecomb-0.0.2/src/pyrarecomb/compare_enrichment.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     9593 2023-07-06 17:29:52.000000 pyrarecomb-0.0.2/src/pyrarecomb/compare_enrichment_depletion.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)    10440 2023-07-06 17:29:48.000000 pyrarecomb-0.0.2/src/pyrarecomb/compare_enrichment_modifiers.py
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:30:56.242798 pyrarecomb-0.0.2/src/pyrarecomb/utils/
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:28:54.000000 pyrarecomb-0.0.2/src/pyrarecomb/utils/__init__.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     6483 2023-07-03 16:24:22.000000 pyrarecomb-0.0.2/src/pyrarecomb/utils/helpers.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     2766 2023-07-05 17:25:55.000000 pyrarecomb-0.0.2/src/pyrarecomb/utils/run_apriori_freqitems.py
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:30:56.216677 pyrarecomb-0.0.2/src/pyrarecomb.egg-info/
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3555 2023-07-06 17:30:56.000000 pyrarecomb-0.0.2/src/pyrarecomb.egg-info/PKG-INFO
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      512 2023-07-06 17:30:56.000000 pyrarecomb-0.0.2/src/pyrarecomb.egg-info/SOURCES.txt
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        1 2023-07-06 17:30:56.000000 pyrarecomb-0.0.2/src/pyrarecomb.egg-info/dependency_links.txt
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       27 2023-07-06 17:30:56.000000 pyrarecomb-0.0.2/src/pyrarecomb.egg-info/requires.txt
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       11 2023-07-06 17:30:56.000000 pyrarecomb-0.0.2/src/pyrarecomb.egg-info/top_level.txt
```

### Comparing `pyrarecomb-0.0.1/LICENSE` & `pyrarecomb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrarecomb-0.0.1/PKG-INFO` & `pyrarecomb-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrarecomb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python tool to identify oligogenic combinations of genes with rare variants
 Home-page: https://github.com/deeprob/pyrarecomb
 Author: Deepro Banerjee
 Author-email: deepro.2.4@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,8 +63,9 @@
 
 # Internal use
 ## Package creation
 ```bash
 $ python3 -m pip install --upgrade pip
 $ python3 -m pip install --upgrade build
 $ python3 -m pip install --upgrade twine
-$ 
+$ python -m build
+$ python3 -m twine upload dist/*
```

### Comparing `pyrarecomb-0.0.1/README.md` & `pyrarecomb-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,8 +49,9 @@
 
 # Internal use
 ## Package creation
 ```bash
 $ python3 -m pip install --upgrade pip
 $ python3 -m pip install --upgrade build
 $ python3 -m pip install --upgrade twine
-$ 
+$ python -m build
+$ python3 -m twine upload dist/*
```

### Comparing `pyrarecomb-0.0.1/setup.cfg` & `pyrarecomb-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrarecomb
-version = 0.0.1
+version = 0.0.2
 author = Deepro Banerjee
 author_email = deepro.2.4@gmail.com
 description = A python tool to identify oligogenic combinations of genes with rare variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/deeprob/pyrarecomb
 classifiers =
```

### Comparing `pyrarecomb-0.0.1/src/pyrarecomb/compare_enrichment.py` & `pyrarecomb-0.0.2/src/pyrarecomb/compare_enrichment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 from scipy.stats import binomtest
 from statsmodels.stats.multitest import multipletests
 
-from run_apriori_freqitems import run_apriori_freqitems
-import helpers as hp
+from utils.run_apriori_freqitems import run_apriori_freqitems
+from utils import helpers as hp
 
 
 def compare_enrichment(
         boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
         pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
         ):
     ##########
```

### Comparing `pyrarecomb-0.0.1/src/pyrarecomb/compare_enrichment_depletion.py` & `pyrarecomb-0.0.2/src/pyrarecomb/compare_enrichment_depletion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pandas as pd
 from collections import Counter
 from scipy.stats import binomtest
 from statsmodels.stats.multitest import multipletests
 
-from run_apriori_freqitems import run_apriori_freqitems
-import helpers as hp
+from utils.run_apriori_freqitems import run_apriori_freqitems
+from utils import helpers as hp
 
 
 def compare_enrichment_depletion(
         boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
         pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
         ):
     ##########
```

### Comparing `pyrarecomb-0.0.1/src/pyrarecomb/compare_enrichment_modifiers.py` & `pyrarecomb-0.0.2/src/pyrarecomb/compare_enrichment_modifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 from scipy.stats import binomtest
 from statsmodels.stats.multitest import multipletests
 
-from run_apriori_freqitems import run_apriori_freqitems
-import helpers as hp
+from utils.run_apriori_freqitems import run_apriori_freqitems
+from utils import helpers as hp
 
 
 def compare_enrichment_modifiers(
         boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
         primary_input_entities, pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
         ):
     ##########
```

### Comparing `pyrarecomb-0.0.1/src/pyrarecomb/helpers.py` & `pyrarecomb-0.0.2/src/pyrarecomb/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrarecomb-0.0.1/src/pyrarecomb/run_apriori_freqitems.py` & `pyrarecomb-0.0.2/src/pyrarecomb/utils/run_apriori_freqitems.py`

 * *Files identical despite different names*

### Comparing `pyrarecomb-0.0.1/src/pyrarecomb.egg-info/PKG-INFO` & `pyrarecomb-0.0.2/src/pyrarecomb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrarecomb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python tool to identify oligogenic combinations of genes with rare variants
 Home-page: https://github.com/deeprob/pyrarecomb
 Author: Deepro Banerjee
 Author-email: deepro.2.4@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,8 +63,9 @@
 
 # Internal use
 ## Package creation
 ```bash
 $ python3 -m pip install --upgrade pip
 $ python3 -m pip install --upgrade build
 $ python3 -m pip install --upgrade twine
-$ 
+$ python -m build
+$ python3 -m twine upload dist/*
```

