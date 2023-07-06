# Comparing `tmp/chunkdot-0.2.4.tar.gz` & `tmp/chunkdot-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunkdot-0.2.4.tar", max compression
+gzip compressed data, was "chunkdot-0.2.6.tar", max compression
```

## Comparing `chunkdot-0.2.4.tar` & `chunkdot-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     2869 2023-04-25 01:47:51.729168 chunkdot-0.2.4/README.md
--rw-r--r--   0        0        0      131 2023-04-25 01:49:13.433855 chunkdot-0.2.4/chunkdot/__init__.py
--rw-r--r--   0        0        0     3032 2023-04-24 10:44:08.694869 chunkdot-0.2.4/chunkdot/chunkdot.py
--rw-r--r--   0        0        0     7681 2023-04-24 10:44:18.808767 chunkdot-0.2.4/chunkdot/chunkdot_sparse.py
--rw-r--r--   0        0        0     3966 2023-04-24 10:47:15.290030 chunkdot-0.2.4/chunkdot/cosine_similarity_top_k.py
--rw-r--r--   0        0        0     4094 2023-04-24 10:34:50.140798 chunkdot-0.2.4/chunkdot/numba_argpartition.py
--rw-r--r--   0        0        0     4702 2023-04-24 10:34:50.142160 chunkdot-0.2.4/chunkdot/utils.py
--rw-r--r--   0        0        0     1141 2023-04-25 01:49:11.535003 chunkdot-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 chunkdot-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2869 2023-05-18 03:49:36.883362 chunkdot-0.2.6/README.md
+-rw-r--r--   0        0        0      131 2023-07-06 08:22:06.480537 chunkdot-0.2.6/chunkdot/__init__.py
+-rw-r--r--   0        0        0     2959 2023-07-06 08:15:12.157613 chunkdot-0.2.6/chunkdot/chunkdot.py
+-rw-r--r--   0        0        0     7681 2023-05-18 03:49:36.883994 chunkdot-0.2.6/chunkdot/chunkdot_sparse.py
+-rw-r--r--   0        0        0     3966 2023-05-18 03:49:36.884165 chunkdot-0.2.6/chunkdot/cosine_similarity_top_k.py
+-rw-r--r--   0        0        0     4629 2023-07-06 08:15:12.157956 chunkdot-0.2.6/chunkdot/utils.py
+-rw-r--r--   0        0        0     1141 2023-07-06 08:22:06.034332 chunkdot-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 chunkdot-0.2.6/PKG-INFO
```

### Comparing `chunkdot-0.2.4/README.md` & `chunkdot-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `chunkdot-0.2.4/chunkdot/chunkdot.py` & `chunkdot-0.2.6/chunkdot/chunkdot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import math
 
 import numpy as np
 from numba import njit, prange
 from numba_progress import ProgressBar
 from scipy.sparse import csr_matrix
 
-from chunkdot import numba_argpartition  # pylint: disable=unused-import
 from chunkdot.utils import to_sparse
 
 
 def warm_up_chunkdot():
     """Make a dummy run of the "chunkdot" function to compile it."""
     matrix = np.random.randn(10000, 100)
     chunkdot(matrix, matrix.T, 10, 5000)
```

### Comparing `chunkdot-0.2.4/chunkdot/chunkdot_sparse.py` & `chunkdot-0.2.6/chunkdot/chunkdot_sparse.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.2.4/chunkdot/cosine_similarity_top_k.py` & `chunkdot-0.2.6/chunkdot/cosine_similarity_top_k.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.2.4/chunkdot/utils.py` & `chunkdot-0.2.6/chunkdot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import warnings
 
 import numba
 from numba import njit
 import numpy as np
 import psutil
 
-from chunkdot import numba_argpartition  # pylint: disable=unused-import
 
 LOGGER = logging.getLogger(__name__)
 
 
 # Noting to parallelize in this function. It will raise an error if setting parallel to True since
 # the calling functions are already being parallelized.
 @njit(parallel=False)
```

### Comparing `chunkdot-0.2.4/pyproject.toml` & `chunkdot-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "chunkdot"
-version = "0.2.4"
+version = "0.2.6"
 description = "Multi-threaded matrix multiplication and cosine similarity calculations."
 authors = ["Rodrigo Agundez <rragundez@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/rragundez/chunkdot"
 classifiers = [
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-numba = "^0.56.4"
+numba = "^0.57.0"
 numpy = "^1.23"
 scipy = "^1.10.1"
 numba-progress = "^0.0.4"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 scikit-learn = "^1.2.1"
```

### Comparing `chunkdot-0.2.4/PKG-INFO` & `chunkdot-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: chunkdot
-Version: 0.2.4
+Version: 0.2.6
 Summary: Multi-threaded matrix multiplication and cosine similarity calculations.
 Home-page: https://github.com/rragundez/chunkdot
 Author: Rodrigo Agundez
 Author-email: rragundez@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Dist: numba (>=0.56.4,<0.57.0)
+Requires-Dist: numba (>=0.57.0,<0.58.0)
 Requires-Dist: numba-progress (>=0.0.4,<0.0.5)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Repository, https://github.com/rragundez/chunkdot
 Description-Content-Type: text/markdown
 
 # ChunkDot
```

