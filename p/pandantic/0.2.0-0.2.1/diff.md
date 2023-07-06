# Comparing `tmp/pandantic-0.2.0.tar.gz` & `tmp/pandantic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandantic-0.2.0.tar", max compression
+gzip compressed data, was "pandantic-0.2.1.tar", max compression
```

## Comparing `pandantic-0.2.0.tar` & `pandantic-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3512 2023-05-02 19:16:57.940573 pandantic-0.2.0/README.md
--rw-r--r--   0        0        0      840 2023-05-02 19:16:59.720597 pandantic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      156 2023-05-02 19:16:57.940573 pandantic-0.2.0/src/pandantic/__init__.py
--rw-r--r--   0        0        0     4541 2023-05-02 19:16:57.940573 pandantic-0.2.0/src/pandantic/basemodel.py
--rw-r--r--   0        0        0     4029 1970-01-01 00:00:00.000000 pandantic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3419 2023-07-06 11:39:52.192189 pandantic-0.2.1/README.md
+-rw-r--r--   0        0        0      841 2023-07-06 11:39:53.948053 pandantic-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-07-06 11:39:52.192189 pandantic-0.2.1/src/pandantic/__init__.py
+-rw-r--r--   0        0        0     4541 2023-07-06 11:39:52.192189 pandantic-0.2.1/src/pandantic/basemodel.py
+-rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 pandantic-0.2.1/PKG-INFO
```

### Comparing `pandantic-0.2.0/README.md` & `pandantic-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -82,9 +82,8 @@
 
 df_raised_error = DataFrameSchema.parse_df(
     dataframe=example_df_invalid,
     errors="raise",
 )
 ```
 ## Docs
-
-Need to work on this, I know. I do wrote an [Medium blogpost](https://duckduckgo.com) about the usage and possibilites of the `pandantic` package (including some benchmarks).
+Documentation can be found [here](https://pandantic-rtd.readthedocs.io/en/latest/)
```

### Comparing `pandantic-0.2.0/pyproject.toml` & `pandantic-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pandantic"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["wessel.huising <wessel.huising@mollie.com>"]
 readme = "README.md"
 
 packages = [
     { include = "pandantic", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.0.0"
-pydantic = "2.0a2"
+pydantic = "^2.0.0"
 multiprocess = "^0.70.14"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pre-commit = "^3.2.2"
 black = "^23.3.0"
 pylint = "^2.17.2"
```

### Comparing `pandantic-0.2.0/src/pandantic/basemodel.py` & `pandantic-0.2.1/src/pandantic/basemodel.py`

 * *Files identical despite different names*

### Comparing `pandantic-0.2.0/PKG-INFO` & `pandantic-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pandantic
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: wessel.huising
 Author-email: wessel.huising@mollie.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: pydantic (==2.0a2)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pandantic
 
 `pandantic` introduces the ability to validate (`pandas`) DataFrames using `pydantic.BaseModel`s. The `pandantic` package is using the V2 version of `pydantic` as it has significant improvements over its V1 versions (a performance increase up to 50 times).
 
 First, install `pandantic` by using pip (or any other package managing tool).
@@ -98,10 +98,9 @@
 
 df_raised_error = DataFrameSchema.parse_df(
     dataframe=example_df_invalid,
     errors="raise",
 )
 ```
 ## Docs
-
-Need to work on this, I know. I do wrote an [Medium blogpost](https://duckduckgo.com) about the usage and possibilites of the `pandantic` package (including some benchmarks).
+Documentation can be found [here](https://pandantic-rtd.readthedocs.io/en/latest/)
```

