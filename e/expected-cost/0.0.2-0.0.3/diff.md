# Comparing `tmp/expected_cost-0.0.2.tar.gz` & `tmp/expected_cost-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expected_cost-0.0.2.tar", last modified: Thu Jun 29 12:19:21 2023, max compression
+gzip compressed data, was "expected_cost-0.0.3.tar", last modified: Thu Jul  6 12:43:53 2023, max compression
```

## Comparing `expected_cost-0.0.2.tar` & `expected_cost-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-06-29 12:19:21.093452 expected_cost-0.0.2/
--rw-r--r--   0 lferrer    (501) staff       (20)    35149 2023-05-23 20:28:51.000000 expected_cost-0.0.2/LICENSE
--rw-r--r--   0 lferrer    (501) staff       (20)     4110 2023-06-29 12:19:21.093624 expected_cost-0.0.2/PKG-INFO
--rw-r--r--   0 lferrer    (501) staff       (20)     3590 2023-06-28 15:01:52.000000 expected_cost-0.0.2/README.md
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-06-29 12:19:21.065439 expected_cost-0.0.2/expected_cost/
--rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-22 14:36:03.000000 expected_cost-0.0.2/expected_cost/__init__.py
--rw-r--r--   0 lferrer    (501) staff       (20)     4279 2023-06-15 20:46:03.000000 expected_cost-0.0.2/expected_cost/calibration.py
--rw-r--r--   0 lferrer    (501) staff       (20)    11682 2023-06-28 15:43:42.000000 expected_cost-0.0.2/expected_cost/data.py
--rw-r--r--   0 lferrer    (501) staff       (20)    22199 2023-06-28 15:22:16.000000 expected_cost-0.0.2/expected_cost/ec.py
--rw-r--r--   0 lferrer    (501) staff       (20)     1480 2023-06-27 13:26:21.000000 expected_cost-0.0.2/expected_cost/psrcal_wrappers.py
--rw-r--r--   0 lferrer    (501) staff       (20)     7531 2023-06-21 19:56:14.000000 expected_cost-0.0.2/expected_cost/utils.py
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-06-29 12:19:21.068419 expected_cost-0.0.2/expected_cost.egg-info/
--rw-r--r--   0 lferrer    (501) staff       (20)     4110 2023-06-29 12:19:21.000000 expected_cost-0.0.2/expected_cost.egg-info/PKG-INFO
--rw-r--r--   0 lferrer    (501) staff       (20)      693 2023-06-29 12:19:21.000000 expected_cost-0.0.2/expected_cost.egg-info/SOURCES.txt
--rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-29 12:19:21.000000 expected_cost-0.0.2/expected_cost.egg-info/dependency_links.txt
--rw-r--r--   0 lferrer    (501) staff       (20)       65 2023-06-29 12:19:21.000000 expected_cost-0.0.2/expected_cost.egg-info/requires.txt
--rw-r--r--   0 lferrer    (501) staff       (20)       31 2023-06-29 12:19:21.000000 expected_cost-0.0.2/expected_cost.egg-info/top_level.txt
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-06-29 12:19:21.069119 expected_cost-0.0.2/notebooks/
--rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-22 14:55:57.000000 expected_cost-0.0.2/notebooks/__init__.py
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-06-29 12:19:21.079625 expected_cost-0.0.2/psrcal/
--rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.2/psrcal/__init.__.py
--rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.2/psrcal/__init__.py
--rw-r--r--   0 lferrer    (501) staff       (20)     5536 2023-06-28 12:01:53.000000 expected_cost-0.0.2/psrcal/calibration.py
--rw-r--r--   0 lferrer    (501) staff       (20)     8885 2023-06-28 12:02:00.000000 expected_cost-0.0.2/psrcal/losses.py
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-06-29 12:19:21.090740 expected_cost-0.0.2/psrcal/optim/
--rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.2/psrcal/optim/__init__.py
--rw-r--r--   0 lferrer    (501) staff       (20)      504 2023-06-08 15:20:51.000000 expected_cost-0.0.2/psrcal/optim/example.py
--rw-r--r--   0 lferrer    (501) staff       (20)     1768 2023-06-08 15:20:51.000000 expected_cost-0.0.2/psrcal/optim/fullbatch_optim.py
--rw-r--r--   0 lferrer    (501) staff       (20)     3514 2023-06-08 15:20:51.000000 expected_cost-0.0.2/psrcal/optim/vecmodule.py
--rw-r--r--   0 lferrer    (501) staff       (20)      567 2023-06-08 15:20:51.000000 expected_cost-0.0.2/psrcal/psr.py
--rw-r--r--   0 lferrer    (501) staff       (20)      706 2023-06-08 15:20:51.000000 expected_cost-0.0.2/psrcal/utils.py
--rw-r--r--   0 lferrer    (501) staff       (20)       84 2023-06-22 15:01:18.000000 expected_cost-0.0.2/pyproject.toml
--rw-r--r--   0 lferrer    (501) staff       (20)      727 2023-06-29 12:19:21.094401 expected_cost-0.0.2/setup.cfg
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-06-29 12:19:21.092517 expected_cost-0.0.2/test/
--rw-r--r--   0 lferrer    (501) staff       (20)      850 2023-06-28 15:25:15.000000 expected_cost-0.0.2/test/test.py
--rw-r--r--   0 lferrer    (501) staff       (20)      782 2023-06-28 15:46:12.000000 expected_cost-0.0.2/test/test_psrcal.py
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-07-06 12:43:53.697190 expected_cost-0.0.3/
+-rw-r--r--   0 lferrer    (501) staff       (20)     1071 2023-07-05 13:01:22.000000 expected_cost-0.0.3/LICENSE.md
+-rw-r--r--   0 lferrer    (501) staff       (20)     4087 2023-07-06 12:43:53.697358 expected_cost-0.0.3/PKG-INFO
+-rw-r--r--   0 lferrer    (501) staff       (20)     3590 2023-06-28 15:01:52.000000 expected_cost-0.0.3/README.md
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-07-06 12:43:53.664430 expected_cost-0.0.3/expected_cost/
+-rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-22 14:36:03.000000 expected_cost-0.0.3/expected_cost/__init__.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     4279 2023-06-15 20:46:03.000000 expected_cost-0.0.3/expected_cost/calibration.py
+-rw-r--r--   0 lferrer    (501) staff       (20)    11682 2023-06-28 15:43:42.000000 expected_cost-0.0.3/expected_cost/data.py
+-rw-r--r--   0 lferrer    (501) staff       (20)    22199 2023-06-28 15:22:16.000000 expected_cost-0.0.3/expected_cost/ec.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     1480 2023-06-27 13:26:21.000000 expected_cost-0.0.3/expected_cost/psrcal_wrappers.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     7531 2023-06-21 19:56:14.000000 expected_cost-0.0.3/expected_cost/utils.py
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-07-06 12:43:53.668626 expected_cost-0.0.3/expected_cost.egg-info/
+-rw-r--r--   0 lferrer    (501) staff       (20)     4087 2023-07-06 12:43:53.000000 expected_cost-0.0.3/expected_cost.egg-info/PKG-INFO
+-rw-r--r--   0 lferrer    (501) staff       (20)      696 2023-07-06 12:43:53.000000 expected_cost-0.0.3/expected_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-07-06 12:43:53.000000 expected_cost-0.0.3/expected_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 lferrer    (501) staff       (20)       65 2023-07-06 12:43:53.000000 expected_cost-0.0.3/expected_cost.egg-info/requires.txt
+-rw-r--r--   0 lferrer    (501) staff       (20)       31 2023-07-06 12:43:53.000000 expected_cost-0.0.3/expected_cost.egg-info/top_level.txt
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-07-06 12:43:53.669046 expected_cost-0.0.3/notebooks/
+-rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-22 14:55:57.000000 expected_cost-0.0.3/notebooks/__init__.py
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-07-06 12:43:53.681933 expected_cost-0.0.3/psrcal/
+-rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.3/psrcal/__init.__.py
+-rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.3/psrcal/__init__.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     5536 2023-06-28 12:01:53.000000 expected_cost-0.0.3/psrcal/calibration.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     8885 2023-06-28 12:02:00.000000 expected_cost-0.0.3/psrcal/losses.py
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-07-06 12:43:53.695049 expected_cost-0.0.3/psrcal/optim/
+-rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.3/psrcal/optim/__init__.py
+-rw-r--r--   0 lferrer    (501) staff       (20)      504 2023-06-08 15:20:51.000000 expected_cost-0.0.3/psrcal/optim/example.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     1768 2023-06-08 15:20:51.000000 expected_cost-0.0.3/psrcal/optim/fullbatch_optim.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     3514 2023-06-08 15:20:51.000000 expected_cost-0.0.3/psrcal/optim/vecmodule.py
+-rw-r--r--   0 lferrer    (501) staff       (20)      567 2023-06-08 15:20:51.000000 expected_cost-0.0.3/psrcal/psr.py
+-rw-r--r--   0 lferrer    (501) staff       (20)      706 2023-06-08 15:20:51.000000 expected_cost-0.0.3/psrcal/utils.py
+-rw-r--r--   0 lferrer    (501) staff       (20)       84 2023-06-22 15:01:18.000000 expected_cost-0.0.3/pyproject.toml
+-rw-r--r--   0 lferrer    (501) staff       (20)      701 2023-07-06 12:43:53.697960 expected_cost-0.0.3/setup.cfg
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-07-06 12:43:53.696474 expected_cost-0.0.3/test/
+-rw-r--r--   0 lferrer    (501) staff       (20)      850 2023-06-28 15:25:15.000000 expected_cost-0.0.3/test/test.py
+-rw-r--r--   0 lferrer    (501) staff       (20)      782 2023-06-28 15:46:12.000000 expected_cost-0.0.3/test/test_psrcal.py
```

### Comparing `expected_cost-0.0.2/PKG-INFO` & `expected_cost-0.0.3/expected_cost.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: expected_cost
-Version: 0.0.2
+Name: expected-cost
+Version: 0.0.3
 Summary: Methods for computing the expected cost metric for evaluation of classification systems
 Home-page: https://github.com/luferrer/expected_cost
 Author: Luciana Ferrer
 Author-email: lferrer@dc.uba.ar
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 
 # Expected cost
 
 Methods for computing the expected cost (EC) on an evaluation dataset, as defined in statistical learning text books (e.g., Bishop's "Pattern recognition and machine learning", and Hastie's et al "The elements of statistical learning"). 
 Given a matrix of user-defined costs with elements $c_{y\ d}$, where $y$ is the true class of a sample and $d$ is the decision made by the system for that sample, 
 this metric is estimated as the average of the costs across all samples in the dataset. That is:
```

### Comparing `expected_cost-0.0.2/README.md` & `expected_cost-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/expected_cost/calibration.py` & `expected_cost-0.0.3/expected_cost/calibration.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/expected_cost/data.py` & `expected_cost-0.0.3/expected_cost/data.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/expected_cost/ec.py` & `expected_cost-0.0.3/expected_cost/ec.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/expected_cost/psrcal_wrappers.py` & `expected_cost-0.0.3/expected_cost/psrcal_wrappers.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/expected_cost/utils.py` & `expected_cost-0.0.3/expected_cost/utils.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/expected_cost.egg-info/PKG-INFO` & `expected_cost-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: expected-cost
-Version: 0.0.2
+Name: expected_cost
+Version: 0.0.3
 Summary: Methods for computing the expected cost metric for evaluation of classification systems
 Home-page: https://github.com/luferrer/expected_cost
 Author: Luciana Ferrer
 Author-email: lferrer@dc.uba.ar
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 
 # Expected cost
 
 Methods for computing the expected cost (EC) on an evaluation dataset, as defined in statistical learning text books (e.g., Bishop's "Pattern recognition and machine learning", and Hastie's et al "The elements of statistical learning"). 
 Given a matrix of user-defined costs with elements $c_{y\ d}$, where $y$ is the true class of a sample and $d$ is the decision made by the system for that sample, 
 this metric is estimated as the average of the costs across all samples in the dataset. That is:
```

### Comparing `expected_cost-0.0.2/expected_cost.egg-info/SOURCES.txt` & `expected_cost-0.0.3/expected_cost.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE
+LICENSE.md
 README.md
 pyproject.toml
 setup.cfg
 ./expected_cost/__init__.py
 ./expected_cost/calibration.py
 ./expected_cost/data.py
 ./expected_cost/ec.py
```

### Comparing `expected_cost-0.0.2/psrcal/calibration.py` & `expected_cost-0.0.3/psrcal/calibration.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/psrcal/losses.py` & `expected_cost-0.0.3/psrcal/losses.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/psrcal/optim/fullbatch_optim.py` & `expected_cost-0.0.3/psrcal/optim/fullbatch_optim.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/psrcal/optim/vecmodule.py` & `expected_cost-0.0.3/psrcal/optim/vecmodule.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/psrcal/psr.py` & `expected_cost-0.0.3/psrcal/psr.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/psrcal/utils.py` & `expected_cost-0.0.3/psrcal/utils.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/setup.cfg` & `expected_cost-0.0.3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = expected_cost
-version = 0.0.2
+version = 0.0.3
 author = Luciana Ferrer
 author_email = lferrer@dc.uba.ar
 description = Methods for computing the expected cost metric for evaluation of classification systems
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/luferrer/expected_cost
 classifiers = 
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= ./
 packages = find:
 python_requires = >=3.6
```

### Comparing `expected_cost-0.0.2/test/test.py` & `expected_cost-0.0.3/test/test.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.2/test/test_psrcal.py` & `expected_cost-0.0.3/test/test_psrcal.py`

 * *Files identical despite different names*

