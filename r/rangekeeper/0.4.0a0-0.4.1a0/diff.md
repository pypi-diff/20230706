# Comparing `tmp/rangekeeper-0.4.0a0.tar.gz` & `tmp/rangekeeper-0.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rangekeeper-0.4.0a0.tar", max compression
+gzip compressed data, was "rangekeeper-0.4.1a0.tar", max compression
```

## Comparing `rangekeeper-0.4.0a0.tar` & `rangekeeper-0.4.1a0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0    16725 2023-05-17 15:02:56.622311 rangekeeper-0.4.0a0/LICENSE
--rwxr-xr-x   0        0        0     1615 2023-06-16 00:51:56.463723 rangekeeper-0.4.0a0/README.md
--rwxr-xr-x   0        0        0     1107 2023-07-03 04:31:13.220499 rangekeeper-0.4.0a0/pyproject.toml
--rwxr-xr-x   0        0        0     1742 2023-06-16 00:51:56.561615 rangekeeper-0.4.0a0/rangekeeper/__init__.py
--rwxr-xr-x   0        0        0     4790 2023-06-25 13:20:04.785577 rangekeeper-0.4.0a0/rangekeeper/api.py
--rwxr-xr-x   0        0        0     9159 2023-05-17 15:02:56.651782 rangekeeper-0.4.0a0/rangekeeper/distribution.py
--rwxr-xr-x   0        0        0      207 2023-05-17 15:02:56.651889 rangekeeper-0.4.0a0/rangekeeper/dynamics/__init__.py
--rwxr-xr-x   0        0        0     2512 2023-05-17 15:02:56.651986 rangekeeper-0.4.0a0/rangekeeper/dynamics/black_swan.py
--rwxr-xr-x   0        0        0    16122 2023-06-16 00:51:56.562003 rangekeeper-0.4.0a0/rangekeeper/dynamics/cyclicality.py
--rwxr-xr-x   0        0        0    14841 2023-05-17 15:02:56.652228 rangekeeper-0.4.0a0/rangekeeper/dynamics/market.py
--rwxr-xr-x   0        0        0     1320 2023-05-17 15:02:56.652316 rangekeeper-0.4.0a0/rangekeeper/dynamics/noise.py
--rwxr-xr-x   0        0        0     2361 2023-05-17 15:02:56.652407 rangekeeper-0.4.0a0/rangekeeper/dynamics/trend.py
--rwxr-xr-x   0        0        0     5158 2023-05-17 15:02:56.652500 rangekeeper-0.4.0a0/rangekeeper/dynamics/volatility.py
--rwxr-xr-x   0        0        0     2974 2023-05-17 15:02:56.652595 rangekeeper-0.4.0a0/rangekeeper/extrapolation.py
--rwxr-xr-x   0        0        0    25969 2023-06-29 14:34:44.921352 rangekeeper-0.4.0a0/rangekeeper/flux.py
--rwxr-xr-x   0        0        0    27006 2023-06-30 03:17:42.028832 rangekeeper-0.4.0a0/rangekeeper/graph.py
--rwxr-xr-x   0        0        0     4138 2023-05-17 15:02:56.653017 rangekeeper-0.4.0a0/rangekeeper/measure.py
--rwxr-xr-x   0        0        0      199 2023-05-17 15:02:56.653120 rangekeeper-0.4.0a0/rangekeeper/models/__init__.py
--rwxr-xr-x   0        0        0     5461 2023-05-17 15:02:56.653249 rangekeeper-0.4.0a0/rangekeeper/models/deterministic.py
--rwxr-xr-x   0        0        0     6878 2023-05-17 15:02:56.653370 rangekeeper-0.4.0a0/rangekeeper/models/flexible.py
--rwxr-xr-x   0        0        0     5627 2023-05-17 15:02:56.653494 rangekeeper-0.4.0a0/rangekeeper/models/linear.py
--rwxr-xr-x   0        0        0     6389 2023-05-17 15:02:56.653612 rangekeeper-0.4.0a0/rangekeeper/models/linear_graph.py
--rwxr-xr-x   0        0        0     6116 2023-05-17 15:02:56.653737 rangekeeper-0.4.0a0/rangekeeper/models/probabilistic.py
--rwxr-xr-x   0        0        0     8591 2023-06-29 14:34:44.924722 rangekeeper-0.4.0a0/rangekeeper/periodicity.py
--rw-r--r--   0        0        0      567 2023-06-16 00:51:56.562404 rangekeeper-0.4.0a0/rangekeeper/policy.py
--rwxr-xr-x   0        0        0     8891 2023-06-29 14:34:44.925138 rangekeeper-0.4.0a0/rangekeeper/projection.py
--rwxr-xr-x   0        0        0     6856 2023-05-17 15:02:56.654323 rangekeeper-0.4.0a0/rangekeeper/segmentation.py
--rwxr-xr-x   0        0        0     1163 2023-06-16 00:51:56.562561 rangekeeper-0.4.0a0/rangekeeper/space.py
--rwxr-xr-x   0        0        0     7738 2023-06-29 14:34:44.925484 rangekeeper-0.4.0a0/rangekeeper/span.py
--rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 rangekeeper-0.4.0a0/PKG-INFO
+-rwxr-xr-x   0        0        0    16725 2023-05-17 15:02:56.622311 rangekeeper-0.4.1a0/LICENSE
+-rwxr-xr-x   0        0        0     1954 2023-07-06 03:41:45.379980 rangekeeper-0.4.1a0/README.md
+-rwxr-xr-x   0        0        0     1086 2023-07-06 05:17:40.678911 rangekeeper-0.4.1a0/pyproject.toml
+-rwxr-xr-x   0        0        0     1742 2023-06-16 00:51:56.561615 rangekeeper-0.4.1a0/rangekeeper/__init__.py
+-rwxr-xr-x   0        0        0     4790 2023-06-25 13:20:04.785577 rangekeeper-0.4.1a0/rangekeeper/api.py
+-rwxr-xr-x   0        0        0     9159 2023-05-17 15:02:56.651782 rangekeeper-0.4.1a0/rangekeeper/distribution.py
+-rwxr-xr-x   0        0        0      207 2023-05-17 15:02:56.651889 rangekeeper-0.4.1a0/rangekeeper/dynamics/__init__.py
+-rwxr-xr-x   0        0        0     2512 2023-05-17 15:02:56.651986 rangekeeper-0.4.1a0/rangekeeper/dynamics/black_swan.py
+-rwxr-xr-x   0        0        0    16122 2023-06-16 00:51:56.562003 rangekeeper-0.4.1a0/rangekeeper/dynamics/cyclicality.py
+-rwxr-xr-x   0        0        0    14841 2023-05-17 15:02:56.652228 rangekeeper-0.4.1a0/rangekeeper/dynamics/market.py
+-rwxr-xr-x   0        0        0     1320 2023-05-17 15:02:56.652316 rangekeeper-0.4.1a0/rangekeeper/dynamics/noise.py
+-rwxr-xr-x   0        0        0     2361 2023-05-17 15:02:56.652407 rangekeeper-0.4.1a0/rangekeeper/dynamics/trend.py
+-rwxr-xr-x   0        0        0     5158 2023-05-17 15:02:56.652500 rangekeeper-0.4.1a0/rangekeeper/dynamics/volatility.py
+-rwxr-xr-x   0        0        0     2974 2023-05-17 15:02:56.652595 rangekeeper-0.4.1a0/rangekeeper/extrapolation.py
+-rwxr-xr-x   0        0        0    25969 2023-06-29 14:34:44.921352 rangekeeper-0.4.1a0/rangekeeper/flux.py
+-rwxr-xr-x   0        0        0    27006 2023-07-06 03:41:45.390518 rangekeeper-0.4.1a0/rangekeeper/graph.py
+-rwxr-xr-x   0        0        0     4138 2023-05-17 15:02:56.653017 rangekeeper-0.4.1a0/rangekeeper/measure.py
+-rwxr-xr-x   0        0        0      199 2023-05-17 15:02:56.653120 rangekeeper-0.4.1a0/rangekeeper/models/__init__.py
+-rwxr-xr-x   0        0        0     5461 2023-05-17 15:02:56.653249 rangekeeper-0.4.1a0/rangekeeper/models/deterministic.py
+-rwxr-xr-x   0        0        0     6878 2023-05-17 15:02:56.653370 rangekeeper-0.4.1a0/rangekeeper/models/flexible.py
+-rwxr-xr-x   0        0        0     5627 2023-05-17 15:02:56.653494 rangekeeper-0.4.1a0/rangekeeper/models/linear.py
+-rwxr-xr-x   0        0        0     6389 2023-05-17 15:02:56.653612 rangekeeper-0.4.1a0/rangekeeper/models/linear_graph.py
+-rwxr-xr-x   0        0        0     6116 2023-05-17 15:02:56.653737 rangekeeper-0.4.1a0/rangekeeper/models/probabilistic.py
+-rwxr-xr-x   0        0        0     8591 2023-06-29 14:34:44.924722 rangekeeper-0.4.1a0/rangekeeper/periodicity.py
+-rw-r--r--   0        0        0      567 2023-06-16 00:51:56.562404 rangekeeper-0.4.1a0/rangekeeper/policy.py
+-rwxr-xr-x   0        0        0     8891 2023-06-29 14:34:44.925138 rangekeeper-0.4.1a0/rangekeeper/projection.py
+-rwxr-xr-x   0        0        0     6856 2023-05-17 15:02:56.654323 rangekeeper-0.4.1a0/rangekeeper/segmentation.py
+-rwxr-xr-x   0        0        0     1163 2023-06-16 00:51:56.562561 rangekeeper-0.4.1a0/rangekeeper/space.py
+-rwxr-xr-x   0        0        0     7738 2023-06-29 14:34:44.925484 rangekeeper-0.4.1a0/rangekeeper/span.py
+-rw-r--r--   0        0        0     3489 1970-01-01 00:00:00.000000 rangekeeper-0.4.1a0/PKG-INFO
```

### Comparing `rangekeeper-0.4.0a0/LICENSE` & `rangekeeper-0.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/README.md` & `rangekeeper-0.4.1a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,45 @@
 <img src="https://github.com/daniel-fink/rangekeeper/blob/v0.2.0/walkthrough/resources/rangekeeper.jpg?raw=true" width="300">
 
 # Rangekeeper
-Rangekeeper is a library assisting financial modelling in real estate scenario planning, decision-making, cashflow forecasting, and the like.
+Rangekeeper is an open-source library for financial modelling in real estate 
+asset & development planning, decision-making, cashflow forecasting, and 
+scenario analysis.
+
+Rangekeeper enables real estate valuation at all stages and resolutions of 
+description — from early-stage ‘back-of-the-envelope’ models to detailed 
+commercial assessments, and can be completely synchronised with 3D design, 
+engineering, and logistics modelling.
+
+It decomposes elements of the Discounted Cash Flow (DCF) Proforma modelling 
+approach into recomposable code functions that can be wired together to form a 
+full model. More elaborate and worked-through examples of these classes and 
+functions can be found in the [walkthrough documentation](https://daniel-fink.github.io/rangekeeper/).
 
-It decomposes elements of the Discounted Cash Flow (DCF) Proforma modelling approach into recomposable code functions that can be wired together to form a full model. More elaborate and worked-through examples of these classes and functions can be found in the [walkthrough documentation](https://daniel-fink.github.io/rangekeeper/).
+Development of the library follows the rigorous methodology established by 
+Profs Geltner and de Neufville in their book [Flexibility and Real Estate Valuation under Uncertainty: A Practical Guide for Developers](https://doi.org/10.1002/9781119106470).
 
-Development of the library follows the rigorous methodology established by Profs Geltner and de Neufville in their book [Flexibility and Real Estate Valuation under Uncertainty: A Practical Guide for Developers](https://doi.org/10.1002/9781119106470).
 
-## Dependencies:
+## Installation
+`pip install rangekeeper` or `poetry add rangekeeper`
+
+
+## Development
+
+### Dependencies
 
 - Python >= 3.9 & < 3.11
 
-- Poetry: <https://python-poetry.org/>, a package manager (although it is possible to roll your own; YMMV)
+- Poetry: <https://python-poetry.org/>, a package manager (although it is 
+possible to roll your own; YMMV)
 
-## Installation
+### Environment Setup
 
 1. Install poetry, if you haven't yet: <https://python-poetry.org/docs/master/#installing-with-the-official-installer>
 
 2. Clone this repo.
 
 3. Use a terminal to install poetry packages from the repo's directory: `<path_to_repo>$ poetry install`
 
-4. Currently, this library is not yet available on Python Package Index (PyPI). If you wish to use this repo with other projects locally, you may install the Rangekeeper library via `<path_to_repo>$ poetry run pip install -e <path_to_rangekeeper_repo>`, replacing `<path_to_rangekeeper_repo>` with its location on your system.
+4. If you wish to develop this repo alongside other projects locally, you may 
+install the local Rangekeeper library via `<path_to_repo>$ poetry run pip install -e <path_to_rangekeeper_repo>`,
+replacing `<path_to_rangekeeper_repo>` with its location on your system.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rangekeeper-0.4.0a0/pyproject.toml` & `rangekeeper-0.4.1a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Rangekeeper"
-version = "0.4.0-alpha"
+version = "0.4.1-alpha"
 description = "A Python library assisting financial modelling in scenario planning, decision-making, cashflow forecasting, and the like"
 authors = ["Daniel Fink <danfink@mit.edu>"]
 license = "MPL-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
@@ -26,15 +26,14 @@
 jupyterlab = "^4.0.0"
 docutils = "0.17.1" # See https://jupyterbook.org/en/stable/content/citations.html#citations-and-bibliographies
 tqdm = "^4.65.0"
 multiprocess = "^0.70.14"
 seaborn = "^0.12.2"
 jupyter-book = "^0.15.1"
 sphinx-rtd-theme = "^1.2.0"
-pygraphviz = "^1.11"
 pyvis = "^0.3.2"
 plotly = "^5.15.0"
 pyppeteer = "^1.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
```

### Comparing `rangekeeper-0.4.0a0/rangekeeper/__init__.py` & `rangekeeper-0.4.1a0/rangekeeper/__init__.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/api.py` & `rangekeeper-0.4.1a0/rangekeeper/api.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/distribution.py` & `rangekeeper-0.4.1a0/rangekeeper/distribution.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/dynamics/black_swan.py` & `rangekeeper-0.4.1a0/rangekeeper/dynamics/black_swan.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/dynamics/cyclicality.py` & `rangekeeper-0.4.1a0/rangekeeper/dynamics/cyclicality.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/dynamics/market.py` & `rangekeeper-0.4.1a0/rangekeeper/dynamics/market.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/dynamics/noise.py` & `rangekeeper-0.4.1a0/rangekeeper/dynamics/noise.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/dynamics/trend.py` & `rangekeeper-0.4.1a0/rangekeeper/dynamics/trend.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/dynamics/volatility.py` & `rangekeeper-0.4.1a0/rangekeeper/dynamics/volatility.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/extrapolation.py` & `rangekeeper-0.4.1a0/rangekeeper/extrapolation.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/flux.py` & `rangekeeper-0.4.1a0/rangekeeper/flux.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/graph.py` & `rangekeeper-0.4.1a0/rangekeeper/graph.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/measure.py` & `rangekeeper-0.4.1a0/rangekeeper/measure.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/models/deterministic.py` & `rangekeeper-0.4.1a0/rangekeeper/models/deterministic.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/models/flexible.py` & `rangekeeper-0.4.1a0/rangekeeper/models/flexible.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/models/linear.py` & `rangekeeper-0.4.1a0/rangekeeper/models/linear.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/models/linear_graph.py` & `rangekeeper-0.4.1a0/rangekeeper/models/linear_graph.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/models/probabilistic.py` & `rangekeeper-0.4.1a0/rangekeeper/models/probabilistic.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/periodicity.py` & `rangekeeper-0.4.1a0/rangekeeper/periodicity.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/policy.py` & `rangekeeper-0.4.1a0/rangekeeper/policy.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/projection.py` & `rangekeeper-0.4.1a0/rangekeeper/projection.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/segmentation.py` & `rangekeeper-0.4.1a0/rangekeeper/segmentation.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/space.py` & `rangekeeper-0.4.1a0/rangekeeper/space.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/rangekeeper/span.py` & `rangekeeper-0.4.1a0/rangekeeper/span.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.4.0a0/PKG-INFO` & `rangekeeper-0.4.1a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rangekeeper
-Version: 0.4.0a0
+Version: 0.4.1a0
 Summary: A Python library assisting financial modelling in scenario planning, decision-making, cashflow forecasting, and the like
 License: MPL-2.0
 Author: Daniel Fink
 Author-email: danfink@mit.edu
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,14 @@
 Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numba (>=0.57.0,<0.58.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: py-linq (>=1.4.0,<2.0.0)
 Requires-Dist: py-moneyed (>=3.0,<4.0)
-Requires-Dist: pygraphviz (>=1.11,<2.0)
 Requires-Dist: pyppeteer (>=1.0.2,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyvis (>=0.3.2,<0.4.0)
 Requires-Dist: pyxirr (>=0.9.0,<0.10.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: specklepy (>=2.12.0,<3.0.0)
@@ -37,29 +36,50 @@
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <img src="https://github.com/daniel-fink/rangekeeper/blob/v0.2.0/walkthrough/resources/rangekeeper.jpg?raw=true" width="300">
 
 # Rangekeeper
-Rangekeeper is a library assisting financial modelling in real estate scenario planning, decision-making, cashflow forecasting, and the like.
+Rangekeeper is an open-source library for financial modelling in real estate 
+asset & development planning, decision-making, cashflow forecasting, and 
+scenario analysis.
+
+Rangekeeper enables real estate valuation at all stages and resolutions of 
+description — from early-stage ‘back-of-the-envelope’ models to detailed 
+commercial assessments, and can be completely synchronised with 3D design, 
+engineering, and logistics modelling.
+
+It decomposes elements of the Discounted Cash Flow (DCF) Proforma modelling 
+approach into recomposable code functions that can be wired together to form a 
+full model. More elaborate and worked-through examples of these classes and 
+functions can be found in the [walkthrough documentation](https://daniel-fink.github.io/rangekeeper/).
 
-It decomposes elements of the Discounted Cash Flow (DCF) Proforma modelling approach into recomposable code functions that can be wired together to form a full model. More elaborate and worked-through examples of these classes and functions can be found in the [walkthrough documentation](https://daniel-fink.github.io/rangekeeper/).
+Development of the library follows the rigorous methodology established by 
+Profs Geltner and de Neufville in their book [Flexibility and Real Estate Valuation under Uncertainty: A Practical Guide for Developers](https://doi.org/10.1002/9781119106470).
 
-Development of the library follows the rigorous methodology established by Profs Geltner and de Neufville in their book [Flexibility and Real Estate Valuation under Uncertainty: A Practical Guide for Developers](https://doi.org/10.1002/9781119106470).
 
-## Dependencies:
+## Installation
+`pip install rangekeeper` or `poetry add rangekeeper`
+
+
+## Development
+
+### Dependencies
 
 - Python >= 3.9 & < 3.11
 
-- Poetry: <https://python-poetry.org/>, a package manager (although it is possible to roll your own; YMMV)
+- Poetry: <https://python-poetry.org/>, a package manager (although it is 
+possible to roll your own; YMMV)
 
-## Installation
+### Environment Setup
 
 1. Install poetry, if you haven't yet: <https://python-poetry.org/docs/master/#installing-with-the-official-installer>
 
 2. Clone this repo.
 
 3. Use a terminal to install poetry packages from the repo's directory: `<path_to_repo>$ poetry install`
 
-4. Currently, this library is not yet available on Python Package Index (PyPI). If you wish to use this repo with other projects locally, you may install the Rangekeeper library via `<path_to_repo>$ poetry run pip install -e <path_to_rangekeeper_repo>`, replacing `<path_to_rangekeeper_repo>` with its location on your system.
+4. If you wish to develop this repo alongside other projects locally, you may 
+install the local Rangekeeper library via `<path_to_repo>$ poetry run pip install -e <path_to_rangekeeper_repo>`,
+replacing `<path_to_rangekeeper_repo>` with its location on your system.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

