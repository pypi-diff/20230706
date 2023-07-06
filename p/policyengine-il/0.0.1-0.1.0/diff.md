# Comparing `tmp/policyengine-il-0.0.1.tar.gz` & `tmp/policyengine-il-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyengine-il-0.0.1.tar", last modified: Wed Jul  5 14:09:09 2023, max compression
+gzip compressed data, was "policyengine-il-0.1.0.tar", last modified: Thu Jul  6 16:37:41 2023, max compression
```

## Comparing `policyengine-il-0.0.1.tar` & `policyengine-il-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/policyengine_il/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/modelled_policies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.156921 policyengine-il-0.0.1/policyengine_il/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/policyengine_il/parameters/gov/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/parameters/gov/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/policyengine_il/parameters/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/parameters/simulation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/parameters/simulation/marginal_tax_rate_adults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/policyengine_il/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/age.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/employment_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/gross_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/household_benefits.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/household_market_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/household_net_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/household_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/policyengine_il/variables/input/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/input/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/policyengine_il/variables/input/demographic/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/input/demographic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/input/demographic/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/is_adult.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/market_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/policyengine_il/variables/tax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/policyengine_il.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-05 14:09:09.000000 policyengine-il-0.0.1/policyengine_il.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-05 14:09:09.000000 policyengine-il-0.0.1/policyengine_il.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:09:09.000000 policyengine-il-0.0.1/policyengine_il.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-05 14:09:09.000000 policyengine-il-0.0.1/policyengine_il.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 14:09:09.000000 policyengine-il-0.0.1/policyengine_il.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 14:09:09.000000 policyengine-il-0.0.1/policyengine_il.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:09:09.160921 policyengine-il-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-05 14:08:16.000000 policyengine-il-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.640693 policyengine-il-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-06 16:37:41.640693 policyengine-il-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/modelled_policies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/parameters/gov/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/parameters/gov/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/parameters/gov/low_income_municipal_tax_reduction_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/parameters/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/parameters/simulation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/parameters/simulation/marginal_tax_rate_adults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/tests/household_net_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/tests/max_low_income_municipal_tax_reduction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/tests/max_low_income_municipal_tax_reduction_rate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/employment_income.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/variables/gov/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/variables/gov/low_income_municipal_tax_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/gov/low_income_municipal_tax_reduction/low_income_municipal_tax_reduction_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/gov/low_income_municipal_tax_reduction/max_low_income_municipal_tax_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/gov/low_income_municipal_tax_reduction/max_low_income_municipal_tax_reduction_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/gov/municipal_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/gross_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/household_benefits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/household_market_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/household_net_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/household_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/household_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il/variables/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/input/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.640693 policyengine-il-0.1.0/policyengine_il/variables/input/demographic/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/input/demographic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/input/demographic/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/is_adult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/market_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/pension_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/self_employment_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/policyengine_il/variables/tax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:37:41.636692 policyengine-il-0.1.0/policyengine_il.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-06 16:37:41.000000 policyengine-il-0.1.0/policyengine_il.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-06 16:37:41.000000 policyengine-il-0.1.0/policyengine_il.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:37:41.000000 policyengine-il-0.1.0/policyengine_il.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 16:37:41.000000 policyengine-il-0.1.0/policyengine_il.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 16:37:41.000000 policyengine-il-0.1.0/policyengine_il.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 16:37:41.000000 policyengine-il-0.1.0/policyengine_il.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:37:41.640693 policyengine-il-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-06 16:36:45.000000 policyengine-il-0.1.0/setup.py
```

### Comparing `policyengine-il-0.0.1/LICENSE` & `policyengine-il-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `policyengine-il-0.0.1/PKG-INFO` & `policyengine-il-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-il
-Version: 0.0.1
+Version: 0.1.0
 Summary: Core microsimulation engine enabling country-specific policy models.
 Home-page: https://github.com/policyengine/policyengine-core
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-il-0.0.1/policyengine_il/__init__.py` & `policyengine-il-0.1.0/policyengine_il/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-il-0.0.1/policyengine_il/entities.py` & `policyengine-il-0.1.0/policyengine_il/entities.py`

 * *Files identical despite different names*

### Comparing `policyengine-il-0.0.1/policyengine_il/variables/marginal_tax_rate.py` & `policyengine-il-0.1.0/policyengine_il/variables/marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `policyengine-il-0.0.1/policyengine_il.egg-info/PKG-INFO` & `policyengine-il-0.1.0/policyengine_il.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-il
-Version: 0.0.1
+Version: 0.1.0
 Summary: Core microsimulation engine enabling country-specific policy models.
 Home-page: https://github.com/policyengine/policyengine-core
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-il-0.0.1/setup.py` & `policyengine-il-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "sphinx>=4.5.0,<5",
     "sphinx-argparse>=0.3.2,<1",
     "sphinx-math-dollar>=1.2.1,<2",
 ]
 
 setup(
     name="policyengine-il",
-    version="0.0.1",
+    version="0.1.0",
     author="PolicyEngine",
     author_email="hello@policyengine.org",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
```

