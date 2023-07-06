# Comparing `tmp/common_butia-0.0.1.tar.gz` & `tmp/common_butia-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_butia-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "common_butia-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `common_butia-0.0.1.tar` & `common_butia-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      255 2023-07-06 16:38:31.126442 common_butia-0.0.1/LICENSE
--rw-r--r--   0        0        0       14 2023-07-06 16:38:31.126442 common_butia-0.0.1/README.md
--rw-r--r--   0        0        0       94 2023-07-06 16:38:31.126442 common_butia-0.0.1/common-butia/__init__.py
--rw-r--r--   0        0        0     6944 2023-07-06 16:38:31.126442 common_butia-0.0.1/common-butia/common.py
--rw-r--r--   0        0        0      582 2023-07-06 16:38:31.514444 common_butia-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 common_butia-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-07-06 17:21:03.022745 common_butia-0.0.3/LICENSE
+-rw-r--r--   0        0        0       14 2023-07-06 17:21:03.022745 common_butia-0.0.3/README.md
+-rw-r--r--   0        0        0       95 2023-07-06 17:21:03.022745 common_butia-0.0.3/common_butia/__init__.py
+-rw-r--r--   0        0        0     6944 2023-07-06 17:21:03.022745 common_butia-0.0.3/common_butia/common.py
+-rw-r--r--   0        0        0      582 2023-07-06 17:21:03.426769 common_butia-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 common_butia-0.0.3/PKG-INFO
```

### Comparing `common_butia-0.0.1/common-butia/common.py` & `common_butia-0.0.3/common_butia/common.py`

 * *Files identical despite different names*

### Comparing `common_butia-0.0.1/pyproject.toml` & `common_butia-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "numpy",
     "pandas",
     "quantstats",
     "plotly"
 ]
 
 [tool.flit.module]
-name = "common-butia"
+name = "common_butia"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "mypy",
     "flake8",
 ]
```

### Comparing `common_butia-0.0.1/PKG-INFO` & `common_butia-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-butia
-Version: 0.0.1
+Version: 0.0.3
 Summary: A package bundling useful functions for backtesting financial data
 Author-email: Felipe Sadock <fsadock@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: quantstats
```

